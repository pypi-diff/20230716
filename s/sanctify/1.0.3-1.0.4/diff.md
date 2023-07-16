# Comparing `tmp/sanctify-1.0.3.tar.gz` & `tmp/sanctify-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sanctify-1.0.3.tar", last modified: Wed Jul 12 20:57:47 2023, max compression
+gzip compressed data, was "sanctify-1.0.4.tar", last modified: Sun Jul 16 14:34:30 2023, max compression
```

## Comparing `sanctify-1.0.3.tar` & `sanctify-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-12 20:57:47.059981 sanctify-1.0.3/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.3/LICENSE.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-12 20:57:47.059734 sanctify-1.0.3/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9411 2023-07-12 20:56:28.000000 sanctify-1.0.3/README.md
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1552 2023-07-12 20:57:01.000000 sanctify-1.0.3/pyproject.toml
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-12 20:57:47.058703 sanctify-1.0.3/sanctify/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      833 2023-07-12 20:57:32.000000 sanctify-1.0.3/sanctify/__init__.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7629 2023-07-12 20:53:57.000000 sanctify-1.0.3/sanctify/cleanser.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2613 2023-07-12 20:53:57.000000 sanctify-1.0.3/sanctify/constants.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.3/sanctify/exception.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12024 2023-07-12 20:57:32.000000 sanctify-1.0.3/sanctify/processor.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8744 2023-07-12 20:53:57.000000 sanctify-1.0.3/sanctify/transformer.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3417 2023-07-12 20:53:57.000000 sanctify-1.0.3/sanctify/utils.py
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9129 2023-07-12 20:57:32.000000 sanctify-1.0.3/sanctify/validator.py
-drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-12 20:57:47.059471 sanctify-1.0.3/sanctify.egg-info/
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-12 20:57:47.000000 sanctify-1.0.3/sanctify.egg-info/PKG-INFO
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-12 20:57:47.000000 sanctify-1.0.3/sanctify.egg-info/SOURCES.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-12 20:57:47.000000 sanctify-1.0.3/sanctify.egg-info/dependency_links.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-12 20:57:47.000000 sanctify-1.0.3/sanctify.egg-info/top_level.txt
--rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-12 20:57:47.060037 sanctify-1.0.3/setup.cfg
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-16 14:34:30.942379 sanctify-1.0.4/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1068 2023-07-07 16:45:27.000000 sanctify-1.0.4/LICENSE.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-16 14:34:30.942130 sanctify-1.0.4/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9411 2023-07-12 20:56:28.000000 sanctify-1.0.4/README.md
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     1552 2023-07-16 14:34:24.000000 sanctify-1.0.4/pyproject.toml
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-16 14:34:30.941338 sanctify-1.0.4/sanctify/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      833 2023-07-16 14:31:35.000000 sanctify-1.0.4/sanctify/__init__.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     7629 2023-07-12 20:53:57.000000 sanctify-1.0.4/sanctify/cleanser.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     2613 2023-07-12 20:53:57.000000 sanctify-1.0.4/sanctify/constants.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      221 2023-07-07 16:45:27.000000 sanctify-1.0.4/sanctify/exception.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    12233 2023-07-16 14:31:36.000000 sanctify-1.0.4/sanctify/processor.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     8744 2023-07-12 20:53:57.000000 sanctify-1.0.4/sanctify/transformer.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     3417 2023-07-12 20:53:57.000000 sanctify-1.0.4/sanctify/utils.py
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)     9745 2023-07-16 14:31:36.000000 sanctify-1.0.4/sanctify/validator.py
+drwxr-xr-x   0 avijeetdiwaker   (503) staff       (20)        0 2023-07-16 14:34:30.941949 sanctify-1.0.4/sanctify.egg-info/
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)    10026 2023-07-16 14:34:30.000000 sanctify-1.0.4/sanctify.egg-info/PKG-INFO
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)      336 2023-07-16 14:34:30.000000 sanctify-1.0.4/sanctify.egg-info/SOURCES.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        1 2023-07-16 14:34:30.000000 sanctify-1.0.4/sanctify.egg-info/dependency_links.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)        9 2023-07-16 14:34:30.000000 sanctify-1.0.4/sanctify.egg-info/top_level.txt
+-rw-r--r--   0 avijeetdiwaker   (503) staff       (20)       38 2023-07-16 14:34:30.942443 sanctify-1.0.4/setup.cfg
```

### Comparing `sanctify-1.0.3/LICENSE.txt` & `sanctify-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.3/PKG-INFO` & `sanctify-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.3
+Version: 1.0.4
 Summary: Allowed config based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sanctify-1.0.3/README.md` & `sanctify-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.3/pyproject.toml` & `sanctify-1.0.4/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
 [tool.pytest.ini_options]
 log_cli=true
 log_cli_level='DEBUG'
 
 [project]
 name = "sanctify"
-version = "1.0.3"
+version = "1.0.4"
 authors = [{name = "Avijeet Diwaker", email = "avijeetdiwaker@gmail.com"}]
 description = "Allowed config based cleansing and validations for a given pandas dataframe"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
```

### Comparing `sanctify-1.0.3/sanctify/__init__.py` & `sanctify-1.0.4/sanctify/__init__.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.3/sanctify/cleanser.py` & `sanctify-1.0.4/sanctify/cleanser.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.3/sanctify/constants.py` & `sanctify-1.0.4/sanctify/constants.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.3/sanctify/processor.py` & `sanctify-1.0.4/sanctify/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,35 +183,40 @@
 
     Returns:
         pd.Series: Series containing the modified value and error message (if any).
     """
     func_value = value
     error_message = None
 
-    for function in functions:
-        func = function
-        kwargs = {}
-
-        if isinstance(function, tuple):
-            func = function[0]
-            kwargs = function[1]
-
-        logger.debug(f"Running {func.__name__ = } with {value = } | {kwargs = }")
-
-        try:
-            func_value = func(func_value, **kwargs)
-
-        except Exception as err:
-            logger.error(f"FAILED: {func.__name__ = } with {value = } | {kwargs = } | {(str(err)) = }")
-            logger.error(f"{err = }")
-            error_message = f"{col_name} : {str(err)} | {func_value}"
-            func_value = None
-            break
+    if not func_value:  # All possible absent value cases
+        error_message = f"{col_name} is required"
+        func_value = None
+
+    else:
+        for function in functions:
+            func = function
+            kwargs = {}
+
+            if isinstance(function, tuple):
+                func = function[0]
+                kwargs = function[1]
+
+            logger.debug(f"Running {func.__name__ = } with {value = } | {kwargs = }")
+
+            try:
+                func_value = func(func_value, **kwargs)
+
+            except Exception as err:
+                logger.error(f"FAILED: {func.__name__ = } with {value = } | {kwargs = } | {(str(err)) = }")
+                logger.error(f"{err = }")
+                error_message = f"{col_name} : {str(err)} | {func_value}"
+                func_value = None
+                break
 
-        logger.debug(f"Result: {func.__name__ = } with {value = } | {kwargs = } | {func_value = }")
+            logger.debug(f"Result: {func.__name__ = } with {value = } | {kwargs = } | {func_value = }")
 
     # Return the modified value and error message (if any)
     return pd.Series(
         [func_value, error_message],
         index=[DefaultColumns.VALUE_PLACEHOLDER.value, DefaultColumns.ERROR.value],
     )
```

### Comparing `sanctify-1.0.3/sanctify/transformer.py` & `sanctify-1.0.4/sanctify/transformer.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.3/sanctify/utils.py` & `sanctify-1.0.4/sanctify/utils.py`

 * *Files identical despite different names*

### Comparing `sanctify-1.0.3/sanctify/validator.py` & `sanctify-1.0.4/sanctify/validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from sanctify.constants import ComparisonOperations
 from sanctify.exception import ValidationError
 from sanctify.transformer import Transformer
 from sanctify.utils import calculate_age, match_comparision_operation
 
 
 class Validator:
+    SSN_VALIDATION_ERROR_MSG = "Should be 4 digits"
+
     @staticmethod
     def validate_comparison_operations(value: Any, comparison_operations: dict[str: int | None]) -> Any | Exception:
         """
         Validate a value against a set of comparison operations.
 
         Args:
             value: The value to be validated.
@@ -34,50 +36,74 @@
         else:
             raise ValidationError(f"Comparison Failed for {comparison_operations = }")
 
     @staticmethod
     def validate_age(
         value: str | int,
         date_order_tuple: tuple,
-        comparison_operations: dict[str: int | None] = None,
+        comparison_operations: dict[str:int],
     ) -> str | int | Exception:
         """
         Validate the age based on comparison operations.
 
         Args:
-            value: The value representing the date of birth.
+            value: The value representing a date.
             date_order_tuple: A tuple specifying the order of year, month, and day in the date.
             comparison_operations: A dictionary of comparison operations and their operands.
 
         Returns:
             The validated age value if all comparison operations pass.
 
         Raises:
             ValidationError: If any comparison operation fails.
         """
         parsed_datetime = Transformer.parse_date_from_string(
             value=value, date_order_tuple=date_order_tuple, return_datetime=True
         )
         age = calculate_age(date_of_birth=parsed_datetime.date())
 
-        if isinstance(comparison_operations, dict):
+        # Raises err on validation failure
+        _ = Validator.validate_comparison_operations(value=age, comparison_operations=comparison_operations)
+
+        return str(parsed_datetime.date())
+
+    @staticmethod
+    def validate_date_of_birth(
+        value: str | int,
+        date_order_tuple: tuple,
+    ) -> str | int | Exception:
+        """
+        Validate the age based on comparison operations.
+
+        Args:
+            value: The value representing the date of birth.
+            date_order_tuple: A tuple specifying the order of year, month, and day in the date.
+
+        Returns:
+            The validated date of birth date if it is valid
+
+        Raises:
+            ValidationError: If any comparison operation fails.
+        """
+        parsed_datetime = Transformer.parse_date_from_string(
+            value=value, date_order_tuple=date_order_tuple, return_datetime=True
+        )
+        age = calculate_age(date_of_birth=parsed_datetime.date())
+
+        try:
             # Raises err on validation failure
-            _ = Validator.validate_comparison_operations(value=age, comparison_operations=comparison_operations)
-        else:
-            try:
-                # Raises err on validation failure
-                _ = Validator.validate_comparison_operations(
-                    value=age,
-                    comparison_operations={
-                        ComparisonOperations.GREATER_THAN_EQUALS.value: 18,
-                        ComparisonOperations.LESS_THAN_EQUALS.value: 100,
-                    },
-                )
-            except ValidationError:
-                raise ValidationError("Age should be >=18 and <=100")
+            _ = Validator.validate_comparison_operations(
+                value=age,
+                comparison_operations={
+                    ComparisonOperations.GREATER_THAN_EQUALS.value: 18,
+                    ComparisonOperations.LESS_THAN_EQUALS.value: 100,
+                },
+            )
+        except ValidationError:
+            raise ValidationError("Age should be >=18 and <=100")
 
         return value
 
     @staticmethod
     def validate_due_date(
         value: str | int,
         date_order_tuple: tuple,
@@ -88,15 +114,15 @@
 
         Args:
             value: The value representing the date of birth.
             date_order_tuple: A tuple specifying the order of year, month, and day in the date.
             comparison_operations: A dictionary of comparison operations and their operands.
 
         Returns:
-            The validated age value if all comparison operations pass.
+            The validated due date if it is valid
 
         Raises:
             ValidationError: If any comparison operation fails.
         """
         parsed_datetime = Transformer.parse_date_from_string(
             value=value, date_order_tuple=date_order_tuple, return_datetime=True
         )
@@ -182,23 +208,18 @@
         Raises:
             ValidationError: If the SSN is not valid.
         """
         # Extract the ssn
         digits_only = Transformer.extract_digits_from_string(value=value)
 
         # Validate based on the number of digits
-        match len(digits_only):
-            case 12:
-                return digits_only[-4:]
-
-            case 4:
-                return digits_only
-
-            case _:
-                raise ValidationError("Should be either 12 or 4 digits")
+        if len(digits_only) < 4:
+            raise ValidationError(Validator.SSN_VALIDATION_ERROR_MSG)
+        else:
+            return digits_only[-4:]
 
     @staticmethod
     def validate_zip_code(value: str):
         """
         Validate a zip code.
 
         Args:
```

### Comparing `sanctify-1.0.3/sanctify.egg-info/PKG-INFO` & `sanctify-1.0.4/sanctify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sanctify
-Version: 1.0.3
+Version: 1.0.4
 Summary: Allowed config based cleansing and validations for a given pandas dataframe
 Author-email: Avijeet Diwaker <avijeetdiwaker@gmail.com>
 Project-URL: Homepage, https://github.com/skit-ai/sanctify
 Project-URL: Bug Tracker, https://github.com/skit-ai/sanctify/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

