# Comparing `tmp/scrape_schema-0.3.4.tar.gz` & `tmp/scrape_schema-0.3.5.tar.gz`

## Comparing `scrape_schema-0.3.4.tar` & `scrape_schema-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/_logger.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/_protocols.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/_typing.py
--rw-r--r--   0        0        0    13216 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/base.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/field.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/nested.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/type_caster.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/special_methods/__init__.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/special_methods/base.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/scrape_schema/special_methods/methods.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/LICENSE
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/README.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/pyproject.toml
--rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 scrape_schema-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/_logger.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/_protocols.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/_typing.py
+-rw-r--r--   0        0        0    13216 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/base.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/field.py
+-rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/nested.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/type_caster.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/special_methods/__init__.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/special_methods/base.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/special_methods/methods.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/LICENSE
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/README.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/PKG-INFO
```

### Comparing `scrape_schema-0.3.4/scrape_schema/_protocols.py` & `scrape_schema-0.3.5/scrape_schema/_protocols.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/scrape_schema/_typing.py` & `scrape_schema-0.3.5/scrape_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/scrape_schema/base.py` & `scrape_schema-0.3.5/scrape_schema/base.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/scrape_schema/field.py` & `scrape_schema-0.3.5/scrape_schema/field.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/scrape_schema/nested.py` & `scrape_schema-0.3.5/scrape_schema/nested.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,22 +21,22 @@
     def _prepare_markup(self, markup):
         raise NotImplementedError(
             "_prepare_markup not allowed in Nested"
         )  # pragma: no cover
 
     def sc_parse(self, markup) -> Any:
         if not self.type_:
-            raise AttributeError("Nested required annotation or `type_` param")
+            raise TypeError("Nested required annotation or `type_` param")
         elif get_origin(self.type_) is list and (
             len(get_args(self.type_)) != 0
             and issubclass(get_args(self.type_)[0], BaseSchema)
         ):
             pass
         elif not issubclass(self.type_, BaseSchema):
-            raise AttributeError(
+            raise TypeError(
                 f"type should be List[BaseSchema] or BaseSchema, not {self.type_}"
             )
 
         if len(get_args(self.type_)) != 0 and issubclass(
             get_args(self.type_)[0], BaseSchema
         ):
             cls_schema = get_args(self.type_)[0]
```

### Comparing `scrape_schema-0.3.4/scrape_schema/type_caster.py` & `scrape_schema-0.3.5/scrape_schema/type_caster.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/scrape_schema/special_methods/__init__.py` & `scrape_schema-0.3.5/scrape_schema/special_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/scrape_schema/special_methods/base.py` & `scrape_schema-0.3.5/scrape_schema/special_methods/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,32 +17,32 @@
 
 class MarkupMethod(NamedTuple):
     METHOD_NAME: Union[str, SpecialMethods]
     args: Tuple[Any, ...] = ()
     kwargs: Dict[str, Any] = {}
 
     def __repr__(self):
-        return f"{self.METHOD_NAME} args={self.args}, kwargs={self.kwargs}"
+        return f"{self.METHOD_NAME} args={self.args}, kwargs={self.kwargs}"  # pragma: no cover
 
 
 class SpecialMethodCallable(Protocol):
     def __call__(self, markup: Any, method: MarkupMethod, **kwargs):
-        pass
+        pass  # pragma: no cover
 
 
 class BaseSpecialMethodStrategy:
     @abstractmethod
     def __call__(self, markup: Any, method: MarkupMethod, **kwargs):
-        pass
+        pass  # pragma: no cover
 
 
 class SpecialMethodsHandler:
     def __init__(self):
         self.spec_methods_dict: Dict[SpecialMethods, SpecialMethodCallable] = {}  # type: ignore
 
     def add_method(self, spec_method: SpecialMethods, strategy: SpecialMethodCallable):
         self.spec_methods_dict[spec_method] = strategy
 
     def handle(self, method: MarkupMethod, markup: Any, **kwargs):
         if isinstance(method.METHOD_NAME, SpecialMethods):
             return self.spec_methods_dict[method.METHOD_NAME](markup, method, **kwargs)
-        raise TypeError("Unknown special method")
+        raise TypeError("Unknown special method")  # pragma: no cover
```

### Comparing `scrape_schema-0.3.4/scrape_schema/special_methods/methods.py` & `scrape_schema-0.3.5/scrape_schema/special_methods/methods.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/.gitignore` & `scrape_schema-0.3.5/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/LICENSE` & `scrape_schema-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/README.md` & `scrape_schema-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/pyproject.toml` & `scrape_schema-0.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.4/PKG-INFO` & `scrape_schema-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.3.4
+Version: 0.3.5
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

