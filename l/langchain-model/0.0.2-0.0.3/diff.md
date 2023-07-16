# Comparing `tmp/langchain_model-0.0.2.tar.gz` & `tmp/langchain_model-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_model-0.0.2.tar", last modified: Sun Jul 16 15:01:58 2023, max compression
+gzip compressed data, was "langchain_model-0.0.3.tar", last modified: Sun Jul 16 15:04:08 2023, max compression
```

## Comparing `langchain_model-0.0.2.tar` & `langchain_model-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:01:58.096296 langchain_model-0.0.2/
--rw-r--r--   0 harrisonchase   (501) staff       (20)      108 2023-07-16 15:01:58.096191 langchain_model-0.0.2/PKG-INFO
--rw-r--r--   0 harrisonchase   (501) staff       (20)      107 2023-07-16 14:03:13.000000 langchain_model-0.0.2/README.md
-drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:01:58.096061 langchain_model-0.0.2/langchain_model.egg-info/
--rw-r--r--   0 harrisonchase   (501) staff       (20)      108 2023-07-16 15:01:58.000000 langchain_model-0.0.2/langchain_model.egg-info/PKG-INFO
--rw-r--r--   0 harrisonchase   (501) staff       (20)      212 2023-07-16 15:01:58.000000 langchain_model-0.0.2/langchain_model.egg-info/SOURCES.txt
--rw-r--r--   0 harrisonchase   (501) staff       (20)        1 2023-07-16 15:01:58.000000 langchain_model-0.0.2/langchain_model.egg-info/dependency_links.txt
--rw-r--r--   0 harrisonchase   (501) staff       (20)       21 2023-07-16 15:01:58.000000 langchain_model-0.0.2/langchain_model.egg-info/requires.txt
--rw-r--r--   0 harrisonchase   (501) staff       (20)        1 2023-07-16 15:01:58.000000 langchain_model-0.0.2/langchain_model.egg-info/top_level.txt
--rw-r--r--   0 harrisonchase   (501) staff       (20)       38 2023-07-16 15:01:58.096327 langchain_model-0.0.2/setup.cfg
--rw-r--r--   0 harrisonchase   (501) staff       (20)      265 2023-07-16 15:01:50.000000 langchain_model-0.0.2/setup.py
+drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:04:08.229159 langchain_model-0.0.3/
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      108 2023-07-16 15:04:08.229047 langchain_model-0.0.3/PKG-INFO
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      107 2023-07-16 14:03:13.000000 langchain_model-0.0.3/README.md
+drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:04:08.228898 langchain_model-0.0.3/langchain_model.egg-info/
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      108 2023-07-16 15:04:08.000000 langchain_model-0.0.3/langchain_model.egg-info/PKG-INFO
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      212 2023-07-16 15:04:08.000000 langchain_model-0.0.3/langchain_model.egg-info/SOURCES.txt
+-rw-r--r--   0 harrisonchase   (501) staff       (20)        1 2023-07-16 15:04:08.000000 langchain_model-0.0.3/langchain_model.egg-info/dependency_links.txt
+-rw-r--r--   0 harrisonchase   (501) staff       (20)       21 2023-07-16 15:04:08.000000 langchain_model-0.0.3/langchain_model.egg-info/requires.txt
+-rw-r--r--   0 harrisonchase   (501) staff       (20)        1 2023-07-16 15:04:08.000000 langchain_model-0.0.3/langchain_model.egg-info/top_level.txt
+-rw-r--r--   0 harrisonchase   (501) staff       (20)       38 2023-07-16 15:04:08.229194 langchain_model-0.0.3/setup.cfg
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      265 2023-07-16 15:03:51.000000 langchain_model-0.0.3/setup.py
```

