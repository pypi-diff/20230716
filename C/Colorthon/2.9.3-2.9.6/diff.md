# Comparing `tmp/colorthon-2.9.3.tar.gz` & `tmp/Colorthon-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorthon-2.9.3.tar", last modified: Sun Jul 16 15:52:03 2023, max compression
+gzip compressed data, was "Colorthon-2.9.6.tar", last modified: Sun Jul 16 16:01:57 2023, max compression
```

## Comparing `colorthon-2.9.3.tar` & `Colorthon-2.9.6.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 15:52:03.788437 colorthon-2.9.3/
--rw-rw-rw-   0        0        0      331 2023-07-16 15:52:03.788437 colorthon-2.9.3/PKG-INFO
--rw-rw-rw-   0        0        0     2330 2023-07-11 19:38:35.000000 colorthon-2.9.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 15:52:03.788437 colorthon-2.9.3/colorthon.egg-info/
--rw-rw-rw-   0        0        0      331 2023-07-16 15:52:03.000000 colorthon-2.9.3/colorthon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      160 2023-07-16 15:52:03.000000 colorthon-2.9.3/colorthon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 15:52:03.000000 colorthon-2.9.3/colorthon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 15:52:03.000000 colorthon-2.9.3/colorthon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-16 15:52:03.789436 colorthon-2.9.3/setup.cfg
--rw-rw-rw-   0        0        0      398 2023-07-16 15:43:17.000000 colorthon-2.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:01:57.952760 Colorthon-2.9.6/
+drwxrwxrwx   0        0        0        0 2023-07-16 16:01:57.950758 Colorthon-2.9.6/Colorthon.egg-info/
+-rw-rw-rw-   0        0        0     3776 2023-07-16 16:01:57.000000 Colorthon-2.9.6/Colorthon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2023-07-16 16:01:57.000000 Colorthon-2.9.6/Colorthon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 16:01:57.000000 Colorthon-2.9.6/Colorthon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 16:01:57.000000 Colorthon-2.9.6/Colorthon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3776 2023-07-16 16:01:57.952760 Colorthon-2.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2330 2023-07-11 19:38:35.000000 Colorthon-2.9.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 16:01:57.951758 Colorthon-2.9.6/colorthon/
+-rw-rw-rw-   0        0        0      113 2023-07-16 15:34:52.000000 Colorthon-2.9.6/colorthon/__init__.py
+-rw-rw-rw-   0        0        0      438 2023-07-11 19:23:23.000000 Colorthon-2.9.6/colorthon/utils.py
+-rw-rw-rw-   0        0        0       42 2023-07-16 16:01:57.952760 Colorthon-2.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2023-07-16 16:00:07.000000 Colorthon-2.9.6/setup.py
```

### Comparing `colorthon-2.9.3/README.md` & `Colorthon-2.9.6/README.md`

 * *Files identical despite different names*

