# Comparing `tmp/pydantic_apply-0.1.5.tar.gz` & `tmp/pydantic_apply-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_apply-0.1.5.tar", max compression
+gzip compressed data, was "pydantic_apply-0.5.0.tar", max compression
```

## Comparing `pydantic_apply-0.1.5.tar` & `pydantic_apply-0.5.0.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1078 2023-03-08 13:01:32.724858 pydantic_apply-0.1.5/LICENSE
--rw-r--r--   0        0        0     2038 2023-03-08 13:01:32.724858 pydantic_apply-0.1.5/README.md
--rw-r--r--   0        0        0       35 2023-03-08 13:01:32.724858 pydantic_apply-0.1.5/pydantic_apply/__init__.py
--rw-r--r--   0        0        0     4544 2023-03-08 13:01:32.724858 pydantic_apply-0.1.5/pydantic_apply/apply.py
--rw-r--r--   0        0        0        0 2023-03-08 13:01:32.724858 pydantic_apply-0.1.5/pydantic_apply/py.typed
--rw-r--r--   0        0        0      821 2023-03-08 13:01:32.724858 pydantic_apply-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2791 1970-01-01 00:00:00.000000 pydantic_apply-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-07-16 12:42:19.876437 pydantic_apply-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2258 2023-07-16 12:42:19.876437 pydantic_apply-0.5.0/README.md
+-rw-r--r--   0        0        0       35 2023-07-16 12:42:19.876437 pydantic_apply-0.5.0/pydantic_apply/__init__.py
+-rw-r--r--   0        0        0     2426 2023-07-16 12:42:19.876437 pydantic_apply-0.5.0/pydantic_apply/_compat.py
+-rw-r--r--   0        0        0     4851 2023-07-16 12:42:19.876437 pydantic_apply-0.5.0/pydantic_apply/apply.py
+-rw-r--r--   0        0        0        0 2023-07-16 12:42:19.880437 pydantic_apply-0.5.0/pydantic_apply/py.typed
+-rw-r--r--   0        0        0      821 2023-07-16 12:42:19.880437 pydantic_apply-0.5.0/pydantic_apply/utils.py
+-rw-r--r--   0        0        0      849 2023-07-16 12:42:19.880437 pydantic_apply-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2961 1970-01-01 00:00:00.000000 pydantic_apply-0.5.0/PKG-INFO
```

### Comparing `pydantic_apply-0.1.5/LICENSE` & `pydantic_apply-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_apply-0.1.5/README.md` & `pydantic_apply-0.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # pydantic-apply
 
 ## Installation
 
 Just use `pip install pydantic-apply` to install the library.
 
+**Note:** `pydantic-apply` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+using `tox`.
+
 ## About
 
 With `pydantic-apply` you can apply changes to your pydantic models by using
 the `ApplyModelMixin` it provides:
 
 ```python
 import pydantic
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pydantic_apply-0.1.5/pydantic_apply/apply.py` & `pydantic_apply-0.5.0/pydantic_apply/apply.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,97 @@
 from typing import Any, Dict, Union
 
 import pydantic
 
+from pydantic_apply._compat import PydanticCompat
+from pydantic_apply.utils import is_pydantic_apply_annotation
+
 
 class ApplyModelMixin(pydantic.BaseModel):
     """Mixin to allow models to apply partly changes to their data."""
 
     def apply(
         self,
         changes: Union[pydantic.BaseModel, Dict[str, Any]],
     ) -> None:
         """Apply (partly) changes to the model data."""
 
+        self_compat = PydanticCompat(self)
+
         if isinstance(changes, pydantic.BaseModel):
-            # Convert model to dict. Do not use `changes.dict()` because it
+            # Convert model to dict. Do not use `changes.model_dump()` because it
             # would convert nested models to dicts, too. We don't want that yet.
             changes = {
                 key: value
                 for key, value
                 in changes.__dict__.items()
-                if key in changes.__fields_set__
+                if key in PydanticCompat(changes).__pydantic_fields_set__
             }
 
         # Prepare the changes
         prepared_changes = {}
-        for field_name, model_field in self.__fields__.items():
+        for field_name, model_field in self_compat.model_fields.items():
             # Make sure the field exists in the changes and
             # get changed field value
             if field_name in changes:
                 changed_field_value = changes[field_name]
             elif model_field.alias in changes:
                 changed_field_value = changes[model_field.alias]
             else:
                 # Field will not be changed
                 continue
 
             # Handle ApplyModelMixin fields:
             # Field type must be ApplyModelMixin....
-            if (
-                isinstance(model_field.type_, type)
-                and issubclass(model_field.type_, ApplyModelMixin)
-            ):
+            field_annotation = self_compat.get_model_field_info_annotation(model_field)
+
+            if is_pydantic_apply_annotation(field_annotation):
                 current_value = getattr(self, field_name)
                 if (
                     # ...AND current attribute value must be a instance
                     #        of ApplyModelMixin (not None)...
                     isinstance(current_value, ApplyModelMixin)
                     # ...AND type of changed value must allow patching.
                     and (
                         isinstance(changed_field_value, dict)
                         or isinstance(changed_field_value, pydantic.BaseModel)
                     )
                 ):
                     # When validation on assignment is enabled we need to
                     # copy the current value first. Otherwise, the validation
                     # might have issues, see below.
-                    if self.__config__.validate_assignment:
-                        current_value = current_value.copy()
+                    if self_compat.get_model_config_value("validate_assignment"):
+                        current_value = PydanticCompat(current_value).model_copy()
 
                     # ...then use `.apply(...)` on the current value to prepare changes
                     current_value.apply(changed_field_value)
                     prepared_changes[field_name] = current_value
                     continue
 
             # Default apply: Just set new value
             prepared_changes[field_name] = changed_field_value
 
         # Apply changes
-        had_validate_assignment = self.__config__.validate_assignment
+        had_validate_assignment = self_compat.get_model_config_value("validate_assignment")
         try:
-            if self.__config__.validate_assignment:
+            if had_validate_assignment:
                 # Disable validation on assignment so we can apply the whole set of
                 # changes without validation problems while the data changes. This
                 # is necessary as validators may depend on other fields. When we change
                 # the fields one by one, the validators may fail as the temporary
                 # combination of two values will not validate. But the validator might
                 # have passed when we would have had the chance to set both values.
-                self.__config__.validate_assignment = False
+                self_compat.set_model_config_value("validate_assignment", False)
 
                 # Run validation as if all changes were applied. We do this by creating
                 # a new (temporary) instance of the model class, just to run the
                 # validation.
                 changed_self = self.__class__(
                     **{
-                        **self.dict(),
+                        **self_compat.model_dump(),
                         **prepared_changes,
                     },
                 )
 
                 # Update the changes with the validated values we now have from the
                 # temporary instance.
                 prepared_changes = {
@@ -99,8 +103,8 @@
 
             for field_name, field_value in prepared_changes.items():
                 setattr(self, field_name, field_value)
 
         finally:
             # Ensure whatever happens here, the validate_assignment flag is reset
             # to its original value.
-            self.__config__.validate_assignment = had_validate_assignment
+            self_compat.set_model_config_value("validate_assignment", had_validate_assignment)
```

### Comparing `pydantic_apply-0.1.5/pyproject.toml` & `pydantic_apply-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "pydantic-apply"
-version = "0.1.5"
+version = "0.5.0"
 description = "Apply changes as patches to pydanic models."
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 repository = "https://github.com/team23/pydantic-apply"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pydantic = ">=1.9.0,<2.0.0"
+python = "^3.8"
+pydantic = ">=1.9.0,<2.1.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.1.2"
+pytest = ">=7.1.2,<8.0.0"
 isort = "^5.10.1"
-mypy = ">=0.971,<1.1"
-flake8 = "^5.0.4"
+mypy = ">=0.971,<2.0"
+flake8 = ">=5.0.4,<7.0.0"
 flake8-builtins = ">=1.5.3,<3.0.0"
-flake8-annotations = "^2.9.1"
+flake8-annotations = ">=2.9.1,<4.0.0"
 flake8-commas = "^2.1.0"
 flake8-isort = ">=4.2,<7.0"
 flake8-print = "^5.0.0"
 flake8-debugger = "^4.1.2"
 pytest-cov = ">=3,<5"
-tox = "^3.26.0"
+tox = ">=3.26,<5.0"
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 line_length = 115
 
 [build-system]
```

### Comparing `pydantic_apply-0.1.5/PKG-INFO` & `pydantic_apply-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,36 @@
 Metadata-Version: 2.1
 Name: pydantic-apply
-Version: 0.1.5
+Version: 0.5.0
 Summary: Apply changes as patches to pydanic models.
 Home-page: https://github.com/team23/pydantic-apply
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: pydantic (>=1.9.0,<2.1.0)
 Project-URL: Repository, https://github.com/team23/pydantic-apply
 Description-Content-Type: text/markdown
 
 # pydantic-apply
 
 ## Installation
 
 Just use `pip install pydantic-apply` to install the library.
 
+**Note:** `pydantic-apply` is compatible with `pydantic` versions `1.9`, `1.10` and even `2.0` (🥳) on
+Python `3.8`, `3.9`, `3.10` and `3.11`. This is also ensured running all tests on all those versions
+using `tox`.
+
 ## About
 
 With `pydantic-apply` you can apply changes to your pydantic models by using
 the `ApplyModelMixin` it provides:
 
 ```python
 import pydantic
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

