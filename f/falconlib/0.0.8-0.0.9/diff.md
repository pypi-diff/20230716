# Comparing `tmp/falconlib-0.0.8.tar.gz` & `tmp/falconlib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "falconlib-0.0.8.tar", last modified: Tue Jul  4 15:32:05 2023, max compression
+gzip compressed data, was "falconlib-0.0.9.tar", last modified: Sat Jul 15 22:09:37 2023, max compression
```

## Comparing `falconlib-0.0.8.tar` & `falconlib-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.698062 falconlib-0.0.8/
--rw-rw-rw-   0        0        0     1344 2022-10-29 19:56:38.000000 falconlib-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       36 2022-10-29 19:56:38.000000 falconlib-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     9223 2023-07-04 15:32:05.697062 falconlib-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     6866 2022-10-29 19:56:38.000000 falconlib-0.0.8/README.md
--rw-rw-rw-   0        0        0     1067 2023-07-04 15:24:59.000000 falconlib-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-04 15:32:05.699062 falconlib-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.571890 falconlib-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.616210 falconlib-0.0.8/src/falconlib/
--rw-rw-rw-   0        0        0       42 2022-10-29 19:56:38.000000 falconlib-0.0.8/src/falconlib/conftest.py
--rw-rw-rw-   0        0        0    17166 2023-07-04 15:23:56.000000 falconlib-0.0.8/src/falconlib/falconlib.py
-drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.694065 falconlib-0.0.8/src/falconlib/tests/
--rw-rw-rw-   0        0        0     6644 2022-10-29 19:56:38.000000 falconlib-0.0.8/src/falconlib/tests/gendoc.py
--rw-rw-rw-   0        0        0     7831 2022-10-29 20:18:46.000000 falconlib-0.0.8/src/falconlib/tests/test_010_lib.py
--rw-rw-rw-   0        0        0        0 2022-10-29 19:56:38.000000 falconlib-0.0.8/src/falconlib/x__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-04 15:32:05.660168 falconlib-0.0.8/src/falconlib.egg-info/
--rw-rw-rw-   0        0        0     9223 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-04 15:32:05.000000 falconlib-0.0.8/src/falconlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 22:09:37.550196 falconlib-0.0.9/
+-rw-rw-rw-   0        0        0     1344 2022-10-29 19:56:38.000000 falconlib-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       36 2022-10-29 19:56:38.000000 falconlib-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     9223 2023-07-15 22:09:37.549196 falconlib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6866 2022-10-29 19:56:38.000000 falconlib-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1067 2023-07-15 22:06:44.000000 falconlib-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 22:09:37.551194 falconlib-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 22:09:37.384310 falconlib-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 22:09:37.453273 falconlib-0.0.9/src/falconlib/
+-rw-rw-rw-   0        0        0       42 2022-10-29 19:56:38.000000 falconlib-0.0.9/src/falconlib/conftest.py
+-rw-rw-rw-   0        0        0    17805 2023-07-15 22:06:01.000000 falconlib-0.0.9/src/falconlib/falconlib.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:09:37.546198 falconlib-0.0.9/src/falconlib/tests/
+-rw-rw-rw-   0        0        0     6644 2022-10-29 19:56:38.000000 falconlib-0.0.9/src/falconlib/tests/gendoc.py
+-rw-rw-rw-   0        0        0     7831 2022-10-29 20:18:46.000000 falconlib-0.0.9/src/falconlib/tests/test_010_lib.py
+-rw-rw-rw-   0        0        0        0 2022-10-29 19:56:38.000000 falconlib-0.0.9/src/falconlib/x__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:09:37.502285 falconlib-0.0.9/src/falconlib.egg-info/
+-rw-rw-rw-   0        0        0     9223 2023-07-15 22:09:37.000000 falconlib-0.0.9/src/falconlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2023-07-15 22:09:37.000000 falconlib-0.0.9/src/falconlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 22:09:37.000000 falconlib-0.0.9/src/falconlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-15 22:09:37.000000 falconlib-0.0.9/src/falconlib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 22:09:37.000000 falconlib-0.0.9/src/falconlib.egg-info/top_level.txt
```

### Comparing `falconlib-0.0.8/LICENSE` & `falconlib-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `falconlib-0.0.8/PKG-INFO` & `falconlib-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falconlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Client-side library for accessing the falconapi restful service.
 Author-email: "Thomas J. Daley, Esq." <tjd@powerdaley.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, Tom Daley
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: falconlib Version: 0.0.8 Summary: Client-side
+Metadata-Version: 2.1 Name: falconlib Version: 0.0.9 Summary: Client-side
 library for accessing the falconapi restful service. Author-email: "Thomas J.
 Daley, Esq."
 powerdaley.com> License: BSD 2-Clause License Copyright (c) 2022, Tom Daley All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
```

### Comparing `falconlib-0.0.8/README.md` & `falconlib-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `falconlib-0.0.8/pyproject.toml` & `falconlib-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "falconlib"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
     {name="Thomas J. Daley, Esq.", email="tjd@powerdaley.com"},
 ]
 description = "Client-side library for accessing the falconapi restful service."
 readme = "README.md"
 license = {file="LICENSE"}
 requires-python = ">3.9"
```

### Comparing `falconlib-0.0.8/src/falconlib/falconlib.py` & `falconlib-0.0.9/src/falconlib/falconlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -229,14 +229,30 @@
             (dict): Response from server. You can inquire the last_response for more information.
         """
         r = self.__get('/documents/props/?doc_id=' + document_id)
         self.last_response = r
         if r.status_code == 200:
             return _success(r.status_code, 'Extended document properties retrieved', r.json())
         return _error(r.status_code, 'Extended document properties retrieval failed', r.json())
+
+    def get_csv_tables(self, document_id: str) -> FalconStatus:
+        """
+        GetCsvTables - Get CSV tables from a document
+
+        Args:
+            document_id (str): Document to get CSV tables from
+
+        Returns:
+            (dict): Response from server. You can inquire the last_response for more information.
+        """
+        r = self.__get('/documents/tables/?doc_id=' + document_id)
+        self.last_response = r
+        if r.status_code == 200:
+            return _success(r.status_code, 'CSV tables retrieved', r.json())
+        return _error(r.status_code, 'CSV tables retrieval failed', r.json())
     
     def get_tracker_categories(self, tracker_id: str) -> FalconStatus:
         """
         GetTrackerCategories - Get categories for a tracker
 
         Args:
             tracker_id (str): Tracker to get categories for
```

### Comparing `falconlib-0.0.8/src/falconlib/tests/gendoc.py` & `falconlib-0.0.9/src/falconlib/tests/gendoc.py`

 * *Files identical despite different names*

### Comparing `falconlib-0.0.8/src/falconlib/tests/test_010_lib.py` & `falconlib-0.0.9/src/falconlib/tests/test_010_lib.py`

 * *Files identical despite different names*

### Comparing `falconlib-0.0.8/src/falconlib.egg-info/PKG-INFO` & `falconlib-0.0.9/src/falconlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: falconlib
-Version: 0.0.8
+Version: 0.0.9
 Summary: Client-side library for accessing the falconapi restful service.
 Author-email: "Thomas J. Daley, Esq." <tjd@powerdaley.com>
 License: BSD 2-Clause License
         
         Copyright (c) 2022, Tom Daley
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: falconlib Version: 0.0.8 Summary: Client-side
+Metadata-Version: 2.1 Name: falconlib Version: 0.0.9 Summary: Client-side
 library for accessing the falconapi restful service. Author-email: "Thomas J.
 Daley, Esq."
 powerdaley.com> License: BSD 2-Clause License Copyright (c) 2022, Tom Daley All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
```

