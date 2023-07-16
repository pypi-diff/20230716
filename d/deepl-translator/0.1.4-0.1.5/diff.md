# Comparing `tmp/deepl_translator-0.1.4.tar.gz` & `tmp/deepl_translator-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepl_translator-0.1.4.tar", last modified: Sun Jul 16 15:31:38 2023, max compression
+gzip compressed data, was "deepl_translator-0.1.5.tar", last modified: Sun Jul 16 15:33:49 2023, max compression
```

## Comparing `deepl_translator-0.1.4.tar` & `deepl_translator-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:31:38.815081 deepl_translator-0.1.4/
--rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:31:38.814961 deepl_translator-0.1.4/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      170 2023-07-16 14:44:23.000000 deepl_translator-0.1.4/README.md
-drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:31:38.814770 deepl_translator-0.1.4/deepl_translator.egg-info/
--rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:31:38.000000 deepl_translator-0.1.4/deepl_translator.egg-info/PKG-INFO
--rw-r--r--   0 lunox      (501) staff       (20)      280 2023-07-16 15:31:38.000000 deepl_translator-0.1.4/deepl_translator.egg-info/SOURCES.txt
--rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-16 15:31:38.000000 deepl_translator-0.1.4/deepl_translator.egg-info/dependency_links.txt
--rw-r--r--   0 lunox      (501) staff       (20)       58 2023-07-16 15:31:38.000000 deepl_translator-0.1.4/deepl_translator.egg-info/entry_points.txt
--rw-r--r--   0 lunox      (501) staff       (20)        6 2023-07-16 15:31:38.000000 deepl_translator-0.1.4/deepl_translator.egg-info/requires.txt
--rw-r--r--   0 lunox      (501) staff       (20)       17 2023-07-16 15:31:38.000000 deepl_translator-0.1.4/deepl_translator.egg-info/top_level.txt
--rw-r--r--   0 lunox      (501) staff       (20)     1737 2023-07-16 15:11:04.000000 deepl_translator-0.1.4/deepl_translator.py
--rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-16 15:31:38.815122 deepl_translator-0.1.4/setup.cfg
--rw-r--r--   0 lunox      (501) staff       (20)      261 2023-07-16 15:31:37.000000 deepl_translator-0.1.4/setup.py
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:33:49.373574 deepl_translator-0.1.5/
+-rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:33:49.373464 deepl_translator-0.1.5/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      170 2023-07-16 14:44:23.000000 deepl_translator-0.1.5/README.md
+drwxr-xr-x   0 lunox      (501) staff       (20)        0 2023-07-16 15:33:49.373305 deepl_translator-0.1.5/deepl_translator.egg-info/
+-rw-r--r--   0 lunox      (501) staff       (20)       60 2023-07-16 15:33:49.000000 deepl_translator-0.1.5/deepl_translator.egg-info/PKG-INFO
+-rw-r--r--   0 lunox      (501) staff       (20)      280 2023-07-16 15:33:49.000000 deepl_translator-0.1.5/deepl_translator.egg-info/SOURCES.txt
+-rw-r--r--   0 lunox      (501) staff       (20)        1 2023-07-16 15:33:49.000000 deepl_translator-0.1.5/deepl_translator.egg-info/dependency_links.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       58 2023-07-16 15:33:49.000000 deepl_translator-0.1.5/deepl_translator.egg-info/entry_points.txt
+-rw-r--r--   0 lunox      (501) staff       (20)        6 2023-07-16 15:33:49.000000 deepl_translator-0.1.5/deepl_translator.egg-info/requires.txt
+-rw-r--r--   0 lunox      (501) staff       (20)       37 2023-07-16 15:33:49.000000 deepl_translator-0.1.5/deepl_translator.egg-info/top_level.txt
+-rw-r--r--   0 lunox      (501) staff       (20)     1737 2023-07-16 15:11:04.000000 deepl_translator-0.1.5/deepl_translator.py
+-rw-r--r--   0 lunox      (501) staff       (20)       38 2023-07-16 15:33:49.373614 deepl_translator-0.1.5/setup.cfg
+-rw-r--r--   0 lunox      (501) staff       (20)      287 2023-07-16 15:33:43.000000 deepl_translator-0.1.5/setup.py
```

### Comparing `deepl_translator-0.1.4/deepl_translator.py` & `deepl_translator-0.1.5/deepl_translator.py`

 * *Files identical despite different names*

