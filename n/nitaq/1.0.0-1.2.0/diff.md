# Comparing `tmp/nitaq-1.0.0.tar.gz` & `tmp/nitaq-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitaq-1.0.0.tar", last modified: Sun Jul 16 10:18:02 2023, max compression
+gzip compressed data, was "nitaq-1.2.0.tar", last modified: Sun Jul 16 10:28:30 2023, max compression
```

## Comparing `nitaq-1.0.0.tar` & `nitaq-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 10:18:02.669611 nitaq-1.0.0/
--rw-rw-rw-   0        0        0      199 2023-07-16 10:18:02.662611 nitaq-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       13 2023-07-16 10:13:32.000000 nitaq-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 10:18:02.640611 nitaq-1.0.0/nitaq/
--rw-rw-rw-   0        0        0       19 2023-07-16 10:17:55.000000 nitaq-1.0.0/nitaq/__init__.py
--rw-rw-rw-   0        0        0     3066 2023-07-16 10:17:21.000000 nitaq-1.0.0/nitaq/nitaq.py
-drwxrwxrwx   0        0        0        0 2023-07-16 10:18:02.660610 nitaq-1.0.0/nitaq.egg-info/
--rw-rw-rw-   0        0        0      199 2023-07-16 10:18:02.000000 nitaq-1.0.0/nitaq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-07-16 10:18:02.000000 nitaq-1.0.0/nitaq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 10:18:02.000000 nitaq-1.0.0/nitaq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-16 10:18:02.000000 nitaq-1.0.0/nitaq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-16 10:18:02.000000 nitaq-1.0.0/nitaq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 10:18:02.670610 nitaq-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      251 2023-07-16 10:13:09.000000 nitaq-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:28:30.062171 nitaq-1.2.0/
+-rw-rw-rw-   0        0        0      199 2023-07-16 10:28:30.062171 nitaq-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       13 2023-07-16 10:13:32.000000 nitaq-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 10:28:30.040173 nitaq-1.2.0/nitaq/
+-rw-rw-rw-   0        0        0       19 2023-07-16 10:28:20.000000 nitaq-1.2.0/nitaq/__init__.py
+-rw-rw-rw-   0        0        0     3066 2023-07-16 10:17:21.000000 nitaq-1.2.0/nitaq/nitaq.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:28:30.060169 nitaq-1.2.0/nitaq.egg-info/
+-rw-rw-rw-   0        0        0      199 2023-07-16 10:28:29.000000 nitaq-1.2.0/nitaq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      195 2023-07-16 10:28:29.000000 nitaq-1.2.0/nitaq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:28:29.000000 nitaq-1.2.0/nitaq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-07-16 10:28:29.000000 nitaq-1.2.0/nitaq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-16 10:28:29.000000 nitaq-1.2.0/nitaq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:28:30.062171 nitaq-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      251 2023-07-16 10:25:49.000000 nitaq-1.2.0/setup.py
```

### Comparing `nitaq-1.0.0/nitaq/nitaq.py` & `nitaq-1.2.0/nitaq/nitaq.py`

 * *Files identical despite different names*

