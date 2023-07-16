# Comparing `tmp/python_injection-0.2.1.tar.gz` & `tmp/python_injection-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_injection-0.2.1.tar", max compression
+gzip compressed data, was "python_injection-0.2.2.tar", max compression
```

## Comparing `python_injection-0.2.1.tar` & `python_injection-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2538 2023-07-15 13:17:13.335254 python_injection-0.2.1/README.md
--rw-r--r--   0        0        0       38 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/__init__.py
--rw-r--r--   0        0        0     3657 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/core.py
--rw-r--r--   0        0        0      340 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/core.pyi
--rw-r--r--   0        0        0       39 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/exceptions.py
--rw-r--r--   0        0        0      461 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/utils.py
--rw-r--r--   0        0        0       81 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/utils.pyi
--rw-r--r--   0        0        0      561 2023-07-15 13:17:34.087188 python_injection-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 python_injection-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2538 2023-07-16 12:05:40.851462 python_injection-0.2.2/README.md
+-rw-r--r--   0        0        0       38 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/__init__.py
+-rw-r--r--   0        0        0     4038 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/core.py
+-rw-r--r--   0        0        0      340 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/core.pyi
+-rw-r--r--   0        0        0       39 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/exceptions.py
+-rw-r--r--   0        0        0      461 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/utils.py
+-rw-r--r--   0        0        0       81 2023-07-16 12:05:40.851462 python_injection-0.2.2/injection/utils.pyi
+-rw-r--r--   0        0        0      561 2023-07-16 12:06:03.571627 python_injection-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 python_injection-0.2.2/PKG-INFO
```

### Comparing `python_injection-0.2.1/README.md` & `python_injection-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `python_injection-0.2.1/injection/core.py` & `python_injection-0.2.2/injection/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import inspect
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from functools import cached_property, wraps
 from inspect import Parameter
-from typing import Callable, Generic, TypeVar
+from typing import Callable, Generic, Iterable, TypeVar
 
 from injection.exceptions import NoInjectable
 
 T = TypeVar("T")
 
 
 @dataclass(repr=False, frozen=True, slots=True)
@@ -36,29 +36,36 @@
         return self.__instance
 
 
 @dataclass(repr=False, frozen=True, slots=True)
 class InjectionManager:
     __container: dict[type, Injectable] = field(default_factory=dict, init=False)
 
-    def __getitem__(self, reference: type) -> Injectable:
+    def get(self, reference: type) -> Injectable:
         try:
             return self.__container[reference]
         except KeyError as exc:
             raise NoInjectable(f"No injectable for {reference.__name__}.") from exc
 
-    def __setitem__(self, reference: type, injectable: Injectable):
+    def set_multiple(self, references: Iterable[type], injectable: Injectable):
+        def reference_parser():
+            for reference in references:
+                self.check_if_exists(reference)
+                yield reference, injectable
+
+        new_values = reference_parser()
+        self.__container.update(new_values)
+
+    def check_if_exists(self, reference: type):
         if reference in self.__container:
             raise RuntimeError(
                 f"An injectable already exists for the "
                 f"reference class `{reference.__name__}`."
             )
 
-        self.__container[reference] = injectable
-
 
 _manager = InjectionManager()
 
 del InjectionManager
 
 
 @dataclass(repr=False, frozen=True, slots=True)
@@ -66,38 +73,41 @@
     __injectable_class: type[Injectable]
 
     def __repr__(self) -> str:
         return f"<{self.__injectable_class.__name__} decorator>"  # pragma: no cover
 
     def __call__(self, wp=None, /, **kwargs):
         def decorator(wrapped):
-            injectable = self.__injectable_class(wrapped)
+            def iter_references():
+                if isinstance(wrapped, type):
+                    yield wrapped
 
-            if isinstance(wrapped, type):
-                _manager[wrapped] = injectable
+                if reference := kwargs.pop("reference", None):
+                    yield reference
 
-            if reference := kwargs.pop("reference", None):
-                _manager[reference] = injectable
+                for reference in kwargs.pop("references", ()):
+                    yield reference
 
-            for reference in kwargs.pop("references", ()):
-                _manager[reference] = injectable
+            references = iter_references()
+            injectable = self.__injectable_class(wrapped)
+            _manager.set_multiple(references, injectable)
 
             return wrapped
 
         return decorator(wp) if wp else decorator
 
 
 new = Decorator(NewInjectable)
 unique = Decorator(UniqueInjectable)
 
 del Decorator
 
 
 def get_instance(reference: type[T]) -> T:
-    return _manager[reference].get_instance()
+    return _manager.get(reference).get_instance()
 
 
 def inject(fn=None):
     def decorator(function):
         @wraps(function)
         def wrapper(*args, **kwargs):
             signature = inspect.signature(function)
@@ -116,15 +126,15 @@
 
                 match parameter.kind:
                     case Parameter.POSITIONAL_ONLY:
                         args.append(value)
                     case Parameter.VAR_POSITIONAL:
                         args.extend(value)
                     case Parameter.VAR_KEYWORD:
-                        kwargs |= value
+                        kwargs.update(value)
                     case _:
                         kwargs[name] = value
 
             return function(*args, **kwargs)
 
         return wrapper
```

### Comparing `python_injection-0.2.1/pyproject.toml` & `python_injection-0.2.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-injection"
-version = "0.2.1"
+version = "0.2.2"
 description = "Fast and easy dependency injection framework."
 authors = ["remimd"]
 keywords = ["dependencies", "inject", "injection"]
 license = "MIT"
 packages = [{ include = "injection" }]
 readme = "README.md"
 repository = "https://github.com/soon-app/injection"
```

### Comparing `python_injection-0.2.1/PKG-INFO` & `python_injection-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-injection
-Version: 0.2.1
+Version: 0.2.2
 Summary: Fast and easy dependency injection framework.
 Home-page: https://github.com/soon-app/injection
 License: MIT
 Keywords: dependencies,inject,injection
 Author: remimd
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
```

