# Comparing `tmp/talkytimes_package-0.1.1.tar.gz` & `tmp/talkytimes_package-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.1.1.tar", last modified: Sun Jul 16 06:41:32 2023, max compression
+gzip compressed data, was "talkytimes_package-0.1.2.tar", last modified: Sun Jul 16 06:43:38 2023, max compression
```

## Comparing `talkytimes_package-0.1.1.tar` & `talkytimes_package-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 06:41:32.444594 talkytimes_package-0.1.1/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 06:41:32.444594 talkytimes_package-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.1/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 06:41:32.445594 talkytimes_package-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      461 2023-07-16 06:40:36.000000 talkytimes_package-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:41:32.421596 talkytimes_package-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 06:41:32.429599 talkytimes_package-0.1.1/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.1/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.1/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     1385 2023-07-16 06:22:57.000000 talkytimes_package-0.1.1/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:41:32.432597 talkytimes_package-0.1.1/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 06:41:27.000000 talkytimes_package-0.1.1/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.1/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     2375 2023-07-16 06:26:53.000000 talkytimes_package-0.1.1/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 06:41:32.443596 talkytimes_package-0.1.1/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 06:41:32.000000 talkytimes_package-0.1.1/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 06:41:32.000000 talkytimes_package-0.1.1/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 06:41:32.000000 talkytimes_package-0.1.1/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-07-16 06:41:32.000000 talkytimes_package-0.1.1/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 06:41:32.000000 talkytimes_package-0.1.1/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 06:43:38.657534 talkytimes_package-0.1.2/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 06:43:38.657534 talkytimes_package-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.2/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 06:43:38.659530 talkytimes_package-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:43:38.630529 talkytimes_package-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 06:43:38.637529 talkytimes_package-0.1.2/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.2/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.2/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     1385 2023-07-16 06:22:57.000000 talkytimes_package-0.1.2/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:43:38.640529 talkytimes_package-0.1.2/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 06:43:35.000000 talkytimes_package-0.1.2/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.2/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     2375 2023-07-16 06:26:53.000000 talkytimes_package-0.1.2/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:43:38.656531 talkytimes_package-0.1.2/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 06:43:38.000000 talkytimes_package-0.1.2/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 06:43:38.000000 talkytimes_package-0.1.2/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:43:38.000000 talkytimes_package-0.1.2/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 06:43:38.000000 talkytimes_package-0.1.2/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 06:43:38.000000 talkytimes_package-0.1.2/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.1.1/LICENSE` & `talkytimes_package-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.1/src/dynamodb/dynamodb.py` & `talkytimes_package-0.1.2/src/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.1/src/talkytimes/base.py` & `talkytimes_package-0.1.2/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.1/src/talkytimes/talkytimes.py` & `talkytimes_package-0.1.2/src/talkytimes/talkytimes.py`

 * *Files identical despite different names*

