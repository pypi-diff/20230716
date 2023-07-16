# Comparing `tmp/drf_pydantic-0.4.1.tar.gz` & `tmp/drf_pydantic-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_pydantic-0.4.1.tar", max compression
+gzip compressed data, was "drf_pydantic-0.5.0.tar", max compression
```

## Comparing `drf_pydantic-0.4.1.tar` & `drf_pydantic-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1072 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/LICENSE
--rw-r--r--   0        0        0     3481 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/README.md
--rw-r--r--   0        0        0     2148 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       66 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/src/drf_pydantic/__init__.py
--rw-r--r--   0        0        0      626 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/src/drf_pydantic/base_model.py
--rw-r--r--   0        0        0     6029 2023-04-15 21:41:25.720297 drf_pydantic-0.4.1/src/drf_pydantic/parse.py
--rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 drf_pydantic-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-07-16 00:45:04.147081 drf_pydantic-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3481 2023-07-16 00:45:04.147081 drf_pydantic-0.5.0/README.md
+-rw-r--r--   0        0        0     2148 2023-07-16 00:45:04.147081 drf_pydantic-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-07-16 00:45:04.147081 drf_pydantic-0.5.0/src/drf_pydantic/__init__.py
+-rw-r--r--   0        0        0      626 2023-07-16 00:45:04.147081 drf_pydantic-0.5.0/src/drf_pydantic/base_model.py
+-rw-r--r--   0        0        0     1421 2023-07-16 00:45:04.147081 drf_pydantic-0.5.0/src/drf_pydantic/fields.py
+-rw-r--r--   0        0        0     6260 2023-07-16 00:45:04.147081 drf_pydantic-0.5.0/src/drf_pydantic/parse.py
+-rw-r--r--   0        0        0     4698 1970-01-01 00:00:00.000000 drf_pydantic-0.5.0/PKG-INFO
```

### Comparing `drf_pydantic-0.4.1/LICENSE` & `drf_pydantic-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_pydantic-0.4.1/README.md` & `drf_pydantic-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `drf_pydantic-0.4.1/pyproject.toml` & `drf_pydantic-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-pydantic"
-version = "0.4.1"
+version = "0.5.0"
 description = "Use pydantic with the Django REST framework"
 license = "MIT"
 authors = ["George Bocharov <bocharovgeorgii@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/georgebv/drf-pydantic"
 repository = "https://github.com/georgebv/drf-pydantic"
 keywords = ["django", "drf", "pydantic", "typing", "rest", "api"]
```

### Comparing `drf_pydantic-0.4.1/src/drf_pydantic/base_model.py` & `drf_pydantic-0.5.0/src/drf_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `drf_pydantic-0.4.1/src/drf_pydantic/parse.py` & `drf_pydantic-0.5.0/src/drf_pydantic/parse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import datetime
 import decimal
 import inspect
 import types
 import typing
 import uuid
 import warnings
+from enum import Enum
 
 import pydantic
 
 from rest_framework import serializers
+from drf_pydantic.fields import EnumField
 
 # Cache serializer classes to ensure that there is a one-to-one relationship
 # between pydantic models and serializer classes
 # This is useful during introspection in tools such as drf_spectacular, so that
 # it doesn't pick the same serializer as distinct objects due to dynamic generation
 SERIALIZER_REGISTRY: dict[type, type[serializers.Serializer]] = {}
 
@@ -34,14 +36,16 @@
     datetime.date: serializers.DateField,
     datetime.time: serializers.TimeField,
     datetime.datetime: serializers.DateTimeField,
     datetime.timedelta: serializers.DurationField,
     # Constraint fields
     pydantic.ConstrainedStr: serializers.CharField,
     pydantic.ConstrainedInt: serializers.IntegerField,
+    # Enum fields
+    Enum: EnumField
 }
 
 
 def create_serializer_from_model(
     model_class: type[pydantic.BaseModel],
 ) -> type[serializers.Serializer]:
     """
@@ -118,14 +122,19 @@
     # String field with constraints
     if inspect.isclass(field.type_) and issubclass(
         field.type_, pydantic.types.ConstrainedStr
     ):
         extra_kwargs["min_length"] = field.type_.min_length
         extra_kwargs["max_length"] = field.type_.max_length
 
+    if inspect.isclass(field.type_) and issubclass(
+        field.type_, Enum
+    ):
+        extra_kwargs['enum'] = field.type_
+
     # Scalar field
     if field.outer_type_ is field.type_:
         # Normal class
         if inspect.isclass(field.type_):
             return _convert_type(field.type_)(**extra_kwargs)
 
         # Alias
```

### Comparing `drf_pydantic-0.4.1/PKG-INFO` & `drf_pydantic-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-pydantic
-Version: 0.4.1
+Version: 0.5.0
 Summary: Use pydantic with the Django REST framework
 Home-page: https://github.com/georgebv/drf-pydantic
 License: MIT
 Keywords: django,drf,pydantic,typing,rest,api
 Author: George Bocharov
 Author-email: bocharovgeorgii@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -15,15 +15,14 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: djangorestframework (>=3.13.0,<4.0.0)
 Requires-Dist: pydantic[email] (>=1.9.0,<2.0.0)
 Project-URL: Repository, https://github.com/georgebv/drf-pydantic
 Description-Content-Type: text/markdown
```

