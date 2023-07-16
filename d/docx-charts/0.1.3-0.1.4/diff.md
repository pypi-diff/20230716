# Comparing `tmp/docx_charts-0.1.3.tar.gz` & `tmp/docx_charts-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_charts-0.1.3.tar", max compression
+gzip compressed data, was "docx_charts-0.1.4.tar", max compression
```

## Comparing `docx_charts-0.1.3.tar` & `docx_charts-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.3/LICENSE
--rw-r--r--   0        0        0      247 2023-07-16 14:30:02.509753 docx_charts-0.1.3/README.md
--rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.3/docx_charts/__init__.py
--rw-r--r--   0        0        0     2603 2023-07-16 14:15:35.194707 docx_charts-0.1.3/docx_charts/chart.py
--rw-r--r--   0        0        0     2452 2023-07-16 14:12:48.053698 docx_charts-0.1.3/docx_charts/document.py
--rw-r--r--   0        0        0      485 2023-07-16 14:27:01.284743 docx_charts-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 docx_charts-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.4/LICENSE
+-rw-r--r--   0        0        0      247 2023-07-16 14:30:02.509753 docx_charts-0.1.4/README.md
+-rw-r--r--   0        0        0       78 2023-07-16 13:44:16.854606 docx_charts-0.1.4/docx_charts/__init__.py
+-rw-r--r--   0        0        0     2603 2023-07-16 14:15:35.194707 docx_charts-0.1.4/docx_charts/chart.py
+-rw-r--r--   0        0        0     3214 2023-07-16 14:45:55.672804 docx_charts-0.1.4/docx_charts/document.py
+-rw-r--r--   0        0        0      485 2023-07-16 14:46:24.485805 docx_charts-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 docx_charts-0.1.4/PKG-INFO
```

### Comparing `docx_charts-0.1.3/LICENSE` & `docx_charts-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.3/docx_charts/chart.py` & `docx_charts-0.1.4/docx_charts/chart.py`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.3/docx_charts/document.py` & `docx_charts-0.1.4/docx_charts/document.py`

 * *Files 21% similar despite different names*

```diff
@@ -33,14 +33,27 @@
 	def __del__(self):
 		'''
 		Cleans up the temporary directory when the Document object is destroyed.
 		'''
 		self.extracted.cleanup()
 
 
+	def save(self, file_path: str|None = None):
+		'''
+		Re-archives the Word document and saves it to the specified path.
+
+		Args:
+			file_path (str): The path to save the Word document to. If not specified, the original file will be overwritten.
+		'''
+		if file_path is None:
+			file_path = self.file_path
+		shutil.make_archive(file_path, 'zip', self.extracted.name)
+		shutil.move(f'{file_path}.zip', file_path)
+
+
 	def list_contents(self):
 		'''
 		Lists the contents of the Word document.
 
 		Returns:
 			A list of files in the root of the extracted archive
 		'''
@@ -78,7 +91,22 @@
 		Returns:
 			A list of objects representing the charts in the Word document with the specified name.
 
 		Note:
 			Generally this will only return one chart, but it is possible for there to be multiple charts with the same name.
 		'''
 		return [chart for chart in self.list_charts() if chart.name == name]
+
+
+if __name__ == '__main__':
+	doc = Document('files/test/yeet2.docx')
+	chart = doc.find_charts_by_name('Chart 2')[0]
+	data = chart.data()
+
+	data[0][0] = (data[0][0][0], data[0][0][1] + 0.3)
+	data[0][1] = (data[0][1][0], data[0][1][1] - 0.2)
+	data[0][2] = (data[0][1][0], data[0][1][1] - 0.1)
+	chart.write_data(data)
+
+	doc.save()
+
+	print(chart.data())
```

### Comparing `docx_charts-0.1.3/PKG-INFO` & `docx_charts-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docx-charts
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python library for manipulating chart data in word documents
 Author: Julia van der Kris
 Author-email: julia@juuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuuulia.dev
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

