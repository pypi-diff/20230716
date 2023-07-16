# Comparing `tmp/poeditor-1.1.2.tar.gz` & `tmp/poeditor-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/poeditor-1.1.2.tar", last modified: Thu Mar 14 12:02:25 2019, max compression
+gzip compressed data, was "poeditor-1.1.3.tar", last modified: Sun Jul 16 17:28:38 2023, max compression
```

## Comparing `poeditor-1.1.2.tar` & `poeditor-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 karl       (501) staff       (20)        0 2019-03-14 12:02:25.000000 poeditor-1.1.2/
--rw-r--r--   0 karl       (501) staff       (20)     2553 2019-03-14 12:02:25.000000 poeditor-1.1.2/PKG-INFO
--rw-r--r--   0 karl       (501) staff       (20)     1076 2018-07-13 07:50:55.000000 poeditor-1.1.2/LICENSE.md
--rw-r--r--   0 karl       (501) staff       (20)       45 2018-07-13 07:50:55.000000 poeditor-1.1.2/MANIFEST.in
--rw-r--r--   0 karl       (501) staff       (20)     1117 2019-03-14 11:58:26.000000 poeditor-1.1.2/setup.py
-drwxr-xr-x   0 karl       (501) staff       (20)        0 2019-03-14 12:02:25.000000 poeditor-1.1.2/poeditor/
--rw-r--r--   0 karl       (501) staff       (20)    25407 2019-03-14 11:48:59.000000 poeditor-1.1.2/poeditor/client.py
-drwxr-xr-x   0 karl       (501) staff       (20)        0 2019-03-14 12:02:25.000000 poeditor-1.1.2/poeditor/tests/
--rw-r--r--   0 karl       (501) staff       (20)        0 2018-07-13 07:50:55.000000 poeditor-1.1.2/poeditor/tests/__init__.py
--rw-r--r--   0 karl       (501) staff       (20)     9270 2018-07-13 12:35:13.000000 poeditor-1.1.2/poeditor/tests/test_client.py
--rw-r--r--   0 karl       (501) staff       (20)      357 2019-03-14 11:55:59.000000 poeditor-1.1.2/poeditor/__init__.py
--rw-r--r--   0 karl       (501) staff       (20)      977 2018-07-17 12:05:47.000000 poeditor-1.1.2/poeditor/dummy.py
--rw-r--r--   0 karl       (501) staff       (20)       38 2019-03-14 12:02:25.000000 poeditor-1.1.2/setup.cfg
-drwxr-xr-x   0 karl       (501) staff       (20)        0 2019-03-14 12:02:25.000000 poeditor-1.1.2/poeditor.egg-info/
--rw-r--r--   0 karl       (501) staff       (20)     2553 2019-03-14 12:02:25.000000 poeditor-1.1.2/poeditor.egg-info/PKG-INFO
--rw-r--r--   0 karl       (501) staff       (20)      316 2019-03-14 12:02:25.000000 poeditor-1.1.2/poeditor.egg-info/SOURCES.txt
--rw-r--r--   0 karl       (501) staff       (20)        9 2019-03-14 12:02:25.000000 poeditor-1.1.2/poeditor.egg-info/requires.txt
--rw-r--r--   0 karl       (501) staff       (20)        9 2019-03-14 12:02:25.000000 poeditor-1.1.2/poeditor.egg-info/top_level.txt
--rw-r--r--   0 karl       (501) staff       (20)        1 2019-03-14 12:02:25.000000 poeditor-1.1.2/poeditor.egg-info/dependency_links.txt
--rw-r--r--   0 karl       (501) staff       (20)     1321 2018-07-13 15:00:46.000000 poeditor-1.1.2/README.rst
+drwxr-xr-x   0 karl       (501) staff       (20)        0 2023-07-16 17:28:38.166597 poeditor-1.1.3/
+-rw-r--r--   0 karl       (501) staff       (20)     1076 2018-07-13 07:50:55.000000 poeditor-1.1.3/LICENSE.md
+-rw-r--r--   0 karl       (501) staff       (20)       45 2018-07-13 07:50:55.000000 poeditor-1.1.3/MANIFEST.in
+-rw-r--r--   0 karl       (501) staff       (20)     2123 2023-07-16 17:28:38.166488 poeditor-1.1.3/PKG-INFO
+-rw-r--r--   0 karl       (501) staff       (20)     1321 2018-07-13 15:00:46.000000 poeditor-1.1.3/README.rst
+drwxr-xr-x   0 karl       (501) staff       (20)        0 2023-07-16 17:28:38.165617 poeditor-1.1.3/poeditor/
+-rw-r--r--   0 karl       (501) staff       (20)      357 2023-07-16 13:58:29.000000 poeditor-1.1.3/poeditor/__init__.py
+-rw-r--r--   0 karl       (501) staff       (20)    25324 2023-07-16 13:56:25.000000 poeditor-1.1.3/poeditor/client.py
+-rw-r--r--   0 karl       (501) staff       (20)      977 2018-07-17 12:05:47.000000 poeditor-1.1.3/poeditor/dummy.py
+drwxr-xr-x   0 karl       (501) staff       (20)        0 2023-07-16 17:28:38.166349 poeditor-1.1.3/poeditor/tests/
+-rw-r--r--   0 karl       (501) staff       (20)        0 2018-07-13 07:50:55.000000 poeditor-1.1.3/poeditor/tests/__init__.py
+-rw-r--r--   0 karl       (501) staff       (20)     9270 2023-07-16 08:59:35.000000 poeditor-1.1.3/poeditor/tests/test_client.py
+drwxr-xr-x   0 karl       (501) staff       (20)        0 2023-07-16 17:28:38.166154 poeditor-1.1.3/poeditor.egg-info/
+-rw-r--r--   0 karl       (501) staff       (20)     2123 2023-07-16 17:28:38.000000 poeditor-1.1.3/poeditor.egg-info/PKG-INFO
+-rw-r--r--   0 karl       (501) staff       (20)      316 2023-07-16 17:28:38.000000 poeditor-1.1.3/poeditor.egg-info/SOURCES.txt
+-rw-r--r--   0 karl       (501) staff       (20)        1 2023-07-16 17:28:38.000000 poeditor-1.1.3/poeditor.egg-info/dependency_links.txt
+-rw-r--r--   0 karl       (501) staff       (20)        9 2023-07-16 17:28:38.000000 poeditor-1.1.3/poeditor.egg-info/requires.txt
+-rw-r--r--   0 karl       (501) staff       (20)        9 2023-07-16 17:28:38.000000 poeditor-1.1.3/poeditor.egg-info/top_level.txt
+-rw-r--r--   0 karl       (501) staff       (20)       38 2023-07-16 17:28:38.166629 poeditor-1.1.3/setup.cfg
+-rw-r--r--   0 karl       (501) staff       (20)     1117 2019-03-14 11:58:26.000000 poeditor-1.1.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `poeditor-1.1.2/LICENSE.md` & `poeditor-1.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `poeditor-1.1.2/setup.py` & `poeditor-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `poeditor-1.1.2/poeditor/client.py` & `poeditor-1.1.3/poeditor/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,35 +10,22 @@
 
 import json
 import requests
 import sys
 import tempfile
 import warnings
 
+from contextlib import nullcontext
 from datetime import datetime
 
 __all__ = ['POEditorException', 'POEditorArgsException', 'POEditorAPI']
 
 
-if sys.version_info < (3, 2):
-    from datetime import timedelta
-
-    def parse_datetime(dt_string):
-        # Hacky and not really equivalent to the Python3.2 version but will do for most use cases,
-        # that way we can avoid adding an extra dependency like dateutil or iso8601
-        ret = datetime.strptime(dt_string[:19], '%Y-%m-%dT%H:%M:%S')
-        if dt_string[19] == '+':
-           ret -= timedelta(hours=int(dt_string[20:22]), minutes=int(dt_string[22:]))
-        elif dt_string[19] == '-':
-           ret += timedelta(hours=int(dt_string[20:22]), minutes=int(dt_string[22:]))
-        return ret
-else:
-    # https://docs.python.org/3/whatsnew/3.2.html#datetime-and-time
-    def parse_datetime(dt_string):
-        return datetime.strptime(dt_string, '%Y-%m-%dT%H:%M:%S%z')
+def parse_datetime(dt_string):
+    return datetime.strptime(dt_string, '%Y-%m-%dT%H:%M:%S%z')
 
 
 class POEditorException(Exception):
     """
     POEditor API exception
     """
     def __init__(self, error_code, status, message):
@@ -67,17 +54,18 @@
     Connect your software to POEditor with its simple API
     Please refers to https://poeditor.com/docs/api if you have questions
     """
 
     HOST = "https://api.poeditor.com/v2/"
 
     SUCCESS_CODE = "success"
-    FILE_TYPES = ['po', 'pot', 'mo', 'xls', 'csv', 'resx', 'resw', 'android_strings',
-                  'apple_strings', 'xliff', 'properties', 'key_value_json', 'json',
-                  'xmb', 'xtb']
+    FILE_TYPES = ['arb', 'csv', 'ini', 'key_value_json', 'json', 'po', 'pot',
+                  'mo', 'properties', 'resw', 'resx', 'ts', 'apple_strings',
+                  'xliff', 'xliff_1_2', 'xlf', 'xmb', 'xtb', 'rise_360_xliff',
+                  'xls', 'xlsx', 'android_strings', 'yml']
     FILTER_BY = ['translated', 'untranslated', 'fuzzy', 'not_fuzzy',
                  'automatic', 'not_automatic', 'proofread', 'not_proofread']
 
     UPDATING_TERMS = 'terms'
     UPDATING_TERMS_TRANSLATIONS = 'terms_translations'
     UPDATING_TRANSLATIONS = 'translations'
 
@@ -194,26 +182,28 @@
             url_path="projects/add",
             name=name,
             description=description
         )
         return data['result']['project']['id']
 
     def update_project(self, project_id, name=None, description=None,
-                       reference_language=None):
+                       reference_language=None, fallback_language=None):
         """
         Updates project settings (name, description, reference language)
         If optional parameters are not sent, their respective fields are not updated.
         """
         kwargs = {}
         if name is not None:
             kwargs['name'] = name
         if description is not None:
             kwargs['description'] = description
         if reference_language is not None:
             kwargs['reference_language'] = reference_language
+        if fallback_language is not None:
+            kwargs['fallback_language'] = fallback_language
 
         data = self._run(
             url_path="projects/update",
             id=project_id,
             **kwargs
         )
         return data['result']['project']['id']
@@ -340,36 +330,14 @@
             data=json.dumps(data)
         )
         return data['result']['terms']
 
     def update_terms(self, project_id, data, fuzzy_trigger=None):
         """
         Updates project terms. Lets you change the text, context, reference, plural and tags.
-
-        >>> data = [
-                {
-                    "term": "Add new list",
-                    "context": "",
-                    "new_term": "Save list",
-                    "new_context": "",
-                    "reference": "\/projects",
-                    "plural": "",
-                    "comment": "",
-                    "tags": [
-                        "first_tag",
-                        "second_tag"
-                    ]
-                },
-                {
-                    "term": "Display list",
-                    "context": "",
-                    "new_term": "Show list",
-                    "new_context": ""
-                }
-            ]
         """
         kwargs = {}
         if fuzzy_trigger is not None:
             kwargs['fuzzy_trigger'] = fuzzy_trigger
 
         data = self._run(
             url_path="terms/update",
@@ -495,22 +463,26 @@
             language=language_code,
             data=json.dumps(data),
             **kwargs
         )
         return data['result']['translations']
 
     def export(self, project_id, language_code, file_type='po', filters=None,
-               tags=None, local_file=None):
+               tags=None, order=None, options=None, local_file=None):
         """
         Return terms / translations
 
         filters - filter by self._filter_by
         tags - filter results by tags;
+        order - Set it to 'terms' to order results by 'terms' alphabetically.
+        options - Set specific advanced options for particular formats (where these exist).
+            The value must be a JSON array of objects. Can be used to export in Android XML
+            format without wrapping the strings in quotes: options=[{"unquoted": 1}]
         local_file - save content into it. If None, save content into
-            random temp file.
+            random temp file. If False, don't download at all.
 
         >>> tags = 'name-of-tag'
         >>> tags = ["name-of-tag"]
         >>> tags = ["name-of-tag", "name-of-another-tag"]
 
         >>> filters = 'translated'
         >>> filters = ["translated"]
@@ -529,30 +501,43 @@
 
         data = self._run(
             url_path="projects/export",
             id=project_id,
             language=language_code,
             type=file_type,
             filters=filters,
-            tags=tags
+            tags=tags,
+            order=order,
+            options=options
         )
         # The link of the file (expires after 10 minutes).
         file_url = data['result']['url']
 
-        # Download file content:
-        res = requests.get(file_url, stream=True)
-        if not local_file:
-            tmp_file = tempfile.NamedTemporaryFile(
-                delete=False, suffix='.{}'.format(file_type))
-            tmp_file.close()
-            local_file = tmp_file.name
-
-        with open(local_file, 'w+b') as po_file:
-            for data in res.iter_content(chunk_size=1024):
-                po_file.write(data)
+        if local_file is not False:
+           
+            # Setup a file context manager
+            if local_file is None:
+                context_manager = tempfile.NamedTemporaryFile(delete=False, suffix='.{}'.format(file_type))
+                local_file = context_manager.name
+            elif callable(getattr(local_file, 'write', None)):  # Does it quack?
+                # If the caller of this export method passed a local_file writable object,
+                # it is their responsibility to eventually close it.
+                context_manager = nullcontext(local_file)
+            elif isinstance(local_file, str):
+                context_manager = open(local_file, 'w+b')
+            else:
+                raise ValueError(f"Unexpected value for local_file={local_file}")
+
+            # Download the file
+            res = requests.get(file_url, stream=True)
+
+            with context_manager as f:
+                for data in res.iter_content(chunk_size=1024):
+                    f.write(data)
+
         return file_url, local_file
 
     def _upload(self, project_id, updating, file_path, language_code=None,
                 overwrite=False, sync_terms=False, tags=None, fuzzy_trigger=None):
         """
         Internal: updates terms / translations
```

### Comparing `poeditor-1.1.2/poeditor/tests/test_client.py` & `poeditor-1.1.3/poeditor/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `poeditor-1.1.2/poeditor/dummy.py` & `poeditor-1.1.3/poeditor/dummy.py`

 * *Files identical despite different names*

### Comparing `poeditor-1.1.2/README.rst` & `poeditor-1.1.3/README.rst`

 * *Files identical despite different names*

