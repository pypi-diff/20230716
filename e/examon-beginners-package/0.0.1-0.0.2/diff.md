# Comparing `tmp/examon_beginners_package-0.0.1.tar.gz` & `tmp/examon_beginners_package-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "examon_beginners_package-0.0.1.tar", max compression
+gzip compressed data, was "examon_beginners_package-0.0.2.tar", max compression
```

## Comparing `examon_beginners_package-0.0.1.tar` & `examon_beginners_package-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      317 2023-07-16 20:12:47.166285 examon_beginners_package-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       12 2023-07-16 20:17:34.378052 examon_beginners_package-0.0.1/src/__init__.py
--rw-r--r--   0        0        0      392 2023-07-16 20:23:09.417533 examon_beginners_package-0.0.1/src/beginners.py
--rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 examon_beginners_package-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      317 2023-07-16 20:33:56.618671 examon_beginners_package-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-07-16 20:33:56.622876 examon_beginners_package-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0      392 2023-07-16 20:23:09.417533 examon_beginners_package-0.0.2/src/beginners.py
+-rw-r--r--   0        0        0      399 1970-01-01 00:00:00.000000 examon_beginners_package-0.0.2/PKG-INFO
```

