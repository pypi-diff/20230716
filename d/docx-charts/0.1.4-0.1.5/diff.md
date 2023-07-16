# Comparing `tmp/docx_charts-0.1.4.tar.gz` & `tmp/docx_charts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_charts-0.1.4.tar", max compression
+gzip compressed data, was "docx_charts-0.1.5.tar", max compression
```

## Comparing `docx_charts-0.1.4.tar` & `docx_charts-0.1.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.4/LICENSE
--rw-r--r--   0        0        0      247 2023-07-16 14:30:02.509753 docx_charts-0.1.4/README.md
--rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.4/docx_charts/__init__.py
--rw-r--r--   0        0        0     2603 2023-07-16 14:15:35.194707 docx_charts-0.1.4/docx_charts/chart.py
--rw-r--r--   0        0        0     3214 2023-07-16 14:45:55.672804 docx_charts-0.1.4/docx_charts/document.py
--rw-r--r--   0        0        0      485 2023-07-16 14:46:24.485805 docx_charts-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 docx_charts-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.5/LICENSE
+-rw-r--r--   0        0        0      247 2023-07-16 14:30:02.509753 docx_charts-0.1.5/README.md
+-rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.5/docx_charts/__init__.py
+-rw-r--r--   0        0        0     2603 2023-07-16 14:15:35.194707 docx_charts-0.1.5/docx_charts/chart.py
+-rw-r--r--   0        0        0     2864 2023-07-16 14:49:58.132817 docx_charts-0.1.5/docx_charts/document.py
+-rw-r--r--   0        0        0      485 2023-07-16 14:50:38.052819 docx_charts-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 docx_charts-0.1.5/PKG-INFO
```

### Comparing `docx_charts-0.1.4/LICENSE` & `docx_charts-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.4/docx_charts/chart.py` & `docx_charts-0.1.5/docx_charts/chart.py`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.4/docx_charts/document.py` & `docx_charts-0.1.5/docx_charts/document.py`

 * *Files 20% similar despite different names*

```diff
@@ -91,22 +91,7 @@
 		Returns:
 			A list of objects representing the charts in the Word document with the specified name.
 
 		Note:
 			Generally this will only return one chart, but it is possible for there to be multiple charts with the same name.
 		'''
 		return [chart for chart in self.list_charts() if chart.name == name]
-
-
-if __name__ == '__main__':
-	doc = Document('files/test/yeet2.docx')
-	chart = doc.find_charts_by_name('Chart 2')[0]
-	data = chart.data()
-
-	data[0][0] = (data[0][0][0], data[0][0][1] + 0.3)
-	data[0][1] = (data[0][1][0], data[0][1][1] - 0.2)
-	data[0][2] = (data[0][1][0], data[0][1][1] - 0.1)
-	chart.write_data(data)
-
-	doc.save()
-
-	print(chart.data())
```

