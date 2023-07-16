# Comparing `tmp/clashbyte-0.0.4.tar.gz` & `tmp/clashbyte-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clashbyte-0.0.4.tar", last modified: Sun Jul 16 01:52:47 2023, max compression
+gzip compressed data, was "clashbyte-0.0.5.tar", last modified: Sun Jul 16 01:54:41 2023, max compression
```

## Comparing `clashbyte-0.0.4.tar` & `clashbyte-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:52:47.913893 clashbyte-0.0.4/
--rw-rw-rw-   0        0        0     1085 2023-07-15 15:59:16.000000 clashbyte-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1182 2023-07-16 01:52:47.912894 clashbyte-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-07-16 01:48:27.000000 clashbyte-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 01:52:47.899894 clashbyte-0.0.4/clashbyte/
--rw-rw-rw-   0        0        0      287 2023-07-16 01:52:45.000000 clashbyte-0.0.4/clashbyte/__init__.py
--rw-rw-rw-   0        0        0     4972 2023-07-16 01:46:14.000000 clashbyte-0.0.4/clashbyte/apis.py
--rw-rw-rw-   0        0        0     2137 2023-07-15 20:34:49.000000 clashbyte-0.0.4/clashbyte/toolbox.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:52:47.909895 clashbyte-0.0.4/clashbyte.egg-info/
--rw-rw-rw-   0        0        0     1182 2023-07-16 01:52:47.000000 clashbyte-0.0.4/clashbyte.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-07-16 01:52:47.000000 clashbyte-0.0.4/clashbyte.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:52:47.000000 clashbyte-0.0.4/clashbyte.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-16 01:52:47.000000 clashbyte-0.0.4/clashbyte.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:52:47.000000 clashbyte-0.0.4/clashbyte.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 01:52:47.913893 clashbyte-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1270 2023-07-16 01:52:36.000000 clashbyte-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:52:47.910894 clashbyte-0.0.4/tests/
--rw-rw-rw-   0        0        0     2158 2023-07-16 01:44:22.000000 clashbyte-0.0.4/tests/test_clash_meta_apis.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:54:41.495542 clashbyte-0.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-07-15 15:59:16.000000 clashbyte-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1182 2023-07-16 01:54:41.493502 clashbyte-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-07-16 01:48:27.000000 clashbyte-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 01:54:41.483503 clashbyte-0.0.5/clashbyte/
+-rw-rw-rw-   0        0        0      287 2023-07-16 01:54:15.000000 clashbyte-0.0.5/clashbyte/__init__.py
+-rw-rw-rw-   0        0        0     4972 2023-07-16 01:46:14.000000 clashbyte-0.0.5/clashbyte/apis.py
+-rw-rw-rw-   0        0        0     2137 2023-07-15 20:34:49.000000 clashbyte-0.0.5/clashbyte/toolbox.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:54:41.491503 clashbyte-0.0.5/clashbyte.egg-info/
+-rw-rw-rw-   0        0        0     1182 2023-07-16 01:54:41.000000 clashbyte-0.0.5/clashbyte.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-16 01:54:41.000000 clashbyte-0.0.5/clashbyte.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 01:54:41.000000 clashbyte-0.0.5/clashbyte.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-16 01:54:41.000000 clashbyte-0.0.5/clashbyte.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 01:54:41.000000 clashbyte-0.0.5/clashbyte.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 01:54:41.495542 clashbyte-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1283 2023-07-16 01:53:52.000000 clashbyte-0.0.5/setup.py
```

### Comparing `clashbyte-0.0.4/LICENSE` & `clashbyte-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `clashbyte-0.0.4/PKG-INFO` & `clashbyte-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clashbyte
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/QIN2DIM/ClashByte
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 License: MIT
 Keywords: clashbyte,clash,clash-meta,clashapi
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `clashbyte-0.0.4/clashbyte/apis.py` & `clashbyte-0.0.5/clashbyte/apis.py`

 * *Files identical despite different names*

### Comparing `clashbyte-0.0.4/clashbyte/toolbox.py` & `clashbyte-0.0.5/clashbyte/toolbox.py`

 * *Files identical despite different names*

### Comparing `clashbyte-0.0.4/clashbyte.egg-info/PKG-INFO` & `clashbyte-0.0.5/clashbyte.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clashbyte
-Version: 0.0.4
+Version: 0.0.5
 Home-page: https://github.com/QIN2DIM/ClashByte
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 License: MIT
 Keywords: clashbyte,clash,clash-meta,clashapi
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `clashbyte-0.0.4/setup.py` & `clashbyte-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     keywords=["clashbyte", "clash", "clash-meta", "clashapi"],
     author="QIN2DIM",
     author_email="yaoqinse@gmail.com",
     long_description=Path(__file__).parent.joinpath("README.md").read_text(encoding="utf8"),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/QIN2DIM/ClashByte",
-    packages=find_packages(include=["clashbyte.*", "LICENSE"], exclude=["tests"]),
+    packages=find_packages(include=["clashbyte", "clashbyte.*", "LICENSE"], exclude=["tests"]),
     install_requires=["loguru>=0.7.0", "httpx>=0.24.1"],
     extras_require={"dev": ["nox", "pytest"], "test": ["pytest", "black"]},
     python_requires=">=3.8",
     classifiers=[
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
```

