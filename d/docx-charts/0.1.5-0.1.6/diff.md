# Comparing `tmp/docx_charts-0.1.5.tar.gz` & `tmp/docx_charts-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_charts-0.1.5.tar", max compression
+gzip compressed data, was "docx_charts-0.1.6.tar", max compression
```

## Comparing `docx_charts-0.1.5.tar` & `docx_charts-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.5/LICENSE
--rw-r--r--   0        0        0      247 2023-07-16 14:30:02.509753 docx_charts-0.1.5/README.md
--rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.5/docx_charts/__init__.py
--rw-r--r--   0        0        0     2603 2023-07-16 14:15:35.194707 docx_charts-0.1.5/docx_charts/chart.py
--rw-r--r--   0        0        0     2864 2023-07-16 14:49:58.132817 docx_charts-0.1.5/docx_charts/document.py
--rw-r--r--   0        0        0      485 2023-07-16 14:50:38.052819 docx_charts-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 docx_charts-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.6/LICENSE
+-rw-r--r--   0        0        0      247 2023-07-16 14:30:02.509753 docx_charts-0.1.6/README.md
+-rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.6/docx_charts/__init__.py
+-rw-r--r--   0        0        0     2880 2023-07-16 16:29:12.559205 docx_charts-0.1.6/docx_charts/chart.py
+-rw-r--r--   0        0        0     2864 2023-07-16 16:05:17.775128 docx_charts-0.1.6/docx_charts/document.py
+-rw-r--r--   0        0        0      485 2023-07-16 16:29:25.738206 docx_charts-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 docx_charts-0.1.6/PKG-INFO
```

### Comparing `docx_charts-0.1.5/LICENSE` & `docx_charts-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.5/docx_charts/chart.py` & `docx_charts-0.1.6/docx_charts/chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import io
 from xml.dom import minidom
 
 
-DataPoint = tuple[str, float]
-Series = list[DataPoint]
+Series = dict[str, float]
 
 
 class Chart:
 	'''
 	Represents a chart in a Word document.
 
 	Attributes:
@@ -50,21 +49,21 @@
 
 
 	def data(self) -> list[Series]:
 		'''
 		Gets the internal table data the chart is based on.
 
 		Returns:
-			A list of Series objects representing the data for the chart.
+			A list of Series dictionaries representing the data for the chart.
 		'''
 		dom = minidom.parse(self.file)
 		series = [
-			list(zip(
+			dict(zip(
 				[cat.firstChild.nodeValue for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
-					if cat.firstChild and isinstance(cat.firstChild, minidom.Text)],
+					if cat.firstChild and isinstance(cat.firstChild, minidom.Text) and isinstance(cat.firstChild.nodeValue, str)],
 				[float(val.firstChild.nodeValue) for val in series.getElementsByTagName('c:val')[0].getElementsByTagName('c:v')
 					if val.firstChild and isinstance(val.firstChild, minidom.Text)]
 			))
 			for series in dom.getElementsByTagName('c:ser')
 		]
 		self.file.seek(0)
 		return series
@@ -74,26 +73,30 @@
 		'''
 		Overwrites the data of the chart.
 
 		Args:
 			data (list[Series]): The data to write to the chart.
 
 		Note:
-			The data must be in the same size and shape as the original data.
-			(i.e. the same number of series, categories, and values)
+			The data must be in the same number of series as the original data.
+			However, unchanged categories may be left out.
 		'''
+		assert len(data) == len(self.data()), 'The new data must have the same number of series as the original data.'
 		dom = minidom.parse(self.file)
-		for series, series_data in zip(dom.getElementsByTagName('c:ser'), data):
+		for series, new_series in zip(dom.getElementsByTagName('c:ser'), data):
 			cats = [cat.firstChild for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
 				if cat.firstChild and isinstance(cat.firstChild, minidom.Text)]
 			vals = [val.firstChild for val in series.getElementsByTagName('c:val')[0].getElementsByTagName('c:v')
 				if val.firstChild and isinstance(val.firstChild, minidom.Text)]
 
-			for cat, val, (new_cat, new_val) in zip(cats, vals, series_data):
-				cat.replaceWholeText(new_cat)
-				val.replaceWholeText(str(new_val))
+			for new_cat, new_val in new_series.items():
+				assert new_cat in [cat.nodeValue for cat in cats], 'The new data must have the same categories as the original data.'
+				for cat, val in zip(cats, vals):
+					if cat.nodeValue == new_cat:
+						val.replaceWholeText(str(new_val))
+						break
 
 		self.file.seek(0)
 		self.file.truncate()
 		self.file.write(dom.toxml())
 		self.file.flush()
 		self.file.seek(0)
```

### Comparing `docx_charts-0.1.5/docx_charts/document.py` & `docx_charts-0.1.6/docx_charts/document.py`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.5/PKG-INFO` & `docx_charts-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-charts
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python library for manipulating chart data in word documents
 Author: Julia van der Kris
 Author-email: julia@juuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuulia.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

