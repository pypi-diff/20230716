# Comparing `tmp/django-expanded-test-cases-0.4.0.tar.gz` & `tmp/django-expanded-test-cases-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-expanded-test-cases-0.4.0.tar", last modified: Mon Jun 12 20:22:26 2023, max compression
+gzip compressed data, was "django-expanded-test-cases-0.5.0.tar", last modified: Sun Jul 16 11:27:32 2023, max compression
```

## Comparing `django-expanded-test-cases-0.4.0.tar` & `django-expanded-test-cases-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,47 @@
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-06-03 17:01:28.000000 django-expanded-test-cases-0.4.0/LICENSE
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/MANIFEST.in
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/PKG-INFO
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2022-06-13 15:23:33.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10124 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/constants.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      325 2022-06-24 03:18:02.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    37636 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/core_mixin.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    29825 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/response_mixin.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/templates/
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/templates/django_expanded_test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1376 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    16722 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/base_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    57283 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/integration_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     7790 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/live_server_test_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1093 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_urls.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5168 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/PKG-INFO
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1116 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/SOURCES.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/dependency_links.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/requires.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       33 2023-06-12 20:22:26.000000 django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/top_level.txt
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1781 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/pyproject.toml
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/readme.md
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/setup.cfg
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/tests/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-01 21:20:22.000000 django-expanded-test-cases-0.4.0/tests/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      198 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/apps.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      360 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/asgi.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3527 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/settings.py
-drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-06-12 20:22:26.726703 django-expanded-test-cases-0.4.0/tests/test_cases/
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2023-03-01 21:20:22.000000 django-expanded-test-cases-0.4.0/tests/test_cases/__init__.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   100821 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/tests/test_cases/test_base_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   300318 2023-06-12 20:21:48.000000 django-expanded-test-cases-0.4.0/tests/test_cases/test_integration_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2230 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/test_cases/test_live_server_case.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/urls.py
--rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3964 2023-06-12 17:34:53.000000 django-expanded-test-cases-0.4.0/tests/views.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.357761 django-expanded-test-cases-0.5.0/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1074 2022-08-22 15:23:55.000000 django-expanded-test-cases-0.5.0/LICENSE
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       91 2023-03-21 17:27:50.000000 django-expanded-test-cases-0.5.0/MANIFEST.in
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5246 2023-07-16 11:27:32.357761 django-expanded-test-cases-0.5.0/PKG-INFO
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.353760 django-expanded-test-cases-0.5.0/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      181 2022-08-22 15:23:55.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    10690 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/constants.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.353760 django-expanded-test-cases-0.5.0/django_expanded_test_cases/mixins/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      325 2022-08-22 15:23:55.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/mixins/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    44963 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/mixins/core_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    18314 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/mixins/live_server_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    34790 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/mixins/response_mixin.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.353760 django-expanded-test-cases-0.5.0/django_expanded_test_cases/templates/
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.353760 django-expanded-test-cases-0.5.0/django_expanded_test_cases/templates/django_expanded_test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      528 2023-03-21 17:27:50.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.357761 django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2540 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    16722 2023-07-03 13:16:53.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/base_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5140 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/channels_live_server_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)    62625 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/integration_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5868 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/live_server_test_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1471 2023-07-07 02:49:58.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_urls.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.353760 django-expanded-test-cases-0.5.0/django_expanded_test_cases.egg-info/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5246 2023-07-16 11:27:32.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases.egg-info/PKG-INFO
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1369 2023-07-16 11:27:32.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases.egg-info/SOURCES.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        1 2023-07-16 11:27:32.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases.egg-info/dependency_links.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      112 2023-07-16 11:27:32.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases.egg-info/requires.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)       33 2023-07-16 11:27:32.000000 django-expanded-test-cases-0.5.0/django_expanded_test_cases.egg-info/top_level.txt
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1849 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/pyproject.toml
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2335 2023-07-03 13:16:53.000000 django-expanded-test-cases-0.5.0/readme.md
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     1192 2023-07-16 11:27:32.357761 django-expanded-test-cases-0.5.0/setup.cfg
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.357761 django-expanded-test-cases-0.5.0/tests/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-08-22 15:23:55.000000 django-expanded-test-cases-0.5.0/tests/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      198 2023-03-21 17:27:50.000000 django-expanded-test-cases-0.5.0/tests/apps.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      566 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/tests/asgi.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.357761 django-expanded-test-cases-0.5.0/tests/mock_pages/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/tests/mock_pages/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     3536 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/tests/settings.py
+drwxrwxr-x   0 brodriguez  (1000) brodriguez  (1000)        0 2023-07-16 11:27:32.357761 django-expanded-test-cases-0.5.0/tests/test_cases/
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)        0 2022-08-22 15:23:55.000000 django-expanded-test-cases-0.5.0/tests/test_cases/__init__.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   127689 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/tests/test_cases/test_base_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2609 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/tests/test_cases/test_channels_live_server_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   336836 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/tests/test_cases/test_integration_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     2484 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/tests/test_cases/test_live_server_case.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)   122615 2023-07-16 11:23:42.000000 django-expanded-test-cases-0.5.0/tests/test_cases/universal_live_test_mixin.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)      316 2023-03-21 17:27:50.000000 django-expanded-test-cases-0.5.0/tests/urls.py
+-rw-rw-r--   0 brodriguez  (1000) brodriguez  (1000)     5443 2023-07-07 02:49:58.000000 django-expanded-test-cases-0.5.0/tests/views.py
```

### Comparing `django-expanded-test-cases-0.4.0/LICENSE` & `django-expanded-test-cases-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.4.0/PKG-INFO` & `django-expanded-test-cases-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.4.0
+Version: 0.5.0
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
         
@@ -34,14 +34,16 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases/constants.py` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -165,21 +165,32 @@
 
 # Indicates whether the additional debug information should be output.
 ETC_DEBUG_PRINT = bool(getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_DEBUG_PRINT',
     True,
 ))
-# Indicates whether partial matches are allowed for messages.
+# Indicates whether partial matches are allowed for site title assertions.
+# IE: Will pass as long as provided text appears as a subsection of the full site title.
+# Defaults to needing exact match.
+ETC_ALLOW_TITLE_PARTIALS = bool(getattr(
+    settings,
+    'DJANGO_EXPANDED_TESTCASES_ALLOW_TITLE_PARTIALS',
+    False,
+))
+# Indicates whether partial matches are allowed for message assertions.
+# IE: Will pass as long as provided text appears as a subsection of one or more messages.
+# Defaults to needing exact match.
 ETC_ALLOW_MESSAGE_PARTIALS = bool(getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_ALLOW_MESSAGE_PARTIALS',
-    True,
+    False,
 ))
 # Indicates whether tests fail when there are messages in the response that were not explicitly tested for.
+# Aka, when doing ANY message assertion, if this is True, then ALL messages in response need to be checked.
 ETC_MATCH_ALL_CONTEXT_MESSAGES = bool(getattr(
     settings,
     'DJANGO_EXPANDED_TESTCASES_MATCH_ALL_CONTEXT_MESSAGES',
     False,
 ))
```

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/core_mixin.py` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases/mixins/core_mixin.py`

 * *Files 20% similar despite different names*

```diff
@@ -89,14 +89,16 @@
         """
         # Check user debug_print option.
         if debug_print is not None:
             cls._debug_print_bool = bool(debug_print)
         else:
             cls._debug_print_bool = ETC_DEBUG_PRINT
 
+        cls._site_root_url = None
+
     @classmethod
     def set_up_test_data(cls, extra_usergen_kwargs=None):
         """
         Acts as the equivalent of the UnitTesting "setUpTestData()" function.
 
         However, since this is not inheriting from a given TestCase, calling the literal function
         here would override instead.
@@ -259,15 +261,15 @@
             print(back, end='')
             print(style, end='')
             print(*args, **kwargs, end='')
             print(ETC_OUTPUT_RESET_COLOR)
 
     # region Custom Assertions
 
-    def assertText(self, expected_text, actual_text, strip=True):
+    def assertText(self, expected_text, actual_text, compare_index=None, strip=True):
         """Wrapper for assertEqual(), that prints full values to console on mismatch.
 
         :param expected_text: Expected text value to check against.
         :param actual_text: Actual text value to compare.
         :param strip: Bool indicating if outer whitespace should be stripped. Defaults to True.
         """
         # Enforce str type.
@@ -275,14 +277,20 @@
         actual_text = str(actual_text)
 
         # Handle optional cleaning params.
         if strip:
             expected_text = expected_text.strip()
             actual_text = actual_text.strip()
 
+        # Sanitize compare_index, used for startsWith() and endsWith() versions.
+        if compare_index is not None:
+            compare_index = int(compare_index)
+            if compare_index == 0:
+                compare_index = None
+
         # Attempt assertion.
         try:
             self.assertEqual(expected_text, actual_text)
         except AssertionError as err:
             # Assertion failed. Provide debug output.
 
             # Loop through to calculate color output differences.
@@ -301,29 +309,52 @@
             if len(split_actual) > len(split_expected):
                 max_lines = len(split_actual)
             else:
                 max_lines = len(split_expected)
 
             formatted_expected_output = ''
             formatted_actual_output = ''
+            total_actual_count_thus_far = 0
+            total_actual_index = None
+            actual_text_total_len = len(actual_text)
+            if compare_index is not None:
+                if compare_index > 0:
+                    # Is positive, so starstWith().
+                    total_actual_index = 0
+                else:
+                    # Is negative, so endsWith().
+                    total_actual_index = actual_text_total_len
+
+            # Loop through all lines.
             for line_index in range(max_lines):
+
+                # Check if expected/actual each have lines up to this index.
                 try:
                     curr_expected_line = split_expected[line_index]
                     if append_newline:
                         curr_expected_line = '\n{0}'.format(curr_expected_line)
                 except IndexError:
                     curr_expected_line = None
                 try:
                     curr_actual_line = split_actual[line_index]
                     if append_newline:
                         curr_actual_line = '\n{0}'.format(curr_actual_line)
                 except IndexError:
                     curr_actual_line = None
                 append_newline = False
 
+                # Handle if compare_index value is provided.
+                if compare_index is not None and line_index > 0:
+                    if compare_index > 0:
+                        # Is positive, so startsWith. Count from start of text.
+                        total_actual_index = total_actual_count_thus_far
+                    else:
+                        # Is negative, so endsWith(). Count from end of text.
+                        total_actual_index = actual_text_total_len - total_actual_count_thus_far
+
                 if curr_expected_line == curr_actual_line:
                     # Line is full match and correct.
                     curr_expected_line = '{0}{1}{2}\n'.format(ETC_OUTPUT_EXPECTED_MATCH_COLOR, curr_expected_line, ETC_OUTPUT_RESET_COLOR)
                     curr_actual_line = '{0}{1}{2}\n'.format(ETC_OUTPUT_ACTUALS_MATCH_COLOR, curr_actual_line, ETC_OUTPUT_RESET_COLOR)
                 elif curr_expected_line is None:
                     # "Actual" output is longer than "expected" output. Impossible to match current line.
                     curr_expected_line = ''
@@ -350,33 +381,62 @@
 
                     # Check each character and determine where non-match happens.
                     curr_expected_color = ETC_OUTPUT_RESET_COLOR
                     curr_actual_color = ETC_OUTPUT_RESET_COLOR
                     curr_expected_char_line = ''
                     curr_actual_char_line = ''
                     for char_index in range(max_chars):
+
+                        # Handle if starstWith() or endsWith().
+                        do_char_compare = True
+                        if compare_index is not None:
+                            if compare_index > 0:
+                                # Is positive, so startsWith()
+                                total_actual_index += 1
+
+                                # Skip comparison if actual_index is past compare_index.
+                                if total_actual_index > compare_index:
+                                    do_char_compare = False
+                            else:
+                                # Is negative, so endsWith().
+                                total_actual_index -= 1
+
+                                # Skip comparison if actual_index is before compare_index.
+                                if total_actual_index > - compare_index:
+                                    do_char_compare = False
+
                         # Grab current character.
                         try:
                             expected_char = curr_expected_line[char_index]
                         except IndexError:
                             expected_char = ''
                         try:
                             actual_char = curr_actual_line[char_index]
                         except IndexError:
                             actual_char = ''
 
                         # Format based on match.
-                        if expected_char == actual_char:
+                        if not do_char_compare:
+                            # Skip comparison, for either startsWith() or endsWith() assertions.
+                            if curr_expected_color != ETC_OUTPUT_RESET_COLOR:
+                                curr_expected_color = ETC_OUTPUT_RESET_COLOR
+                                curr_expected_char_line += curr_expected_color
+                            if curr_actual_color != ETC_OUTPUT_RESET_COLOR:
+                                curr_actual_color = ETC_OUTPUT_RESET_COLOR
+                                curr_actual_char_line += curr_actual_color
+
+                        elif expected_char == actual_char:
                             # Match.
                             if curr_expected_color != ETC_OUTPUT_EXPECTED_MATCH_COLOR:
                                 curr_expected_color = ETC_OUTPUT_EXPECTED_MATCH_COLOR
                                 curr_expected_char_line += curr_expected_color
                             if curr_actual_color != ETC_OUTPUT_ACTUALS_MATCH_COLOR:
                                 curr_actual_color = ETC_OUTPUT_ACTUALS_MATCH_COLOR
                                 curr_actual_char_line += curr_actual_color
+
                         else:
                             # Non-match.
                             if curr_expected_color != ETC_OUTPUT_EXPECTED_ERROR_COLOR:
                                 curr_expected_color = ETC_OUTPUT_EXPECTED_ERROR_COLOR
                                 curr_expected_char_line += curr_expected_color
                             if curr_actual_color != ETC_OUTPUT_ACTUALS_ERROR_COLOR:
                                 curr_actual_color = ETC_OUTPUT_ACTUALS_ERROR_COLOR
@@ -391,55 +451,105 @@
                     formatted_actual_output += curr_actual_char_line
                     continue
 
                 # Update output strings.
                 formatted_expected_output += curr_expected_line
                 formatted_actual_output += curr_actual_line
 
+                # Update total actual length.
+                total_actual_count_thus_far += len(curr_actual_line)
+
             # Finally print actual debug output.
             self._debug_print('')
             self._debug_print('')
             self._debug_print('EXPECTED:', fore=ETC_OUTPUT_EXPECTED_MATCH_COLOR)
             self._debug_print(formatted_expected_output)
             self._debug_print('')
             self._debug_print('')
             self._debug_print('ACTUAL:', fore=ETC_OUTPUT_ACTUALS_MATCH_COLOR)
             self._debug_print(formatted_actual_output)
             self._debug_print('')
             self._debug_print('')
 
             # Raise original error.
-            raise AssertionError(err) from err
+            raise err
+
+    def assertTextStartsWith(self, expected_text, actual_text, strip=True):
+        """Modiefied wrapper for assertEqual(), that prints full values to console on mismatch.
+
+        Considered a pass if entire string of "expected_text" is at the beginning of "actual_text" variable.
+        """
+        # Enforce str type.
+        expected_text = str(expected_text)
+        actual_text = str(actual_text)
+
+        # Handle optional cleaning params.
+        if strip:
+            expected_text = expected_text.strip()
+            actual_text = actual_text.strip()
+
+        # Check if start matches.
+        if not str(actual_text).startswith(expected_text):
+            # Failed to match. Call original assertText for output handling.
+            text_length = len(expected_text)
+            return self.assertText(expected_text, actual_text, text_length, strip=strip)
+
+        # Passed.
+        return True
+
+    def assertTextEndsWith(self, expected_text, actual_text, strip=True):
+        """Modified wrapper for assertEqual(), that prints full values to console on mismatch.
+
+        Considered a pass if entire string of "expected_text" is at the beginning of "actual_text" variable.
+        """
+        # Enforce str type.
+        expected_text = str(expected_text)
+        actual_text = str(actual_text)
+
+        # Handle optional cleaning params.
+        if strip:
+            expected_text = expected_text.strip()
+            actual_text = actual_text.strip()
+
+        # Check if ending matches.
+        if not str(actual_text).endswith(expected_text):
+            # Failed to match. Call original assertText for output handling.
+            text_length = len(expected_text)
+            return self.assertText(expected_text, actual_text, compare_index=-text_length, strip=strip)
+
+        # Passed.
+        return True
 
     # endregion Custom Assertions
 
     # region User Management Functions
 
     def get_user(self, user, password=ETC_DEFAULT_USER_PASSWORD, extra_usergen_kwargs=None):
         """Returns user matching provided value.
 
         :param user: User model, or corresponding user identifier, to use.
         :param password: Password str to assign to user.
         :param extra_usergen_kwargs: Optional extra kwargs to pass into the get_user_model().objects.create_user()
                                      function.
         :return: User object
         """
+
         # Check if instance is User model.
         if isinstance(user, get_user_model()):
             # Already User model. This is fine.
             pass
 
         # Handle all "special cases" for testing logic.
-        elif user == ETC_DEFAULT_SUPER_USER_IDENTIFIER:
+        elif ETC_AUTO_GENERATE_USERS is True and user == ETC_DEFAULT_SUPER_USER_IDENTIFIER:
             user = self.test_superuser
-        elif user == ETC_DEFAULT_ADMIN_USER_IDENTIFIER:
+        elif ETC_AUTO_GENERATE_USERS is True and user == ETC_DEFAULT_ADMIN_USER_IDENTIFIER:
             user = self.test_admin
-        elif user == ETC_DEFAULT_INACTIVE_USER_IDENTIFIER:
+        elif ETC_AUTO_GENERATE_USERS is True and user == ETC_DEFAULT_INACTIVE_USER_IDENTIFIER:
             user = self.test_inactive_user
-        elif user == ETC_DEFAULT_STANDARD_USER_IDENTIFIER:
+        elif ETC_AUTO_GENERATE_USERS is True and user == ETC_DEFAULT_STANDARD_USER_IDENTIFIER:
             user = self.test_user
         else:
             # Is not User model. Get or create.
 
             # First validate optional extra kwargs.
             if extra_usergen_kwargs is None:
                 extra_usergen_kwargs = {}
@@ -468,23 +578,23 @@
                 password = ETC_DEFAULT_USER_PASSWORD
             user.set_password(password)
             user.unhashed_password = password
             user.save()
 
         return user
 
-    def add_user_permission(self, user_permission, user=ETC_DEFAULT_STANDARD_USER_IDENTIFIER):
+    def add_user_permission(self, user_permission, user=None):
         """Adds Permission to given user.
 
         :param user_permission: Permission to add.
         :param user: User to add Permission to. If not provided, defaults to test_user model.
         :return: Updated user object.
         """
         # Django imports here to avoid situational "Apps aren't loaded yet" error.
-        from django.contrib.auth.models import Permission
+        from django.contrib.auth.models import AnonymousUser, Permission
 
         # Check if instance is a Permission model.
         if isinstance(user_permission, Permission):
             # Already Permission model. This is fine.
             permission = user_permission
 
         else:
@@ -496,29 +606,41 @@
                 # Failed to get by codename. Attempt again with name.
                 try:
                     permission = Permission.objects.get(name=user_permission)
                 except Permission.DoesNotExist as pde:
                     raise ValueError('Failed to find permission of "{0}".'.format(user_permission)) from pde
 
         # If we made it this far, then valid Permission was found. Apply to user.
-        user = self.get_user(user)
+        # But first determine what user we're applying to.
+        if user is not None:
+            # Actual user arg provided to function. Use that.
+            user = self.get_user(user)
+        elif self.user and not isinstance(self.user, AnonymousUser):
+            # No arg provided to function. Fall back to class user, if provided.
+            user = self.get_user(self.user)
+        else:
+            # No arg provided to function AND no class user defined.
+            # Resort to "default standard user" as final fallback.
+            user = self.get_user(ETC_DEFAULT_STANDARD_USER_IDENTIFIER)
+
+        # Actually add permission.
         user.user_permissions.add(permission)
 
         # Return user object in case user wants to run additional checks.
         return user
 
-    def add_user_group(self, user_group, user=ETC_DEFAULT_STANDARD_USER_IDENTIFIER):
+    def add_user_group(self, user_group, user=None):
         """Adds Group to given user.
 
         :param user_group: Group to add.
         :param user: User to add Group to. If not provided, defaults to test_user model.
         :return: Updated user object.
         """
         # Django imports here to avoid situational "Apps aren't loaded yet" error.
-        from django.contrib.auth.models import Group
+        from django.contrib.auth.models import AnonymousUser, Group
 
         # Check if instance is a Group model.
         if isinstance(user_group, Group):
             # Already Group model. This is fine.
             group = user_group
 
         else:
@@ -526,15 +648,27 @@
             user_group = str(user_group)
             try:
                 group = Group.objects.get(name=user_group)
             except Group.DoesNotExist as gde:
                 raise ValueError('Failed to find Group of "{0}".'.format(user_group)) from gde
 
         # If we made it this far, then valid Group was found. Apply to user.
-        user = self.get_user(user)
+        # But first determine what user we're applying to.
+        if user is not None:
+            # Actual user arg provided to function. Use that.
+            user = self.get_user(user)
+        elif self.user and not isinstance(self.user, AnonymousUser):
+            # No arg provided to function. Fall back to class user, if provided.
+            user = self.get_user(self.user)
+        else:
+            # No arg provided to function AND no class user defined.
+            # Resort to "default standard user" as final fallback.
+            user = self.get_user(ETC_DEFAULT_STANDARD_USER_IDENTIFIER)
+
+        # Actually add groups.
         user.groups.add(group)
 
         # Return user object in case user wants to run additional checks.
         return user
 
     # endregion User Management Functions
 
@@ -557,17 +691,34 @@
         value_error = 'No url provided. Please provide the "url" param or set the "self.url" class value.'
         if url is None:
             raise ValueError(value_error)
         url = str(url).strip()
         if len(url) == 0:
             raise ValueError(value_error)
 
+        # If kwargs were provided, trim final slash if url ends with such.
+        while url.endswith('/'):
+            url = url[:-1]
+
+        # Trim final ? if url ends with such.
+        while url.endswith('?'):
+            url = url[:-1]
+
+        # If kwargs were provided, trim final slash if url ends with such.
+        # Makes sure handling is consistent, even if ordering of ? and / are weird.
+        while url.endswith('/'):
+            url = url[:-1]
+
         # Finally, generate actual url and return.
         get_params = urlencode(kwargs)
-        get_url = url + ('' if get_params == '' else '?' + get_params)
+        get_url = '{0}/{1}'.format(
+            url,
+            ('' if get_params == '' else '?' + get_params)
+        )
+
         self._debug_print('URL: {0}'.format(get_url))
         return get_url
 
     def standardize_characters(self, value):
         """Standardizes various characters in provided str.
 
         Helps make testing easier.
@@ -803,15 +954,32 @@
     # endregion Class Functions
 
     # region Properties
 
     @property
     def site_root_url(self):
         """"""
-        return self._site_root_url
+        if (
+            self._site_root_url is None
+            or self._site_root_url == ''
+        ):
+            # No site root populated. Check for "live_server_url", which is auto-populated for Selenium tests.
+            if (
+                hasattr(self, 'live_server_url')
+                and self.live_server_url is not None
+                and self.live_server_url != ''
+            ):
+                return self.live_server_url
+
+            # Failed to get auto-populated Selenium url.
+            # Return default (will apply in most cases).
+            return '127.0.0.1'
+        else:
+            # Site root is populated. Return value.
+            return self._site_root_url
 
     @site_root_url.setter
     def site_root_url(self, value):
         """"""
         # Validate.
         value = str(value).strip()
         while len(value) > 0 and value[-1] == '/':
```

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases/mixins/response_mixin.py` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases/mixins/response_mixin.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 """
 Core testing logic that pertains to handling Response objects.
 """
 
 # System Imports.
 import logging, re
+from urllib.parse import parse_qs
 
 # Third-Party Imports.
 from bs4 import BeautifulSoup
+from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.http.response import HttpResponseBase
 
 # Internal Imports.
 from . import CoreTestCaseMixin
+from django.urls import reverse
+from django.urls.exceptions import NoReverseMatch
 from django_expanded_test_cases.constants import (
     ETC_OUTPUT_ERROR_COLOR,
     ETC_RESPONSE_DEBUG_CONTENT_COLOR,
     ETC_RESPONSE_DEBUG_HEADER_COLOR,
     ETC_RESPONSE_DEBUG_CONTEXT_COLOR,
     ETC_RESPONSE_DEBUG_MESSAGE_COLOR,
     ETC_RESPONSE_DEBUG_SESSION_COLOR,
+    ETC_RESPONSE_DEBUG_URL_COLOR,
     ETC_RESPONSE_DEBUG_FORM_COLOR,
     ETC_RESPONSE_DEBUG_USER_INFO_COLOR,
     ETC_OUTPUT_EMPHASIS_COLOR,
 )
 
 
 # Initialize logging.
@@ -44,14 +49,26 @@
                             Param overrides setting value if both param and setting are set.
         """
         # Run parent setup logic.
         super().set_up_class(debug_print=debug_print)
 
     # region Debug Output Functions
 
+    def show_debug_url(self, url):
+        """Prints debug url output."""
+
+        # Ensure url is in consistent format.
+        url = self.standardize_url(url, append_root=True)
+        message = 'Attempting to access url "{0}"'.format(url)
+
+        self._debug_print('\n\n')
+        self._debug_print('{0}'.format('-' * len(message)), fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
+        self._debug_print(message, fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
+        self._debug_print('{0}'.format('-' * len(message)), fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
+
     def show_debug_content(self, response_content):
         """Prints debug response page output."""
 
         # Handle for potential param types.
         if isinstance(response_content, HttpResponseBase):
             response_content = response_content.content.decode('utf-8')
         elif isinstance(response_content, bytes):
@@ -204,15 +221,15 @@
         self._debug_print(
             '{0} {1} {0}'.format('=' * 10, 'Form Data'),
             fore=ETC_RESPONSE_DEBUG_FORM_COLOR,
             style=ETC_OUTPUT_EMPHASIS_COLOR,
         )
 
         # Check if form or formset data is actually present.
-        if 'form' in response_context or 'formset' in response_context:
+        if response_context is not None and ('form' in response_context or 'formset' in response_context):
             # Form or formset present on page.
 
             # Attempt to get form data.
             form_present = False
             if 'form' in response_context:
                 form_present = True
                 form = response_context['form']
@@ -311,14 +328,108 @@
                 type(get_user_model()),
             ), fore=ETC_OUTPUT_ERROR_COLOR)
         self._debug_print()
         self._debug_print()
 
     # endregion Debug Output Functions.
 
+    def standardize_url(self, url, url_args=None, url_kwargs=None, url_query_params=None, append_root=True):
+        """Attempts to standardize URL value, such as in event url is in format for reverse() function.
+
+        :param url: Url value to attempt to parse and standardize.
+        :param url_args: Additional "args" to pass for reverse() function, if applicable.
+        :param url_kwargs: Additional "kwargs" to pass for reverse() function, if applicable.
+        :param append_root: Bool indicating if "site root" should be included in url (if not already).
+        :return: Attempt at fully-formatted url.
+        """
+
+        # Handle mutable data defaults.
+        url_args = url_args or ()
+        url_kwargs = url_kwargs or {}
+        url_query_params = url_query_params or {}
+
+        # Preprocess all potential url values.
+        url = str(url).strip()
+
+        # Attempt to get reverse of provided url.
+        try:
+            url = reverse(url, args=url_args, kwargs=url_kwargs)
+
+            # Provide warning based on APPEND_SLASH setting.
+            # See https://stackoverflow.com/a/42213107 for discussion on why this setting exists
+            # as well as how Django generally handles url composition.
+            if settings.APPEND_SLASH:
+                if len(url) > 0 and url[-1] != '/':
+                    warn_msg = (
+                        'Django setting APPEND_SLASH is set to True, '
+                        'but url did not resolve with trailing slash. '
+                        'This may cause UnitTests with ETC to fail. Url was: {0}'
+                    ).format(url)
+                    logging.warning(warn_msg)
+            else:
+                if len(url) > 0 and url[-1] == '/':
+                    warn_msg = (
+                        'Django setting APPEND_SLASH is set to False, '
+                        'but url resolved with trailing slash. '
+                        'This may cause UnitTests with ETC to fail. Url was: {0}'
+                    ).format(url)
+                    logging.warning(warn_msg)
+
+        except NoReverseMatch:
+            # Could not find as reverse. Assume is literal url.
+
+            # Trim any known extra values on literal url str.
+            url = str(url).strip().lstrip('/').rstrip('/')
+            if url.startswith(self.site_root_url):
+                url = url.lstrip(self.site_root_url)
+            elif url.startswith('127.0.0.1'):
+                url = url.lstrip('127.0.0.1')
+
+            # Check if empty url.
+            if len(url) == 0:
+                # Empty url. Populate to single slash.
+                url = '/'
+            else:
+                # Non-empty url.
+
+                # Handle for prepend slash.
+                # Only apply if not already present.
+                if not url.startswith('/'):
+                    url = '/{0}'.format(url)
+
+                # Handle if GET args are included within url.
+                split_url = url.split('?')
+                if len(split_url) == 1:
+                    # No GET args found.
+                    url = split_url[0]
+                else:
+                    # Url GET args found. Temporarily split to prevent errors.
+                    url = split_url.pop(0)
+
+                    # Convert query params to expected dictionary format for passing as proper kwargs.
+                    url_args = '{0}'.format('?'.join(x for x in split_url))
+                    temp_dict = parse_qs(url_args)
+                    for key, value in temp_dict.items():
+                        url_query_params[key] = value[0]
+
+                # Handle for append slash.
+                # Only apply if not already present and settings.APPEND_SLASH is true.
+                if settings.APPEND_SLASH and not url.endswith('/'):
+                    url = '{0}/'.format(url)
+
+        if url_query_params:
+            url = self.generate_get_url(url, **url_query_params)
+
+        # Finally, prepend site root to url, if applicable.
+        if append_root:
+            url = '{0}{1}'.format(self.site_root_url, url)
+
+        # Return final full url.
+        return url
+
     def standardize_html_tags(self, value):
         """Standardizes spacing around html-esque elements, to remove unnecessary spacing.
 
         For example, "<h1> MyHeader </h1>" will simplify down to "<h1>MyHeader</h1>".
 
         Ensures that the actual expected value can be directly checked,
         instead of trying to account for extraneous template whitespacing.
```

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases/templates/django_expanded_test_cases/index.html`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/__init__.py` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,28 +7,58 @@
 from .base_test_case import BaseTestCase
 
 
 # Expanded "Integration" TestCase utility class.
 from .integration_test_case import IntegrationTestCase
 
 
-# Expanded "Live Server" TestCase utility class.
+# Expanded "Django Live Server" TestCase utility class.
 try:
     from .live_server_test_case import LiveServerTestCase
 except ModuleNotFoundError:
-    # Project likely does not have DjangoChannels package installed.
+    # Project likely does not have selenium package installed.
     # This is okay, as we don't want this logic as a hard requirement to use this library.
 
     # However, we do want to define a dummy class to give feedback errors.
     class LiveServerTestCase(BaseTestCase):
         err_msg = """
-        Cannot use LiveServerTestCase class without "channels" package installed.
+        Cannot use LiveServerTestCase class without "selenium" package installed.
+        To use this TestCase, add the following packages to your project:
+            * selenium              # Required
+            * webdriver-manager     # Required
+
+        For more information, see:
+        https://www.selenium.dev/documentation/webdriver/getting_started/
+        """
+        @classmethod
+        def setUpClass(cls):
+            raise Exception(cls.err_msg)
+
+        def setUp(self):
+            raise Exception(self.err_msg)
+
+        def __int__(self):
+            raise Exception(self.err_msg)
+
+
+# Expanded "Channels Live Server" TestCase utility class.
+try:
+    from .channels_live_server_test_case import ChannelsLiveServerTestCase
+except ModuleNotFoundError:
+    # Project likely does not have DjangoChannels package or associated daphne package installed.
+    # This is okay, as we don't want this logic as a hard requirement to use this library.
+
+    # However, we do want to define a dummy class to give feedback errors.
+    class ChannelsLiveServerTestCase(BaseTestCase):
+        err_msg = """
+        Cannot use ChannelsLiveServerTestCase class without "channels" package installed.
         To use this TestCase, add the following packages to your project:
             * channels              # Required
-            * webdriver-manager     # Optional
+            * daphne                # Required
+            * webdriver-manager     # Required
 
         For more information, see:
         https://www.selenium.dev/documentation/webdriver/getting_started/
         """
         @classmethod
         def setUpClass(cls):
             raise Exception(cls.err_msg)
```

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/base_test_case.py` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/base_test_case.py`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases/test_cases/integration_test_case.py` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases/test_cases/integration_test_case.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 """
 Testing logic for views and other multi-part components.
 """
 
 # System Imports.
-import logging, re, textwrap
+import re, textwrap
 
 # Third-Party Imports.
 from django.conf import settings
 from django.core.exceptions import ValidationError
 from django.http.response import HttpResponseBase
 from django.urls import reverse
 from django.urls.exceptions import NoReverseMatch
 
 # Internal Imports.
 from .base_test_case import BaseTestCase
 from django_expanded_test_cases.constants import (
+    ETC_INCLUDE_RESPONSE_DEBUG_URL,
     ETC_INCLUDE_RESPONSE_DEBUG_CONTENT,
     ETC_INCLUDE_RESPONSE_DEBUG_CONTEXT,
     ETC_INCLUDE_RESPONSE_DEBUG_FORMS,
     ETC_INCLUDE_RESPONSE_DEBUG_HEADER,
     ETC_INCLUDE_RESPONSE_DEBUG_MESSAGES,
     ETC_INCLUDE_RESPONSE_DEBUG_SESSION,
-    ETC_INCLUDE_RESPONSE_DEBUG_URL,
     ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO,
+    ETC_ALLOW_TITLE_PARTIALS,
     ETC_ALLOW_MESSAGE_PARTIALS,
     ETC_REQUEST_USER_STRICTNESS,
     ETC_DEFAULT_STANDARD_USER_IDENTIFIER,
     ETC_RESPONSE_DEBUG_URL_COLOR,
     ETC_OUTPUT_EMPHASIS_COLOR,
+    ETC_OUTPUT_ERROR_COLOR,
+    ETC_OUTPUT_RESET_COLOR,
+    ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+    ETC_OUTPUT_EXPECTED_MATCH_COLOR,
     VOID_ELEMENT_LIST,
 )
 from django_expanded_test_cases.mixins import ResponseTestCaseMixin
 
 
 class IntegrationTestCase(BaseTestCase, ResponseTestCaseMixin):
     """Testing functionality for views and other multi-part components."""
@@ -42,25 +47,27 @@
 
         # Initialize url variables.
         try:
             cls.login_url = reverse(settings.LOGIN_URL)
         except NoReverseMatch:
             # Login url is not defined.
             cls.login_url = None
-        cls._site_root_url = None
 
     # region Custom Assertions
 
     def assertResponse(
         self,
         url, *args,
-        get=True, data=None,
-        expected_redirect_url=None, expected_status=200,
+        get=True, data=None, secure=True,
+        expected_status=200,
+        expected_redirect_url=None,
+        url_args=None, url_kwargs=None, url_query_params=None,
+        redirect_args=None, redirect_kwargs=None, redirect_query_params=None,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None, extra_usergen_kwargs=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Verifies the view response object at given URL matches provided parameters.
 
         At minimum, gets a response object from parsing provided url, then asserts the status code matches.
         Optionally also allows testing:
@@ -68,50 +75,69 @@
             * Header (H1 tag) - The expected H1 header tag on the page.
             * Messages - One or more messages, generated from the Django messages framework.
             * Content - One or more values that should physically appear within html rendering.
 
         :param url: Url to get response object from.
         :param get: Bool indicating if response is GET or POST. Defaults to GET.
         :param data: Optional dict of items to pass into response generation.
+        :param secure: Bool indicating if request should be retrieved as HTTP or HTTPS.
         :param expected_redirect_url: Expected url, after any redirections.
+        :param url_args: Values to provide for URL population, in "arg" format.
+        :param url_kwargs: Values to provide for URL population, in "kwarg" format.
+        :param url_query_params: Query parameter values to provide for URL population.
+        :param redirect_args: Values to provide for redirect URL population, in "arg" format.
+        :param redirect_kwargs: Values to provide for redirect URL population, in "kwarg" format.
+        :param redirect_query_params: Query parameter values to provide for redirect URL population.
         :param expected_status: Expected status code, after any redirections. Default code of 200.
         :param expected_title: Expected page title to verify. Skips title test if left as None.
         :param expected_header: Expected page h1 to verify. Skips header test if left as None.
         :param expected_messages: Expected context messages to verify. Skips message test if left as None.
         :param expected_content: Expected page content elements to verify. Skips content test if left as None.
         :param auto_login: Bool indicating if user should be auto-logged-in.
         :param user: User to log in with, if auto_login is True. Defaults to `test_user`.
         :param user_permissions: Optional permissions to provide to login user.
         :param user_groups: Optional groups to provide to login user.
+        :param extra_usergen_kwargs: Optional dictionary of values to pass to _get_login_user__extra_user_auth_setup().
         :param ignore_content_ordering: Bool indicating if ordering should be verified. Defaults to checking ordering.
         :param content_starts_after: The HTML that expected_content should occur after. This HTML and everything
                                      preceding is stripped out of the "search space" for the expected_content value.
         :param content_ends_before: The HTML that expected_content should occur before. This HTML and everything
                                     following is stripped out of the "search space" for the expected_content value.
         """
-        # Django imports here to avoid situational "Apps aren't loaded yet" error.
-        from django.contrib.auth.models import AnonymousUser
+
+        # Handle mutable data defaults.
+        data = data or {}
+        url_args = (*args, *kwargs.pop('args', []), *(url_args or []))
+        url_query_params = url_query_params or {}
+        redirect_args = (*args, *(redirect_args or []))
+        redirect_kwargs = {**kwargs, **(redirect_kwargs or {})}
+        redirect_query_params = redirect_query_params or {}
+        url_kwargs = {**kwargs.pop('kwargs', {}), **(url_kwargs or {}), **kwargs}
+        extra_usergen_kwargs = extra_usergen_kwargs or {}
 
         # Reset client "user login" state for new response generation.
         self.client.logout()
 
         # Handle getting user.
         user = self._get_default_request_user(user, auto_login)
 
         # Run logic to get corresponding response object.
         response = self._get_page_response(
             url,
-            *args,
             get=get,
             data=data,
+            secure=secure,
+            url_args=url_args,
+            url_kwargs=url_kwargs,
+            query_params=url_query_params,
             auto_login=auto_login,
             user=user,
             user_permissions=user_permissions,
             user_groups=user_groups,
-            **kwargs,
+            extra_usergen_kwargs=extra_usergen_kwargs,
         )
 
         # Optionally output all debug info for found response.
         if self._debug_print_bool:
             if ETC_INCLUDE_RESPONSE_DEBUG_CONTENT:
                 self.show_debug_content(response)
             if ETC_INCLUDE_RESPONSE_DEBUG_HEADER:
@@ -125,33 +151,43 @@
             if ETC_INCLUDE_RESPONSE_DEBUG_FORMS:
                 self.show_debug_form_data(response)
             if ETC_INCLUDE_RESPONSE_DEBUG_USER_INFO:
                 self.show_debug_user_info(response.user)
 
         # Optional hook for running custom pre-builtin-test logic.
         self._assertResponse__pre_builtin_tests(
-            url, *args,
+            response.url, *args,
             response=response,
-            get=get, data=data,
-            expected_redirect_url=expected_redirect_url, expected_status=expected_status,
+            get=get, data=data, secure=secure,
+            expected_status=expected_status,
+            expected_redirect_url=expected_redirect_url,
+            url_args=url_args, url_kwargs=url_kwargs, url_query_params=url_query_params,
+            redirect_args=redirect_args, redirect_kwargs=redirect_kwargs, redirect_query_params=redirect_query_params,
             expected_title=expected_title, expected_header=expected_header, expected_messages=expected_messages,
             expected_content=expected_content,
             auto_login=auto_login, user=user, user_permissions=user_permissions, user_groups=user_groups,
+            extra_usergen_kwargs=extra_usergen_kwargs,
             ignore_content_ordering=ignore_content_ordering, content_starts_after=content_starts_after,
             content_ends_before=content_ends_before,
             **kwargs,
         )
 
-        # Verify page redirect.
-        if expected_redirect_url is not None:
-            self.assertRedirects(response, expected_redirect_url)
-
         # Verify page status code.
         self.assertStatusCode(response, expected_status)
 
+        # Verify page redirect.
+        if expected_redirect_url is not None:
+            self.assertRedirects(
+                response,
+                expected_redirect_url,
+                redirect_args=redirect_args,
+                redirect_kwargs=redirect_kwargs,
+                redirect_query_params=redirect_query_params,
+            )
+
         # Verify page title.
         if expected_title is not None:
             self.assertPageTitle(response, expected_title)
 
         # Verify page header.
         if expected_header is not None:
             self.assertPageHeader(response, expected_header)
@@ -169,128 +205,182 @@
                 content_starts_after=content_starts_after,
                 content_ends_before=content_ends_before,
                 debug_output=False,
             )
 
         # Optional hook for running custom post-builtin-test logic.
         self._assertResponse__post_builtin_tests(
-            url, *args,
+            response.url, *args,
             response=response,
-            get=get, data=data,
-            expected_redirect_url=expected_redirect_url, expected_status=expected_status,
+            get=get, data=data, secure=secure,
+            expected_status=expected_status,
+            expected_redirect_url=expected_redirect_url,
+            url_args=url_args, url_kwargs=url_kwargs, url_query_params=url_query_params,
+            redirect_args=redirect_args, redirect_kwargs=redirect_kwargs, redirect_query_params=redirect_query_params,
             expected_title=expected_title, expected_header=expected_header, expected_messages=expected_messages,
             expected_content=expected_content,
             auto_login=auto_login, user=user, user_permissions=user_permissions, user_groups=user_groups,
+            extra_usergen_kwargs=extra_usergen_kwargs,
             ignore_content_ordering=ignore_content_ordering, content_starts_after=content_starts_after,
             content_ends_before=content_ends_before,
             **kwargs,
         )
 
         # All assertions passed so far. Return response in case user wants to do further checks.
         return response
 
     def assertGetResponse(
         self,
         url, *args,
-        data=None,
-        expected_redirect_url=None, expected_status=200,
+        data=None, secure=True,
+        expected_status=200,
+        expected_redirect_url=None,
+        url_args=None, url_kwargs=None, url_query_params=None,
+        redirect_args=None, redirect_kwargs=None, redirect_query_params=None,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None, extra_usergen_kwargs=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Verifies a GET response was found at given URL, and matches provided parameters."""
 
+        # Handle mutable data defaults.
+        data = data or {}
+        url_args = url_args or []
+        url_kwargs = url_kwargs or {}
+        url_query_params = url_query_params or []
+        redirect_args = redirect_args or []
+        redirect_kwargs = redirect_kwargs or {}
+        redirect_query_params = redirect_query_params or {}
+        extra_usergen_kwargs = extra_usergen_kwargs or {}
+
         # Call base function to handle actual logic.
         return self.assertResponse(
             url,
             *args,
             get=True,
             data=data,
-            expected_redirect_url=expected_redirect_url,
+            secure=secure,
             expected_status=expected_status,
+            expected_redirect_url=expected_redirect_url,
+            url_args=url_args,
+            url_kwargs=url_kwargs,
+            url_query_params=url_query_params,
+            redirect_args=redirect_args,
+            redirect_kwargs=redirect_kwargs,
+            redirect_query_params=redirect_query_params,
             expected_title=expected_title,
             expected_header=expected_header,
             expected_messages=expected_messages,
             expected_content=expected_content,
             auto_login=auto_login,
             user=user,
             user_permissions=user_permissions,
             user_groups=user_groups,
+            extra_usergen_kwargs=extra_usergen_kwargs,
             ignore_content_ordering=ignore_content_ordering,
             content_starts_after=content_starts_after,
             content_ends_before=content_ends_before,
             **kwargs,
         )
 
     def assertPostResponse(
         self,
         url, *args,
-        data=None,
-        expected_redirect_url=None, expected_status=200,
+        data=None, secure=True,
+        expected_status=200,
+        expected_redirect_url=None,
+        url_args=None, url_kwargs=None, url_query_params=None,
+        redirect_args=None, redirect_kwargs=None, redirect_query_params=None,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None, extra_usergen_kwargs=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Verifies a GET response was found at given URL, and matches provided parameters."""
 
         # Handle mutable data defaults.
         data = data or {}
+        url_args = url_args or []
+        url_kwargs = url_kwargs or {}
+        url_query_params = url_query_params or {}
+        redirect_args = redirect_args or []
+        redirect_kwargs = redirect_kwargs or {}
+        redirect_query_params = redirect_query_params or {}
+        extra_usergen_kwargs = extra_usergen_kwargs or {}
 
         # Forcibly add values to "data" dict, so that POST doesn't validate to empty in view.
         # This guarantees that view serves as POST, like this specific assertion expects.
         if data == {}:
             # Has no values. Forcibly add a single key-value pair.
             data = {'UnitTest': True}
 
         # Call base function to handle actual logic.
         return self.assertResponse(
             url,
             *args,
             get=False,
             data=data,
-            expected_redirect_url=expected_redirect_url,
+            secure=secure,
             expected_status=expected_status,
+            expected_redirect_url=expected_redirect_url,
+            url_args=url_args,
+            url_kwargs=url_kwargs,
+            url_query_params=url_query_params,
+            redirect_args=redirect_args,
+            redirect_kwargs=redirect_kwargs,
+            redirect_query_params=redirect_query_params,
             expected_title=expected_title,
             expected_header=expected_header,
             expected_messages=expected_messages,
             expected_content=expected_content,
             auto_login=auto_login,
             user=user,
             user_permissions=user_permissions,
             user_groups=user_groups,
+            extra_usergen_kwargs=extra_usergen_kwargs,
             ignore_content_ordering=ignore_content_ordering,
             content_starts_after=content_starts_after,
             content_ends_before=content_ends_before,
             **kwargs,
         )
 
-    def assertRedirects(self, response, expected_redirect_url, *args, **kwargs):
+    def assertRedirects(
+        self,
+        response, expected_redirect_url, *args,
+        redirect_args=None, redirect_kwargs=None, redirect_query_params=None, **kwargs,
+    ):
         """Assert that a response redirected to a specific URL and that the redirect URL can be loaded.
 
         Most functionality is in the default Django assertRedirects() function.
         However, this acts as a wrapper to also:
             * Check that provided response param is a valid Response object. Attempts to generate one if not.
             * Attempt url as reverse, before trying assertion.
         """
+        # Handle mutable data defaults.
+        redirect_args = redirect_args or []
+        redirect_kwargs = redirect_kwargs or {}
+        redirect_query_params = redirect_query_params or {}
+
         # Ensure provided response is actual response.
         if isinstance(response, HttpResponseBase):
             # Is literal response.
             pass
         else:
             # Is not response. Attempt to get.
             response = self._get_page_response(response)
 
-        # Try to get reverse of provided redirect.
-        try:
-            expected_redirect_url = reverse(expected_redirect_url)
-        except NoReverseMatch:
-            # Not a reverse for url. Assume is a literal url.
-            pass
+        # Sanitize redirect url.
+        expected_redirect_url = self.standardize_url(
+            expected_redirect_url,
+            url_args=redirect_args,
+            url_kwargs=redirect_kwargs,
+            url_query_params=redirect_query_params,
+            append_root=False,
+        )
 
         # Run assertion on provided value.
         try:
             return super().assertRedirects(response, expected_redirect_url, *args, **kwargs)
         except AssertionError:
             self.fail('Response didn\'t redirect as expected. Response code was {0} (expected 302).'.format(
                 response.status_code
@@ -317,49 +407,57 @@
                 actual_status,
             ),
         )
 
         # Return status in case user wants to run additional logic on it.
         return actual_status
 
-    def assertPageTitle(self, response, expected_title, exact_match=True):
+    def assertPageTitle(self, response, expected_title, allow_partials=None):
         """Verifies the page title HTML element.
 
         Note: Some sites have titles with nested elements.
             Ex: "<title><page> | <app> | <website></title>"
 
         Thus the "exact_match" bool exists, to allow only testing for a specific unit in the title, instead of
         always having to type the full title for every test.
 
         :param response: Response object to check against.
         :param expected_title: Expected full string in title HTML element.
-        :param exact_match: Bool indicating if title should be exact match, or partial.
+        :param allow_partials: Bool indicating if title should be exact match, or partial.
         :return: Parsed out title string.
         """
+        # Parse out settings values.
+        if allow_partials is None:
+            allow_partials = ETC_ALLOW_TITLE_PARTIALS
+        else:
+            allow_partials = bool(allow_partials)
+
         # Parse out title element from response.
         actual_title = self.get_page_title(response)
 
         # Remove title tag from expected value, if present.
         expected_title = str(expected_title).strip()
         if expected_title.startswith('<title>'):
             expected_title = expected_title[7:]
         if expected_title.endswith('</title>'):
             expected_title = expected_title[:-8]
         expected_title = expected_title.strip()
 
         # Check element.
         err_msg = 'Expected title HTML contents of "{0}" ({1}). Actual value was "{2}".'
-        if exact_match:
+        if not allow_partials:
+            # Check using exact match.
             if expected_title != actual_title:
                 self.fail(err_msg.format(
                     expected_title,
                     'using exact matching',
                     actual_title,
                 ))
         else:
+            # Check using partial match.
             if expected_title not in actual_title:
                 self.fail(err_msg.format(
                     expected_title,
                     'using partial matching',
                     actual_title,
                 ))
 
@@ -462,17 +560,17 @@
 
                     # Loop through all context messages until found, or all are checked.
                     if expected_message in actual_messages:
                         message_found = True
 
                 # Raise assertion error if not found.
                 if not message_found:
-                    self.fail('Failed to find message "{0}" in context (Partial matching {1} allowed).'.format(
+                    self.fail('Failed to find message "{0}" in context (using {1} matching).'.format(
                         expected_message,
-                        'is' if allow_partials else 'is NOT'
+                        'partial' if allow_partials else 'exact'
                     ))
 
     def assertPageContent(
         self,
         response, expected_content,
         ignore_ordering=False, content_starts_after=None, content_ends_before=None, debug_output=True,
     ):
@@ -493,15 +591,28 @@
         :param debug_output: Bool indicating if debug output should be shown or not. Used for debugging test failures.
         :return: Parsed out and formatted content string.
         """
         if debug_output:
             # Print out actual response content, for debug output.
             self.show_debug_content(response)
 
-        main_err_msg = 'Could not find expected content value in response. Provided value was:\n{0}'
+        main_err_msg = (
+            'Could not find expected content value in response. Provided value was:\n'
+            '{0}\n'
+        )
+        checked_content_str_addon = (
+            '\n'
+            '\n'
+            'Surrounding Checks:\n'
+            '{0}'
+            '{1}'
+            '{2}'
+            '{3}'
+            '{4}'
+        )
         ordering_err_msg = 'Expected content value was found, but ordering of values do not match. Problem value:\n{0}'
         casing_err_msg = (
             'Expected content value was found, but letter capitalization did not match. Expected was:\n'
             '{0}\n'
             '\n'
             'Found was:\n'
             '... {1} ...'
@@ -518,15 +629,46 @@
 
         # Handle possible types.
         if expected_content is None:
             expected_content = ''
         if isinstance(expected_content, list) or isinstance(expected_content, tuple):
             # The expected_content param is an array of items. Verify they all exist on page.
             trimmed_content = trimmed_original_content
-            for expected in expected_content:
+            for index in range(len(expected_content)):
+                expected = expected_content[index]
+
+                # Update str in event of error.
+                updated_checked_content_str_addon = checked_content_str_addon.format(
+                    '{1}    * {0}{2}\n'.format(
+                        expected_content[index - 2],
+                        ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                        ETC_OUTPUT_RESET_COLOR,
+                    ) if index >= 2 else '',
+                    '{1}    * {0}{2}\n'.format(
+                        expected_content[index - 1],
+                        ETC_OUTPUT_EXPECTED_MATCH_COLOR,
+                        ETC_OUTPUT_RESET_COLOR,
+                    ) if index >= 1 else '',
+                    '{1}  > * {0}{2}\n'.format(
+                        expected_content[index],
+                        ETC_OUTPUT_ERROR_COLOR,
+                        ETC_OUTPUT_RESET_COLOR,
+                    ),
+                    '{1}    * {0}{2}\n'.format(
+                        expected_content[index + 1],
+                        ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                        ETC_OUTPUT_RESET_COLOR,
+                    ) if (len(expected_content) - index) > 1 else '',
+                    '{1}    * {0}{2}\n'.format(
+                        expected_content[index + 2],
+                        ETC_OUTPUT_ACTUALS_MATCH_COLOR,
+                        ETC_OUTPUT_RESET_COLOR,
+                    ) if (len(expected_content) - index) > 2 else '',
+                )
+
                 stripped_expected = self.get_minimized_response_content(expected, strip_newlines=True)
                 if ignore_ordering:
                     # Ignoring ordering. Check as-is.
                     if stripped_expected not in trimmed_original_content:
                         # Expected value not found in provided content section.
                         display_expected = self.get_minimized_response_content(expected, strip_newlines=False)
 
@@ -551,14 +693,15 @@
                             self._assertPageContent(
                                 sanitized_original_content,
                                 stripped_expected,
                                 display_expected,
                                 content_starts_after,
                                 content_ends_before,
                                 main_err_msg,
+                                updated_checked_content_str_addon,
                             )
                 else:
                     # Verifying ordering.
                     # Attempt initial assertion in provided subsection.
                     if stripped_expected not in trimmed_content:
                         # Failed to find content in subsection. Check full content set.
                         if stripped_expected not in trimmed_original_content:
@@ -586,18 +729,21 @@
                                 self._assertPageContent(
                                     sanitized_original_content,
                                     stripped_expected,
                                     display_expected,
                                     content_starts_after,
                                     content_ends_before,
                                     main_err_msg,
+                                    updated_checked_content_str_addon,
                                 )
 
                         # If we made it this far, then item was found in full content, but came after a previous
                         # expected value. Raise error.
+                        if updated_checked_content_str_addon:
+                            ordering_err_msg += updated_checked_content_str_addon
                         self.fail(ordering_err_msg.format(expected))
 
                 # If we made it this far, then value was found. Handle for ordering.
                 if not ignore_ordering:
                     # Ordering is being checked. Strip off first section of matching.
                     trimmed_content = stripped_expected.join(
                         trimmed_content.split(stripped_expected)[1:],
@@ -631,20 +777,26 @@
                     self._assertPageContent(
                         sanitized_original_content,
                         stripped_expected,
                         display_expected,
                         content_starts_after,
                         content_ends_before,
                         main_err_msg,
+                        '',
                     )
 
         # Return page content in case user wants to run additional logic on it.
         return trimmed_original_content
 
-    def _assertPageContent(self, actual_content, minimized_expected, display_expected, strip_actual_start, strip_actual_end, err_msg):
+    def _assertPageContent(
+        self,
+        actual_content, minimized_expected, display_expected,
+        strip_actual_start, strip_actual_end,
+        err_msg, checked_content_str_addon
+    ):
         """Internal sub-assertion for assertPageContent() function."""
         strip_err_msg = 'Expected content value was found, but occurred in "{0}" section. Expected was:\n{1}'
 
         # Check if error was due to content_starts_after/content_ends_before variables.
         found_expected = False
         if strip_actual_start:
             stripped_start_section = str(actual_content.split(strip_actual_start)[0] + strip_actual_start)
@@ -655,18 +807,22 @@
             stripped_end_section = str(strip_actual_end + actual_content.split(strip_actual_end)[-1])
             if minimized_expected in stripped_end_section:
                 found_expected = 'content_ends_before'
 
         # Output message based on above searches.
         if found_expected:
             # Content value was in stripped section. Raise corresponding strip message.
+            if checked_content_str_addon:
+                strip_err_msg += checked_content_str_addon
             self.fail(strip_err_msg.format(found_expected, display_expected))
 
         else:
             # Content value was physically not present at all. Raise "main" message.
+            if checked_content_str_addon:
+                err_msg += checked_content_str_addon
             self.fail(err_msg.format(display_expected))
 
     def assertRepeatingElement(
         self,
         response, expected_repeating_element, repeat_count,
         content_starts_after=None, content_ends_before=None, debug_output=True,
     ):
@@ -790,130 +946,78 @@
         # Return calculated user.
         return user
 
     def _get_page_response(
         self,
         url,
         *args,
-        get=True, data=None,
-        auto_login=True, user=None, user_permissions=None, user_groups=None,
+        get=True, data=None, secure=True,
+        url_args=None, url_kwargs=None, query_params=None,
+        auto_login=True, user=None, user_permissions=None, user_groups=None, extra_usergen_kwargs=None,
         **kwargs,
     ):
         """Helper function for assertResponse().
 
         Fully parses provided user url, and returns corresponding response object.
 
         :param url: Url to get response object from.
         :param get: Bool indicating if response is GET or POST. Defaults to GET.
         :param data: Optional dict of items to pass into response generation.
+        :param secure: Bool indicating if request should be retrieved as HTTP or HTTPS.
+        :param url_args: Values to provide for URL population, in "arg" format.
+        :param url_kwargs: Values to provide for URL population, in "kwarg" format.
         :param auto_login: Bool indicating if User should be "logged in" to client or not.
         :param user_permissions: Set of Django Permissions to give to test user before accessing page.
         :param user_groups: Set of Django PermissionGroups to give to test user before accessing page.
+        :param extra_usergen_kwargs: Optional dictionary of values to pass to _get_login_user__extra_user_auth_setup().
         :return: Django response object for provided url.
         """
         # Handle mutable data defaults.
         data = data or {}
+        url_args = (*args, *kwargs.pop('args', []), *(url_args or []))
+        url_kwargs = {**kwargs.pop('kwargs', {}), **(url_kwargs or {}), **kwargs}
+        query_params = query_params or {}
+        extra_usergen_kwargs = {**kwargs, **(extra_usergen_kwargs or {})}
 
         # Validate data types.
         if not isinstance(data, dict):
             raise TypeError('Provided "data" arg must be a dict, for passing into POST requests.')
 
         # Handle getting user.
         user = self._get_default_request_user(user, auto_login)
-
         user = self._get_login_user(
             user,
             *args,
-            url=url,
-            get=get,
-            data=data,
             auto_login=auto_login,
             user_permissions=user_permissions,
             user_groups=user_groups,
-            **kwargs,
+            **extra_usergen_kwargs,
         )
 
-        # Preprocess all potential url values.
-        url = str(url).strip()
-        current_site = '127.0.0.1'
-        url_args = ()
-        url_kwargs = {}
-
-        # Handle site_root_url value.
-        if self.site_root_url is not None:
-            current_site = self.site_root_url
-
-        # Standardize if literal site url was provided and included site_root.
-        if url.startswith(current_site):
-            url = url[len(current_site):]
-
-        # If "args" key or "kwargs" key exists in function kwargs param, assume is meant for url reverse.
-        if 'args' in kwargs.keys():
-            url_args = kwargs['args']
-        if 'kwargs' in kwargs.keys():
-            url_kwargs = kwargs['kwargs']
-
-        # Attempt to get reverse of provided url.
-        try:
-            url = reverse(url, args=url_args, kwargs=url_kwargs)
-
-            # Provide warning based on APPEND_SLASH setting.
-            # See https://stackoverflow.com/a/42213107 for discussion on why this setting exists
-            # as well as how Django generally handles url composition.
-            if settings.APPEND_SLASH:
-                if len(url) > 0 and url[-1] != '/':
-                    warn_msg = (
-                        'Django setting APPEND_SLASH is set to True, '
-                        'but url did not resolve with trailing slash. '
-                        'This may cause UnitTests with ETC to fail. Url was: {0}'
-                    ).format(url)
-                    logging.warning(warn_msg)
-            else:
-                if len(url) > 0 and url[-1] == '/':
-                    warn_msg = (
-                        'Django setting APPEND_SLASH is set to False, '
-                        'but url resolved with trailing slash. '
-                        'This may cause UnitTests with ETC to fail. Url was: {0}'
-                    ).format(url)
-                    logging.warning(warn_msg)
-        except NoReverseMatch:
-            # Could not find as reverse. Assume is literal url.
-            pass
-
-        # Make sure exactly one slash is prepended to the url value.
-        url = url.lstrip('/').rstrip('/')
-        if len(url) == 0:
-            url = '/'
-        else:
-            if settings.APPEND_SLASH:
-                url = '/{0}/'.format(url)
-            else:
-                url = '/{0}'.format(url)
-
-        # Log url we're attempting to access.
-        if self.site_root_url is not None:
-            current_site = '{0}{1}'.format(self.site_root_url, url)
-        else:
-            current_site = '127.0.0.1{0}'.format(url)
-        message = 'Attempting to access url "{0}"'.format(current_site)
-
-        self._debug_print('\n\n')
+        # Handle url sanitization.
+        url = self.standardize_url(
+            url,
+            url_args=url_args,
+            url_kwargs=url_kwargs,
+            url_query_params=query_params,
+            append_root=False,
+        )
+        full_url = '{0}{1}'.format(self.site_root_url, url)
         if ETC_INCLUDE_RESPONSE_DEBUG_URL:
-            self._debug_print('{0}'.format('-' * len(message)), fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
-            self._debug_print(message, fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
-            self._debug_print('{0}'.format('-' * len(message)), fore=ETC_RESPONSE_DEBUG_URL_COLOR, style=ETC_OUTPUT_EMPHASIS_COLOR)
+            self.show_debug_url(full_url)
 
         # Get response object.
         if bool(get):
-            response = self.client.get(url, data=data, follow=True)
+            response = self.client.get(url, data=data, secure=secure, follow=True)
         else:
-            response = self.client.post(url, data=data, follow=True)
+            response = self.client.post(url, data=data, secure=secure, follow=True)
 
         # Update response object with additional useful values for further testing/analysis.
-        response.url = current_site
+        response.url = url
+        response.full_url = full_url
         response.user = user
 
         # Return generated response.
         return response
 
     def _get_login_user(self, user, *args, auto_login=True, user_permissions=None, user_groups=None, **kwargs):
         """Handles simulating user login with corresponding permissions/groups/etc.
@@ -1187,15 +1291,17 @@
 
     # region Hook Functions
 
     def _assertResponse__pre_builtin_tests(
         self,
         url, *args,
         get=True, data=None,
-        expected_redirect_url=None, expected_status=200,
+        expected_status=200,
+        expected_redirect_url=None,
+        url_args=None, url_kwargs=None, redirect_args=None, redirect_kwargs=None,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
         auto_login=True, user=None, user_permissions=None, user_groups=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Hook function to allow injecting code prior to running any of the built-in assertResponse() tests.
 
@@ -1206,15 +1312,17 @@
         """
         pass
 
     def _assertResponse__post_builtin_tests(
         self,
         url, *args,
         get=True, data=None,
-        expected_redirect_url=None, expected_status=200,
+        expected_status=200,
+        expected_redirect_url=None,
+        url_args=None, url_kwargs=None, redirect_args=None, redirect_kwargs=None,
         expected_title=None, expected_header=None, expected_messages=None, expected_content=None,
         auto_login=True, user=None, user_permissions=None, user_groups=None,
         ignore_content_ordering=False, content_starts_after=None, content_ends_before=None,
         **kwargs,
     ):
         """Hook function to allow injecting code after running all of the built-in assertResponse() tests.
 
@@ -1225,14 +1333,15 @@
         """
         pass
 
     def _get_login_user__extra_user_auth_setup(
         self,
         user,
         *args,
+        auto_login=True,
         user_permissions=None, user_groups=None,
         **kwargs,
     ):
         """Hook function, to allow running extra authentication setup logic on User object.
 
         Useful such as for running things like 2-Factor setup logic for User.
```

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/PKG-INFO` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-expanded-test-cases
-Version: 0.4.0
+Version: 0.5.0
 Summary: Expands the existing Django TestCase class with extra functionality.
 Home-page: https://github.com/brodriguez8774/django-expanded-test-cases
 Author: Brandon Rodriguez
 Author-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 Maintainer-email: Brandon Rodriguez <brodriguez8774@gmail.com>
 License: MIT License
         
@@ -34,14 +34,16 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-expanded-test-cases-0.4.0/django_expanded_test_cases.egg-info/SOURCES.txt` & `django-expanded-test-cases-0.5.0/django_expanded_test_cases.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,23 +9,28 @@
 django_expanded_test_cases.egg-info/PKG-INFO
 django_expanded_test_cases.egg-info/SOURCES.txt
 django_expanded_test_cases.egg-info/dependency_links.txt
 django_expanded_test_cases.egg-info/requires.txt
 django_expanded_test_cases.egg-info/top_level.txt
 django_expanded_test_cases/mixins/__init__.py
 django_expanded_test_cases/mixins/core_mixin.py
+django_expanded_test_cases/mixins/live_server_mixin.py
 django_expanded_test_cases/mixins/response_mixin.py
 django_expanded_test_cases/templates/django_expanded_test_cases/index.html
 django_expanded_test_cases/test_cases/__init__.py
 django_expanded_test_cases/test_cases/base_test_case.py
+django_expanded_test_cases/test_cases/channels_live_server_test_case.py
 django_expanded_test_cases/test_cases/integration_test_case.py
 django_expanded_test_cases/test_cases/live_server_test_case.py
 tests/__init__.py
 tests/apps.py
 tests/asgi.py
 tests/settings.py
 tests/urls.py
 tests/views.py
+tests/mock_pages/__init__.py
 tests/test_cases/__init__.py
 tests/test_cases/test_base_case.py
+tests/test_cases/test_channels_live_server_case.py
 tests/test_cases/test_integration_case.py
-tests/test_cases/test_live_server_case.py
+tests/test_cases/test_live_server_case.py
+tests/test_cases/universal_live_test_mixin.py
```

### Comparing `django-expanded-test-cases-0.4.0/pyproject.toml` & `django-expanded-test-cases-0.5.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0', 'wheel']
 build-backend = 'setuptools.build_meta:__legacy__'
 
 [project]
 name = "django-expanded-test-cases"
-version = "0.4.0"
+version = "0.5.0"
 description = "Expands the existing Django TestCase class with extra functionality."
 readme = "readme.md"
 authors = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
 ]
 maintainers = [
     { name = "Brandon Rodriguez", email = "brodriguez8774@gmail.com" },
@@ -19,14 +19,16 @@
     "Framework :: Django",
     "Framework :: Django :: 3",
     "Framework :: Django :: 3.0",
     "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
```

### Comparing `django-expanded-test-cases-0.4.0/readme.md` & `django-expanded-test-cases-0.5.0/readme.md`

 * *Files identical despite different names*

### Comparing `django-expanded-test-cases-0.4.0/setup.cfg` & `django-expanded-test-cases-0.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-expanded-test-cases
-version = 0.4.0
+version = 0.5.0
 description = Expands the existing Django TestCase class with extra functionality.
 long_description = file: readme.md
 url = https://github.com/brodriguez8774/django-expanded-test-cases
 author = Brandon Rodriguez
 author_email = brodriguez8774@gmail.com
 license = MIT License
 classifiers =
```

### Comparing `django-expanded-test-cases-0.4.0/tests/settings.py` & `django-expanded-test-cases-0.5.0/tests/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     'django.contrib.auth',
     'django.contrib.contenttypes',
     'django.contrib.sessions',
     'django.contrib.messages',
     'django.contrib.staticfiles',
 )
 if CHANNELS_PACKAGE_INSTALLED:
-    INSTALLED_APPS += ('channels',)
+    INSTALLED_APPS += ('channels', 'daphne')
 ASGI_APPLICATION = 'tests.asgi.application'
 
 
 DATABASES = {
     'default': {
         'ENGINE': 'django.db.backends.sqlite3',
         'NAME': ':memory:',
```

### Comparing `django-expanded-test-cases-0.4.0/tests/test_cases/test_integration_case.py` & `django-expanded-test-cases-0.5.0/tests/test_cases/test_integration_case.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 # Third-Party Imports.
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import AnonymousUser, Group, Permission
 from django.contrib.contenttypes.models import ContentType
 from django.core.exceptions import ValidationError
 from django.http import HttpResponse
+from django.urls import reverse
 
 # Internal Imports.
 from django_expanded_test_cases import IntegrationTestCase
 
 
 class IntegrationClassTest__Base(IntegrationTestCase):
     """Tests for IntegrationTestCase class."""
@@ -27,121 +28,339 @@
     def test__assertResponse__url(self):
         """
         Tests URL value returned response object in assertResponse() function.
         """
         with self.subTest('With no site_root_url value defined - Via literal value'):
             # Test 404 page url.
             response = self.assertResponse('bad_url', expected_status=404)
-            self.assertEqual(response.url, '127.0.0.1/bad_url/')
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
             response = self.assertResponse('bad_url/', expected_status=404)
-            self.assertEqual(response.url, '127.0.0.1/bad_url/')
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
             response = self.assertResponse('127.0.0.1/bad_url/', expected_status=404)
-            self.assertEqual(response.url, '127.0.0.1/bad_url/')
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
             response = self.assertResponse('///bad_url///', expected_status=404)
-            self.assertEqual(response.url, '127.0.0.1/bad_url/')
+            self.assertText('/bad_url/', response.url)
+            self.assertText('127.0.0.1/bad_url/', response.full_url)
 
             # Test "index" page url.
             response = self.assertResponse('')
-            self.assertEqual(response.url, '127.0.0.1/')
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
             response = self.assertResponse('/')
-            self.assertEqual(response.url, '127.0.0.1/')
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
             response = self.assertResponse('127.0.0.1/')
-            self.assertEqual(response.url, '127.0.0.1/')
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
 
             # Test "login" page url.
             response = self.assertResponse('login/')
-            self.assertEqual(response.url, '127.0.0.1/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
             response = self.assertResponse('/login/')
-            self.assertEqual(response.url, '127.0.0.1/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
             response = self.assertResponse('127.0.0.1/login/')
-            self.assertEqual(response.url, '127.0.0.1/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
 
             # Test "one message" page url.
-            response = self.assertResponse('one-message/')
-            self.assertEqual(response.url, '127.0.0.1/one-message/')
-            response = self.assertResponse('/one-message/')
-            self.assertEqual(response.url, '127.0.0.1/one-message/')
-            response = self.assertResponse('127.0.0.1/one-message/')
-            self.assertEqual(response.url, '127.0.0.1/one-message/')
+            response = self.assertResponse('views/one-message/')
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+            response = self.assertResponse('/views/one-message/')
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
+            response = self.assertResponse('127.0.0.1/views/one-message/')
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
 
             # Test "two messages" page url.
-            response = self.assertResponse('two-messages/')
-            self.assertEqual(response.url, '127.0.0.1/two-messages/')
-            response = self.assertResponse('/two-messages/')
-            self.assertEqual(response.url, '127.0.0.1/two-messages/')
-            response = self.assertResponse('127.0.0.1/two-messages/')
-            self.assertEqual(response.url, '127.0.0.1/two-messages/')
+            response = self.assertResponse('views/two-messages/')
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+            response = self.assertResponse('/views/two-messages/')
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+            response = self.assertResponse('127.0.0.1/views/two-messages/')
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+
+            # Test "three messages" page url.
+            response = self.assertResponse('views/three-messages/')
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+            response = self.assertResponse('/views/three-messages/')
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
+            response = self.assertResponse('127.0.0.1/views/three-messages/')
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
 
             # Test "user detail" page url via args.
             response = self.assertResponse('user/detail/1/')
-            self.assertEqual(response.url, '127.0.0.1/user/detail/1/')
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
             response = self.assertResponse('/user/detail/1/')
-            self.assertEqual(response.url, '127.0.0.1/user/detail/1/')
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
             response = self.assertResponse('127.0.0.1/user/detail/1/')
-            self.assertEqual(response.url, '127.0.0.1/user/detail/1/')
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
 
             # Test "user detail" page url via kwargs.
             response = self.assertResponse('user/detail/2/')
-            self.assertEqual(response.url, '127.0.0.1/user/detail/2/')
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
             response = self.assertResponse('/user/detail/2/')
-            self.assertEqual(response.url, '127.0.0.1/user/detail/2/')
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
             response = self.assertResponse('127.0.0.1/user/detail/2/')
-            self.assertEqual(response.url, '127.0.0.1/user/detail/2/')
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
 
         with self.subTest('With no site_root_url value defined - Via reverse()'):
             # Test "index" page url.
             response = self.assertResponse('django_expanded_test_cases:index')
-            self.assertEqual(response.url, '127.0.0.1/')
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
 
             # Test "login" page url.
             response = self.assertResponse('django_expanded_test_cases:login')
-            self.assertEqual(response.url, '127.0.0.1/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('127.0.0.1/login/', response.full_url)
 
             # Test "one message" page url.
-            response = self.assertResponse('django_expanded_test_cases:one-message')
-            self.assertEqual(response.url, '127.0.0.1/one-message/')
+            response = self.assertResponse('django_expanded_test_cases:response-with-one-message')
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('127.0.0.1/views/one-message/', response.full_url)
 
             # Test "two messages" page url.
-            response = self.assertResponse('django_expanded_test_cases:two-messages')
-            self.assertEqual(response.url, '127.0.0.1/two-messages/')
-
-            # Test "user detail" page url via args.
-            response = self.assertResponse('django_expanded_test_cases:user-detail', args=(1,))
-            self.assertEqual(response.url, '127.0.0.1/user/detail/1/')
-
-            # Test "user detail" page url via kwargs.
-            response = self.assertResponse('django_expanded_test_cases:user-detail', kwargs={'pk': 2})
-            self.assertEqual(response.url, '127.0.0.1/user/detail/2/')
+            response = self.assertResponse('django_expanded_test_cases:response-with-two-messages')
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('127.0.0.1/views/two-messages/', response.full_url)
+
+            # Test "three messages" page url.
+            response = self.assertResponse('django_expanded_test_cases:response-with-three-messages')
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('127.0.0.1/views/three-messages/', response.full_url)
 
         with self.subTest('With custom site_root_url value defined'):
             self.site_root_url = 'https://my_really_cool_site.com/'
 
             # Test "index" page url.
             response = self.assertResponse('django_expanded_test_cases:index')
-            self.assertEqual(response.url, 'https://my_really_cool_site.com/')
+            self.assertText('/', response.url)
+            self.assertText('https://my_really_cool_site.com/', response.full_url)
 
             # Test "login" page url.
             response = self.assertResponse('django_expanded_test_cases:login')
-            self.assertEqual(response.url, 'https://my_really_cool_site.com/login/')
+            self.assertText('/login/', response.url)
+            self.assertText('https://my_really_cool_site.com/login/', response.full_url)
 
             # Test "one message" page url.
-            response = self.assertResponse('django_expanded_test_cases:one-message')
-            self.assertEqual(response.url, 'https://my_really_cool_site.com/one-message/')
+            response = self.assertResponse('django_expanded_test_cases:response-with-one-message')
+            self.assertText('/views/one-message/', response.url)
+            self.assertText('https://my_really_cool_site.com/views/one-message/', response.full_url)
 
             # Test "two messages" page url.
-            response = self.assertResponse('django_expanded_test_cases:two-messages')
-            self.assertEqual(response.url, 'https://my_really_cool_site.com/two-messages/')
+            response = self.assertResponse('django_expanded_test_cases:response-with-two-messages')
+            self.assertText('/views/two-messages/', response.url)
+            self.assertText('https://my_really_cool_site.com/views/two-messages/', response.full_url)
+
+            # Test "three messages" page url.
+            response = self.assertResponse('django_expanded_test_cases:response-with-three-messages')
+            self.assertText('/views/three-messages/', response.url)
+            self.assertText('https://my_really_cool_site.com/views/three-messages/', response.full_url)
+
+    def test__assertResponse__url__with_args(self):
+        """
+        Tests URL value returned response object in assertResponse() function.
+        """
+        with self.subTest('With no site_root_url value defined - Via standard args/kwargs'):
 
             # Test "user detail" page url via args.
             response = self.assertResponse('django_expanded_test_cases:user-detail', args=(1,))
-            self.assertEqual(response.url, 'https://my_really_cool_site.com/user/detail/1/')
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
 
             # Test "user detail" page url via kwargs.
             response = self.assertResponse('django_expanded_test_cases:user-detail', kwargs={'pk': 2})
-            self.assertEqual(response.url, 'https://my_really_cool_site.com/user/detail/2/')
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+            # Test "user detail" page url via args plus query params.
+            response = self.assertResponse(
+                'django_expanded_test_cases:user-detail',
+                args=(1,),
+                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+            )
+            self.assertText('/user/detail/1/?test_1=aaa&test_2=bbb', response.url)
+            self.assertText('127.0.0.1/user/detail/1/?test_1=aaa&test_2=bbb', response.full_url)
+
+            # Test "user detail" page url via kwargs plus query params.
+            response = self.assertResponse(
+                'django_expanded_test_cases:user-detail',
+                kwargs={'pk': 2},
+                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+            )
+            self.assertText('/user/detail/2/?test_1=aaa&test_2=bbb', response.url)
+            self.assertText('127.0.0.1/user/detail/2/?test_1=aaa&test_2=bbb', response.full_url)
+
+        with self.subTest('With no site_root_url value defined - Via url_args/url_kwargs'):
+
+            # Test "user detail" page url via args.
+            response = self.assertResponse('django_expanded_test_cases:user-detail', url_args=(1,))
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertResponse('django_expanded_test_cases:user-detail', url_kwargs={'pk': 2})
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+            # Test "user detail" page url via args plus query params.
+            response = self.assertResponse(
+                'django_expanded_test_cases:user-detail',
+                url_args=(1,),
+                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+            )
+            self.assertText('/user/detail/1/?test_1=aaa&test_2=bbb', response.url)
+            self.assertText('127.0.0.1/user/detail/1/?test_1=aaa&test_2=bbb', response.full_url)
+
+            # Test "user detail" page url via kwargs plus query params.
+            response = self.assertResponse(
+                'django_expanded_test_cases:user-detail',
+                url_kwargs={'pk': 2},
+                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+            )
+            self.assertText('/user/detail/2/?test_1=aaa&test_2=bbb', response.url)
+            self.assertText('127.0.0.1/user/detail/2/?test_1=aaa&test_2=bbb', response.full_url)
+
+        with self.subTest('With no site_root_url value defined - Via reverse()'):
+
+            # Test "user detail" page url via args.
+            response = self.assertResponse(reverse('django_expanded_test_cases:user-detail', args=(1,)))
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertResponse(reverse('django_expanded_test_cases:user-detail', kwargs={'pk': 2}))
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+            # Test "user detail" page url via args plus query params.
+            response = self.assertResponse(
+                reverse('django_expanded_test_cases:user-detail', args=(1,)),
+                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+            )
+            self.assertText('/user/detail/1/?test_1=aaa&test_2=bbb', response.url)
+            self.assertText('127.0.0.1/user/detail/1/?test_1=aaa&test_2=bbb', response.full_url)
+
+            # Test "user detail" page url via kwargs plus query params.
+            response = self.assertResponse(
+                reverse('django_expanded_test_cases:user-detail', kwargs={'pk': 2}),
+                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+            )
+            self.assertText('/user/detail/2/?test_1=aaa&test_2=bbb', response.url)
+            self.assertText('127.0.0.1/user/detail/2/?test_1=aaa&test_2=bbb', response.full_url)
+
+        with self.subTest('With custom site_root_url value defined'):
+            self.site_root_url = 'https://my_really_cool_site.com/'
+
+            # Test "user detail" page url via args.
+            response = self.assertResponse(
+                'django_expanded_test_cases:user-detail',
+                args=(1,),
+                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+            )
+            self.assertText('/user/detail/1/?test_1=aaa&test_2=bbb', response.url)
+            self.assertText('https://my_really_cool_site.com/user/detail/1/?test_1=aaa&test_2=bbb', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertResponse(
+                'django_expanded_test_cases:user-detail',
+                kwargs={'pk': 2},
+                url_query_params={'test_1': 'aaa', 'test_2': 'bbb'},
+            )
+            self.assertText('/user/detail/2/?test_1=aaa&test_2=bbb', response.url)
+            self.assertText('https://my_really_cool_site.com/user/detail/2/?test_1=aaa&test_2=bbb', response.full_url)
+
+    def test__assertResponse__url__with_query_params(self):
+        """
+        Tests URL value returned response object in assertResponse() function.
+        """
+        with self.subTest('Login page with "next" built into url - No ending slash'):
+            # Test base url.
+            response = self.assertResponse('/login?next=%2Fhome_page%2F')
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+            # Test with site root.
+            response = self.assertResponse('127.0.0.1/login?next=%2Fhome_page%2F')
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+        with self.subTest('Login page with "next" built into url - With ending slash'):
+            # Test base url.
+            response = self.assertResponse('/login/?next=%2Fhome_page%2F')
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+            # Test with site root.
+            response = self.assertResponse('127.0.0.1/login/?next=%2Fhome_page%2F')
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+        with self.subTest('Login page with "next" built via generate_get_url() function - No ending slash'):
+            # Test base url.
+            response = self.assertResponse(self.generate_get_url('/login', next='/home_page/'))
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+            # Test with site root.
+            response = self.assertResponse(self.generate_get_url('/login', next='/home_page/'))
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+        with self.subTest('Login page with "next" built via generate_get_url() function - With ending slash'):
+            # Test base url.
+            response = self.assertResponse(self.generate_get_url('/login/', next='/home_page/'))
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+            # Test with site root.
+            response = self.assertResponse(self.generate_get_url('/login/', next='/home_page/'))
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+        with self.subTest('Login page with "next" provided as query_param kwarg - No ending slash'):
+            # Test base url.
+            response = self.assertResponse('/login', url_query_params={'next': '/home_page/'})
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+            # Test with site root.
+            response = self.assertResponse('127.0.0.1/login', url_query_params={'next': '/home_page/'})
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+        with self.subTest('Login page with "next" provided as query_param kwarg - With ending slash'):
+            # Test base url.
+            response = self.assertResponse('/login/', url_query_params={'next': '/home_page/'})
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
+
+            # Test with site root.
+            response = self.assertResponse('127.0.0.1/login/', url_query_params={'next': '/home_page/'})
+            self.assertText('/login/?next=%2Fhome_page%2F', response.url)
+            self.assertText('127.0.0.1/login/?next=%2Fhome_page%2F', response.full_url)
 
     def test__assertResponse__url_redirect(self):
         """
         Tests "url_redirect" functionality of assertResponse() function.
         """
         exception_msg = 'Response didn\'t redirect as expected. Response code was 200 (expected 302).'
 
@@ -160,33 +379,170 @@
             )
 
         with self.subTest('With view that does not redirect'):
             # Using direct url.
             self.assertResponse('')
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('', expected_redirect_url='/')
-            self.assertEqual(str(err.exception), exception_msg)
+            self.assertText(exception_msg, str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('', expected_redirect_url='django_expanded_test_cases:index')
-            self.assertEqual(str(err.exception), exception_msg)
+            self.assertText(exception_msg, str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('login/', expected_redirect_url='django_expanded_test_cases:index')
-            self.assertEqual(str(err.exception), exception_msg)
+            self.assertText(exception_msg, str(err.exception))
 
             # Using reverse.
             self.assertResponse('django_expanded_test_cases:index')
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_redirect_url='/')
-            self.assertEqual(str(err.exception), exception_msg)
+            self.assertText(exception_msg, str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_redirect_url='django_expanded_test_cases:index')
-            self.assertEqual(str(err.exception), exception_msg)
+            self.assertText(exception_msg, str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:login', expected_redirect_url='django_expanded_test_cases:index')
-            self.assertEqual(str(err.exception), exception_msg)
+            self.assertText(exception_msg, str(err.exception))
+
+    def test__assertResponse__url_redirect__with_args(self):
+        """
+        Tests "url_redirect" functionality of assertResponse() function,
+        when accessing a view via url args.
+        """
+
+        with self.subTest('Provide via standard reverse'):
+
+            # Reverse, as args.
+            self.assertResponse(
+
+                # Standard url reverse, as the passed url.
+                reverse(
+                    'django_expanded_test_cases:redirect-with-args',
+                    args=(1, 'As standard url reverse() args'),
+                ),
+
+                # Url we expect to end up at.
+                expected_redirect_url=reverse(
+                    'django_expanded_test_cases:template-response-with-args',
+                    args=(1, 'As standard url reverse() args'),
+                ),
+
+                # Expected content on final page.
+                expected_content=[
+                    'id: "1"',
+                    'name: "As standard url reverse() args"',
+                ],
+            )
+
+            # Reverse, as kwargs.
+            self.assertResponse(
+
+                # Standard url reverse, as the passed url.
+                reverse(
+                    'django_expanded_test_cases:redirect-with-args',
+                    kwargs={'id': 2, 'name': 'As standard url reverse() kwargs'},
+                ),
+
+                # Url we expect to end up at.
+                expected_redirect_url=reverse(
+                    'django_expanded_test_cases:template-response-with-args',
+                    kwargs={'id': 2, 'name': 'As standard url reverse() kwargs'},
+                ),
+
+                # Expected content on final page.
+                expected_content=[
+                    'id: "2"',
+                    'name: "As standard url reverse() kwargs"',
+                ],
+            )
+
+        with self.subTest('Provide via individually passed values'):
+
+            # As args.
+            self.assertResponse(
+
+                # Desired url, as standard reverse string.
+                'django_expanded_test_cases:redirect-with-args',
+
+                # Individual args to use for url.
+                3,
+                'As passed args',
+
+                # Url we expect to end up at.
+                expected_redirect_url=reverse(
+                    'django_expanded_test_cases:template-response-with-args',
+                    args=(3, 'As passed args'),
+                ),
+
+                # Expected content on final page.
+                expected_content=[
+                    'id: "3"',
+                    'name: "As passed args"',
+                ],
+            )
+
+            # As kwargs.
+            self.assertResponse(
+                # Desired url, as standard reverse string.
+                'django_expanded_test_cases:redirect-with-args',
+
+                # Url we expect to end up at.
+                expected_redirect_url=reverse(
+                    'django_expanded_test_cases:template-response-with-args',
+                    args=(6, 'As individually passed kwargs'),
+                ),
+
+                # Individual args to use for url.
+                id=6,
+                name='As individually passed kwargs',
+
+                # Expected content on final page.
+                expected_content=[
+                    'id: "6"',
+                    'name: "As individually passed kwargs"',
+                ],
+            )
+
+        with self.subTest('Provide via args keyword'):
+            self.assertResponse(
+                # Desired url, as standard reverse string.
+                'django_expanded_test_cases:redirect-with-args',
+
+                # Url we expect to end up at.
+                expected_redirect_url='django_expanded_test_cases:template-response-with-args',
+
+                # Args for url.
+                url_args=[4, 'As url_args'],
+                redirect_args=(4, 'As url_args'),
+
+                # Expected content on final page.
+                expected_content=[
+                    'id: "4"',
+                    'name: "As url_args"',
+                ],
+            )
+
+        with self.subTest('Provide via kwargs keyword'):
+            self.assertResponse(
+                # Desired url, as standard reverse string.
+                'django_expanded_test_cases:redirect-with-args',
+
+                # Url we expect to end up at.
+                expected_redirect_url='django_expanded_test_cases:template-response-with-args',
+
+                # Args for url.
+                url_kwargs={'id': 5, 'name': 'As redirect_args'},
+                redirect_kwargs={'id': 5, 'name': 'As redirect_args'},
+
+                # Expected content on final page.
+                expected_content=[
+                    'id: "5"',
+                    'name: "As redirect_args"',
+                ],
+            )
 
     def test__assertResponse__status_code(self):
         """
         Tests "status_code" functionality of assertResponse() function.
         """
         exception_msg = '{0} != {1} : Expected status code (after potential redirects) of "{1}". Actual code was "{0}".'
 
@@ -198,15 +554,15 @@
             # Test 200 in reverse() url.
             response = self.assertResponse('django_expanded_test_cases:index')
             self.assertEqual(response.status_code, 200)
 
             # With non-200 code provided.
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_status=400)
-            self.assertEqual(str(err.exception), exception_msg.format(200, 400))
+            self.assertText(exception_msg.format(200, 400), str(err.exception))
 
         with self.subTest('With status_code=200 - View with params'):
             # Test 200 in direct url.
             response = self.assertResponse('user/detail/1/')
             self.assertEqual(response.status_code, 200)
 
             # Test 200 in reverse() url, via args.
@@ -216,15 +572,15 @@
             # Test 200 in reverse() url, via kwargs.
             response = self.assertResponse('django_expanded_test_cases:user-detail', kwargs={'pk': 3})
             self.assertEqual(response.status_code, 200)
 
             # With non-200 code provided.
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('user/detail/1/', expected_status=500)
-            self.assertEqual(str(err.exception), exception_msg.format(200, 500))
+            self.assertText(exception_msg.format(200, 500), str(err.exception))
 
         with self.subTest('With status_code=404'):
             # Test 404 in direct url.
             response = self.assertResponse('bad_url', expected_status=404)
             self.assertEqual(response.status_code, 404)
 
             # Test 404 in reverse() url, via args.
@@ -234,15 +590,15 @@
             # Test 404 in reverse() url, via kwargs.
             response = self.assertResponse('django_expanded_test_cases:user-detail', kwargs={'pk': 345}, expected_status=404)
             self.assertEqual(response.status_code, 404)
 
             # With non-404 code provided.
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('bad_url', expected_status=200)
-            self.assertEqual(str(err.exception), exception_msg.format(404, 200))
+            self.assertText(exception_msg.format(404, 200), str(err.exception))
 
     def test__assertResponse__expected_title(self):
         """
         Tests "expected_title" functionality of assertResponse() function.
         """
         exception_msg = (
             'Expected title HTML contents of "Wrong Title" (using exact matching). '
@@ -251,70 +607,70 @@
 
         with self.subTest('Title match'):
             self.assertResponse('django_expanded_test_cases:index', expected_title='Home Page | Test Views')
 
         with self.subTest('Title mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_title='Wrong Title')
-            self.assertEqual(str(err.exception), exception_msg)
+            self.assertText(exception_msg, str(err.exception))
 
     def test__assertResponse__expected_header(self):
         """
         Tests "expected_header" functionality of assertResponse() function.
         """
         exception_msg = 'Expected H1 header HTML contents of "Wrong Header". Actual value was "Home Page Header".'
 
         with self.subTest('Header match'):
             self.assertResponse('django_expanded_test_cases:index', expected_header='Home Page Header')
 
         with self.subTest('Header mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_header='Wrong Header')
-            self.assertEqual(str(err.exception), exception_msg)
+            self.assertText(exception_msg, str(err.exception))
 
     def test__assertResponse__expected_messages(self):
         """
         Tests "expected_messages" functionality of assertResponse() function.
         """
-        exception_msg = 'Failed to find message "{0}" in context (Partial matching {1} allowed).'
+        exception_msg = 'Failed to find message "{0}" in context (using {1} matching).'
 
         with self.subTest('No messages on page - match'):
             self.assertResponse('django_expanded_test_cases:index', expected_messages='')
             self.assertResponse('django_expanded_test_cases:index', expected_messages=[''])
 
         with self.subTest('No messages on page - mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_messages='Wrong message.')
-            self.assertEqual(str(err.exception), exception_msg.format('Wrong message.', 'is'))
+            self.assertText(exception_msg.format('Wrong message.', 'exact'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_messages=['Wrong message.'])
-            self.assertEqual(str(err.exception), exception_msg.format('Wrong message.', 'is'))
+            self.assertText(exception_msg.format('Wrong message.', 'exact'), str(err.exception))
 
         with self.subTest('Multiple messages on page - match'):
-            self.assertResponse('django_expanded_test_cases:three-messages', expected_messages='Test info message.')
-            self.assertResponse('django_expanded_test_cases:three-messages', expected_messages=['Test warning message.'])
+            self.assertResponse('django_expanded_test_cases:response-with-three-messages', expected_messages='Test info message.')
+            self.assertResponse('django_expanded_test_cases:response-with-three-messages', expected_messages=['Test warning message.'])
             self.assertResponse(
-                'django_expanded_test_cases:three-messages',
+                'django_expanded_test_cases:response-with-three-messages',
                 expected_messages=['Test info message.', 'Test warning message.'],
             )
             self.assertResponse(
-                'django_expanded_test_cases:three-messages',
+                'django_expanded_test_cases:response-with-three-messages',
                 expected_messages=['Test info message.', 'Test warning message.', 'Test error message.'],
             )
 
         with self.subTest('Multiple messages on page - mismatch'):
             with self.assertRaises(AssertionError) as err:
-                self.assertResponse('django_expanded_test_cases:three-messages', expected_messages='Wrong message.')
-            self.assertEqual(str(err.exception), exception_msg.format('Wrong message.', 'is'))
+                self.assertResponse('django_expanded_test_cases:response-with-three-messages', expected_messages='Wrong message.')
+            self.assertText(exception_msg.format('Wrong message.', 'exact'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse(
-                    'django_expanded_test_cases:three-messages',
+                    'django_expanded_test_cases:response-with-three-messages',
                     expected_messages=['Test info message.', 'Wrong message.'],
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('Wrong message.', 'is'))
+            self.assertText(exception_msg.format('Wrong message.', 'exact'), str(err.exception))
 
     def test__assertResponse__expected_content(self):
         """
         Tests "expected_content" functionality of assertResponse() function.
         """
         exception_msg = 'Could not find expected content value in response. Provided value was:\n{0}'
 
@@ -367,25 +723,25 @@
                 ],
                 ignore_content_ordering=True,  # Ignore because we recheck the same values.
             )
 
         with self.subTest('Content mismatch'):
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse('django_expanded_test_cases:index', expected_content='Wrong value')
-            self.assertEqual(str(err.exception), exception_msg.format('Wrong value'))
+            self.assertText(exception_msg.format('Wrong value'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertResponse(
                     'django_expanded_test_cases:index',
                     expected_content=[
                         'Home Page Header',
                         'Pretend this is',
-                        'Wrong value'
+                        'Wrong value',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('Wrong value'))
+            self.assertTextStartsWith(exception_msg.format('Wrong value'), str(err.exception))
 
         with self.subTest('With search subsections'):
             # Strip start.
             self.assertResponse(
                 'django_expanded_test_cases:index',
                 expected_content='<p>Pretend this is the project landing page.</p>',
                 content_starts_after='<h1>Home Page Header</h1>',
@@ -480,29 +836,169 @@
 
     def test__assertGetResponse(self):
         """
         Tests assertGetResponse() function.
         Note: Most logic in here passes into the assertResponse() function.
             Thus we just do basic checks here and do most of the heavy-testing in assertResponse().
         """
-        response = self.assertGetResponse('django_expanded_test_cases:index')
 
-        self.assertEqual(response.url, '127.0.0.1/')
-        self.assertEqual(response.status_code, 200)
+        with self.subTest('Basic response test.'):
+            response = self.assertGetResponse('django_expanded_test_cases:index')
+
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+            self.assertEqual(response.status_code, 200)
+
+        with self.subTest('View with params, provided as standard args/kwargs'):
+            # Test "user detail" page url via args.
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:user-detail',
+                args=(1,),
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_superuser"</p></li>',
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:user-detail',
+                kwargs={'pk': 2},
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_admin"</p></li>',
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+        with self.subTest('View with params, provided as url_args/url_kwargs'):
+            # Test "user detail" page url via args.
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:user-detail',
+                url_args=(1,),
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_superuser"</p></li>',
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertGetResponse(
+                'django_expanded_test_cases:user-detail',
+                url_kwargs={'pk': 2},
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_admin"</p></li>',
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+        with self.subTest('View with params, provided as reverse()'):
+            # Test "user detail" page url via args.
+            response = self.assertGetResponse(
+                reverse('django_expanded_test_cases:user-detail', args=(1,)),
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_superuser"</p></li>',
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertGetResponse(
+                reverse('django_expanded_test_cases:user-detail', kwargs={'pk': 2}),
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_admin"</p></li>',
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
 
     def test__assertPostResponse(self):
         """
         Tests assertPostResponse() function.
         Note: Most logic in here passes into the assertResponse() function.
             Thus we just do basic checks here and do most of the heavy-testing in assertResponse().
         """
-        response = self.assertPostResponse('django_expanded_test_cases:index')
 
-        self.assertEqual(response.url, '127.0.0.1/')
-        self.assertEqual(response.status_code, 200)
+        with self.subTest('Basic response test.'):
+            response = self.assertPostResponse('django_expanded_test_cases:index')
+
+            self.assertText('/', response.url)
+            self.assertText('127.0.0.1/', response.full_url)
+            self.assertEqual(response.status_code, 200)
+
+        with self.subTest('View with params, provided as standard args/kwargs'):
+            # Test "user detail" page url via args.
+            response = self.assertPostResponse(
+                'django_expanded_test_cases:user-detail',
+                args=(1,),
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_superuser"</p></li>',
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertPostResponse(
+                'django_expanded_test_cases:user-detail',
+                kwargs={'pk': 2},
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_admin"</p></li>',
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+        with self.subTest('View with params, provided as url_args/url_kwargs'):
+            # Test "user detail" page url via args.
+            response = self.assertPostResponse(
+                'django_expanded_test_cases:user-detail',
+                url_args=(1,),
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_superuser"</p></li>',
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertPostResponse(
+                'django_expanded_test_cases:user-detail',
+                url_kwargs={'pk': 2},
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_admin"</p></li>',
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
+
+        with self.subTest('View with params, provided as reverse()'):
+            # Test "user detail" page url via args.
+            response = self.assertPostResponse(
+                reverse('django_expanded_test_cases:user-detail', args=(1,)),
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_superuser"</p></li>',
+            )
+            self.assertText('/user/detail/1/', response.url)
+            self.assertText('127.0.0.1/user/detail/1/', response.full_url)
+
+            # Test "user detail" page url via kwargs.
+            response = self.assertPostResponse(
+                reverse('django_expanded_test_cases:user-detail', kwargs={'pk': 2}),
+                expected_title='User Detail Page | Test Views',
+                expected_header='User Detail Page Header',
+                expected_content='<li><p>Username: "test_admin"</p></li>',
+            )
+            self.assertText('/user/detail/2/', response.url)
+            self.assertText('127.0.0.1/user/detail/2/', response.full_url)
 
     # endregion Response Assertion Tests
 
     # region Element Assertion Tests
 
     def test__assertResponseRedirects__success(self):
         """
@@ -526,36 +1022,36 @@
         """
         exception_msg = 'Response didn\'t redirect as expected. Response code was {0} (expected 302).'
 
         with self.subTest('With view that does not redirect - Invalid page'):
             request = self._get_page_response('bad_page/')
             with self.assertRaises(AssertionError) as err:
                 self.assertRedirects(request, expected_redirect_url='/')
-            self.assertEqual(str(err.exception), exception_msg.format(request.status_code))
+            self.assertText(exception_msg.format(request.status_code), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertRedirects(request, expected_redirect_url='django_expanded_test_cases:invalid')
-            self.assertEqual(str(err.exception), exception_msg.format(request.status_code))
+            self.assertText(exception_msg.format(request.status_code), str(err.exception))
 
         with self.subTest('With view that does not redirect - Index page'):
             request = self._get_page_response('')
             with self.assertRaises(AssertionError) as err:
                 self.assertRedirects(request, expected_redirect_url='/')
-            self.assertEqual(str(err.exception), exception_msg.format(request.status_code))
+            self.assertText(exception_msg.format(request.status_code), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertRedirects(request, expected_redirect_url='django_expanded_test_cases:index')
-            self.assertEqual(str(err.exception), exception_msg.format(request.status_code))
+            self.assertText(exception_msg.format(request.status_code), str(err.exception))
 
         with self.subTest('With view that does not redirect - Non-index page'):
             request = self._get_page_response('login/')
             with self.assertRaises(AssertionError) as err:
                 self.assertRedirects(request, expected_redirect_url='/')
-            self.assertEqual(str(err.exception), exception_msg.format(request.status_code))
+            self.assertText(exception_msg.format(request.status_code), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertRedirects(request, expected_redirect_url='django_expanded_test_cases:login')
-            self.assertEqual(str(err.exception), exception_msg.format(request.status_code))
+            self.assertText(exception_msg.format(request.status_code), str(err.exception))
 
     def test__assertStatusCode__success(self):
         """
         Tests assertStatusCode() function, in cases when it should succeed.
         """
         with self.subTest('Status 200'):
             response = HttpResponse(status=200)
@@ -588,45 +1084,45 @@
         """
         exception_msg = '{0} != {1} : Expected status code (after potential redirects) of "{1}". Actual code was "{0}".'
 
         with self.subTest('Expected 200, got 404'):
             response = HttpResponse(status=404)
             with self.assertRaises(AssertionError) as err:
                 self.assertStatusCode(response, 200)
-            self.assertEqual(str(err.exception), exception_msg.format('404', '200'))
+            self.assertText(exception_msg.format('404', '200'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertStatusCode(response.status_code, 200)
-            self.assertEqual(str(err.exception), exception_msg.format('404', '200'))
+            self.assertText(exception_msg.format('404', '200'), str(err.exception))
 
         with self.subTest('Expected 404, got 200'):
             response = HttpResponse(status=200)
             with self.assertRaises(AssertionError) as err:
                 self.assertStatusCode(response, 404)
-            self.assertEqual(str(err.exception), exception_msg.format('200', '404'))
+            self.assertText(exception_msg.format('200', '404'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertStatusCode(response.status_code, 404)
-            self.assertEqual(str(err.exception), exception_msg.format('200', '404'))
+            self.assertText(exception_msg.format('200', '404'), str(err.exception))
 
         with self.subTest('Expected 200, got 500'):
             response = HttpResponse(status=500)
             with self.assertRaises(AssertionError) as err:
                 self.assertStatusCode(response, 200)
-            self.assertEqual(str(err.exception), exception_msg.format('500', '200'))
+            self.assertText(exception_msg.format('500', '200'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertStatusCode(response.status_code, 200)
-            self.assertEqual(str(err.exception), exception_msg.format('500', '200'))
+            self.assertText(exception_msg.format('500', '200'), str(err.exception))
 
         with self.subTest('Expected 500, got 200'):
             response = HttpResponse(status=200)
             with self.assertRaises(AssertionError) as err:
                 self.assertStatusCode(response, 500)
-            self.assertEqual(str(err.exception), exception_msg.format('200', '500'))
+            self.assertText(exception_msg.format('200', '500'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertStatusCode(response.status_code, 500)
-            self.assertEqual(str(err.exception), exception_msg.format('200', '500'))
+            self.assertText(exception_msg.format('200', '500'), str(err.exception))
 
     def test__assertPageTitle__success(self):
         """
         Tests assertPageTitle() function, in cases when it should succeed.
         """
         with self.subTest('Including title tag in expected'):
             response = HttpResponse('<title>Test Title</title>')
@@ -654,162 +1150,174 @@
 
         with self.subTest('Basic title, with extra whitespace (to simulate Django templating)'):
             response = HttpResponse('<title>   Test    Title   </title>')
             self.assertPageTitle(response, 'Test Title')
 
         with self.subTest('Complex title - Exact Match'):
             response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
-            self.assertPageTitle(response, 'Test Title | My Custom App | My Really Cool Site', exact_match=True)
+            self.assertPageTitle(response, 'Test Title | My Custom App | My Really Cool Site', allow_partials=False)
 
         with self.subTest('Complex title, with extra whitespace (to simulate Django templating) - Exact Match'):
             response = HttpResponse(
                 '<title>   Test   Title    \n|\n   My Custom App   \n|\n   My Really Cool Site   </title>'
             )
-            self.assertPageTitle(response, 'Test Title | My Custom App | My Really Cool Site', exact_match=True)
+            self.assertPageTitle(response, 'Test Title | My Custom App | My Really Cool Site', allow_partials=False)
 
         with self.subTest('Complex title - Loose Match'):
             response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
-            self.assertPageTitle(response, 'Test Title', exact_match=False)
-            self.assertPageTitle(response, 'My Custom App', exact_match=False)
-            self.assertPageTitle(response, 'My Really Cool Site', exact_match=False)
+            self.assertPageTitle(response, 'Test Title', allow_partials=True)
+            self.assertPageTitle(response, 'My Custom App', allow_partials=True)
+            self.assertPageTitle(response, 'My Really Cool Site', allow_partials=True)
 
         with self.subTest('Complex title, with extra whitespace (to simulate Django templating) - Loose Match'):
             response = HttpResponse(
                 '<title>   Test   Title    \n|\n   My Custom App   \n|\n   My Really Cool Site   </title>'
             )
-            self.assertPageTitle(response, 'Test Title', exact_match=False)
-            self.assertPageTitle(response, 'My Custom App', exact_match=False)
-            self.assertPageTitle(response, 'My Really Cool Site', exact_match=False)
+            self.assertPageTitle(response, 'Test Title', allow_partials=True)
+            self.assertPageTitle(response, 'My Custom App', allow_partials=True)
+            self.assertPageTitle(response, 'My Really Cool Site', allow_partials=True)
 
     def test__assertPageTitle__failure(self):
         """
         Tests assertPageTitle() function, in cases when it should fail.
         """
-        exception_msg = 'Expected title HTML contents of "{0}" (using exact matching). Actual value was "{1}".'
+        exception_msg = 'Expected title HTML contents of "{0}" (using {2} matching). Actual value was "{1}".'
 
         with self.subTest('Checking for title when none exists'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertPageTitle(response, 'Test Title')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Title', ''))
+            self.assertText(exception_msg.format('Test Title', '', 'exact'), str(err.exception))
 
         with self.subTest('Expected value is on page, but not in title tag'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('Test Title')
                 self.assertPageTitle(response, 'Test Title')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Title', ''))
+            self.assertText(exception_msg.format('Test Title', '', 'exact'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1><p>Test Title</p>')
                 self.assertPageTitle(response, 'Test Title')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Title', ''))
+            self.assertText(exception_msg.format('Test Title', '', 'exact'), str(err.exception))
 
         with self.subTest('Assuming extra whitespace is still present'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>   Test    Title   </title>')
                 self.assertPageTitle(response, '   Test    Title   ')
-            self.assertEqual(str(err.exception), exception_msg.format('Test    Title', 'Test Title'))
+            self.assertText(exception_msg.format('Test    Title', 'Test Title', 'exact'), str(err.exception))
 
         with self.subTest('Set to exact match, but only passing in title subsection'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
                 self.assertPageTitle(response, 'Test Title')
-            self.assertEqual(str(err.exception), exception_msg.format(
-                'Test Title',
-                'Test Title | My Custom App | My Really Cool Site',
-            ))
+            self.assertText(
+                exception_msg.format(
+                    'Test Title',
+                    'Test Title | My Custom App | My Really Cool Site',
+                    'exact',
+                ),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
                 self.assertPageTitle(response, 'My Custom App')
-            self.assertEqual(str(err.exception), exception_msg.format(
-                'My Custom App',
-                'Test Title | My Custom App | My Really Cool Site',
-            ))
+            self.assertText(
+                exception_msg.format(
+                    'My Custom App',
+                    'Test Title | My Custom App | My Really Cool Site',
+                    'exact',
+                ),
+                str(err.exception),
+            )
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
                 self.assertPageTitle(response, 'My Really Cool Site')
-            self.assertEqual(str(err.exception), exception_msg.format(
-                'My Really Cool Site',
-                'Test Title | My Custom App | My Really Cool Site',
-            ))
+            self.assertText(
+                exception_msg.format(
+                    'My Really Cool Site',
+                    'Test Title | My Custom App | My Really Cool Site',
+                    'exact',
+                ),
+                str(err.exception),
+            )
 
         with self.subTest('Set to partial match, but value is not in title'):
             # Full mismatch.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('Test Title')
-                self.assertPageTitle(response, 'Wrong Value')
-            self.assertEqual(str(err.exception), exception_msg.format('Wrong Value', ''))
+                self.assertPageTitle(response, 'Wrong Value', allow_partials=True)
+            self.assertText(exception_msg.format('Wrong Value', '', 'partial'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Test Title</title>')
-                self.assertPageTitle(response, 'Wrong Value')
-            self.assertEqual(str(err.exception), exception_msg.format('Wrong Value', 'Test Title'))
+                self.assertPageTitle(response, 'Wrong Value', allow_partials=True)
+            self.assertText(exception_msg.format('Wrong Value', 'Test Title', 'partial'), str(err.exception))
 
             # Partial match, but also has extra.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('Test Title')
-                self.assertPageTitle(response, 'Test Title and More')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Title and More', ''))
+                self.assertPageTitle(response, 'Test Title and More', allow_partials=True)
+            self.assertText(exception_msg.format('Test Title and More', '', 'partial'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Test Title</title>')
-                self.assertPageTitle(response, 'Test Title and More')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Title and More', 'Test Title'))
+                self.assertPageTitle(response, 'Test Title and More', allow_partials=True)
+            self.assertText(exception_msg.format('Test Title and More', 'Test Title', 'partial'), str(err.exception))
 
         with self.subTest('Multiple Titles - Two and no spaces'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Title 1</title><title>Title 2</title>')
                 self.assertPageTitle(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple titles (2 total). There should only be one <title> tag per page.\n'
                     'For further reference on <title> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_title.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title'
-                )
+                ),
+                str(err.exception),
             )
 
         with self.subTest('Multiple Titles - Two with spaces'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title > Title 1 < /title><title > Title 2 < /title>')
                 self.assertPageTitle(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple titles (2 total). There should only be one <title> tag per page.\n'
                     'For further reference on <title> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_title.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title'
-                )
+                ),
+                str(err.exception),
             )
 
         with self.subTest('Multiple Titles - Two with line breaks'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Title 1</title>\n<br>\n<title>Title 2</title>')
                 self.assertPageTitle(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple titles (2 total). There should only be one <title> tag per page.\n'
                     'For further reference on <title> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_title.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title'
-                )
+                ),
+                str(err.exception),
             )
 
         with self.subTest('Multiple Titles - Three'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<title>Title 1</title><title>Title 2</title><title>Title 3</title>')
                 self.assertPageTitle(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple titles (3 total). There should only be one <title> tag per page.\n'
                     'For further reference on <title> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_title.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title'
-                )
+                ),
+                str(err.exception),
             )
 
         with self.subTest('Multiple Titles - Many, assorted'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse(
                     """
                     <title>Testing</title
@@ -817,22 +1325,22 @@
 
                     <br>
 
                     <title>Title 3</title><p>This is a test p tag.</p></title><title > Title 4 < /title><title>Title 5</title>
                     """
                 )
                 self.assertPageTitle(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple titles (5 total). There should only be one <title> tag per page.\n'
                     'For further reference on <title> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_title.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/title'
-                )
+                ),
+                str(err.exception),
             )
 
     def test__assertPageHeader__success(self):
         """
         Tests assertPageHeader() function, in cases when it should succeed.
         """
         with self.subTest('Including header tag in expected'):
@@ -869,92 +1377,92 @@
         """
         exception_msg = 'Expected H1 header HTML contents of "{0}". Actual value was "{1}".'
 
         with self.subTest('Checking for header when none exists'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertPageHeader(response, 'Test Header')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Header', ''))
+            self.assertText(exception_msg.format('Test Header', ''), str(err.exception))
 
         with self.subTest('Expected value is on page, but not in header tag'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('Test Header')
                 self.assertPageHeader(response, 'Test Header')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Header', ''))
+            self.assertText(exception_msg.format('Test Header', ''), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h2>Test Header</h2><p>Test Header</p>')
                 self.assertPageHeader(response, 'Test Header')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Header', ''))
+            self.assertText(exception_msg.format('Test Header', ''), str(err.exception))
 
         with self.subTest('Assuming extra whitespace is still present'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>   Test    Header   </h1>')
                 self.assertPageHeader(response, '   Test    Header   ')
-            self.assertEqual(str(err.exception), exception_msg.format('Test    Header', 'Test Header'))
+            self.assertText(exception_msg.format('Test    Header', 'Test Header'), str(err.exception))
 
         with self.subTest('Expected value is present, plus extra'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Header</h1>')
                 self.assertPageHeader(response, 'Test Header plus Extra')
-            self.assertEqual(str(err.exception), exception_msg.format('Test Header plus Extra', 'Test Header'))
+            self.assertText(exception_msg.format('Test Header plus Extra', 'Test Header'), str(err.exception))
 
         with self.subTest('Multiple Headers - Two and no spaces'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Header 1</h1><h1>Header 2</h1>')
                 self.assertPageHeader(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple headers (2 total). There should only be one <h1> tag per page.\n'
                     'For further reference on <h1> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_hn.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements'
-                )
+                ),
+                str(err.exception),
             )
 
         with self.subTest('Multiple Headers - Two with spaces'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1 > Header 1 < /h1><h1 > Header 2 < /h1>')
                 self.assertPageHeader(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple headers (2 total). There should only be one <h1> tag per page.\n'
                     'For further reference on <h1> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_hn.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements'
-                )
+                ),
+                str(err.exception)
             )
 
         with self.subTest('Multiple Headers - Two with line breaks'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Header 1</h1>\n<br>\n<h1>Header 2</h1>')
                 self.assertPageHeader(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple headers (2 total). There should only be one <h1> tag per page.\n'
                     'For further reference on <h1> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_hn.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements'
-                )
+                ),
+                str(err.exception),
             )
 
         with self.subTest('Multiple Headers - Three'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Header 1</h1><h1>Header 2</h1><h1>Header 3</h1>')
                 self.assertPageHeader(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple headers (3 total). There should only be one <h1> tag per page.\n'
                     'For further reference on <h1> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_hn.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements'
-                )
+                ),
+                str(err.exception),
             )
 
         with self.subTest('Multiple Headers - Many, assorted'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse(
                     """
                     <h1>Testing</h1
@@ -962,141 +1470,170 @@
 
                     <br>
 
                     <h1>Header 3</h1><p>This is a test p tag.</p></h1><h1 > Header 4 < /h1><h1>Header 5</h1>
                     """
                 )
                 self.assertPageHeader(response, '')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 (
                     'Found multiple headers (5 total). There should only be one <h1> tag per page.\n'
                     'For further reference on <h1> tags, consider consulting:\n'
                     '    * https://www.w3schools.com/tags/tag_hn.asp\n'
                     '    * https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Heading_Elements'
-                )
+                ),
+                str(err.exception),
             )
 
     @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_ALLOW_MESSAGE_PARTIALS', True)
     def test__assertContextMessages__success__allow_partials(self):
         """
         Tests assertContextMessages() function, in cases when it should succeed.
 
         We only do a minimal amount of testing for this function here.
         We assume a majority of testing will occur in the "disallow_partials" set.
         """
         with self.subTest('Check for single message partial, single message exists'):
-            response = self._get_page_response('django_expanded_test_cases:one-message')
+            response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             self.assertContextMessages(response, 'This is a test message.')
             self.assertContextMessages(response, 'is a test message')
             self.assertContextMessages(response, 'test')
 
         with self.subTest('Check for three message partials, three messages exists'):
-            response = self._get_page_response('django_expanded_test_cases:three-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
             self.assertContextMessages(response, ['info', 'warning message', 'Test error'])
 
     @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_ALLOW_MESSAGE_PARTIALS', False)
     def test__assertContextMessages__success__disallow_partials(self):
         """
         Tests assertContextMessages() function, in cases when it should succeed.
 
         The majority of tests for this function exist here.
         """
         with self.subTest('Check for single message, single message exists'):
-            response = self._get_page_response('django_expanded_test_cases:one-message')
+            response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             self.assertContextMessages(response, 'This is a test message.')
 
         with self.subTest('Check for single message, two messages exists'):
-            response = self._get_page_response('django_expanded_test_cases:two-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-two-messages')
             self.assertContextMessages(response, 'Test message #1.')
             self.assertContextMessages(response, 'Test message #2.')
 
         with self.subTest('Check for single message, three messages exists'):
-            response = self._get_page_response('django_expanded_test_cases:three-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
             self.assertContextMessages(response, 'Test info message.')
             self.assertContextMessages(response, 'Test warning message.')
             self.assertContextMessages(response, 'Test error message.')
 
         with self.subTest('Check for two messages, two messages exists'):
-            response = self._get_page_response('django_expanded_test_cases:two-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-two-messages')
             self.assertContextMessages(response, ['Test message #1.', 'Test message #2.'])
 
         with self.subTest('Check for two messages, three messages exists'):
-            response = self._get_page_response('django_expanded_test_cases:three-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
             self.assertContextMessages(response, ['Test info message.', 'Test warning message.'])
             self.assertContextMessages(response, ['Test info message.', 'Test error message.'])
             self.assertContextMessages(response, ['Test warning message.', 'Test error message.'])
 
         with self.subTest('Check for three messages, three messages exists'):
-            response = self._get_page_response('django_expanded_test_cases:three-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
             self.assertContextMessages(response, ['Test info message.', 'Test warning message.', 'Test error message.'])
 
     @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_ALLOW_MESSAGE_PARTIALS', False)
     def test__assertContextMessages__failure(self):
         """
         Tests assertContextMessages() function, in cases when it should fail.
         """
-        exception_msg = 'Failed to find message "{0}" in context (Partial matching {1} allowed).'
+        exception_msg = 'Failed to find message "{0}" in context (using {1} matching).'
 
         with self.subTest('Checking for single message, none exist'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
                 self.assertContextMessages(response, 'This is a test message.')
-            self.assertEqual(str(err.exception), exception_msg.format('This is a test message.', 'is NOT'))
+            self.assertText(exception_msg.format('This is a test message.', 'exact'), str(err.exception))
 
         with self.subTest('Checking for single message, one exists but doesn\'t match'):
             with self.assertRaises(AssertionError) as err:
-                response = self._get_page_response('django_expanded_test_cases:one-message')
+                response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
                 self.assertContextMessages(response, 'Testing!')
-            self.assertEqual(str(err.exception), exception_msg.format('Testing!', 'is NOT'))
+            self.assertText(exception_msg.format('Testing!', 'exact'), str(err.exception))
 
         with self.subTest('Checking for single message, but it\'s only a partial match'):
-            response = self._get_page_response('django_expanded_test_cases:one-message')
+            response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             with self.assertRaises(AssertionError) as err:
                 self.assertContextMessages(response, 'This is a test message')
-            self.assertEqual(str(err.exception), exception_msg.format('This is a test message', 'is NOT'))
+            self.assertText(exception_msg.format('This is a test message', 'exact'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertContextMessages(response, 'test message.')
-            self.assertEqual(str(err.exception), exception_msg.format('test message.', 'is NOT'))
+            self.assertText(exception_msg.format('test message.', 'exact'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertContextMessages(response, 'test')
-            self.assertEqual(str(err.exception), exception_msg.format('test', 'is NOT'))
+            self.assertText(exception_msg.format('test', 'exact'), str(err.exception))
 
         with self.subTest('Checking for single message, multiple exist but don\'t match'):
             with self.assertRaises(AssertionError) as err:
-                response = self._get_page_response('django_expanded_test_cases:three-messages')
+                response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
                 self.assertContextMessages(response, 'Testing!')
-            self.assertEqual(str(err.exception), exception_msg.format('Testing!', 'is NOT'))
+            self.assertText(exception_msg.format('Testing!', 'exact'), str(err.exception))
 
         with self.subTest('Checking for two messages, none exist'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
                 self.assertContextMessages(response, ['This is a test message.', 'Another message.'])
-            self.assertEqual(str(err.exception), exception_msg.format('This is a test message.', 'is NOT'))
+            self.assertText(exception_msg.format('This is a test message.', 'exact'), str(err.exception))
 
         with self.subTest('Checking for two messages, but only one exists'):
             with self.assertRaises(AssertionError) as err:
-                response = self._get_page_response('django_expanded_test_cases:one-message')
+                response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
                 self.assertContextMessages(response, ['This is a test message.', 'Another message.'])
-            self.assertEqual(str(err.exception), exception_msg.format('Another message.', 'is NOT'))
+            self.assertText(exception_msg.format('Another message.', 'exact'), str(err.exception))
 
         with self.subTest('Checking for two messages, multiple exist but one doesn\'t match'):
-            response = self._get_page_response('django_expanded_test_cases:three-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
             with self.assertRaises(AssertionError) as err:
                 self.assertContextMessages(response, ['Test info message.', 'Another message.'])
-            self.assertEqual(str(err.exception), exception_msg.format('Another message.', 'is NOT'))
+            self.assertText(exception_msg.format('Another message.', 'exact'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertContextMessages(response, ['Bad message', 'Test info message.'])
-            self.assertEqual(str(err.exception), exception_msg.format('Bad message', 'is NOT'))
+            self.assertText(exception_msg.format('Bad message', 'exact'), str(err.exception))
 
         with self.subTest('Checking for two messages, multiple exist but none match'):
             with self.assertRaises(AssertionError) as err:
-                response = self._get_page_response('django_expanded_test_cases:three-messages')
+                response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
                 self.assertContextMessages(response, ['Testing!', 'Testing again!'])
-            self.assertEqual(str(err.exception), exception_msg.format('Testing!', 'is NOT'))
+            self.assertText(exception_msg.format('Testing!', 'exact'), str(err.exception))
+
+        with self.subTest('Set to partial match, but value is not in title'):
+            # Full mismatch.
+            with self.assertRaises(AssertionError) as err:
+                response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
+                self.assertContextMessages(response, 'Wrong Value', allow_partials=True)
+            self.assertText(exception_msg.format('Wrong Value', 'partial'), str(err.exception))
+            with self.assertRaises(AssertionError) as err:
+                response = self._get_page_response('django_expanded_test_cases:response-with-two-messages')
+                self.assertContextMessages(response, 'Wrong Value', allow_partials=True)
+            self.assertText(exception_msg.format('Wrong Value', 'partial'), str(err.exception))
+            with self.assertRaises(AssertionError) as err:
+                response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
+                self.assertContextMessages(response, 'Wrong Value', allow_partials=True)
+            self.assertText(exception_msg.format('Wrong Value', 'partial'), str(err.exception))
+
+            # Partial match, but also has extra.
+            with self.assertRaises(AssertionError) as err:
+                response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
+                self.assertContextMessages(response, 'This is a test message, testing', allow_partials=True)
+            self.assertText(exception_msg.format('This is a test message, testing', 'partial'), str(err.exception))
+            with self.assertRaises(AssertionError) as err:
+                response = self._get_page_response('django_expanded_test_cases:response-with-two-messages')
+                self.assertContextMessages(response, 'This is and more', allow_partials=True)
+            self.assertText(exception_msg.format('This is and more','partial'), str(err.exception))
+            with self.assertRaises(AssertionError) as err:
+                response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
+                self.assertContextMessages(response, 'info message and more', allow_partials=True)
+            self.assertText(exception_msg.format('info message and more','partial'), str(err.exception))
 
     def test__assertPageContent__success(self):
         """
         Tests assertPageContent() function, in cases when it should succeed.
         """
         with self.subTest('Empty response, no value passed.'):
             response = HttpResponse('')
@@ -1144,15 +1681,15 @@
             self.assertPageContent(response, '<h1>Home Page Header</h1><p>Pretend this is the project landing page.</p>')
 
         with self.subTest('Standard Response - TemplateResponse Home Page'):
             response = self._get_page_response('django_expanded_test_cases:template-response-index')
             self.assertPageContent(response, '<h1>Home Page Header</h1><p>Pretend this is the project landing page.</p>')
 
         with self.subTest('Standard Response - One Message Page'):
-            response = self._get_page_response('django_expanded_test_cases:one-message')
+            response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             self.assertPageContent(
                 response,
                 (
                     '<ul><li><p>This is a test message.</p></li></ul>'
                     '<h1>View with One Message Header</h1>'
                     '<p>Pretend useful stuff is displayed here, for one-message render() view.</p>'
                 ),
@@ -1446,72 +1983,72 @@
             'Expected content value was found, but ordering of values do not match. Problem value:\n{0}'
         )
 
         with self.subTest('Empty response, but value passed.'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('<h1>Test Title</h1>'))
+            self.assertText(exception_msg_not_found.format('<h1>Test Title</h1>'), str(err.exception))
 
         with self.subTest('Minimal Response - Wrong value passed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1>')
                 self.assertPageContent(response, '<h1>Testing</h1>')
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('<h1>Testing</h1>'))
+            self.assertText(exception_msg_not_found.format('<h1>Testing</h1>'), str(err.exception))
 
         with self.subTest('Standard Response - Wrong value passed'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:login')
                 self.assertPageContent(response, '<h1>Testing Header</h1><p>Pretend this is a page.</p>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg_not_found.format('<h1>Testing Header</h1><p>Pretend this is a page.</p>'),
+                str(err.exception),
             )
 
         with self.subTest('Standard Response - Set of items with wrong values'):
             response = self._get_page_response('django_expanded_test_cases:index')
 
             # Test as list.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ['<h1>Test Page Header</h1>'])
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('<h1>Test Page Header</h1>'))
+            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Test Page Header</h1>'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ['Wrong Content'])
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('Wrong Content'))
+            self.assertTextStartsWith(exception_msg_not_found.format('Wrong Content'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ['<h1>Home Page Wrong'])
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('<h1>Home Page Wrong'))
+            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Home Page Wrong'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ['Wrong Page Header</h1>'])
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('Wrong Page Header</h1>'))
+            self.assertTextStartsWith(exception_msg_not_found.format('Wrong Page Header</h1>'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ['<h1>Home Page Header</h1>', 'Wrong text'])
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('Wrong text'))
+            self.assertTextStartsWith(exception_msg_not_found.format('Wrong text'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ['<h1>Wrong Header</h1>', 'project landing page'])
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('<h1>Wrong Header</h1>'))
+            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Wrong Header</h1>'), str(err.exception))
             # Test as tuple.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ('<h1>Test Page Header</h1>',))
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('<h1>Test Page Header</h1>'))
+            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Test Page Header</h1>'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ('Wrong Content',))
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('Wrong Content'))
+            self.assertTextStartsWith(exception_msg_not_found.format('Wrong Content'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ('<h1>Home Page Wrong',))
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('<h1>Home Page Wrong'))
+            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Home Page Wrong'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ('Wrong Page Header</h1>',))
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('Wrong Page Header</h1>'))
+            self.assertTextStartsWith(exception_msg_not_found.format('Wrong Page Header</h1>'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ('<h1>Home Page Header</h1>', 'Wrong text'))
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('Wrong text'))
+            self.assertTextStartsWith(exception_msg_not_found.format('Wrong text'), str(err.exception))
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(response, ('<h1>Wrong Header</h1>', 'project landing page'))
-            self.assertEqual(str(err.exception), exception_msg_not_found.format('<h1>Wrong Header</h1>'))
+            self.assertTextStartsWith(exception_msg_not_found.format('<h1>Wrong Header</h1>'), str(err.exception))
 
         with self.subTest('Standard Response - Wrong ordering'):
             response = self._get_page_response('django_expanded_test_cases:user-detail', args=(1,))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string at top.
                 self.assertPageContent(
@@ -1522,15 +2059,15 @@
                         'Username: "test_superuser"',
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('<h1>User Detail Page Header</h1>'))
+            self.assertTextStartsWith(exception_msg_bad_order.format('<h1>User Detail Page Header</h1>'), str(err.exception))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after header.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -1538,15 +2075,15 @@
                         'Username: "test_superuser"',
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('Username: "test_superuser"'))
+            self.assertTextStartsWith(exception_msg_bad_order.format('Username: "test_superuser"'), str(err.exception))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after last name.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -1554,15 +2091,15 @@
                         'Last Name: "SuperUserLast"',
                         'First Name: "SuperUserFirst"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "SuperUserFirst"'))
+            self.assertTextStartsWith(exception_msg_bad_order.format('First Name: "SuperUserFirst"'), str(err.exception))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after active.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -1570,15 +2107,15 @@
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'First Name: "SuperUserFirst"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "SuperUserFirst"'))
+            self.assertTextStartsWith(exception_msg_bad_order.format('First Name: "SuperUserFirst"'), str(err.exception))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after superuser.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -1586,15 +2123,15 @@
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'First Name: "SuperUserFirst"',
                         'Is Staff: "False"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "SuperUserFirst"'))
+            self.assertTextStartsWith(exception_msg_bad_order.format('First Name: "SuperUserFirst"'), str(err.exception))
 
             with self.assertRaises(AssertionError) as err:
                 # Test "first name" string after staff.
                 self.assertPageContent(
                     response,
                     [
                         '<h1>User Detail Page Header</h1>',
@@ -1602,480 +2139,480 @@
                         'Last Name: "SuperUserLast"',
                         'Is Active: "True"',
                         'Is SuperUser: "True"',
                         'Is Staff: "False"',
                         'First Name: "SuperUserFirst"',
                     ],
                 )
-            self.assertEqual(str(err.exception), exception_msg_bad_order.format('First Name: "SuperUserFirst"'))
+            self.assertTextStartsWith(exception_msg_bad_order.format('First Name: "SuperUserFirst"'), str(err.exception))
 
     def test__assertPageContent__failure__with_bad_search_space(self):
         exception_msg = 'Could not find "{0}" value in content response. Provided value was:\n{1}'
         response = self._get_page_response('django_expanded_test_cases:index')
 
         # Bad content_starts_after values.
         with self.subTest('With content_starts_after not found'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_starts_after='Wrong value.',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', 'Wrong value.'))
+            self.assertText(exception_msg.format('content_starts_after', 'Wrong value.'), str(err.exception))
         with self.subTest('With content_starts_after not found'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='Wrong content value.',
                     content_starts_after='Wrong value.',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', 'Wrong value.'))
+            self.assertText(exception_msg.format('content_starts_after', 'Wrong value.'), str(err.exception))
         with self.subTest('With content_starts_after found with extra'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_starts_after='Home Page Header plus Extra',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('content_starts_after', 'Home Page Header plus Extra'),
+                str(err.exception),
             )
 
         # Bad content_ends_before values.
         with self.subTest('With content_ends_before not found'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_ends_before='Wrong value.',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_ends_before', 'Wrong value.'))
+            self.assertText(exception_msg.format('content_ends_before', 'Wrong value.'), str(err.exception))
         with self.subTest('With content_ends_before and expected_content not found'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='Wrong content value.',
                     content_ends_before='Wrong value.',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_ends_before', 'Wrong value.'))
+            self.assertText(exception_msg.format('content_ends_before', 'Wrong value.'), str(err.exception))
         with self.subTest('With content_ends_before found with extra'):
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_ends_before='Home Page Header plus Extra',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('content_ends_before', 'Home Page Header plus Extra'),
+                str(err.exception),
             )
 
     def test__assertPageContent__fail__with_limited_search_space(self):
         exception_msg = 'Expected content value was found, but occurred in "{0}" section. Expected was:\n{1}'
         response = self._get_page_response('django_expanded_test_cases:index')
 
         with self.subTest('Standard Response - With content_starts_after defined'):
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<head>',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', '<head>'))
+            self.assertText(exception_msg.format('content_starts_after', '<head>'), str(err.exception))
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<meta charset="utf-8">',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', '<meta charset="utf-8">'))
+            self.assertText(exception_msg.format('content_starts_after', '<meta charset="utf-8">'), str(err.exception))
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='</head>',
                     content_starts_after='<h1>Home Page Header</h1>',
                     ignore_ordering=True,
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', '</head>'))
+            self.assertText(exception_msg.format('content_starts_after', '</head>'), str(err.exception))
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<body>',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', '<body>'))
+            self.assertText(exception_msg.format('content_starts_after', '<body>'), str(err.exception))
             # Expected as single value - With exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', '<h1>Home Page Header</h1>'))
+            self.assertText(exception_msg.format('content_starts_after', '<h1>Home Page Header</h1>'), str(err.exception))
             # Expected as single value - With partial of exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='h1>',
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', 'h1>'))
+            self.assertText(exception_msg.format('content_starts_after', 'h1>'), str(err.exception))
 
             # Expected as array.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<meta charset="utf-8">',
                         '<title>Home Page | Test Views</title>',
                     ],
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertTextStartsWith(
                 exception_msg.format('content_starts_after', '<meta charset="utf-8">'),
+                str(err.exception),
             )
             # Expected as array - With ignore_ordering.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<meta charset="utf-8">',
                         '<title>Home Page | Test Views</title>',
                     ],
                     ignore_ordering=True,
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertTextStartsWith(
                 exception_msg.format('content_starts_after', '<meta charset="utf-8">'),
+                str(err.exception),
             )
             # Expected as array - With ignore_ordering and content mis-ordered.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<title>Home Page | Test Views</title>',
                         '<meta charset="utf-8">',
                     ],
                     ignore_ordering=True,
                     content_starts_after='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertTextStartsWith(
                 exception_msg.format('content_starts_after', '<title>Home Page | Test Views</title>'),
+                str(err.exception),
             )
 
         with self.subTest('Standard Response - With content_ends_before defined'):
             response = self._get_page_response('django_expanded_test_cases:index')
 
             # Expected as single value - Exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<h1>Home Page Header</h1>',
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_ends_before', '<h1>Home Page Header</h1>'))
+            self.assertText(exception_msg.format('content_ends_before', '<h1>Home Page Header</h1>'), str(err.exception))
             # Expected as single value - Partial of exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='h1>',
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_ends_before', 'h1>'))
+            self.assertText(exception_msg.format('content_ends_before', 'h1>'), str(err.exception))
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<p>Pretend this is the project landing page.</p>',
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('content_ends_before', '<p>Pretend this is the project landing page.</p>'),
+                str(err.exception),
             )
             # Expected as single value - With ignore_ordering (should have no effect here).
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<p>Pretend this is the project landing page.</p>',
                     ignore_ordering=True,
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('content_ends_before', '<p>Pretend this is the project landing page.</p>'),
+                str(err.exception),
             )
             # Expected as single value.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='</body>',
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_ends_before', '</body>'))
+            self.assertText(exception_msg.format('content_ends_before', '</body>'), str(err.exception))
 
             # Expected as array.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<p>Pretend this is the project landing page.</p>',
                         '</body>',
                     ],
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertTextStartsWith(
                 exception_msg.format('content_ends_before', '<p>Pretend this is the project landing page.</p>'),
+                str(err.exception),
             )
             # Expected as array - With ignore_ordering.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<p>Pretend this is the project landing page.</p>',
                         '</body>',
                     ],
                     ignore_ordering=True,
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertTextStartsWith(
                 exception_msg.format('content_ends_before', '<p>Pretend this is the project landing page.</p>'),
+                str(err.exception),
             )
             # Expected as array - With ignore_ordering and content mis-ordered.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '</body>',
                         '<p>Pretend this is the project landing page.</p>',
                     ],
                     ignore_ordering=True,
                     content_ends_before='<h1>Home Page Header</h1>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_ends_before', '</body>'))
+            self.assertTextStartsWith(exception_msg.format('content_ends_before', '</body>'), str(err.exception))
 
         with self.subTest('Standard Response - With both content containers defined'):
             response = self._get_page_response('django_expanded_test_cases:index')
 
             # Expected as single value - above search area.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<meta charset="utf-8">',
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('content_starts_after', '<meta charset="utf-8">'),
+                str(err.exception),
             )
             # Expected as single value - above search area, exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<title>Home Page | Test Views</title>',
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('content_starts_after', '<title>Home Page | Test Views</title>'),
+                str(err.exception),
             )
             # Expected as single value - below search area.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='</body>',
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_ends_before', '</body>'))
+            self.assertText(exception_msg.format('content_ends_before', '</body>'), str(err.exception))
             # Expected as single value - below search area, exact match.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<p>Pretend this is the project landing page.</p>',
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('content_ends_before', '<p>Pretend this is the project landing page.</p>'),
+                str(err.exception),
             )
             # Expected as single value - with ignore_ordering (should have no effect here).
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content='<meta charset="utf-8">',
                     ignore_ordering=True,
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('content_starts_after', '<meta charset="utf-8">'),
+                str(err.exception),
             )
 
             # Expected as array - Above search area.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<head>',
                         '<meta charset="utf-8">',
                     ],
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', '<head>'))
+            self.assertTextStartsWith(exception_msg.format('content_starts_after', '<head>'), str(err.exception))
             # Expected as array - Above search area, with ignore_ordering.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<head>',
                         '<meta charset="utf-8">',
                     ],
                     ignore_ordering=True,
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_starts_after', '<head>'))
+            self.assertTextStartsWith(exception_msg.format('content_starts_after', '<head>'), str(err.exception))
             # Expected as array - Above search area, with ignore_ordering and content mis-ordered.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '<meta charset="utf-8">',
                         '<head>',
                     ],
                     ignore_ordering=True,
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is the project landing page.</p>',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertTextStartsWith(
                 exception_msg.format('content_starts_after', '<meta charset="utf-8">'),
+                str(err.exception),
             )
             # Expected as array - Below search area.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         'the project landing page.</p>',
                         '</body>',
                     ],
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertTextStartsWith(
                 exception_msg.format('content_ends_before', 'the project landing page.</p>'),
+                str(err.exception),
             )
             # Expected as array - Below search area, with ignore_ordering.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         'the project landing page.</p>',
                         '</body>',
                     ],
                     ignore_ordering=True,
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is',
                 )
-            self.assertEqual(
-                str(err.exception),
+            self.assertTextStartsWith(
                 exception_msg.format('content_ends_before', 'the project landing page.</p>'),
+                str(err.exception),
             )
             # Expected as array - Below search area, with ignore_ordering and content mis-ordered.
             with self.assertRaises(AssertionError) as err:
                 self.assertPageContent(
                     response,
                     expected_content=[
                         '</body>',
                         'the project landing page.</p>',
                     ],
                     ignore_ordering=True,
                     content_starts_after='<title>Home Page | Test Views</title>',
                     content_ends_before='<p>Pretend this is',
                 )
-            self.assertEqual(str(err.exception), exception_msg.format('content_ends_before', '</body>'))
+            self.assertTextStartsWith(exception_msg.format('content_ends_before', '</body>'), str(err.exception))
 
     def test__assertPageContent__fail__with_content_casing_mismatch__exact_match(self):
         exception_msg = (
             'Expected content value was found, but letter capitalization did not match. Expected was:\n'
             '{0}\n'
             '\n'
             'Found was:\n'
             '{1}'
         )
 
         with self.subTest('Minimal Response - Exact Match - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <h1>Test Title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <h1>Test Title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response upper and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<H1>TEST TITLE</H1>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <H1>TEST TITLE</H1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response upper and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<H1>TEST TITLE</H1>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <H1>TEST TITLE</H1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response lower and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>test title</h1>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <h1>test title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response lower and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>test title</h1>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <h1>test title</h1> ...'),
+                str(err.exception),
             )
 
     def test__assertPageContent__fail__with_content_casing_mismatch__extra_characters_before(self):
         exception_msg = (
             'Expected content value was found, but letter capitalization did not match. Expected was:\n'
             '{0}\n'
             '\n'
@@ -2083,170 +2620,170 @@
             '{1}'
         )
 
         with self.subTest('Minimal Response - Exact Match - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<div>123456789</div><h1>Test Title</h1>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <div>123456789</div><h1>Test Title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<div><p>This is a test p tag.</p></div><h1>Test Title</h1>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... est p tag.</p></div><h1>Test Title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<p>Testing</p><h1>Test Title</h1>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <p>Testing</p><h1>Test Title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<div>123456789</div><h1>Test Title</h1>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <div>123456789</div><h1>Test Title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<div><p>This is a test p tag.</p></div><h1>Test Title</h1>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... est p tag.</p></div><h1>Test Title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<p>Testing</p><h1>Test Title</h1>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <p>Testing</p><h1>Test Title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response upper and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<DIV>123456789</DIV><H1>TEST TITLE</H1>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <DIV>123456789</DIV><H1>TEST TITLE</H1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response upper and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<DIV><P>THIS IS A TEST P TAG.</P></DIV><H1>TEST TITLE</H1>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... EST P TAG.</P></DIV><H1>TEST TITLE</H1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response upper and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<P>TESTING</P><H1>TEST TITLE</H1>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <P>TESTING</P><H1>TEST TITLE</H1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response upper and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<DIV>123456789</DIV><H1>TEST TITLE</H1>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <DIV>123456789</DIV><H1>TEST TITLE</H1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response upper and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<DIV><P>THIS IS A TEST P TAG.</P></DIV><H1>TEST TITLE</H1>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... EST P TAG.</P></DIV><H1>TEST TITLE</H1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response upper and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<P>TESTING</P><H1>TEST TITLE</H1>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <P>TESTING</P><H1>TEST TITLE</H1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response lower and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<div>123456789</div><h1>test title</h1>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <div>123456789</div><h1>test title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response lower and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<div><p>this is a test p tag.</p></div><h1>test title</h1>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... est p tag.</p></div><h1>test title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response lower and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<p>testing</p><h1>test title</h1>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <p>testing</p><h1>test title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response lower and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<div>123456789</div><h1>test title</h1>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <div>123456789</div><h1>test title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response lower and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<div><p>this is a test p tag.</p></div><h1>test title</h1>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... est p tag.</p></div><h1>test title</h1> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response lower and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<p>testing</p><h1>test title</h1>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <p>testing</p><h1>test title</h1> ...'),
+                str(err.exception),
             )
 
     def test__assertPageContent__fail__with_content_casing_mismatch__extra_characters_after(self):
         exception_msg = (
             'Expected content value was found, but letter capitalization did not match. Expected was:\n'
             '{0}\n'
             '\n'
@@ -2254,170 +2791,170 @@
             '{1}'
         )
 
         with self.subTest('Minimal Response - Exact Match - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1><div>123456789</div>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <h1>Test Title</h1><div>123456789</div> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1><div><p>This is a test p tag.</p></div>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <h1>Test Title</h1><div><p>This is a te ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1><p>Testing</p>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <h1>Test Title</h1><p>Testing</p> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1><div>123456789</div>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <h1>Test Title</h1><div>123456789</div> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1><div><p>This is a test p tag.</p></div>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <h1>Test Title</h1><div><p>This is a te ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>Test Title</h1><p>Testing</p>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <h1>Test Title</h1><p>Testing</p> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response upper and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<H1>TEST TITLE</H1><DIV>123456789</DIV>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <H1>TEST TITLE</H1><DIV>123456789</DIV> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response upper and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<H1>TEST TITLE</H1><DIV><P>THIS IS A TEST P TAG.</P></DIV>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <H1>TEST TITLE</H1><DIV><P>THIS IS A TE ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response upper and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<H1>TEST TITLE</H1><P>TESTING</P>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <H1>TEST TITLE</H1><P>TESTING</P> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response upper and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<H1>TEST TITLE</H1><DIV>123456789</DIV>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <H1>TEST TITLE</H1><DIV>123456789</DIV> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response upper and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<H1>TEST TITLE</H1><DIV><P>THIS IS A TEST P TAG.</P></DIV>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <H1>TEST TITLE</H1><DIV><P>THIS IS A TE ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response upper and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<H1>TEST TITLE</H1><P>TESTING</P>')
                 self.assertPageContent(response, '<h1>test title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>test title</h1>', '... <H1>TEST TITLE</H1><P>TESTING</P> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response lower and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>test title</h1><div>123456789</div>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <h1>test title</h1><div>123456789</div> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response lower and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>test title</h1><div><p>this is a test p tag.</p></div>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <h1>test title</h1><div><p>this is a te ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response lower and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>test title</h1><p>testing/p>')
                 self.assertPageContent(response, '<h1>Test Title</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<h1>Test Title</h1>', '... <h1>test title</h1><p>testing/p> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Exact Match - With response lower and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>test title</h1><div>123456789</div>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <h1>test title</h1><div>123456789</div> ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Extra Match - With response lower and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>test title</h1><div><p>this is a test p tag.</p></div>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <h1>test title</h1><div><p>this is a te ...'),
+                str(err.exception),
             )
 
         with self.subTest('Minimal Response - Lesser Match - With response lower and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<h1>test title</h1><p>testing/p>')
                 self.assertPageContent(response, '<H1>TEST TITLE</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format('<H1>TEST TITLE</H1>', '... <h1>test title</h1><p>testing/p> ...'),
+                str(err.exception),
             )
 
     def test__assertPageContent__fail__with_content_casing_mismatch__actual_response_object(self):
         exception_msg = (
             'Expected content value was found, but letter capitalization did not match. Expected was:\n'
             '{0}\n'
             '\n'
@@ -2425,44 +2962,44 @@
             '{1}'
         )
 
         with self.subTest('Standard Response - With response mixed and check upper'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
                 self.assertPageContent(response, '<H1>HOME PAGE HEADER</H1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format(
                     '<H1>HOME PAGE HEADER</H1>',
                     '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...'
                 ),
+                str(err.exception),
             )
 
         with self.subTest('Standard Response - With response mixed and check lower'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
                 self.assertPageContent(response, '<h1>home page header</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format(
                     '<h1>home page header</h1>',
                     '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...'
                 ),
+                str(err.exception),
             )
 
         with self.subTest('Standard Response - With response mixed and check mixed'):
             with self.assertRaises(AssertionError) as err:
                 response = self._get_page_response('django_expanded_test_cases:index')
                 self.assertPageContent(response, '<h1>home Page header</h1>')
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 exception_msg.format(
                     '<h1>home Page header</h1>',
                     '... /title></head><body><h1>Home Page Header</h1><p>Pretend this is t ...'
                 ),
+                str(err.exception),
             )
 
     def test__assertRepeatingElement__success__standard_elements__basic(self):
         """
         Tests assertPageContent() function, in cases when it should succeed on "standard" (non-void) elements.
         """
         with self.subTest('Response with one item, when one item is expected'):
@@ -2600,243 +3137,243 @@
     def test__assertRepeatingElement__fail__incorrect_count(self):
         exception_msg = 'Expected {0} element opening tags. Found {1}.'
 
         with self.subTest('Providing an expected of less than 1'):
             with self.assertRaises(ValueError) as err:
                 response = HttpResponse('')
                 self.assertRepeatingElement(response, '<li>', 0)
-            self.assertEqual(
-                str(err.exception),
+            self.assertText(
                 'The assertRepeatingElement() function requires an element occurs one or more times.',
+                str(err.exception),
             )
 
         # Empty response tests.
         with self.subTest('Empty response, when one item is expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), exception_msg.format(1, 0))
+            self.assertText(exception_msg.format(1, 0), str(err.exception))
 
         with self.subTest('Empty response, when two items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), exception_msg.format(2, 0))
+            self.assertText(exception_msg.format(2, 0), str(err.exception))
 
         with self.subTest('Empty response, when three items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), exception_msg.format(3, 0))
+            self.assertText(exception_msg.format(3, 0), str(err.exception))
 
         with self.subTest('Empty response, when four items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('')
                 self.assertRepeatingElement(response, '<li>', 4)
-            self.assertEqual(str(err.exception), exception_msg.format(4, 0))
+            self.assertText(exception_msg.format(4, 0), str(err.exception))
 
         # Single item response tests.
         with self.subTest('Response with one item, when two items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li>')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), exception_msg.format(2, 1))
+            self.assertText(exception_msg.format(2, 1), str(err.exception))
 
         with self.subTest('Response with one item, when three items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li>')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), exception_msg.format(3, 1))
+            self.assertText(exception_msg.format(3, 1), str(err.exception))
 
         with self.subTest('Response with one item, when four items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li>')
                 self.assertRepeatingElement(response, '<li>', 4)
-            self.assertEqual(str(err.exception), exception_msg.format(4, 1))
+            self.assertText(exception_msg.format(4, 1), str(err.exception))
 
         # Two item response tests.
         with self.subTest('Response with two items, when one item is expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), exception_msg.format(1, 2))
+            self.assertText(exception_msg.format(1, 2), str(err.exception))
             # With spaces
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), exception_msg.format(1, 2))
+            self.assertText(exception_msg.format(1, 2), str(err.exception))
 
         with self.subTest('Response with two items, when three items are expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), exception_msg.format(3, 2))
+            self.assertText(exception_msg.format(3, 2), str(err.exception))
             # With spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), exception_msg.format(3, 2))
+            self.assertText(exception_msg.format(3, 2), str(err.exception))
 
         with self.subTest('Response with two items, when four items are expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 4)
-            self.assertEqual(str(err.exception), exception_msg.format(4, 2))
+            self.assertText(exception_msg.format(4, 2), str(err.exception))
             # With spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 4)
-            self.assertEqual(str(err.exception), exception_msg.format(4, 2))
+            self.assertText(exception_msg.format(4, 2), str(err.exception))
 
         # Three item response tests.
         with self.subTest('Response with three items, when one item is expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), exception_msg.format(1, 3))
+            self.assertText(exception_msg.format(1, 3), str(err.exception))
             # With spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), exception_msg.format(1, 3))
+            self.assertText(exception_msg.format(1, 3), str(err.exception))
 
         with self.subTest('Response with three items, when two items are expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), exception_msg.format(2, 3))
+            self.assertText(exception_msg.format(2, 3), str(err.exception))
             # With spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), exception_msg.format(2, 3))
+            self.assertText(exception_msg.format(2, 3), str(err.exception))
 
         with self.subTest('Response with three items, when four items are expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 4)
-            self.assertEqual(str(err.exception), exception_msg.format(4, 3))
+            self.assertText(exception_msg.format(4, 3), str(err.exception))
             # With spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 4)
-            self.assertEqual(str(err.exception), exception_msg.format(4, 3))
+            self.assertText(exception_msg.format(4, 3), str(err.exception))
 
         # Four item response tests.
         with self.subTest('Response with four items, when one item is expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li><li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), exception_msg.format(1, 4))
+            self.assertText(exception_msg.format(1, 4), str(err.exception))
             # With spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), exception_msg.format(1, 4))
+            self.assertText(exception_msg.format(1, 4), str(err.exception))
 
         with self.subTest('Response with four items, when two items are expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li><li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), exception_msg.format(2, 4))
+            self.assertText(exception_msg.format(2, 4), str(err.exception))
             # With spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), exception_msg.format(2, 4))
+            self.assertText(exception_msg.format(2, 4), str(err.exception))
 
         with self.subTest('Response with four items, when three items are expected'):
             # No spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li><li></li><li></li><li></li>')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), exception_msg.format(3, 4))
+            self.assertText(exception_msg.format(3, 4), str(err.exception))
             # With spaces.
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li></li>')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), exception_msg.format(3, 4))
+            self.assertText(exception_msg.format(3, 4), str(err.exception))
 
     def test__assertRepeatingElement__fail__incomplete_items(self):
         open_exception_msg = 'Expected {0} element opening tags. Found {1}.'
         close_exception_msg = 'Expected {0} element closing tags. Found {1}.'
 
         with self.subTest('Response with one plus partial items, when one item is expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), open_exception_msg.format(1, 2))
+            self.assertText(open_exception_msg.format(1, 2), str(err.exception))
 
         with self.subTest('Response with one plus partial items, when two items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), close_exception_msg.format(2, 1))
+            self.assertText(close_exception_msg.format(2, 1), str(err.exception))
 
         with self.subTest('Response with two plus partial items, when one item is expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 1)
-            self.assertEqual(str(err.exception), open_exception_msg.format(1, 3))
+            self.assertText(open_exception_msg.format(1, 3), str(err.exception))
 
         with self.subTest('Response with two plus partial items, when two items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), open_exception_msg.format(2, 3))
+            self.assertText(open_exception_msg.format(2, 3), str(err.exception))
 
         with self.subTest('Response with two plus partial items, when three items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), close_exception_msg.format(3, 2))
+            self.assertText(close_exception_msg.format(3, 2), str(err.exception))
 
         with self.subTest('Response with three plus partial items, when two items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 2)
-            self.assertEqual(str(err.exception), open_exception_msg.format(2, 4))
+            self.assertText(open_exception_msg.format(2, 4), str(err.exception))
 
         with self.subTest('Response with three plus partial items, when three items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), open_exception_msg.format(3, 4))
+            self.assertText(open_exception_msg.format(3, 4), str(err.exception))
 
         with self.subTest('Response with three plus partial items, when four items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 4)
-            self.assertEqual(str(err.exception), close_exception_msg.format(4, 3))
+            self.assertText(close_exception_msg.format(4, 3), str(err.exception))
 
         with self.subTest('Response with four plus partial items, when three items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 3)
-            self.assertEqual(str(err.exception), open_exception_msg.format(3, 5))
+            self.assertText(open_exception_msg.format(3, 5), str(err.exception))
 
         with self.subTest('Response with four plus partial items, when four items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 4)
-            self.assertEqual(str(err.exception), open_exception_msg.format(4, 5))
+            self.assertText(open_exception_msg.format(4, 5), str(err.exception))
 
         with self.subTest('Response with four plus partial items, when five items are expected'):
             with self.assertRaises(AssertionError) as err:
                 response = HttpResponse('<li></li> <li></li> <li></li> <li></li> <li>')
                 self.assertRepeatingElement(response, '<li>', 5)
-            self.assertEqual(str(err.exception), close_exception_msg.format(5, 4))
+            self.assertText(close_exception_msg.format(5, 4), str(err.exception))
 
     # endregion Element Assertion Tests
 
     # endregion Assertion Tests
 
     # region Helper Function Tests
 
@@ -3095,128 +3632,128 @@
 
     def test__get_page_title__empty_title(self):
         """
         Tests get_page_title() function, when page title is empty.
         """
         with self.subTest('No title element in response (simulates things like file downloads)'):
             response = HttpResponse('')
-            self.assertEqual(self.get_page_title(response), '')
-            self.assertEqual(self.get_page_title(response.content), '')
-            self.assertEqual(self.get_page_title(response.content.decode('utf-8')), '')
+            self.assertText('', self.get_page_title(response))
+            self.assertText('', self.get_page_title(response.content))
+            self.assertText('', self.get_page_title(response.content.decode('utf-8')))
 
         with self.subTest('Title exists, but is empty'):
             response = HttpResponse('<title></title>')
-            self.assertEqual(self.get_page_title(response), '')
-            self.assertEqual(self.get_page_title(response.content), '')
-            self.assertEqual(self.get_page_title(response.content.decode('utf-8')), '')
+            self.assertText('', self.get_page_title(response))
+            self.assertText('', self.get_page_title(response.content))
+            self.assertText('', self.get_page_title(response.content.decode('utf-8')))
 
         with self.subTest('Title exists, but is whitespace'):
             response = HttpResponse('<title>   </title>')
-            self.assertEqual(self.get_page_title(response), '')
-            self.assertEqual(self.get_page_title(response.content), '')
-            self.assertEqual(self.get_page_title(response.content.decode('utf-8')), '')
+            self.assertText('', self.get_page_title(response))
+            self.assertText('', self.get_page_title(response.content))
+            self.assertText('', self.get_page_title(response.content.decode('utf-8')))
 
     def test__get_page_title__populated_title(self):
         """
         Tests get_page_title() function, when page title is populated.
         """
         with self.subTest('Basic title'):
             response = HttpResponse('<title>Test Title</title>')
-            self.assertEqual(self.get_page_title(response), 'Test Title')
-            self.assertEqual(self.get_page_title(response.content), 'Test Title')
-            self.assertEqual(self.get_page_title(response.content.decode('utf-8')), 'Test Title')
+            self.assertText('Test Title', self.get_page_title(response))
+            self.assertText('Test Title', self.get_page_title(response.content))
+            self.assertText('Test Title', self.get_page_title(response.content.decode('utf-8')))
 
         with self.subTest('Basic title, with extra whitespace (to simulate Django templating)'):
             response = HttpResponse('<title>   Test    Title   </title>')
-            self.assertEqual(self.get_page_title(response), 'Test Title')
-            self.assertEqual(self.get_page_title(response.content), 'Test Title')
-            self.assertEqual(self.get_page_title(response.content.decode('utf-8')), 'Test Title')
+            self.assertText('Test Title', self.get_page_title(response))
+            self.assertText('Test Title', self.get_page_title(response.content))
+            self.assertText('Test Title', self.get_page_title(response.content.decode('utf-8')))
 
         with self.subTest('Complex title'):
             response = HttpResponse('<title>Test Title | My Custom App | My Really Cool Site</title>')
-            self.assertEqual(self.get_page_title(response), 'Test Title | My Custom App | My Really Cool Site')
-            self.assertEqual(self.get_page_title(response.content), 'Test Title | My Custom App | My Really Cool Site')
-            self.assertEqual(
-                self.get_page_title(response.content.decode('utf-8')),
+            self.assertText('Test Title | My Custom App | My Really Cool Site', self.get_page_title(response))
+            self.assertText('Test Title | My Custom App | My Really Cool Site', self.get_page_title(response.content))
+            self.assertText(
                 'Test Title | My Custom App | My Really Cool Site',
+                self.get_page_title(response.content.decode('utf-8')),
             )
 
         with self.subTest('Complex title, with extra whitespace (to simulate Django templating)'):
             response = HttpResponse(
                 '<title>   Test   Title    \n|\n   My Custom App   \n|\n   My Really Cool Site   </title>'
             )
-            self.assertEqual(self.get_page_title(response), 'Test Title | My Custom App | My Really Cool Site')
-            self.assertEqual(self.get_page_title(response.content), 'Test Title | My Custom App | My Really Cool Site')
-            self.assertEqual(
-                self.get_page_title(response.content.decode('utf-8')),
+            self.assertText('Test Title | My Custom App | My Really Cool Site', self.get_page_title(response))
+            self.assertText('Test Title | My Custom App | My Really Cool Site', self.get_page_title(response.content))
+            self.assertText(
                 'Test Title | My Custom App | My Really Cool Site',
+                self.get_page_title(response.content.decode('utf-8')),
             )
 
     def test__get_page_header__empty_header(self):
         """
         Tests get_page_header() function, when page H1 header is empty.
         """
         with self.subTest('No header element in response (simulates things like file downloads)'):
             response = HttpResponse('')
-            self.assertEqual(self.get_page_header(response), '')
-            self.assertEqual(self.get_page_header(response.content), '')
-            self.assertEqual(self.get_page_header(response.content.decode('utf-8')), '')
+            self.assertText('', self.get_page_header(response))
+            self.assertText('', self.get_page_header(response.content))
+            self.assertText('', self.get_page_header(response.content.decode('utf-8')))
 
         with self.subTest('Header exists, but is empty'):
             response = HttpResponse('<h1></h1>')
-            self.assertEqual(self.get_page_header(response), '')
-            self.assertEqual(self.get_page_header(response.content), '')
-            self.assertEqual(self.get_page_header(response.content.decode('utf-8')), '')
+            self.assertText('', self.get_page_header(response))
+            self.assertText('', self.get_page_header(response.content))
+            self.assertText('', self.get_page_header(response.content.decode('utf-8')))
 
         with self.subTest('Header exists, but is whitespace'):
             response = HttpResponse('<h1>   </h1>')
-            self.assertEqual(self.get_page_header(response), '')
-            self.assertEqual(self.get_page_header(response.content), '')
-            self.assertEqual(self.get_page_header(response.content.decode('utf-8')), '')
+            self.assertText('', self.get_page_header(response))
+            self.assertText('', self.get_page_header(response.content))
+            self.assertText('', self.get_page_header(response.content.decode('utf-8')))
 
     def test__get_page_header__populated_header(self):
         """
         Tests get_page_header() function, when page H1 header is populated.
         """
         with self.subTest('Basic header'):
             response = HttpResponse('<h1>Test Header</h1>')
-            self.assertEqual(self.get_page_header(response), 'Test Header')
-            self.assertEqual(self.get_page_header(response.content), 'Test Header')
-            self.assertEqual(self.get_page_header(response.content.decode('utf-8')), 'Test Header')
+            self.assertText('Test Header', self.get_page_header(response))
+            self.assertText('Test Header', self.get_page_header(response.content))
+            self.assertText('Test Header', self.get_page_header(response.content.decode('utf-8')))
 
         with self.subTest('Basic header, with extra whitespace (to simulate Django templating)'):
             response = HttpResponse('<h1>   Test    Header   </h1>')
-            self.assertEqual(self.get_page_header(response), 'Test Header')
-            self.assertEqual(self.get_page_header(response.content), 'Test Header')
-            self.assertEqual(self.get_page_header(response.content.decode('utf-8')), 'Test Header')
+            self.assertText('Test Header', self.get_page_header(response))
+            self.assertText('Test Header', self.get_page_header(response.content))
+            self.assertText('Test Header', self.get_page_header(response.content.decode('utf-8')))
 
     def test__get_context_messages(self):
         """
         Tests get_context_messages() function.
         """
         with self.subTest('No messages'):
             response = self._get_page_response('django_expanded_test_cases:index')
             messages = self.get_context_messages(response)
             self.assertEqual(len(messages), 0)
 
         with self.subTest('Single message'):
-            response = self._get_page_response('django_expanded_test_cases:one-message')
+            response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             messages = self.get_context_messages(response)
             self.assertEqual(len(messages), 1)
             self.assertIn('This is a test message.', messages)
 
         with self.subTest('Two messages'):
-            response = self._get_page_response('django_expanded_test_cases:two-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-two-messages')
             messages = self.get_context_messages(response)
             self.assertEqual(len(messages), 2)
             self.assertIn('Test message #1.', messages)
             self.assertIn('Test message #2.', messages)
 
         with self.subTest('Three messages'):
-            response = self._get_page_response('django_expanded_test_cases:three-messages')
+            response = self._get_page_response('django_expanded_test_cases:response-with-three-messages')
             messages = self.get_context_messages(response)
             self.assertEqual(len(messages), 3)
             self.assertIn('Test info message.', messages)
             self.assertIn('Test warning message.', messages)
             self.assertIn('Test error message.', messages)
 
         with self.subTest('TemplateResponse check'):
@@ -3230,195 +3767,338 @@
     def test__get_minimized_response_content__strip_newlines_is_true(self):
         """
         Tests get_minimized_response_content() function.
         """
         with self.subTest('Minimal Response - No change'):
             response = HttpResponse('<h1>Test Title</h1>')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(response, '<h1>Test Title</h1>')
+            self.assertText('<h1>Test Title</h1>', response)
 
         with self.subTest('Minimal Response - Outer whitespace'):
             response = HttpResponse('&nbsp; <h1>Test Title</h1> &nbsp; ')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(response, '<h1>Test Title</h1>')
+            self.assertText('<h1>Test Title</h1>', response)
 
         with self.subTest('Minimal Response - Inner whitespace'):
             response = HttpResponse('<h1>Test  &nbsp;  Title</h1>')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(response, '<h1>Test Title</h1>')
+            self.assertText('<h1>Test Title</h1>', response)
 
         with self.subTest('Minimal Response - Inner whitespace'):
             response = HttpResponse('<h1>Test  &nbsp;  Title</h1>')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(response, '<h1>Test Title</h1>')
+            self.assertText('<h1>Test Title</h1>', response)
 
         with self.subTest('Minimal Response - With Newlines'):
             response = HttpResponse('<h1>Test  \n  Title</h1>')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(response, '<h1>Test Title</h1>')
+            self.assertText('<h1>Test Title</h1>', response)
 
         with self.subTest('Standard Response - Login Page'):
             response = self._get_page_response('django_expanded_test_cases:login')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(
-                response,
+            self.assertText(
                 (
                     '<head><meta charset="utf-8"><title>Login Page | Test Views</title></head>'
                     '<body>'
                     '<h1>Login Page Header</h1><p>Pretend this is a login page.</p>'
                     '</body>'
                 ),
+                response,
             )
 
         with self.subTest('Standard Response - Render() Home Page'):
             response = self._get_page_response('django_expanded_test_cases:index')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(
-                response,
+            self.assertText(
                 (
                     '<head><meta charset="utf-8"><title>Home Page | Test Views</title></head>'
                     '<body>'
                     '<h1>Home Page Header</h1><p>Pretend this is the project landing page.</p>'
                     '</body>'
                 ),
+                response,
             )
 
         with self.subTest('Standard Response - TemplateResponse Home Page'):
             response = self._get_page_response('django_expanded_test_cases:template-response-index')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(
-                response,
+            self.assertText(
                 (
                     '<head><meta charset="utf-8"><title>Home Page | Test Views</title></head>'
                     '<body>'
                     '<h1>Home Page Header</h1><p>Pretend this is the project landing page.</p>'
                     '</body>'
                 ),
+                response,
             )
 
         with self.subTest('Standard Response - One Message Page'):
-            response = self._get_page_response('django_expanded_test_cases:one-message')
+            response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             response = self.get_minimized_response_content(response, strip_newlines=True)
-            self.assertEqual(
-                response,
+            self.assertText(
                 (
                     '<head><meta charset="utf-8"><title>View with One Message | Test Views</title></head>'
                     '<body>'
                     '<ul><li><p>This is a test message.</p></li></ul>'
                     '<h1>View with One Message Header</h1>'
                     '<p>Pretend useful stuff is displayed here, for one-message render() view.</p>'
                     '</body>'
                 ),
+                response,
             )
 
     def test__get_minimized_response_content__strip_newlines_is_false(self):
         """
         Tests get_minimized_response_content() function.
         """
         with self.subTest('Minimal Response - No change'):
             response = HttpResponse('<h1>Test Title</h1>')
             response = self.get_minimized_response_content(response, strip_newlines=False)
-            self.assertEqual(response, '<h1>Test Title</h1>')
+            self.assertText('<h1>Test Title</h1>', response)
 
         with self.subTest('Minimal Response - Outer whitespace'):
             response = HttpResponse('&nbsp; <h1>Test Title</h1> &nbsp; ')
             response = self.get_minimized_response_content(response, strip_newlines=False)
-            self.assertEqual(response, '<h1>Test Title</h1>')
+            self.assertText('<h1>Test Title</h1>', response)
 
         with self.subTest('Minimal Response - Inner whitespace'):
             response = HttpResponse('<h1>Test  &nbsp;  Title</h1>')
             response = self.get_minimized_response_content(response, strip_newlines=False)
-            self.assertEqual(response, '<h1>Test Title</h1>')
+            self.assertText('<h1>Test Title</h1>', response)
 
         with self.subTest('Minimal Response - With Newlines'):
             response = HttpResponse('<h1>Test  \n  Title</h1>')
             response = self.get_minimized_response_content(response, strip_newlines=False)
-            self.assertEqual(response, '<h1>Test \n Title</h1>')
+            self.assertText('<h1>Test \n Title</h1>', response)
 
         with self.subTest('Standard Response - Login Page'):
             response = self._get_page_response('django_expanded_test_cases:login')
             response = self.get_minimized_response_content(response, strip_newlines=False)
-            self.assertEqual(
-                response,
+            self.assertText(
                 (
                     '<head>\n<meta charset="utf-8">\n<title>Login Page | Test Views</title>\n</head>\n'
                     '<body>\n'
                     '<h1>Login Page Header</h1>\n<p>Pretend this is a login page.</p>\n'
                     '</body>'
-                )
+                ),
+                response,
             )
 
         with self.subTest('Standard Response - Render() Home Page'):
             response = self._get_page_response('django_expanded_test_cases:index')
             response = self.get_minimized_response_content(response, strip_newlines=False)
-            self.assertEqual(
-                response,
+            self.assertText(
                 (
                     '<head>\n<meta charset="utf-8">\n<title>Home Page | Test Views</title>\n</head>\n'
                     '<body>\n'
                     '<h1>Home Page Header</h1>\n<p>Pretend this is the project landing page.</p>\n'
                     '</body>'
-                )
+                ),
+                response,
             )
 
         with self.subTest('Standard Response - TemplateResponse Home Page'):
             response = self._get_page_response('django_expanded_test_cases:template-response-index')
             response = self.get_minimized_response_content(response, strip_newlines=False)
-            self.assertEqual(
-                response,
+            self.assertText(
                 (
                     '<head>\n<meta charset="utf-8">\n<title>Home Page | Test Views</title>\n</head>\n'
                     '<body>\n'
                     '<h1>Home Page Header</h1>\n<p>Pretend this is the project landing page.</p>\n'
                     '</body>'
-                )
+                ),
+                response,
             )
 
         with self.subTest('Standard Response - One Message Page'):
-            response = self._get_page_response('django_expanded_test_cases:one-message')
+            response = self._get_page_response('django_expanded_test_cases:response-with-one-message')
             response = self.get_minimized_response_content(response, strip_newlines=False)
-            self.assertEqual(
-                response,
+            self.assertText(
                 (
                     '<head>\n<meta charset="utf-8">\n<title>View with One Message | Test Views</title>\n</head>\n'
                     '<body>\n'
                     '<ul>\n<li><p>\n This is a test message.\n</p></li>\n</ul>\n'
                     '<h1>View with One Message Header</h1>\n'
                     '<p>Pretend useful stuff is displayed here, for one-message render() view.</p>\n'
                     '</body>'
                 ),
+                response,
             )
 
+    def test__standardize_url__success(self):
+        """
+        Tests standardize_url() function, in situations when it should succeed.
+        """
+
+        with self.subTest('Emtpy url'):
+            # Base url.
+            url = self.standardize_url('', append_root=False)
+            self.assertText('/', url)
+
+            # With site root.
+            url = self.standardize_url('', append_root=True)
+            self.assertText('127.0.0.1/', url)
+
+        with self.subTest('Basic url - No outer slashes'):
+            # Base url.
+            url = self.standardize_url('login', append_root=False)
+            self.assertText('/login/', url)
+
+            # With site root.
+            url = self.standardize_url('login', append_root=True)
+            self.assertText('127.0.0.1/login/', url)
+
+        with self.subTest('Basic url - With outer slashes'):
+            # Base url.
+            url = self.standardize_url('/login/', append_root=False)
+            self.assertText('/login/', url)
+
+            # With site root.
+            url = self.standardize_url('/login/', append_root=True)
+            self.assertText('127.0.0.1/login/', url)
+
+        with self.subTest('Longer url - No outer slashes'):
+            # Base url.
+            url = self.standardize_url('this/is/a/test/url', append_root=False)
+            self.assertText('/this/is/a/test/url/', url)
+
+            # With site root.
+            url = self.standardize_url('/this/is/a/test/url/', append_root=True)
+            self.assertText('127.0.0.1/this/is/a/test/url/', url)
+
+        with self.subTest('With GET args - Provided in url'):
+            # Base url.
+            url = self.standardize_url('/my/url/?arg1=testing&arg2=aaa', append_root=False)
+            self.assertText('/my/url/?arg1=testing&arg2=aaa', url)
+
+            # With site root.
+            url = self.standardize_url('/my/url/?arg1=testing&arg2=aaa', append_root=True)
+            self.assertText('127.0.0.1/my/url/?arg1=testing&arg2=aaa', url)
+
+        with self.subTest('With GET args - Provided via generate_get_url()'):
+            # Base url.
+            url = self.standardize_url(self.generate_get_url('/my/url/', arg1='testing', arg2='aaa'), append_root=False)
+            self.assertText('/my/url/?arg1=testing&arg2=aaa', url)
+
+            # With site root.
+            url = self.standardize_url(self.generate_get_url('/my/url/', arg1='testing', arg2='aaa'), append_root=True)
+            self.assertText('127.0.0.1/my/url/?arg1=testing&arg2=aaa', url)
+
+        with self.subTest('With GET args - Provided in url with mixed characters'):
+            # Base url.
+            url = self.standardize_url('/my/url/?arg1=testing stuff?<blah>weird_values-aaa', append_root=False)
+            self.assertText('/my/url/?arg1=testing+stuff%3F%3Cblah%3Eweird_values-aaa', url)
+
+            # With site root.
+            url = self.standardize_url('/my/url/?arg1=testing stuff?<blah>weird_values-aaa', append_root=True)
+            self.assertText('127.0.0.1/my/url/?arg1=testing+stuff%3F%3Cblah%3Eweird_values-aaa', url)
+
+        with self.subTest('With GET args - Provided in generate_get_url() with mixed characters'):
+            # Base url.
+            url = self.standardize_url(self.generate_get_url('/my/url/?', test='testing stuff?<blah>weird_values-aaa'), append_root=False)
+            self.assertText('/my/url/?test=testing+stuff%3F%3Cblah%3Eweird_values-aaa', url)
+
+            # With site root.
+            url = self.standardize_url(self.generate_get_url('/my/url/?', test='testing stuff?<blah>weird_values-aaa'), append_root=True)
+            self.assertText('127.0.0.1/my/url/?test=testing+stuff%3F%3Cblah%3Eweird_values-aaa', url)
+
+        with self.subTest('Basic resolve url'):
+            # Base url.
+            url = self.standardize_url('django_expanded_test_cases:login', append_root=False)
+            self.assertText('/login/', url)
+
+            # With site root.
+            url = self.standardize_url('django_expanded_test_cases:login', append_root=True)
+            self.assertText('127.0.0.1/login/', url)
+
+        with self.subTest('Resolve url with params as args'):
+            # Base url.
+            url = self.standardize_url(
+                'django_expanded_test_cases:response-with-args',
+                url_args=(11, 'args_test_1'),
+                append_root=False,
+            )
+            self.assertText('/views/11/args_test_1/', url)
+
+            # With site root.
+            url = self.standardize_url(
+                'django_expanded_test_cases:response-with-args',
+                url_args=(12, 'args_test_2'),
+                append_root=True,
+            )
+            self.assertText('127.0.0.1/views/12/args_test_2/', url)
+
+        with self.subTest('Resolve url with params as kwargs'):
+            # Base url.
+            url = self.standardize_url(
+                'django_expanded_test_cases:response-with-args',
+                url_kwargs={'id': 21, 'name': 'kwargs_test_1'},
+                append_root=False,
+            )
+            self.assertText('/views/21/kwargs_test_1/', url)
+
+            # With site root.
+            url = self.standardize_url(
+                'django_expanded_test_cases:response-with-args',
+                url_kwargs={'id': 22, 'name': 'kwargs_test_2'},
+                append_root=True,
+            )
+            self.assertText('127.0.0.1/views/22/kwargs_test_2/', url)
+
+    def test__standardize_url__failure(self):
+        """
+        Tests standardize_url() function, in situations when it should fail.
+        """
+        with self.subTest('Resolve url with with args and kwargs'):
+            # Base url.
+            with self.assertRaises(ValueError):
+                url = self.standardize_url(
+                    'django_expanded_test_cases:response-with-args',
+                    url_args=(31, 'testing'),
+                    url_kwargs={'id': 31, 'name': 'testing'},
+                    append_root=False,
+                )
+
+            # With site root.
+            with self.assertRaises(ValueError):
+                url = self.standardize_url(
+                    'django_expanded_test_cases:response-with-args',
+                    url_args=(31, 'testing'),
+                    url_kwargs={'id': 31, 'name': 'testing'},
+                    append_root=True,
+                )
+
     def test__standardize_html_tags(self):
         """
         Tests letters in standardize_html_tags() functions.
         """
         with self.subTest('Test html tag - No spaces'):
             value = self.standardize_html_tags('<h1>Test Header</h1><p>Aaa</p>')
-            self.assertEqual(value, '<h1>Test Header</h1><p>Aaa</p>')
+            self.assertText('<h1>Test Header</h1><p>Aaa</p>', value)
 
         with self.subTest('Test html tag - With spaces'):
             value = self.standardize_html_tags('  <h1>  Test Header  </h1> <p> Aaa </p>  ')
-            self.assertEqual(value, '<h1>Test Header</h1><p>Aaa</p>')
+            self.assertText('<h1>Test Header</h1><p>Aaa</p>', value)
 
         with self.subTest('Test array - No spaces'):
             value = self.standardize_html_tags('[1, 2, 3]')
-            self.assertEqual(value, '[1, 2, 3]')
+            self.assertText('[1, 2, 3]', value)
 
         with self.subTest('Test array - with spaces'):
             value = self.standardize_html_tags('  [  1, 2, 3  ]  ')
-            self.assertEqual(value, '[1, 2, 3]')
+            self.assertText('[1, 2, 3]', value)
 
         with self.subTest('Test dict - No spaces'):
             value = self.standardize_html_tags('{"one": 1, "two": 2}')
-            self.assertEqual(value, '{"one": 1, "two": 2}')
+            self.assertText('{"one": 1, "two": 2}', value)
 
         with self.subTest('Test dict - With spaces'):
             value = self.standardize_html_tags('{  "one": 1, "two": 2  }  ')
-            self.assertEqual(value, '{"one": 1, "two": 2}')
+            self.assertText('{"one": 1, "two": 2}', value)
 
     def test__find_elements_by_tag__success(self):
         """
         Tests find_elements_by_tag() function, in cases when it should succeed.
         """
         with self.subTest('When expected element is the only item, with standard element'):
             response = HttpResponse('<li></li>')
@@ -3540,40 +4220,40 @@
         with self.subTest('When expected element is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find element "<li>" in content. Provided content was:\n'
 
             # By base element tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, 'li')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element open tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, '<li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element close tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, '</li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected element is not present - Single-item response'):
             response = HttpResponse('<p></p>')
             err_msg = 'Unable to find element "<li>" in content. Provided content was:\n<p></p>'
 
             # By base element tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, 'li')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element open tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, '<li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element close tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, '</li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected element is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p>Some text.</p>
@@ -3591,23 +4271,23 @@
                 '<p>Some text with the str "li" in it.</p>\n'
                 '</div>\n'
             )
 
             # By base element tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, 'li')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element open tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, '<li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element close tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_tag(response, '</li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_element_by_tag__success(self):
         """
         Tests find_element_by_tag() function, in cases when it should succeed.
         """
         with self.subTest('When expected element is the only item, with standard element'):
             response = HttpResponse('<li></li>')
@@ -3680,40 +4360,40 @@
         with self.subTest('When expected element is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find element "<li>" in content. Provided content was:\n'
 
             # By base element tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, 'li')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element open tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, '<li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element close tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, '</li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected element is not present - Single-item response'):
             response = HttpResponse('<p></p>')
             err_msg = 'Unable to find element "<li>" in content. Provided content was:\n<p></p>'
 
             # By base element tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, 'li')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element open tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, '<li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element close tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, '</li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected element is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p>Some text.</p>
@@ -3731,43 +4411,43 @@
                 '<p>Some text with the str "li" in it.</p>\n'
                 '</div>\n'
             )
 
             # By base element tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, 'li')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element open tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, '<li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element close tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, '</li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected element is present multiple times'):
             response = HttpResponse('<li></li><li></li>')
             err_msg = (
                 'Found multiple instances of "<li>" element. Expected only one instance. Content was:\n'
                 '<li></li><li></li>'
             )
 
             # By base element tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, 'li')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element open tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, '<li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
             # By standard element close tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_tag(response, '</li>')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_elements_by_id__success(self):
         """
         Tests find_elements_by_id() function, in cases when it should succeed.
         """
         with self.subTest('When expected id is the only item'):
             # As <li> tag.
@@ -3845,23 +4525,23 @@
         """
         with self.subTest('When expected id is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find id "test_id" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected id is not present - Single-item response'):
             response = HttpResponse('<p id="test"></p>')
             err_msg = 'Unable to find id "test_id" in content. Provided content was:\n<p id="test"></p>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected id is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p id="some_value">Some text.</p>
@@ -3878,15 +4558,15 @@
                 '<p id="another_id">Some more text.</p>\n'
                 '<p>Some text with the str "id" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_element_by_id__success(self):
         """
         Tests find_element_by_id() function, in cases when it should succeed.
         """
         with self.subTest('When expected id is the only item'):
             # As <li> tag.
@@ -3946,23 +4626,23 @@
         """
         with self.subTest('When expected id is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find id "test_id" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected id is not present - Single-item response'):
             response = HttpResponse('<p id="some_id"></p>')
             err_msg = 'Unable to find id "test_id" in content. Provided content was:\n<p id="some_id"></p>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected id is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p id="some_value">Some text.</p>
@@ -3980,49 +4660,49 @@
                 '<p>Some text with the str "id" in it.</p>\n'
                 '</div>\n'
             )
 
             # By base element tag.
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected id is present multiple times'):
             # As <li> tag.
             response = HttpResponse('<li id="test_id"></li><li id="test_id"></li>')
             err_msg = (
                 'Found multiple instances of "test_id" id. Expected only one instance. Content was:\n'
                 '<li id="test_id"></li><li id="test_id"></li>'
             )
             with self.assertRaises(AssertionError) as err:
                 with self.assertLogs(level=logging.WARNING):
                     self.find_element_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # As <p> tag.
             response = HttpResponse('<p id="test_id"></p><p id="test_id"></p>')
             err_msg = (
                 'Found multiple instances of "test_id" id. Expected only one instance. Content was:\n'
                 '<p id="test_id"></p><p id="test_id"></p>'
             )
             with self.assertRaises(AssertionError) as err:
                 with self.assertLogs(level=logging.WARNING):
                     self.find_element_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # As mixed tags.
             response = HttpResponse('<li id="test_id"><p id="test_id">Test</p></li>')
             err_msg = (
                 'Found multiple instances of "test_id" id. Expected only one instance. Content was:\n'
                 '<li id="test_id"><p id="test_id">Test</p></li>'
             )
             with self.assertRaises(AssertionError) as err:
                 with self.assertLogs(level=logging.WARNING):
                     self.find_element_by_id(response, 'test_id')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_elements_by_class__success(self):
         """
         Tests find_elements_by_class() function, in cases when it should succeed.
         """
         with self.subTest('When expected class is the only item'):
             # As <li>  tag.
@@ -4098,23 +4778,23 @@
         """
         with self.subTest('When expected class is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find class "test_class" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_class(response, 'test_class')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected class is not present - Single-item response'):
             response = HttpResponse('<p class="some_class"></p>')
             err_msg = 'Unable to find class "test_class" in content. Provided content was:\n<p class="some_class"></p>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_class(response, 'test_class')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected class is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p>Some text.</p>
@@ -4131,15 +4811,15 @@
                 '<p>Some more text.</p>\n'
                 '<p>Some text with the str "class" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_class(response, 'test_class')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_element_by_class__success(self):
         """
         Tests find_element_by_class() function, in cases when it should succeed.
         """
         with self.subTest('When expected class is the only item'):
             # As <li> tag.
@@ -4193,23 +4873,23 @@
         """
         with self.subTest('When expected class is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find class "test_class" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_class(response, 'test_class')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected class is not present - Single-item response'):
             response = HttpResponse('<p class="some_class"></p>')
             err_msg = 'Unable to find class "test_class" in content. Provided content was:\n<p class="some_class"></p>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_class(response, 'test_class')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected class is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p class="some_class">Some text.</p>
@@ -4226,38 +4906,38 @@
                 '<p class="another_class">Some more text.</p>\n'
                 '<p class="test">Some text with the str "class" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_class(response, 'test_class')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected class is present multiple times'):
             # As <li> tag.
             response = HttpResponse('<li class="test_class"></li><li class="test_class"></li>')
             err_msg = (
                 'Found multiple instances of "test_class" class. Expected only one instance. Content was:\n'
                 '<li class="test_class"></li><li class="test_class"></li>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_class(response, 'test_class')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # As <p> tag.
             response = HttpResponse('<p class="test_class"></p><p class="test_class"></p>')
             err_msg = (
                 'Found multiple instances of "test_class" class. Expected only one instance. Content was:\n'
                 '<p class="test_class"></p><p class="test_class"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_class(response, 'test_class')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_elements_by_css_selector__success(self):
         """
         Tests find_elements_by_css_selector() function, in cases when it should succeed.
         """
         with self.subTest('When expected css_selector is the only item, with standard element'):
             response = HttpResponse('<li><p class="test_class"><a>One</a></p></li>')
@@ -4310,46 +4990,46 @@
         """
         with self.subTest('When expected css_selector is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find css selector "li .test_class > a" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected css_selector is not present - Single-item response'):
             # Missing all parts.
             response = HttpResponse('<p></p>')
             err_msg = 'Unable to find css selector "li .test_class > a" in content. Provided content was:\n<p></p>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # Missing two parts.
             response = HttpResponse('<li></li>')
             err_msg = (
                 'Unable to find css selector "li .test_class > a" in content. '
                 'Provided content was:\n<li></li>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # Missing one part.
             response = HttpResponse('<li><p class="test_class"></p></li>')
             err_msg = (
                 'Unable to find css selector "li .test_class > a" in content. '
                 'Provided content was:\n<li><p class="test_class"></p></li>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected css_selector is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p>Some text.</p>
@@ -4366,15 +5046,15 @@
                 '<p>Some more text.</p>\n'
                 '<p>Some text with the str "css_selector" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_element_by_css_selector__success(self):
         """
         Tests find_element_by_css_selector() function, in cases when it should succeed.
         """
         with self.subTest('When expected css_selector is the only item, with standard element'):
             response = HttpResponse('<li><p class="test_class"><a>One</a></p></li>')
@@ -4408,43 +5088,43 @@
         """
         with self.subTest('When expected css_selector is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find css selector "li .test_class > a" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected css_selector is not present - Single-item response'):
             # Missing all parts.
             response = HttpResponse('<p></p>')
             err_msg = 'Unable to find css selector "li .test_class > a" in content. Provided content was:\n<p></p>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # Missing two parts.
             response = HttpResponse('<li></li>')
             err_msg = 'Unable to find css selector "li .test_class > a" in content. Provided content was:\n<li></li>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # Missing one parts.
             response = HttpResponse('<li><p class="test_class"></p></li>')
             err_msg = (
                 'Unable to find css selector "li .test_class > a" in content. '
                 'Provided content was:\n<li><p class="test_class"></p></li>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected css_selector is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p>Some text.</p>
@@ -4461,15 +5141,15 @@
                 '<p>Some more text.</p>\n'
                 '<p>Some text with the str "css_selector" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected css_selector is present multiple times'):
             response = HttpResponse(
                 """
                 <li><p class="test_class"><a>One</a></p></li>
                 <li><p class="test_class"><a>Two</a></p></li>
                 """
@@ -4479,15 +5159,15 @@
                 ' Content was:\n'
                 '<li><p class="test_class"><a>One</a></p></li>\n'
                 '<li><p class="test_class"><a>Two</a></p></li>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_css_selector(response, 'li .test_class > a')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_elements_by_data_attribute__success(self):
         """
         Tests find_elements_by_data_attribute() function, in cases when it should succeed.
         """
         with self.subTest('When expected data_attribute is the only item, with standard element'):
             # As <li> tag.
@@ -4574,48 +5254,48 @@
         """
         with self.subTest('When expected data_attribute is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find data attribute "my_attr" with value "my_val" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected data_attribute is not present - Single-item response'):
             response = HttpResponse('<p some_attr="some_val"></p>')
             err_msg = (
                 'Unable to find data attribute "my_attr" with value "my_val" in content. '
                 'Provided content was:\n<p some_attr="some_val"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected data_attribute key is not present - Single-item response'):
             response = HttpResponse('<p some_attr="my_val"></p>')
             err_msg = (
                 'Unable to find data attribute "my_attr" with value "my_val" in content. '
                 'Provided content was:\n<p some_attr="my_val"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected data_attribute value is not present - Single-item response'):
             response = HttpResponse('<p my_attr="some_val"></p>')
             err_msg = (
                 'Unable to find data attribute "my_attr" with value "my_val" in content. '
                 'Provided content was:\n<p my_attr="some_val"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected data_attribute is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p some_attr="some_val">Some text.</p>
@@ -4632,15 +5312,15 @@
                 '<p another_attr="another_val">Some more text.</p>\n'
                 '<p test="test">Some text with the str "data_attribute" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_element_by_data_attribute__success(self):
         """
         Tests find_element_by_data_attribute() function, in cases when it should succeed.
         """
         with self.subTest('When expected data_attribute is the only item, with standard element'):
             # As <li> tag.
@@ -4700,48 +5380,48 @@
         """
         with self.subTest('When expected data_attribute is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find data attribute "my_attr" with value "my_val" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected data_attribute is not present - Single-item response'):
             response = HttpResponse('<p some_attr="some_val"></p>')
             err_msg = (
                 'Unable to find data attribute "my_attr" with value "my_val" in content. '
                 'Provided content was:\n<p some_attr="some_val"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected data_attribute key is not present - Single-item response'):
             response = HttpResponse('<p some_attr="my_val"></p>')
             err_msg = (
                 'Unable to find data attribute "my_attr" with value "my_val" in content. '
                 'Provided content was:\n<p some_attr="my_val"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected data_attribute value is not present - Single-item response'):
             response = HttpResponse('<p my_attr="some_val"></p>')
             err_msg = (
                 'Unable to find data attribute "my_attr" with value "my_val" in content. '
                 'Provided content was:\n<p my_attr="some_val"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected data_attribute is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p some_attr="some_val">Some text.</p>
@@ -4758,38 +5438,38 @@
                 '<p another_attr="another_val">Some more text.</p>\n'
                 '<p test="test">Some text with the str "data_attribute" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected element is present multiple times'):
             # As <li> tag.
             response = HttpResponse('<li my_attr="my_val"></li><li my_attr="my_val"></li>')
             err_msg = (
                 'Found multiple instances of "my_attr" data attribute with value "my_val". Expected only one instance. '
                 'Content was:\n<li my_attr="my_val"></li><li my_attr="my_val"></li>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # As <p> tag.
             response = HttpResponse('<p my_attr="my_val"></p><p my_attr="my_val"></p>')
             err_msg = (
                 'Found multiple instances of "my_attr" data attribute with value "my_val". Expected only one instance. '
                 'Content was:\n<p my_attr="my_val"></p><p my_attr="my_val"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_data_attribute(response, 'my_attr', 'my_val')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_elements_by_name__success(self):
         """
         Tests find_elements_by_name() function, in cases when it should succeed.
         """
         with self.subTest('When expected name is the only item'):
             # As <li> tag.
@@ -4876,24 +5556,24 @@
         """
         with self.subTest('When expected name is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find name "test_name" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_name(response, 'test_name')
-            self.assertText(str(err.exception), err_msg)
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected name is not present - Single-item response'):
             response = HttpResponse('<p name="other_name"></p>')
             err_msg = 'Unable to find name "test_name" in content. Provided content was:\n<p name="other_name"></p>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_name(response, 'test_name')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected name is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p name="other_name">Some text.</p>
@@ -4910,15 +5590,15 @@
                 '<p name="another_name">Some more text.</p>\n'
                 '<p name="test">Some text with the str "name" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_name(response, 'test_name')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_element_by_name__success(self):
         """
         Tests find_element_by_name() function, in cases when it should succeed.
         """
         with self.subTest('When expected name is the only item, with standard element'):
             # As <li> tag.
@@ -4974,23 +5654,23 @@
         """
         with self.subTest('When expected name is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find name "test_name" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_name(response, 'test_name')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected name is not present - Single-item response'):
             response = HttpResponse('<p name="other_name"></p>')
             err_msg = 'Unable to find name "test_name" in content. Provided content was:\n<p name="other_name"></p>'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_name(response, 'test_name')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected name is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <p name="other_name">Some text.</p>
@@ -5007,38 +5687,38 @@
                 '<p name="another_name">Some more text.</p>\n'
                 '<p name="test">Some text with the str "li" in it.</p>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_name(response, 'test_name')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected element is present multiple times'):
             # As <li> tag.
             response = HttpResponse('<li name="test_name"></li><li name="test_name"></li>')
             err_msg = (
                 'Found multiple instances of "test_name" name. Expected only one instance. Content was:\n'
                 '<li name="test_name"></li><li name="test_name"></li>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_name(response, 'test_name')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
             # As <p> tag.
             response = HttpResponse('<p name="test_name"></p><p name="test_name"></p>')
             err_msg = (
                 'Found multiple instances of "test_name" name. Expected only one instance. Content was:\n'
                 '<p name="test_name"></p><p name="test_name"></p>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_name(response, 'test_name')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_elements_by_link_text__success(self):
         """
         Tests find_elements_by_link_text() function, in cases when it should succeed.
         """
         with self.subTest('When expected link_text is the only item, with standard element'):
             response = HttpResponse('<a href="test_link_text"></a>')
@@ -5085,26 +5765,26 @@
         """
         with self.subTest('When expected link_text is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find link text "test_link_text" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_link_text(response, 'test_link_text')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected link_text is not present - Single-item response'):
             response = HttpResponse('<a href="other_link_text"></a>')
             err_msg = (
                 'Unable to find link text "test_link_text" in content. '
                 'Provided content was:\n<a href="other_link_text"></a>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_link_text(response, 'test_link_text')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected link_text is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <a href="other_link_text">Some text.</a>
@@ -5120,15 +5800,15 @@
                 '<a href="other_link_text">Some text.</a>\n'
                 '<a href="another_link_text">Some more text.</a>\n'
                 '<a href="test">Some text with the str "link_text" in it.</a>\n'
                 '</div>\n'
             )
             with self.assertRaises(AssertionError) as err:
                 self.find_elements_by_link_text(response, 'test_link_text')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     def test__find_element_by_link_text__success(self):
         """
         Tests find_element_by_link_text() function, in cases when it should succeed.
         """
         with self.subTest('When expected element is the only item, with standard element'):
             response = HttpResponse('<a href="test_link_text"></a>')
@@ -5159,26 +5839,26 @@
         """
         with self.subTest('When expected link_text is not present - Blank response'):
             response = HttpResponse('')
             err_msg = 'Unable to find link text "test_link_text" in content. Provided content was:\n'
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_link_text(response, 'test_link_text')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected link_text is not present - Single-item response'):
             response = HttpResponse('<a href="other_link_text"></a>')
             err_msg = (
                 'Unable to find link text "test_link_text" in content. '
                 'Provided content was:\n<a href="other_link_text"></a>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_link_text(response, 'test_link_text')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected link_text is not present - Multi-item response'):
             response = HttpResponse(
                 """
                 <div>
                     <h1>Page Header</h1>
                     <a href="other_link_text">Some text.</a>
@@ -5195,30 +5875,80 @@
                 '<a href="another_link_text">Some more text.</a>\n'
                 '<a href="test">Some text with the str "link_text" in it.</a>\n'
                 '</div>\n'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_link_text(response, 'test_link_text')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
         with self.subTest('When expected link_text is present multiple times'):
             response = HttpResponse('<a href="test_link_text"></a><a href="test_link_text"></a>')
             err_msg = (
                 'Found multiple instances of "test_link_text" link text. Expected only one instance. Content was:\n'
                 '<a href="test_link_text"></a><a href="test_link_text"></a>'
             )
 
             with self.assertRaises(AssertionError) as err:
                 self.find_element_by_link_text(response, 'test_link_text')
-            self.assertText(str(err.exception), err_msg)
+            self.assertText(err_msg, str(err.exception))
 
     # endregion Helper Function Tests
 
 
+class IntegrationClassTest__WithExtraAuthUpdate(IntegrationClassTest__Base):
+
+    def _get_login_user__extra_user_auth_setup(self, *args, **kwargs):
+        """Modified extra_user_auth_setup function, to mimic actually setting additional logic for user auth."""
+
+        # Add some arbitrary session data.
+        # Being able to save session data is sometimes required for user auth setup,
+        # such as certain 2-factor implementations.
+        session = self.client.session
+        session['etc_testing_session_variable_1'] = True
+        session.save()
+        session['etc_testing_session_variable_2'] = False
+        session.save()
+        session['etc_testing_session_variable_3'] = 'Some Value'
+        session.save()
+
+        # Call parent logic.
+        user = super()._get_login_user__extra_user_auth_setup(*args, **kwargs)
+
+        # Add more arbitrary data.
+        # Ensures we can persist session data both before and after calling parent function logic.
+        session = self.client.session
+        session['etc_testing_session_variable_4'] = True
+        session.save()
+        session['etc_testing_session_variable_5'] = False
+        session.save()
+        session['etc_testing_session_variable_6'] = 'Some Value'
+        session.save()
+
+        # Return original user value.
+        return user
+
+    def test__can_set_session_data_in__extra_user_auth_setup(self):
+        """Verify that we can access our extra session data, set as part of the extra_user_auth function."""
+
+        # Get arbitrary response that has gone through user authentication logic.
+        response = self.assertGetResponse('django_expanded_test_cases:index', user='test_user')
+
+        # Grab session object from response.
+        session = response.client.session
+
+        # Verify expected session data is present.
+        self.assertTrue(session.get('etc_testing_session_variable_1', None))
+        self.assertFalse(session.get('etc_testing_session_variable_2', None))
+        self.assertText('Some Value', session.get('etc_testing_session_variable_3', None))
+        self.assertTrue(session.get('etc_testing_session_variable_4', None))
+        self.assertFalse(session.get('etc_testing_session_variable_5', None))
+        self.assertText('Some Value', session.get('etc_testing_session_variable_6', None))
+
+
 class IntegrationClassTest__StrictnessOfAnonymous(IntegrationTestCase):
     """Tests for IntegrationTestCase class, specifically with user strictness set to "anonymous"."""
 
     @classmethod
     @patch('django_expanded_test_cases.test_cases.integration_test_case.ETC_REQUEST_USER_STRICTNESS', 'anonymous')
     def setUpClass(cls):
         # Run parent setup logic.
```

### Comparing `django-expanded-test-cases-0.4.0/tests/test_cases/test_live_server_case.py` & `django-expanded-test-cases-0.5.0/tests/test_cases/test_channels_live_server_case.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """
-Tests for test_cases/live_server_test_case.py.
+Tests for test_cases/channels_live_server_test_case.py.
 """
 
 # System Imports.
 import unittest
 
 # Internal Imports.
-from django_expanded_test_cases import LiveServerTestCase
+from .universal_live_test_mixin import UniversalLiveTestMixin
+from django_expanded_test_cases import ChannelsLiveServerTestCase
 
 
 def skip_if_channels_not_installed():
-    """Skip decorator, to handle when channels package is not installed."""
+    """Skip decorator, to handle when selenium package is not installed."""
     try:
-        from channels.testing import ChannelsLiveServerTestCase
+        import webdriver_manager
+        from selenium import webdriver
+        from selenium.webdriver.chrome.service import Service as ChromeService
+        from selenium.webdriver.firefox.service import Service as FireFoxService
+        from channels.testing import ChannelsLiveServerTestCase as DjangoChannelsLiveServerTestCase
 
         # If we made it this far, channels is installed. Proceed with test.
         return False
     except ModuleNotFoundError:
         # Failed to import channels. Skip test.
         return True
 
 
-class LiveServerClassTest(LiveServerTestCase):
+class LiveServerClassTest(ChannelsLiveServerTestCase, UniversalLiveTestMixin):
     """Tests for LiveServerTestCase class."""
 
     @classmethod
-    @unittest.skipIf(skip_if_channels_not_installed(), 'Requires "channels" package.')
+    @unittest.skipIf(skip_if_channels_not_installed(), 'Requires "selenium" package.')
     def setUpClass(cls):
         # Run parent setup logic.
         super().setUpClass()
 
-    @unittest.skipIf(skip_if_channels_not_installed(), 'Requires "channels" package.')
+    @unittest.skipIf(skip_if_channels_not_installed(), 'Requires "selenium" package.')
     def setUp(self):
         # Run parent setup logic.
         super().setUp()
 
-    @unittest.skipIf(skip_if_channels_not_installed(), 'Requires "channels" package.')
+    @unittest.skipIf(skip_if_channels_not_installed(), 'Requires "selenium" package.')
     def __int__(self, *args, **kwargs):
         # Run parent setup logic.
         super().__init__(*args, **kwargs)
 
     # def test_window_generate_destroy(self):
     #     driver = self.create_driver()
     #
```

### Comparing `django-expanded-test-cases-0.4.0/tests/views.py` & `django-expanded-test-cases-0.5.0/tests/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,104 +2,148 @@
 Testing views for django-expanded-test-cases project.
 """
 
 # Third-Party Imports.
 from django.contrib import messages
 from django.contrib.auth import get_user_model
 from django.http import JsonResponse
-from django.shortcuts import get_object_or_404, redirect, render
+from django.shortcuts import get_object_or_404, redirect, render, reverse
 from django.template.response import TemplateResponse
 
 
 def index(request):
     """Page that simulates a site index/home."""
+
     # Render response.
     return render(request, 'django_expanded_test_cases/index.html', {
         'header': 'Home Page',
         'text': 'Pretend this is the project landing page.',
     })
 
 
 def template_response_index(request):
     """Page that simulates a site index/home. Specifically served as TemplateResponse."""
+
     # Render response.
     return TemplateResponse(request, 'django_expanded_test_cases/index.html', {
         'header': 'Home Page',
         'text': 'Pretend this is the project landing page.',
     })
 
 
 def login(request):
     """Page that simulates a login page."""
+
     # Render response.
     return render(request, 'django_expanded_test_cases/index.html', {
         'header': 'Login Page',
         'text': 'Pretend this is a login page.',
     })
 
 
 def view_with_one_message(request):
     """Page that simulates a view with a single message."""
+
+    # Generate response messages.
     messages.info(request, 'This is a test message.')
 
     # Render response.
     return render(request, 'django_expanded_test_cases/index.html', {
         'header': 'View with One Message',
         'text': (
             'Pretend useful stuff is displayed here, for one-message render() view.'
         )
     })
 
 
 def view_with_two_messages(request):
     """Page that simulates a view with two messages."""
+
+    # Generate response messages.
     messages.info(request, 'Test message #1.')
     messages.warning(request, 'Test message #2.')
 
     # Render response.
     return render(request, 'django_expanded_test_cases/index.html', {
         'header': 'View with Two Messages',
         'text': (
             'Pretend useful stuff is displayed here, for two-message render() view.'
         )
     })
 
 
 def view_with_three_messages(request):
     """Page that simulates a view with three messages."""
+
+    # Generate response messages.
     messages.info(request, 'Test info message.')
     messages.warning(request, 'Test warning message.')
     messages.error(request, 'Test error message.')
 
     # Render response.
     return render(request, 'django_expanded_test_cases/index.html', {
         'header': 'View with Three Messages',
         'text': (
             'Pretend useful stuff is displayed here, for three-message render() view.'
         )
     })
 
 
+def view_with_args(request, id, name):
+    """Page that simulates a view with passed args."""
+
+    # Render response.
+    return render(request, 'django_expanded_test_cases/index.html', {
+        'header': 'View with Args',
+        'text': (
+            'Pretend useful stuff is displayed here, for render() view with url args.'
+        ),
+        'li_set': (
+            'id: "{0}"'.format(id),
+            'name: "{0}"'.format(name),
+        ),
+    })
+
+
 def template_response_with_three_messages(request):
     """Page that simulates a view with three messages. Specifically served as TemplateResponse."""
+
+    # Generate response messages.
     messages.info(request, 'Test info message.')
     messages.warning(request, 'Test warning message.')
     messages.error(request, 'Test error message.')
 
     # Render response.
     return TemplateResponse(request, 'django_expanded_test_cases/index.html', {
-        'header': 'View with Three Messages',
+        'header': 'TemplateResponse View with Three Messages',
         'text': (
             'Pretend useful stuff is displayed here, for three-message TemplateResponse view.'
         )
     })
 
 
+def template_response_with_args(request, id, name):
+    """Page that simulates a view with passed args. Specifically served as a TemplateResponse."""
+
+    # Render response.
+    return TemplateResponse(request, 'django_expanded_test_cases/index.html', {
+        'header': 'TemplateResponse View with Args',
+        'text': (
+            'Pretend useful stuff is displayed here, for TemplateResponse view with url args.'
+        ),
+        'li_set': (
+            'id: "{0}"'.format(id),
+            'name: "{0}"'.format(name),
+        ),
+    })
+
+
 def user_detail(request, pk):
     """Page that simulates a model detail page."""
+
     # Pull database info.
     user = get_object_or_404(get_user_model(), pk=pk)
 
     # Render response.
     return render(request, 'django_expanded_test_cases/index.html', {
         'header': 'User Detail Page',
         'text': '{0}'.format(user),
@@ -112,8 +156,20 @@
             'Is Staff: "{0}"'.format(user.is_staff),
         )
     })
 
 
 def redirect_to_index(request):
     """Page that simulates a redirect."""
+
+    # Redirect to intended view.
     return redirect('django_expanded_test_cases:index')
+
+
+def redirect_with_args(request, id, name):
+    """Page that simulates a redirect, with included url args."""
+
+    # Redirect to intended view.
+    return redirect(reverse(
+        'django_expanded_test_cases:template-response-with-args',
+        args=(id, name),
+    ))
```

