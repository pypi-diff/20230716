# Comparing `tmp/kthreading-0.1.tar.gz` & `tmp/kthreading-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthreading-0.1.tar", last modified: Wed Jul 12 08:35:59 2023, max compression
+gzip compressed data, was "kthreading-0.2.tar", last modified: Sun Jul 16 05:36:47 2023, max compression
```

## Comparing `kthreading-0.1.tar` & `kthreading-0.2.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:59.198854 kthreading-0.1/
--rw-rw-rw-   0        0        0      119 2023-07-12 08:35:59.198854 kthreading-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:59.176855 kthreading-0.1/kthreading/
--rw-rw-rw-   0        0        0       85 2023-07-12 08:32:46.000000 kthreading-0.1/kthreading/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 08:35:59.196829 kthreading-0.1/kthreading.egg-info/
--rw-rw-rw-   0        0        0      119 2023-07-12 08:35:59.000000 kthreading-0.1/kthreading.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-07-12 08:35:59.000000 kthreading-0.1/kthreading.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 08:35:59.000000 kthreading-0.1/kthreading.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-12 08:35:59.000000 kthreading-0.1/kthreading.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2023-07-12 08:35:59.000000 kthreading-0.1/kthreading.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-12 08:35:59.200852 kthreading-0.1/setup.cfg
--rw-rw-rw-   0        0        0      182 2023-07-12 08:35:36.000000 kthreading-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 05:36:47.163765 kthreading-0.2/
+-rw-rw-rw-   0        0        0     1093 2023-07-16 05:11:51.000000 kthreading-0.2/LICENSE.md
+-rw-rw-rw-   0        0        0     1166 2023-07-16 05:36:47.162767 kthreading-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2023-07-16 05:24:18.000000 kthreading-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 05:36:47.137471 kthreading-0.2/kthreading/
+-rw-rw-rw-   0        0        0      349 2023-07-12 09:40:43.000000 kthreading-0.2/kthreading/__init__.py
+-rw-rw-rw-   0        0        0     1753 2023-07-15 13:47:57.000000 kthreading-0.2/kthreading/classes.py
+-rw-rw-rw-   0        0        0      388 2023-07-12 09:40:43.000000 kthreading-0.2/kthreading/exceptions.py
+-rw-rw-rw-   0        0        0      213 2023-07-12 01:41:50.000000 kthreading-0.2/kthreading/functions.py
+-rw-rw-rw-   0        0        0     2843 2023-07-15 15:05:34.000000 kthreading-0.2/kthreading/kthread.py
+-rw-rw-rw-   0        0        0      626 2023-07-12 09:40:44.000000 kthreading-0.2/kthreading/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 05:36:47.161762 kthreading-0.2/kthreading.egg-info/
+-rw-rw-rw-   0        0        0     1166 2023-07-16 05:36:46.000000 kthreading-0.2/kthreading.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      301 2023-07-16 05:36:47.000000 kthreading-0.2/kthreading.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 05:36:47.000000 kthreading-0.2/kthreading.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-16 05:36:47.000000 kthreading-0.2/kthreading.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 05:36:47.163765 kthreading-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      610 2023-07-16 05:32:07.000000 kthreading-0.2/setup.py
```

