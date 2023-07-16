# Comparing `tmp/potee-0.4.tar.gz` & `tmp/potee-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potee-0.4.tar", last modified: Tue Dec  6 15:51:10 2022, max compression
+gzip compressed data, was "potee-0.5.0.tar", last modified: Sun Jul 16 14:08:53 2023, max compression
```

## Comparing `potee-0.4.tar` & `potee-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,15 @@
-drwxrwxr-x   0 ivanh     (1000) ivanh     (1000)        0 2022-12-06 15:51:10.654153 potee-0.4/
--rw-rw-r--   0 ivanh     (1000) ivanh     (1000)      717 2022-12-06 15:51:10.654153 potee-0.4/PKG-INFO
-drwxrwxr-x   0 ivanh     (1000) ivanh     (1000)        0 2022-12-06 15:51:10.654153 potee-0.4/potee/
--rw-rw-r--   0 ivanh     (1000) ivanh     (1000)       65 2022-12-06 14:31:42.146130 potee-0.4/potee/__init__.py
--rw-rw-r--   0 ivanh     (1000) ivanh     (1000)     1394 2022-12-06 15:43:02.666414 potee-0.4/potee/main.py
--rw-rw-r--   0 ivanh     (1000) ivanh     (1000)     1993 2022-12-06 15:39:38.126922 potee-0.4/potee/testing.py
--rw-rw-r--   0 ivanh     (1000) ivanh     (1000)       40 2022-08-03 11:00:59.618544 potee-0.4/setup.cfg
--rw-rw-r--   0 ivanh     (1000) ivanh     (1000)     1031 2022-12-06 15:44:25.606293 potee-0.4/setup.py
+drwxrwxr-x   0 ivanh     (1000) ivanh     (1000)        0 2023-07-16 14:08:53.482215 potee-0.5.0/
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)     1064 2022-08-03 11:02:32.000000 potee-0.5.0/LICENSE.md
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)      811 2023-07-16 14:08:53.482215 potee-0.5.0/PKG-INFO
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)       10 2022-08-03 11:09:30.000000 potee-0.5.0/README.md
+drwxrwxr-x   0 ivanh     (1000) ivanh     (1000)        0 2023-07-16 14:08:53.478215 potee-0.5.0/potee/
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)       61 2023-06-07 18:05:43.000000 potee-0.5.0/potee/__init__.py
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)     2921 2023-07-16 13:48:19.000000 potee-0.5.0/potee/main.py
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)     1993 2022-12-06 15:39:38.000000 potee-0.5.0/potee/testing.py
+drwxrwxr-x   0 ivanh     (1000) ivanh     (1000)        0 2023-07-16 14:08:53.482215 potee-0.5.0/potee.egg-info/
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)      811 2023-07-16 14:08:53.000000 potee-0.5.0/potee.egg-info/PKG-INFO
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)      210 2023-07-16 14:08:53.000000 potee-0.5.0/potee.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)        1 2023-07-16 14:08:53.000000 potee-0.5.0/potee.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)        6 2023-07-16 14:08:53.000000 potee-0.5.0/potee.egg-info/top_level.txt
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)      964 2023-07-16 14:06:48.000000 potee-0.5.0/pyproject.toml
+-rw-rw-r--   0 ivanh     (1000) ivanh     (1000)       79 2023-07-16 14:08:53.486215 potee-0.5.0/setup.cfg
```

### Comparing `potee-0.4/PKG-INFO` & `potee-0.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: potee
-Version: 0.4
-Summary: A package to simplify the process of writing checkers for the Poteet platform
-Home-page: https://github.com/PoteeDev/
-Author: Ivan Hahanov
-Author-email: ivanhahanov13@gmail.com
-License: MIT
-Description: UNKNOWN
-Keywords: checkers,security,paltform
-Platform: UNKNOWN
+Version: 0.5.0
+Summary: A package to simplify the process of writing checkers for the Potee platform
+Author-email: Ivan Hahanov <ivanhahanov13@gmail.com>
+Project-URL: Homepage, https://github.com/PoteeDev/library
+Project-URL: Bug Tracker, https://github.com/PoteeDev/library/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# library
```

### Comparing `potee-0.4/potee/testing.py` & `potee-0.5.0/potee/testing.py`

 * *Files identical despite different names*

