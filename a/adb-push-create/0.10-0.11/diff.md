# Comparing `tmp/adb_push_create-0.10.tar.gz` & `tmp/adb_push_create-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb_push_create-0.10.tar", last modified: Sun May 28 23:57:07 2023, max compression
+gzip compressed data, was "adb_push_create-0.11.tar", last modified: Sun Jul 16 19:33:08 2023, max compression
```

## Comparing `adb_push_create-0.10.tar` & `adb_push_create-0.11.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 23:57:07.416622 adb_push_create-0.10/
--rw-rw-rw-   0        0        0     1148 2023-05-28 23:57:02.000000 adb_push_create-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      116 2023-05-28 23:57:02.000000 adb_push_create-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     1439 2023-05-28 23:57:07.416622 adb_push_create-0.10/PKG-INFO
--rw-rw-rw-   0        0        0      817 2023-05-28 23:56:47.000000 adb_push_create-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 23:57:07.412634 adb_push_create-0.10/adb_push_create/
--rw-rw-rw-   0        0        0      817 2023-05-28 23:56:47.000000 adb_push_create-0.10/adb_push_create/README.MD
--rw-rw-rw-   0        0        0     3967 2023-05-28 23:54:42.000000 adb_push_create-0.10/adb_push_create/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-28 23:57:06.000000 adb_push_create-0.10/adb_push_create/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-05-28 23:57:06.000000 adb_push_create-0.10/adb_push_create/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-28 23:57:07.415626 adb_push_create-0.10/adb_push_create.egg-info/
--rw-rw-rw-   0        0        0     1439 2023-05-28 23:57:07.000000 adb_push_create-0.10/adb_push_create.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      327 2023-05-28 23:57:07.000000 adb_push_create-0.10/adb_push_create.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 23:57:07.000000 adb_push_create-0.10/adb_push_create.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 23:57:07.000000 adb_push_create-0.10/adb_push_create.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-28 23:57:07.417620 adb_push_create-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1255 2023-05-28 23:57:06.000000 adb_push_create-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 19:33:08.123542 adb_push_create-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-07-16 19:33:02.000000 adb_push_create-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      116 2023-07-16 19:33:01.000000 adb_push_create-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     1439 2023-07-16 19:33:08.123542 adb_push_create-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0      817 2023-05-28 23:59:28.000000 adb_push_create-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 19:33:08.118661 adb_push_create-0.11/adb_push_create/
+-rw-rw-rw-   0        0        0      817 2023-05-28 23:59:28.000000 adb_push_create-0.11/adb_push_create/README.MD
+-rw-rw-rw-   0        0        0     3895 2023-07-16 19:30:17.000000 adb_push_create-0.11/adb_push_create/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 19:33:07.000000 adb_push_create-0.11/adb_push_create/requirements.txt
+-rw-rw-rw-   0        0        0        2 2023-07-16 19:33:07.000000 adb_push_create-0.11/adb_push_create/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-07-16 19:33:08.122566 adb_push_create-0.11/adb_push_create.egg-info/
+-rw-rw-rw-   0        0        0     1439 2023-07-16 19:33:07.000000 adb_push_create-0.11/adb_push_create.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      327 2023-07-16 19:33:08.000000 adb_push_create-0.11/adb_push_create.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 19:33:07.000000 adb_push_create-0.11/adb_push_create.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-16 19:33:07.000000 adb_push_create-0.11/adb_push_create.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-07-16 19:33:08.123542 adb_push_create-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1255 2023-07-16 19:33:07.000000 adb_push_create-0.11/setup.py
```

### Comparing `adb_push_create-0.10/LICENSE.rst` & `adb_push_create-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `adb_push_create-0.10/PKG-INFO` & `adb_push_create-0.11/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb_push_create
-Version: 0.10
+Version: 0.11
 Summary: creates [nested] folders and pushes files with ADB
 Home-page: https://github.com/hansalemaos/adb_push_create
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adb_push_create-0.10/README.md` & `adb_push_create-0.11/README.md`

 * *Files identical despite different names*

### Comparing `adb_push_create-0.10/adb_push_create/README.MD` & `adb_push_create-0.11/adb_push_create/README.MD`

 * *Files identical despite different names*

### Comparing `adb_push_create-0.10/adb_push_create/__init__.py` & `adb_push_create-0.11/adb_push_create/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,20 +40,18 @@
         proc = subprocess.run(
             f'"{adb_path_}" -s {deviceserial} shell mkdir "{path}"',
             capture_output=True,
             **invisibledict,
             shell=False,
         )
         print(f"Creating: {path}", end="\r")
-        if proc.stderr:
-            print(proc.stderr)
-            break
-    else:
-        return True
-    return False
+        # if proc.stderr:
+        #     print(proc.stderr)
+        #     break
+
 
 
 def push_file(adb_path: str, deviceserial: str, file: str, dest: str):
     r"""
     Copies a file from the local machine to an Android device using the Android Debug Bridge (ADB) tool.
 
     Args:
@@ -70,16 +68,15 @@
     # It calls the make_folders function to create the necessary folders on the Android device for the destination path. If the folder creation fails, the function returns False.
     # If the folder creation is successful, it executes the ADB command adb_path -s deviceserial push "file" "dest" using subprocess.run to copy the file to the Android device.
     # If any error occurs during the execution of the ADB command, it prints the error message and returns False.
     # If the file copy is successful, the function returns True.
     adb_path_ = adb_path.strip("\" '")
     file = file.strip("\" '")
     dest = dest.strip("\" '")
-    if not make_folders(adb_path, deviceserial, dest):
-        return False
+    make_folders(adb_path, deviceserial, dest)
     proc = subprocess.run(
         f'"{adb_path_}" -s {deviceserial} push "{file}" "{dest}"',
         capture_output=True,
         **invisibledict,
         shell=False,
     )
     print(f"Copying: {file}", end="\r")
```

### Comparing `adb_push_create-0.10/adb_push_create.egg-info/PKG-INFO` & `adb_push_create-0.11/adb_push_create.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-push-create
-Version: 0.10
+Version: 0.11
 Summary: creates [nested] folders and pushes files with ADB
 Home-page: https://github.com/hansalemaos/adb_push_create
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adb_push_create-0.10/setup.py` & `adb_push_create-0.11/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''creates [nested] folders and pushes files with ADB'''
 
 # Setting up
 setup(
     name="adb_push_create",
     version=VERSION,
     license='MIT',
```

