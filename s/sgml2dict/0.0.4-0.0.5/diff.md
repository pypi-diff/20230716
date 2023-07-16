# Comparing `tmp/sgml2dict-0.0.4.tar.gz` & `tmp/sgml2dict-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sgml2dict-0.0.4.tar", last modified: Sun Jul 16 06:12:39 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `sgml2dict-0.0.4.tar` & `sgml2dict-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,11 @@
-drwxr-xr-x   0 dhbmarcos  (1000) dhbmarcos  (1001)        0 2023-07-16 06:12:39.785990 sgml2dict-0.0.4/
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)     1094 2023-07-16 04:52:54.000000 sgml2dict-0.0.4/LICENSE
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)     1094 2023-07-16 05:43:07.000000 sgml2dict-0.0.4/LICENSE.txt
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)      680 2023-07-16 06:12:39.785990 sgml2dict-0.0.4/PKG-INFO
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)      709 2023-07-16 05:42:50.000000 sgml2dict-0.0.4/README.md
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)       79 2023-07-16 06:12:39.789990 sgml2dict-0.0.4/setup.cfg
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)      847 2023-07-16 06:11:59.000000 sgml2dict-0.0.4/setup.py
-drwxr-xr-x   0 dhbmarcos  (1000) dhbmarcos  (1001)        0 2023-07-16 06:12:39.785990 sgml2dict-0.0.4/sgml2dict/
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)       40 2023-07-16 04:52:54.000000 sgml2dict-0.0.4/sgml2dict/__init__.py
--rwxr-xr-x   0 dhbmarcos  (1000) dhbmarcos  (1001)     4401 2023-07-16 05:33:24.000000 sgml2dict-0.0.4/sgml2dict/sgml2dict.py
-drwxr-xr-x   0 dhbmarcos  (1000) dhbmarcos  (1001)        0 2023-07-16 06:12:39.785990 sgml2dict-0.0.4/sgml2dict.egg-info/
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)      680 2023-07-16 06:12:39.000000 sgml2dict-0.0.4/sgml2dict.egg-info/PKG-INFO
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)      225 2023-07-16 06:12:39.000000 sgml2dict-0.0.4/sgml2dict.egg-info/SOURCES.txt
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)        1 2023-07-16 06:12:39.000000 sgml2dict-0.0.4/sgml2dict.egg-info/dependency_links.txt
--rw-r--r--   0 dhbmarcos  (1000) dhbmarcos  (1001)       10 2023-07-16 06:12:39.000000 sgml2dict-0.0.4/sgml2dict.egg-info/top_level.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/CHANGELOG
+-rwxr-xr-x   0        0        0      741 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/deploy.sh
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/examples/example.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/src/sgml2dict/__init__.py
+-rwxr-xr-x   0        0        0     4401 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/src/sgml2dict/sgml2dict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/tests/.gitkeep
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/LICENSE
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/README.md
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 sgml2dict-0.0.5/PKG-INFO
```

### Comparing `sgml2dict-0.0.4/LICENSE` & `sgml2dict-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sgml2dict-0.0.4/README.md` & `sgml2dict-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sgml2dict-0.0.4/sgml2dict/sgml2dict.py` & `sgml2dict-0.0.5/src/sgml2dict/sgml2dict.py`

 * *Files identical despite different names*

