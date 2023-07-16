# Comparing `tmp/Primice-0.0.1.tar.gz` & `tmp/Primice-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Primice-0.0.1.tar", last modified: Sun Jul 16 07:17:33 2023, max compression
+gzip compressed data, was "Primice-0.0.2.tar", last modified: Sun Jul 16 07:53:22 2023, max compression
```

## Comparing `Primice-0.0.1.tar` & `Primice-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:17:33.330508 Primice-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-07-16 06:14:26.000000 Primice-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      426 2023-07-16 07:17:33.330508 Primice-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 07:17:33.321960 Primice-0.0.1/Primice/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:09:15.000000 Primice-0.0.1/Primice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:17:33.328528 Primice-0.0.1/Primice.egg-info/
--rw-rw-rw-   0        0        0      426 2023-07-16 07:17:33.000000 Primice-0.0.1/Primice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      170 2023-07-16 07:17:33.000000 Primice-0.0.1/Primice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:17:33.000000 Primice-0.0.1/Primice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-16 07:17:33.000000 Primice-0.0.1/Primice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       60 2023-07-16 06:14:49.000000 Primice-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 07:17:33.331488 Primice-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      584 2023-07-16 06:20:40.000000 Primice-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:22.542736 Primice-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-07-16 06:14:26.000000 Primice-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      426 2023-07-16 07:53:22.541735 Primice-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:22.508322 Primice-0.0.2/Primice/
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:22.539733 Primice-0.0.2/Primice/Spider/
+-rw-rw-rw-   0        0        0     2711 2023-07-16 04:28:20.000000 Primice-0.0.2/Primice/Spider/Log.py
+-rw-rw-rw-   0        0        0     3760 2023-05-21 09:51:28.000000 Primice-0.0.2/Primice/Spider/Proxy.py
+-rw-rw-rw-   0        0        0      228 2023-06-13 05:56:41.000000 Primice-0.0.2/Primice/Spider/Twitter爬虫.py
+-rw-rw-rw-   0        0        0        0 2023-05-21 10:56:02.000000 Primice-0.0.2/Primice/Spider/__init__.py
+-rw-rw-rw-   0        0        0     6004 2023-06-13 05:57:15.000000 Primice-0.0.2/Primice/Spider/http_raw2requests.py
+-rw-rw-rw-   0        0        0     3325 2023-06-13 07:14:44.000000 Primice-0.0.2/Primice/Spider/to_Mongodb.py
+-rw-rw-rw-   0        0        0     4340 2023-07-13 05:58:09.000000 Primice-0.0.2/Primice/Spider/to_requests.py
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:09:15.000000 Primice-0.0.2/Primice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:53:22.520633 Primice-0.0.2/Primice.egg-info/
+-rw-rw-rw-   0        0        0      426 2023-07-16 07:53:22.000000 Primice-0.0.2/Primice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2023-07-16 07:53:22.000000 Primice-0.0.2/Primice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 07:53:22.000000 Primice-0.0.2/Primice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 07:53:22.000000 Primice-0.0.2/Primice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       60 2023-07-16 06:14:49.000000 Primice-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 07:53:22.543782 Primice-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      584 2023-07-16 07:53:03.000000 Primice-0.0.2/setup.py
```

### Comparing `Primice-0.0.1/LICENSE` & `Primice-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Primice-0.0.1/setup.py` & `Primice-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("./README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="Primice",
-    version="0.0.1",
+    version="0.0.2",
     author="Primice",
     author_email="1121796946@qq.com",
     description="A small example package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

