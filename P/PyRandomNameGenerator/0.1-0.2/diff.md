# Comparing `tmp/PyRandomNameGenerator-0.1.tar.gz` & `tmp/PyRandomNameGenerator-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyRandomNameGenerator-0.1.tar", last modified: Sun Jul 16 07:21:28 2023, max compression
+gzip compressed data, was "PyRandomNameGenerator-0.2.tar", last modified: Sun Jul 16 10:38:41 2023, max compression
```

## Comparing `PyRandomNameGenerator-0.1.tar` & `PyRandomNameGenerator-0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:21:28.774570 PyRandomNameGenerator-0.1/
--rw-rw-rw-   0        0        0     1098 2023-07-16 07:00:34.000000 PyRandomNameGenerator-0.1/Licence.txt
--rw-rw-rw-   0        0        0      175 2023-07-16 07:21:28.773570 PyRandomNameGenerator-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-16 07:21:28.762578 PyRandomNameGenerator-0.1/PyRandomNameGenerator/
--rw-rw-rw-   0        0        0      344 2023-07-16 07:16:50.000000 PyRandomNameGenerator-0.1/PyRandomNameGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:21:28.771572 PyRandomNameGenerator-0.1/PyRandomNameGenerator.egg-info/
--rw-rw-rw-   0        0        0      175 2023-07-16 07:21:28.000000 PyRandomNameGenerator-0.1/PyRandomNameGenerator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-07-16 07:21:28.000000 PyRandomNameGenerator-0.1/PyRandomNameGenerator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:21:28.000000 PyRandomNameGenerator-0.1/PyRandomNameGenerator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-07-16 07:21:28.000000 PyRandomNameGenerator-0.1/PyRandomNameGenerator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 07:21:28.774570 PyRandomNameGenerator-0.1/setup.cfg
--rw-rw-rw-   0        0        0      266 2023-07-16 07:19:38.000000 PyRandomNameGenerator-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:38:41.317710 PyRandomNameGenerator-0.2/
+-rw-rw-rw-   0        0        0     1098 2023-07-16 08:12:19.000000 PyRandomNameGenerator-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1055 2023-07-16 10:38:41.316712 PyRandomNameGenerator-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-16 10:38:41.304717 PyRandomNameGenerator-0.2/PyRandomNameGenerator/
+-rw-rw-rw-   0        0        0      344 2023-07-16 07:16:50.000000 PyRandomNameGenerator-0.2/PyRandomNameGenerator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 10:38:41.314712 PyRandomNameGenerator-0.2/PyRandomNameGenerator.egg-info/
+-rw-rw-rw-   0        0        0     1055 2023-07-16 10:38:41.000000 PyRandomNameGenerator-0.2/PyRandomNameGenerator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-07-16 10:38:41.000000 PyRandomNameGenerator-0.2/PyRandomNameGenerator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 10:38:41.000000 PyRandomNameGenerator-0.2/PyRandomNameGenerator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-07-16 10:38:41.000000 PyRandomNameGenerator-0.2/PyRandomNameGenerator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      766 2023-07-16 10:33:25.000000 PyRandomNameGenerator-0.2/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-16 10:38:41.318709 PyRandomNameGenerator-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      497 2023-07-16 10:33:48.000000 PyRandomNameGenerator-0.2/setup.py
```

### Comparing `PyRandomNameGenerator-0.1/Licence.txt` & `PyRandomNameGenerator-0.2/LICENSE.txt`

 * *Files identical despite different names*

