# Comparing `tmp/deepl_translator-0.1.6.tar.gz` & `tmp/deepl_translator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepl_translator-0.1.6.tar", last modified: Sun Jul 16 15:39:08 2023, max compression
+gzip compressed data, was "deepl_translator-0.1.7.tar", last modified: Sun Jul 16 15:42:53 2023, max compression
```

## Comparing `deepl_translator-0.1.6.tar` & `deepl_translator-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:39:08.535929 deepl_translator-0.1.6/
--rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:39:08.535814 deepl_translator-0.1.6/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      170 2023-07-16 14:44:23.000000 deepl_translator-0.1.6/README.md
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:39:08.535660 deepl_translator-0.1.6/deepl_translator.egg-info/
--rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:39:08.000000 deepl_translator-0.1.6/deepl_translator.egg-info/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      280 2023-07-16 15:39:08.000000 deepl_translator-0.1.6/deepl_translator.egg-info/SOURCES.txt
--rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-16 15:39:08.000000 deepl_translator-0.1.6/deepl_translator.egg-info/dependency_links.txt
--rw-r--r--   0 lunox      (501) staff       (20)       58 2023-07-16 15:39:08.000000 deepl_translator-0.1.6/deepl_translator.egg-info/entry_points.txt
--rw-r--r--   0 lunox      (501) staff       (20)        6 2023-07-16 15:39:08.000000 deepl_translator-0.1.6/deepl_translator.egg-info/requires.txt
--rw-r--r--   0 lunox      (501) staff       (20)       37 2023-07-16 15:39:08.000000 deepl_translator-0.1.6/deepl_translator.egg-info/top_level.txt
--rw-r--r--   0 lunox      (501) staff       (20)     1737 2023-07-16 15:11:04.000000 deepl_translator-0.1.6/deepl_translator.py
--rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-16 15:39:08.535964 deepl_translator-0.1.6/setup.cfg
--rw-r--r--   0 lunox      (501) staff       (20)      408 2023-07-16 15:38:59.000000 deepl_translator-0.1.6/setup.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:42:53.170601 deepl_translator-0.1.7/
+-rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:42:53.170495 deepl_translator-0.1.7/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      170 2023-07-16 14:44:23.000000 deepl_translator-0.1.7/README.md
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:42:53.170347 deepl_translator-0.1.7/deepl_translator.egg-info/
+-rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:42:53.000000 deepl_translator-0.1.7/deepl_translator.egg-info/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      302 2023-07-16 15:42:53.000000 deepl_translator-0.1.7/deepl_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-16 15:42:53.000000 deepl_translator-0.1.7/deepl_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       58 2023-07-16 15:42:53.000000 deepl_translator-0.1.7/deepl_translator.egg-info/entry_points.txt
+-rw-r--r--   0 lunox      (501) staff       (20)        6 2023-07-16 15:42:53.000000 deepl_translator-0.1.7/deepl_translator.egg-info/requires.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       17 2023-07-16 15:42:53.000000 deepl_translator-0.1.7/deepl_translator.egg-info/top_level.txt
+-rw-r--r--   0 lunox      (501) staff       (20)     1737 2023-07-16 15:11:04.000000 deepl_translator-0.1.7/deepl_translator.py
+-rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-16 15:42:53.170635 deepl_translator-0.1.7/setup.cfg
+-rw-r--r--   0 lunox      (501) staff       (20)      423 2023-07-16 15:42:49.000000 deepl_translator-0.1.7/setup.py
```

### Comparing `deepl_translator-0.1.6/deepl_translator.py` & `deepl_translator-0.1.7/deepl_translator.py`

 * *Files identical despite different names*

