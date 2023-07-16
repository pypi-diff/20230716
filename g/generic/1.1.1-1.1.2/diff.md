# Comparing `tmp/generic-1.1.1.tar.gz` & `tmp/generic-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "generic-1.1.1.tar", max compression
+gzip compressed data, was "generic-1.1.2.tar", max compression
```

## Comparing `generic-1.1.1.tar` & `generic-1.1.2.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1720 2022-11-20 19:25:15.469824 generic-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     2600 2022-11-20 19:25:15.469824 generic-1.1.1/README.md
--rw-r--r--   0        0        0        0 2022-11-20 19:25:15.469824 generic-1.1.1/generic/__init__.py
--rw-r--r--   0        0        0     2806 2022-11-20 19:25:15.469824 generic-1.1.1/generic/event.py
--rw-r--r--   0        0        0     4940 2022-11-20 19:25:15.469824 generic-1.1.1/generic/multidispatch.py
--rw-r--r--   0        0        0     3481 2022-11-20 19:25:15.469824 generic-1.1.1/generic/multimethod.py
--rw-r--r--   0        0        0     5098 2022-11-20 19:25:15.469824 generic-1.1.1/generic/registry.py
--rw-r--r--   0        0        0     2540 2022-11-20 19:25:15.469824 generic-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3350 1970-01-01 00:00:00.000000 generic-1.1.1/setup.py
--rw-r--r--   0        0        0     3715 1970-01-01 00:00:00.000000 generic-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1515 2023-07-16 11:36:13.898727 generic-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     3000 2023-07-16 11:36:13.898727 generic-1.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-07-16 11:36:13.898727 generic-1.1.2/generic/__init__.py
+-rw-r--r--   0        0        0     2806 2023-07-16 11:36:13.898727 generic-1.1.2/generic/event.py
+-rw-r--r--   0        0        0     5000 2023-07-16 11:36:13.898727 generic-1.1.2/generic/multidispatch.py
+-rw-r--r--   0        0        0     3542 2023-07-16 11:36:13.898727 generic-1.1.2/generic/multimethod.py
+-rw-r--r--   0        0        0     5098 2023-07-16 11:36:13.898727 generic-1.1.2/generic/registry.py
+-rw-r--r--   0        0        0     1964 2023-07-16 11:36:13.898727 generic-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4237 1970-01-01 00:00:00.000000 generic-1.1.2/PKG-INFO
```

### Comparing `generic-1.1.1/LICENSE.txt` & `generic-1.1.2/LICENSE.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,28 @@
-A copyright notice accompanies this license document that identifies
-the copyright holders.
+BSD 3-Clause License
+
+Copyright (c) 2010, Generic Library contributors
 
 Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are
-met:
+modification, are permitted provided that the following conditions are met:
 
-1.  Redistributions in source code must retain the accompanying
-    copyright notice, this list of conditions, and the following
-    disclaimer.
-
-2.  Redistributions in binary form must reproduce the accompanying
-    copyright notice, this list of conditions, and the following
-    disclaimer in the documentation and/or other materials provided
-    with the distribution.
-
-3.  Names of the copyright holders must not be used to endorse or
-    promote products derived from this software without prior
-    written permission from the copyright holders.
-
-4.  If any files are modified, you must cause the modified files to
-    carry prominent notices stating that you changed the files and
-    the date of any change.
-
-Disclaimer
-
-  THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS ``AS IS'' AND
-  ANY EXPRESSED OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
-  TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
-  PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
-  HOLDERS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
-  EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
-  TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-  ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR
-  TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF
-  THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
-  SUCH DAMAGE.
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
 
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `generic-1.1.1/README.md` & `generic-1.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,31 @@
 [documentation](http://generic.readthedocs.org/en/latest/index.html) hosted at
 excellent readthedocs.org project. Development takes place on
 [github](http://github.com/gaphor/generic).
 
 
 # Changes
 
+## 1.1.2
+
+- Replace print statements with logging
+- Enable trusted publisher for PyPI
+- Create Security Policy
+- Update LICENSE to BSD 3-Clause
+- Add support for Python 3.12
+- Simplify build: drop tox
+- Update documentation theme to Furo
+- Switch linting to ruff
+
+## 1.1.1
+
+- Add support for Python 3.11
+- Move mypy configuration to pyproject.toml
+- Enable automatic release of new versions with CI
+
 ## 1.1.0
 
 - Rename `master` branch to `main`
 - `generic.event.Manager` executes all handlers and throws an `ExceptionGroup` in case of errors
 
 ## 1.0.1
```

### Comparing `generic-1.1.1/generic/event.py` & `generic-1.1.2/generic/event.py`

 * *Files identical despite different names*

### Comparing `generic-1.1.1/generic/multidispatch.py` & `generic-1.1.2/generic/multidispatch.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,23 +9,26 @@
 Note that this module does not support annotated functions.
 """
 
 from __future__ import annotations
 
 import functools
 import inspect
+import logging
 from typing import Any, Callable, Generic, TypeVar, Union, cast
 
 from generic.registry import Registry, TypeAxis
 
 __all__ = "multidispatch"
 
 T = TypeVar("T", bound=Union[Callable[..., Any], type])
 KeyType = Union[type, None]
 
+logger = logging.getLogger(__name__)
+
 
 def multidispatch(*argtypes: KeyType) -> Callable[[T], FunctionDispatcher[T]]:
     """Declare function as multidispatch.
 
     This decorator takes ``argtypes`` argument types and replace
     decorated function with :class:`.FunctionDispatcher` object, which
     is responsible for multiple dispatch feature.
@@ -122,15 +125,15 @@
         return register_rule
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Dispatch call to appropriate rule."""
         trimmed_args = args[: self.params_arity]
         rule = self.registry.lookup(*trimmed_args)
         if not rule:
-            print(self.registry._tree)
+            logger.debug(self.registry._tree)
             raise TypeError(f"No available rule found for {trimmed_args!r}")
         return rule(*args, **kwargs)
 
 
 def _arity(argspec: inspect.FullArgSpec) -> int:
     """Determinal positional arity of argspec."""
     args = argspec.args or []
```

### Comparing `generic-1.1.1/generic/multimethod.py` & `generic-1.1.2/generic/multimethod.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """Multi-method builds on the functionality provided by `multidispatch` to
 provide generic methods."""
 
 from __future__ import annotations
 
 import functools
 import inspect
+import logging
 import threading
 import types
 from typing import Any, Callable, TypeVar, Union, cast
 
 from generic.multidispatch import FunctionDispatcher, KeyType
 
 __all__ = ("multimethod", "has_multimethods")
 
 C = TypeVar("C")
 T = TypeVar("T", bound=Union[Callable[..., Any], type])
 
+logger = logging.getLogger(__name__)
+
 
 def multimethod(*argtypes: KeyType) -> Callable[[T], MethodDispatcher[T]]:
     """Declare method as multimethod.
 
     This decorator works exactly the same as :func:`.multidispatch` decorator
     but replaces decorated method with :class:`.MethodDispatcher` object
     instead.
@@ -46,15 +49,15 @@
 
 def has_multimethods(cls: type[C]) -> type[C]:
     """Declare class as one that have multimethods.
 
     Should only be used for decorating classes which have methods decorated with
     :func:`.multimethod` decorator.
     """
-    for name, obj in cls.__dict__.items():
+    for _name, obj in cls.__dict__.items():
         if isinstance(obj, MethodDispatcher):
             obj.proceed_unbound_rules(cls)
     return cls
 
 
 class MethodDispatcher(FunctionDispatcher[T]):
     """Multiple dispatch for methods.
@@ -77,15 +80,15 @@
         ``proceed_unbound_rules`` later."""
         self.local.unbound_rules.append((argtypes, func))
 
     def proceed_unbound_rules(self, cls) -> None:
         """Process all unbound rule by binding them to ``cls`` type."""
         for argtypes, func in self.local.unbound_rules:
             argtypes = (cls,) + argtypes
-            print("register rule", argtypes)
+            logger.debug("register rule", argtypes)
             self.register_rule(func, *argtypes)
         self.local.unbound_rules = []
 
     def __get__(self, obj, cls):
         return self if obj is None else types.MethodType(self, obj)
 
     def register(self, *argtypes: KeyType) -> Callable[[T], T]:
```

### Comparing `generic-1.1.1/generic/registry.py` & `generic-1.1.2/generic/registry.py`

 * *Files identical despite different names*

### Comparing `generic-1.1.1/PKG-INFO` & `generic-1.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: generic
-Version: 1.1.1
+Version: 1.1.2
 Summary: Generic programming library for Python
 Home-page: https://generic.readthedocs.io/
 License: BSD License
 Keywords: generic,multi dispatch,dispatch,event
 Author: Andrey Popp
 Author-email: 8mayday@gmail.com
 Maintainer: Arjan Molenaar
@@ -17,15 +17,18 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: exceptiongroup (>=1.0.0-rc.5,<2.0.0)
+Provides-Extra: docs
+Requires-Dist: exceptiongroup (>=1.0.0,<2.0.0)
+Requires-Dist: furo (>=2022,<2024) ; extra == "docs"
+Requires-Dist: sphinx (>=4.3,<7.1) ; extra == "docs"
 Project-URL: Documentation, https://generic.readthedocs.io/
 Project-URL: Repository, https://github.com/gaphor/generic
 Description-Content-Type: text/markdown
 
 # Generic programming library for Python
 
 [![Build state](https://github.com/gaphor/generic/workflows/build/badge.svg)](https://github.com/gaphor/generic/actions)
@@ -47,14 +50,31 @@
 [documentation](http://generic.readthedocs.org/en/latest/index.html) hosted at
 excellent readthedocs.org project. Development takes place on
 [github](http://github.com/gaphor/generic).
 
 
 # Changes
 
+## 1.1.2
+
+- Replace print statements with logging
+- Enable trusted publisher for PyPI
+- Create Security Policy
+- Update LICENSE to BSD 3-Clause
+- Add support for Python 3.12
+- Simplify build: drop tox
+- Update documentation theme to Furo
+- Switch linting to ruff
+
+## 1.1.1
+
+- Add support for Python 3.11
+- Move mypy configuration to pyproject.toml
+- Enable automatic release of new versions with CI
+
 ## 1.1.0
 
 - Rename `master` branch to `main`
 - `generic.event.Manager` executes all handlers and throws an `ExceptionGroup` in case of errors
 
 ## 1.0.1
```

