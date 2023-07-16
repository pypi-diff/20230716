# Comparing `tmp/valcheck-0.5.0.tar.gz` & `tmp/valcheck-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valcheck-0.5.0.tar", last modified: Sun Jul 16 09:09:51 2023, max compression
+gzip compressed data, was "valcheck-0.6.0.tar", last modified: Sun Jul 16 13:23:53 2023, max compression
```

## Comparing `valcheck-0.5.0.tar` & `valcheck-0.6.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 09:09:51.410390 valcheck-0.5.0/
--rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.5.0/LICENSE
--rw-rw-rw-   0        0        0      760 2023-07-16 09:09:51.407176 valcheck-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2674 2023-07-16 09:05:22.000000 valcheck-0.5.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 09:09:51.410390 valcheck-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1568 2023-07-16 09:03:28.000000 valcheck-0.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:09:51.383239 valcheck-0.5.0/valcheck/
--rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.5.0/valcheck/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-07-02 09:39:38.000000 valcheck-0.5.0/valcheck/exceptions.py
--rw-rw-rw-   0        0        0    21775 2023-07-16 07:09:18.000000 valcheck-0.5.0/valcheck/fields.py
--rw-rw-rw-   0        0        0     2694 2023-07-15 05:51:54.000000 valcheck-0.5.0/valcheck/models.py
--rw-rw-rw-   0        0        0     3156 2023-07-16 07:09:18.000000 valcheck-0.5.0/valcheck/utils.py
--rw-rw-rw-   0        0        0     5770 2023-07-16 09:05:02.000000 valcheck-0.5.0/valcheck/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-16 09:09:51.406178 valcheck-0.5.0/valcheck.egg-info/
--rw-rw-rw-   0        0        0      760 2023-07-16 09:09:51.000000 valcheck-0.5.0/valcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-16 09:09:51.000000 valcheck-0.5.0/valcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 09:09:51.000000 valcheck-0.5.0/valcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 09:09:51.000000 valcheck-0.5.0/valcheck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 13:23:53.418991 valcheck-0.6.0/
+-rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0      760 2023-07-16 13:23:53.417992 valcheck-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2674 2023-07-16 13:12:11.000000 valcheck-0.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 13:23:53.419998 valcheck-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-07-16 13:12:11.000000 valcheck-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 13:23:53.396372 valcheck-0.6.0/valcheck/
+-rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.6.0/valcheck/__init__.py
+-rw-rw-rw-   0        0        0     1270 2023-07-02 09:39:38.000000 valcheck-0.6.0/valcheck/exceptions.py
+-rw-rw-rw-   0        0        0    21775 2023-07-16 07:09:18.000000 valcheck-0.6.0/valcheck/fields.py
+-rw-rw-rw-   0        0        0     2694 2023-07-15 05:51:54.000000 valcheck-0.6.0/valcheck/models.py
+-rw-rw-rw-   0        0        0     3156 2023-07-16 07:09:18.000000 valcheck-0.6.0/valcheck/utils.py
+-rw-rw-rw-   0        0        0     6039 2023-07-16 13:10:09.000000 valcheck-0.6.0/valcheck/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-16 13:23:53.415998 valcheck-0.6.0/valcheck.egg-info/
+-rw-rw-rw-   0        0        0      760 2023-07-16 13:23:53.000000 valcheck-0.6.0/valcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-16 13:23:53.000000 valcheck-0.6.0/valcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 13:23:53.000000 valcheck-0.6.0/valcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 13:23:53.000000 valcheck-0.6.0/valcheck.egg-info/top_level.txt
```

### Comparing `valcheck-0.5.0/LICENSE` & `valcheck-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valcheck-0.5.0/PKG-INFO` & `valcheck-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 0.5.0
+Version: 0.6.0
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `valcheck-0.5.0/README.md` & `valcheck-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         pprint([error.as_dict() for error in errors]) # Error list
     else:
         pprint(person_validator.validated_data) # Dictionary having validated data (by field)
 ```
 
 ## Performance benchmarks
 - On comparison of the performance of Django Rest Framework's (version 3.14.0) serializer with Valcheck's
-validator, we found that Valcheck (version 0.5.0) is ~3.8 times faster for cases where the data is
+validator, we found that Valcheck (version 0.6.0) is ~3.8 times faster for cases where the data is
 valid, and ~2.7 times faster for cases where the data is invalid.
 - These numbers are averaged over 25,000 iterations.
 
 ```python
 from rest_framework import serializers
 from valcheck import fields, models, validator
```

### Comparing `valcheck-0.5.0/setup.py` & `valcheck-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import find_packages, setup
 
 # Constants
 PACKAGE_NAME = "valcheck"
-PACKAGE_VERSION = "0.5.0"
+PACKAGE_VERSION = "0.6.0"
 AUTHOR_NAME = "Nishant Rao"
 AUTHOR_EMAIL_ID = "nishant.rao173@gmail.com"
 FILEPATH_TO_README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
 FILEPATH_TO_REQUIREMENTS = os.path.join(os.path.abspath(os.path.dirname(__file__)), "requirements.txt")
 REPOSITORY_URL = "https://github.com/Nishant173/valcheck"
 
 # Requirements
```

### Comparing `valcheck-0.5.0/valcheck/exceptions.py` & `valcheck-0.6.0/valcheck/exceptions.py`

 * *Files identical despite different names*

### Comparing `valcheck-0.5.0/valcheck/fields.py` & `valcheck-0.6.0/valcheck/fields.py`

 * *Files identical despite different names*

### Comparing `valcheck-0.5.0/valcheck/models.py` & `valcheck-0.6.0/valcheck/models.py`

 * *Files identical despite different names*

### Comparing `valcheck-0.5.0/valcheck/utils.py` & `valcheck-0.6.0/valcheck/utils.py`

 * *Files identical despite different names*

### Comparing `valcheck-0.5.0/valcheck/validator.py` & `valcheck-0.6.0/valcheck/validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,30 +5,41 @@
 from valcheck.models import Error
 from valcheck.utils import Empty, is_empty, is_list_of_instances_of_type, set_as_empty
 
 
 class Validator:
     """
     Properties:
+        - context
         - validated_data
 
     Instance methods:
         - get_field_value()
         - list_field_validators()
         - model_validator()
         - run_validations()
     """
 
-    def __init__(self, *, data: Dict[str, Any]) -> None:
+    def __init__(
+            self,
+            *,
+            data: Dict[str, Any],
+            context: Optional[Dict[str, Any]] = None,
+        ) -> None:
         assert isinstance(data, dict), "Param `data` must be a dictionary"
         self.data = data
+        self._context: Dict[str, Any] = context or {}
         self._field_info: Dict[str, Field] = self._initialise_fields()
         self._errors: List[Error] = []
         self._validated_data: Dict[str, Any] = {}
 
+    @property
+    def context(self) -> Dict[str, Any]:
+        return self._context
+
     def list_field_validators(self) -> List[Dict[str, Any]]:
         return [
             {
                 "field_type": field.__class__.__name__,
                 "field_identifier": field_identifier,
                 "field_name": field.field_name,
                 "alias": field.alias,
```

### Comparing `valcheck-0.5.0/valcheck.egg-info/PKG-INFO` & `valcheck-0.6.0/valcheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 0.5.0
+Version: 0.6.0
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

