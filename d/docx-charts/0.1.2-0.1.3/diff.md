# Comparing `tmp/docx_charts-0.1.2.tar.gz` & `tmp/docx_charts-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_charts-0.1.2.tar", max compression
+gzip compressed data, was "docx_charts-0.1.3.tar", max compression
```

## Comparing `docx_charts-0.1.2.tar` & `docx_charts-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.2/LICENSE
--rw-r--r--   0        0        0       14 2023-07-15 15:56:07.324415 docx_charts-0.1.2/README.md
--rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.2/docx_charts/__init__.py
--rw-r--r--   0        0        0     2603 2023-07-16 14:15:35.194707 docx_charts-0.1.2/docx_charts/chart.py
--rw-r--r--   0        0        0     2452 2023-07-16 14:12:48.053698 docx_charts-0.1.2/docx_charts/document.py
--rw-r--r--   0        0        0      425 2023-07-16 14:16:03.477708 docx_charts-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 docx_charts-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.3/LICENSE
+-rw-r--r--   0        0        0      247 2023-07-16 14:30:02.509753 docx_charts-0.1.3/README.md
+-rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.3/docx_charts/__init__.py
+-rw-r--r--   0        0        0     2603 2023-07-16 14:15:35.194707 docx_charts-0.1.3/docx_charts/chart.py
+-rw-r--r--   0        0        0     2452 2023-07-16 14:12:48.053698 docx_charts-0.1.3/docx_charts/document.py
+-rw-r--r--   0        0        0      485 2023-07-16 14:27:01.284743 docx_charts-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 docx_charts-0.1.3/PKG-INFO
```

### Comparing `docx_charts-0.1.2/LICENSE` & `docx_charts-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.2/docx_charts/chart.py` & `docx_charts-0.1.3/docx_charts/chart.py`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.2/docx_charts/document.py` & `docx_charts-0.1.3/docx_charts/document.py`

 * *Files identical despite different names*

