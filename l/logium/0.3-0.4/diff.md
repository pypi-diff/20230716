# Comparing `tmp/logium-0.3.tar.gz` & `tmp/logium-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logium-0.3.tar", last modified: Sat Jul 15 21:22:22 2023, max compression
+gzip compressed data, was "logium-0.4.tar", last modified: Sat Jul 15 22:31:39 2023, max compression
```

## Comparing `logium-0.3.tar` & `logium-0.4.tar`

### file list

```diff
@@ -1,13 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 21:22:22.658045 logium-0.3/
--rw-rw-rw-   0        0        0      157 2023-07-15 21:22:22.658045 logium-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-15 21:22:22.621104 logium-0.3/logium/
--rw-rw-rw-   0        0        0     2301 2023-07-15 21:21:22.000000 logium-0.3/logium/__init__.py
--rw-rw-rw-   0        0        0      510 2023-07-15 20:34:17.000000 logium-0.3/logium/decorators.py
--rw-rw-rw-   0        0        0     3545 2023-07-15 21:03:12.000000 logium-0.3/logium/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-15 21:22:22.658045 logium-0.3/logium.egg-info/
--rw-rw-rw-   0        0        0      157 2023-07-15 21:22:22.000000 logium-0.3/logium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      195 2023-07-15 21:22:22.000000 logium-0.3/logium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 21:22:22.000000 logium-0.3/logium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 21:22:22.000000 logium-0.3/logium.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 21:22:22.666027 logium-0.3/setup.cfg
--rw-rw-rw-   0        0        0      388 2023-07-15 21:20:36.000000 logium-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:31:39.548712 logium-0.4/
+-rw-rw-rw-   0        0        0      157 2023-07-15 22:31:39.548712 logium-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 22:31:39.501051 logium-0.4/logium/
+-rw-rw-rw-   0        0        0     6100 2023-07-15 22:08:34.000000 logium-0.4/logium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 22:31:39.548712 logium-0.4/logium.egg-info/
+-rw-rw-rw-   0        0        0      157 2023-07-15 22:31:39.000000 logium-0.4/logium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2023-07-15 22:31:39.000000 logium-0.4/logium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 22:31:39.000000 logium-0.4/logium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-15 22:31:39.000000 logium-0.4/logium.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 22:31:39.563373 logium-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      388 2023-07-15 22:31:15.000000 logium-0.4/setup.py
```

