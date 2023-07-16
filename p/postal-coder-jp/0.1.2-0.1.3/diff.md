# Comparing `tmp/postal_coder_jp-0.1.2.tar.gz` & `tmp/postal_coder_jp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\postal_coder_jp-0.1.2.tar", last modified: Sun Jul 16 12:36:26 2023, max compression
+gzip compressed data, was "dist\postal_coder_jp-0.1.3.tar", last modified: Sun Jul 16 12:46:52 2023, max compression
```

## Comparing `postal_coder_jp-0.1.2.tar` & `postal_coder_jp-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 12:36:26.491726 postal_coder_jp-0.1.2/
--rw-rw-rw-   0        0        0     1063 2023-06-18 11:53:00.000000 postal_coder_jp-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      537 2023-07-16 12:36:26.488731 postal_coder_jp-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      254 2023-07-16 11:37:22.000000 postal_coder_jp-0.1.2/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-16 12:36:26.477027 postal_coder_jp-0.1.2/postal_coder_jp/
--rw-rw-rw-   0        0        0       24 2023-07-16 11:14:57.000000 postal_coder_jp-0.1.2/postal_coder_jp/__init__.py
--rw-rw-rw-   0        0        0      335 2023-07-16 12:35:56.000000 postal_coder_jp-0.1.2/postal_coder_jp/postal_coder.py
-drwxrwxrwx   0        0        0        0 2023-07-16 12:36:26.487360 postal_coder_jp-0.1.2/postal_coder_jp.egg-info/
--rw-rw-rw-   0        0        0      537 2023-07-16 12:36:25.000000 postal_coder_jp-0.1.2/postal_coder_jp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2023-07-16 12:36:25.000000 postal_coder_jp-0.1.2/postal_coder_jp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 12:36:25.000000 postal_coder_jp-0.1.2/postal_coder_jp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-16 12:36:25.000000 postal_coder_jp-0.1.2/postal_coder_jp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 12:36:26.492687 postal_coder_jp-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      540 2023-07-16 12:36:09.000000 postal_coder_jp-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:46:52.742443 postal_coder_jp-0.1.3/
+-rw-rw-rw-   0        0        0     1063 2023-06-18 11:53:00.000000 postal_coder_jp-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      537 2023-07-16 12:46:52.741414 postal_coder_jp-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      254 2023-07-16 11:37:22.000000 postal_coder_jp-0.1.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 12:46:52.731629 postal_coder_jp-0.1.3/postal_coder_jp/
+-rw-rw-rw-   0        0        0       24 2023-07-16 11:14:57.000000 postal_coder_jp-0.1.3/postal_coder_jp/__init__.py
+-rw-rw-rw-   0        0        0      335 2023-07-16 12:46:05.000000 postal_coder_jp-0.1.3/postal_coder_jp/postal_coder.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:46:52.739243 postal_coder_jp-0.1.3/postal_coder_jp.egg-info/
+-rw-rw-rw-   0        0        0      537 2023-07-16 12:46:52.000000 postal_coder_jp-0.1.3/postal_coder_jp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-07-16 12:46:52.000000 postal_coder_jp-0.1.3/postal_coder_jp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 12:46:52.000000 postal_coder_jp-0.1.3/postal_coder_jp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-16 12:46:52.000000 postal_coder_jp-0.1.3/postal_coder_jp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 12:46:52.742443 postal_coder_jp-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      540 2023-07-16 12:46:39.000000 postal_coder_jp-0.1.3/setup.py
```

### Comparing `postal_coder_jp-0.1.2/LICENSE` & `postal_coder_jp-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postal_coder_jp-0.1.2/PKG-INFO` & `postal_coder_jp-0.1.3/postal_coder_jp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: postal_coder_jp
-Version: 0.1.2
+Name: postal-coder-jp
+Version: 0.1.3
 Summary: postal_coder_jp is a Python module for geocoding Japanese postal codes.
 Home-page: https://pickerlab.net
 Author: picker.
 Author-email: hikaru.tokuhara@chionanthus.jp
 License: MIT
 License-File: LICENSE
```

### Comparing `postal_coder_jp-0.1.2/postal_coder_jp.egg-info/PKG-INFO` & `postal_coder_jp-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: postal-coder-jp
-Version: 0.1.2
+Name: postal_coder_jp
+Version: 0.1.3
 Summary: postal_coder_jp is a Python module for geocoding Japanese postal codes.
 Home-page: https://pickerlab.net
 Author: picker.
 Author-email: hikaru.tokuhara@chionanthus.jp
 License: MIT
 License-File: LICENSE
```

### Comparing `postal_coder_jp-0.1.2/setup.py` & `postal_coder_jp-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.rst", encoding="utf-8") as f:
     readme = f.read()
 
 
 setup(
     name='postal_coder_jp',
-    version='0.1.2',
+    version='0.1.3',
     url='https://pickerlab.net',
     long_description=readme,
     author='picker.',
     author_email='hikaru.tokuhara@chionanthus.jp',
     description='postal_coder_jp is a Python module for geocoding Japanese postal codes.',
     license="MIT",
     install_requires=[],
```

