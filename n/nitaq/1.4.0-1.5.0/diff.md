# Comparing `tmp/nitaq-1.4.0.tar.gz` & `tmp/nitaq-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitaq-1.4.0.tar", last modified: Sun Jul 16 11:00:21 2023, max compression
+gzip compressed data, was "nitaq-1.5.0.tar", last modified: Sun Jul 16 11:42:37 2023, max compression
```

## Comparing `nitaq-1.4.0.tar` & `nitaq-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 11:00:21.416874 nitaq-1.4.0/
--rw-rw-rw-   0        0        0      199 2023-07-16 11:00:21.415874 nitaq-1.4.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-07-16 10:13:32.000000 nitaq-1.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 11:00:21.388873 nitaq-1.4.0/nitaq/
--rw-rw-rw-   0        0        0       25 2023-07-16 10:37:29.000000 nitaq-1.4.0/nitaq/__init__.py
--rw-rw-rw-   0        0        0     3130 2023-07-16 11:00:06.000000 nitaq-1.4.0/nitaq/nitaq.py
-drwxrwxrwx   0        0        0        0 2023-07-16 11:00:21.413874 nitaq-1.4.0/nitaq.egg-info/
--rw-rw-rw-   0        0        0      199 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-16 11:00:21.000000 nitaq-1.4.0/nitaq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 11:00:21.416874 nitaq-1.4.0/setup.cfg
--rw-rw-rw-   0        0        0      251 2023-07-16 11:00:16.000000 nitaq-1.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:42:37.085247 nitaq-1.5.0/
+-rw-rw-rw-   0        0        0      199 2023-07-16 11:42:37.084247 nitaq-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-07-16 10:13:32.000000 nitaq-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 11:42:37.069246 nitaq-1.5.0/nitaq/
+-rw-rw-rw-   0        0        0       25 2023-07-16 10:37:29.000000 nitaq-1.5.0/nitaq/__init__.py
+-rw-rw-rw-   0        0        0     3130 2023-07-16 11:00:06.000000 nitaq-1.5.0/nitaq/nitaq.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:42:37.083248 nitaq-1.5.0/nitaq.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-07-16 11:42:36.000000 nitaq-1.5.0/nitaq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-07-16 11:42:36.000000 nitaq-1.5.0/nitaq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 11:42:36.000000 nitaq-1.5.0/nitaq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 11:42:36.000000 nitaq-1.5.0/nitaq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-16 11:42:36.000000 nitaq-1.5.0/nitaq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 11:42:37.085247 nitaq-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      251 2023-07-16 11:42:28.000000 nitaq-1.5.0/setup.py
```

### Comparing `nitaq-1.4.0/nitaq/nitaq.py` & `nitaq-1.5.0/nitaq/nitaq.py`

 * *Files identical despite different names*

