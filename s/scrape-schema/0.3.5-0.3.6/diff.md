# Comparing `tmp/scrape_schema-0.3.5.tar.gz` & `tmp/scrape_schema-0.3.6.tar.gz`

## Comparing `scrape_schema-0.3.5.tar` & `scrape_schema-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/__init__.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/_logger.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/_protocols.py
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/_typing.py
--rw-r--r--   0        0        0    13216 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/base.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/field.py
--rw-r--r--   0        0        0     1791 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/nested.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/type_caster.py
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/special_methods/__init__.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/special_methods/base.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/scrape_schema/special_methods/methods.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/LICENSE
--rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/README.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/pyproject.toml
--rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 scrape_schema-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/__init__.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/_logger.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/_protocols.py
+-rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/_typing.py
+-rw-r--r--   0        0        0    13309 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/base.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/field.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/nested.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/type_caster.py
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/special_methods/__init__.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/special_methods/base.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/scrape_schema/special_methods/methods.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/LICENSE
+-rw-r--r--   0        0        0    10563 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/README.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    12494 2020-02-02 00:00:00.000000 scrape_schema-0.3.6/PKG-INFO
```

### Comparing `scrape_schema-0.3.5/scrape_schema/_protocols.py` & `scrape_schema-0.3.6/scrape_schema/_protocols.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/scrape_schema/_typing.py` & `scrape_schema-0.3.6/scrape_schema/_typing.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/scrape_schema/base.py` & `scrape_schema-0.3.6/scrape_schema/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     SpecialMethodsHandler,
 )
 from scrape_schema.type_caster import TypeCaster
 
 
 class sc_param(property):
     """Shortcut for adding property-like descriptors in BaseSchema"""
+
     pass  # pragma: no cover
 
 
 class BaseField:
     def __init__(self, auto_type: bool = True, default: Any = ..., **kwargs):
         self._stack_methods: List[MarkupMethod] = []
         self.default = default
@@ -59,15 +60,15 @@
     @staticmethod
     def _accept_method(markup: Any, method: MarkupMethod) -> Any:
         if isinstance(method.METHOD_NAME, str):
             class_method = getattr(markup, method.METHOD_NAME)
             if isinstance(class_method, (property, dict)):  # attrib check
                 return class_method
             return getattr(markup, method.METHOD_NAME)(*method.args, **method.kwargs)
-        raise TypeError(
+        raise TypeError(  # pragma: no cover
             f"`{type(markup).__name__}` is not contains `{method.METHOD_NAME}`"
         )
 
     def _call_stack_methods(self, markup: Any) -> Any:
         result = markup
         _logger.info("start call methods. stack count: %s", len(self._stack_methods))
         for method in self._stack_methods:
@@ -223,15 +224,15 @@
 
         # localns={} kwarg avoid TypeError 'function' object is not subscriptable
         for name, value in get_type_hints(
             cls_schema, localns={}, include_extras=True
         ).items():
             if name in ("__schema_fields__", "__schema_annotations__", "__parsers__"):
                 continue  # pragma: no cover
-            if mcs.__is_type_field(value):
+            if mcs.__is_type_field(value):  # pragma: no cover
                 field_type, field = mcs.__parse_annotated_field(value)
                 __schema_fields__[name] = field
                 __schema_annotations__[name] = field_type
 
         setattr(cls_schema, "__schema_fields__", __schema_fields__)
         setattr(cls_schema, "__schema_annotations__", __schema_annotations__)
         setattr(cls_schema, "__meta_info__", {})
@@ -241,15 +242,17 @@
 class BaseSchema(metaclass=SchemaMeta):
     class Config:
         selector_kwargs: Dict[str, Any] = {}
         type_caster: Optional[TypeCaster] = TypeCaster()  # TODO make interface
 
     @property
     def __sc_params__(self) -> Dict[str, Any]:
-        return {k: v for k, v in self.__dict__.items() if isinstance(v, sc_param)}
+        return {
+            k: v for k, v in self.__class__.__dict__.items() if isinstance(v, sc_param)
+        }
 
     @property
     def __selector__(self) -> Union[Selector, SelectorList]:
         return self._cached_parser
 
     @property
     def __raw__(self) -> str:
@@ -301,15 +304,15 @@
 
     @staticmethod
     def _to_dict(value: Union["BaseSchema", List, Dict, Any]):
         if isinstance(value, BaseSchema):
             return value.dict()
 
         elif isinstance(value, list):
-            if all(isinstance(val, BaseSchema) for val in value):
+            if all(isinstance(val, BaseSchema) for val in value):  # pragma: no cover
                 return [val.dict() for val in value]
         return value
 
     def dict(self):
         result: Dict[str, Any] = {  # type: ignore
             k: self._to_dict(getattr(self, k))
             for k, v in self.__class__.__dict__.items()
```

### Comparing `scrape_schema-0.3.5/scrape_schema/field.py` & `scrape_schema-0.3.6/scrape_schema/field.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/scrape_schema/nested.py` & `scrape_schema-0.3.6/scrape_schema/nested.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,11 +43,11 @@
         else:
             cls_schema = self.type_
 
         chunks = self._crop_field.sc_parse(markup)
         if isinstance(chunks, SelectorList) and get_origin(self.type_) is list:
             return [cls_schema(chunk.get()) for chunk in chunks]
         elif get_origin(self.type_) is list:
-            return [cls_schema(chunk) for chunk in chunks]
+            return [cls_schema(chunk) for chunk in chunks]  # pragma: no cover
         elif isinstance(chunks, Selector) and get_origin(self.type_) is not list:
             return cls_schema(chunks.get())
-        return cls_schema(chunks)
+        return cls_schema(chunks)  # pragma: no cover
```

### Comparing `scrape_schema-0.3.5/scrape_schema/type_caster.py` & `scrape_schema-0.3.6/scrape_schema/type_caster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pragma: no cover
 import sys
 from typing import Any, Type, Union
-from scrape_schema._typing import NoneType
+
 from scrape_schema._logger import _logger
-from scrape_schema._typing import get_args, get_origin
+from scrape_schema._typing import NoneType, get_args, get_origin
 
 
 class TypeCaster:
     def _typing_to_builtin(self, type_hint: Type) -> Type:
         origin = get_origin(type_hint)
         args = get_args(type_hint)
```

### Comparing `scrape_schema-0.3.5/scrape_schema/special_methods/__init__.py` & `scrape_schema-0.3.6/scrape_schema/special_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/scrape_schema/special_methods/base.py` & `scrape_schema-0.3.6/scrape_schema/special_methods/base.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/scrape_schema/special_methods/methods.py` & `scrape_schema-0.3.6/scrape_schema/special_methods/methods.py`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/.gitignore` & `scrape_schema-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/LICENSE` & `scrape_schema-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/README.md` & `scrape_schema-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/pyproject.toml` & `scrape_schema-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scrape_schema-0.3.5/PKG-INFO` & `scrape_schema-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrape-schema
-Version: 0.3.5
+Version: 0.3.6
 Summary: A library for converting any text (xml, html, plain text, stdout, etc) to python datatypes
 Project-URL: Documentation, https://github.com/vypivshiy/scrape-schema#readme
 Project-URL: Issues, https://github.com/vypivshiy/scrape-schema/issues
 Project-URL: Source, https://github.com/vypivshiy/scrape-schema
 Project-URL: Examples, https://github.com/vypivshiy/scrape-schema/examples
 Author: vypivshiy
 License-Expression: MIT
```

