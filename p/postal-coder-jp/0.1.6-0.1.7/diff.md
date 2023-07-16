# Comparing `tmp/postal_coder_jp-0.1.6.tar.gz` & `tmp/postal_coder_jp-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\postal_coder_jp-0.1.6.tar", last modified: Sun Jul 16 13:30:46 2023, max compression
+gzip compressed data, was "dist\postal_coder_jp-0.1.7.tar", last modified: Sun Jul 16 13:33:09 2023, max compression
```

## Comparing `postal_coder_jp-0.1.6.tar` & `postal_coder_jp-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 13:30:46.068703 postal_coder_jp-0.1.6/
--rw-rw-rw-   0        0        0     1063 2023-06-18 11:53:00.000000 postal_coder_jp-0.1.6/LICENSE
--rw-rw-rw-   0        0        0      537 2023-07-16 13:30:46.066621 postal_coder_jp-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-07-16 13:30:07.000000 postal_coder_jp-0.1.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-16 13:30:46.056074 postal_coder_jp-0.1.6/postal_coder_jp/
--rw-rw-rw-   0        0        0        0 2023-07-16 13:03:46.000000 postal_coder_jp-0.1.6/postal_coder_jp/__init__.py
--rw-rw-rw-   0        0        0      335 2023-07-16 13:07:04.000000 postal_coder_jp-0.1.6/postal_coder_jp/postal_coder.py
-drwxrwxrwx   0        0        0        0 2023-07-16 13:30:46.064813 postal_coder_jp-0.1.6/postal_coder_jp.egg-info/
--rw-rw-rw-   0        0        0      537 2023-07-16 13:30:45.000000 postal_coder_jp-0.1.6/postal_coder_jp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-16 13:30:45.000000 postal_coder_jp-0.1.6/postal_coder_jp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 13:30:45.000000 postal_coder_jp-0.1.6/postal_coder_jp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-16 13:30:45.000000 postal_coder_jp-0.1.6/postal_coder_jp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 13:30:46.068703 postal_coder_jp-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      540 2023-07-16 13:30:30.000000 postal_coder_jp-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 13:33:09.113551 postal_coder_jp-0.1.7/
+-rw-rw-rw-   0        0        0     1063 2023-06-18 11:53:00.000000 postal_coder_jp-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0      537 2023-07-16 13:33:09.110794 postal_coder_jp-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2023-07-16 13:30:07.000000 postal_coder_jp-0.1.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 13:33:09.096392 postal_coder_jp-0.1.7/postal_coder_jp/
+-rw-rw-rw-   0        0        0       24 2023-07-16 13:32:31.000000 postal_coder_jp-0.1.7/postal_coder_jp/__init__.py
+-rw-rw-rw-   0        0        0      335 2023-07-16 13:07:04.000000 postal_coder_jp-0.1.7/postal_coder_jp/postal_coder.py
+drwxrwxrwx   0        0        0        0 2023-07-16 13:33:09.106435 postal_coder_jp-0.1.7/postal_coder_jp.egg-info/
+-rw-rw-rw-   0        0        0      537 2023-07-16 13:33:08.000000 postal_coder_jp-0.1.7/postal_coder_jp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-16 13:33:08.000000 postal_coder_jp-0.1.7/postal_coder_jp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 13:33:08.000000 postal_coder_jp-0.1.7/postal_coder_jp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-16 13:33:08.000000 postal_coder_jp-0.1.7/postal_coder_jp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 13:33:09.113551 postal_coder_jp-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      540 2023-07-16 13:32:59.000000 postal_coder_jp-0.1.7/setup.py
```

### Comparing `postal_coder_jp-0.1.6/LICENSE` & `postal_coder_jp-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `postal_coder_jp-0.1.6/PKG-INFO` & `postal_coder_jp-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postal_coder_jp
-Version: 0.1.6
+Version: 0.1.7
 Summary: postal_coder_jp is a Python module for geocoding Japanese postal codes.
 Home-page: https://pickerlab.net
 Author: picker.
 Author-email: hikaru.tokuhara@chionanthus.jp
 License: MIT
 License-File: LICENSE
```

### Comparing `postal_coder_jp-0.1.6/postal_coder_jp.egg-info/PKG-INFO` & `postal_coder_jp-0.1.7/postal_coder_jp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postal-coder-jp
-Version: 0.1.6
+Version: 0.1.7
 Summary: postal_coder_jp is a Python module for geocoding Japanese postal codes.
 Home-page: https://pickerlab.net
 Author: picker.
 Author-email: hikaru.tokuhara@chionanthus.jp
 License: MIT
 License-File: LICENSE
```

### Comparing `postal_coder_jp-0.1.6/setup.py` & `postal_coder_jp-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.rst", encoding="utf-8") as f:
     readme = f.read()
 
 
 setup(
     name='postal_coder_jp',
-    version='0.1.6',
+    version='0.1.7',
     url='https://pickerlab.net',
     long_description=readme,
     author='picker.',
     author_email='hikaru.tokuhara@chionanthus.jp',
     description='postal_coder_jp is a Python module for geocoding Japanese postal codes.',
     license="MIT",
     install_requires=[],
```

