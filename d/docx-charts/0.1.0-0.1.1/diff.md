# Comparing `tmp/docx_charts-0.1.0.tar.gz` & `tmp/docx_charts-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docx_charts-0.1.0.tar", max compression
+gzip compressed data, was "docx_charts-0.1.1.tar", max compression
```

## Comparing `docx_charts-0.1.0.tar` & `docx_charts-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.0/LICENSE
--rw-r--r--   0        0        0       14 2023-07-15 15:56:07.324415 docx_charts-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-15 15:45:00.354379 docx_charts-0.1.0/docx_charts/__init__.py
--rw-r--r--   0        0        0     1884 2023-07-16 13:14:02.888510 docx_charts-0.1.0/docx_charts/chart.py
--rw-r--r--   0        0        0     1746 2023-07-16 13:07:52.153490 docx_charts-0.1.0/docx_charts/document.py
--rw-r--r--   0        0        0      425 2023-07-16 12:09:17.057302 docx_charts-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 docx_charts-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-15 15:55:15.811412 docx_charts-0.1.1/LICENSE
+-rw-r--r--   0        0        0       14 2023-07-15 15:56:07.324415 docx_charts-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 15:45:00.354379 docx_charts-0.1.1/docx_charts/__init__.py
+-rw-r--r--   0        0        0     1634 2023-07-16 13:34:48.345576 docx_charts-0.1.1/docx_charts/chart.py
+-rw-r--r--   0        0        0     1352 2023-07-16 13:33:34.170572 docx_charts-0.1.1/docx_charts/document.py
+-rw-r--r--   0        0        0      425 2023-07-16 13:36:55.307583 docx_charts-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      364 1970-01-01 00:00:00.000000 docx_charts-0.1.1/PKG-INFO
```

### Comparing `docx_charts-0.1.0/LICENSE` & `docx_charts-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `docx_charts-0.1.0/docx_charts/chart.py` & `docx_charts-0.1.1/docx_charts/chart.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 					if val.firstChild and type(val.firstChild) == minidom.Text]
 			))
 			for series in dom.getElementsByTagName('c:ser')
 		]
 		self.file.seek(0)
 		return series
 
+
 	def write_data(self, data: list[Series]) -> None:
 		dom = minidom.parse(self.file)
 		for series, series_data in zip(dom.getElementsByTagName('c:ser'), data):
 			cats = [cat.firstChild for cat in series.getElementsByTagName('c:cat')[0].getElementsByTagName('c:v')
 				if cat.firstChild and type(cat.firstChild) == minidom.Text]
 			vals = [val.firstChild for val in series.getElementsByTagName('c:val')[0].getElementsByTagName('c:v')
 				if val.firstChild and type(val.firstChild) == minidom.Text]
@@ -46,19 +47,7 @@
 				val.replaceWholeText(str(new_val))
 
 		self.file.seek(0)
 		self.file.truncate()
 		self.file.write(dom.toxml())
 		self.file.flush()
 		self.file.seek(0)
-
-
-
-if __name__ == '__main__':
-	chart = Chart('files/test/chart1.xml', 'Chart 2')
-	data = chart.data()
-
-	data[0][0] = (data[0][0][0], data[0][0][1] + 0.1)
-	data[0][1] = (data[0][1][0], data[0][1][1] - 0.1)
-	chart.write_data(data)
-
-	print(chart.data())
```

### Comparing `docx_charts-0.1.0/docx_charts/document.py` & `docx_charts-0.1.1/docx_charts/document.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,52 +1,36 @@
-import io
 import os
 import tempfile
 import shutil
 from xml.dom import minidom
-from pprint import pprint
 
 from docx_charts.chart import Chart
 
 
 class Document:
-	# file: io.IOBase
 	file_path: str
 	extracted: tempfile.TemporaryDirectory
 
 	def __init__(self, file_path: str):
-		# self.file = open(file_path, 'rb')
 		self.file_path = file_path
 		self.extracted = tempfile.TemporaryDirectory()
 		shutil.unpack_archive(file_path, self.extracted.name, format='zip')
 
 	def list_contents(self):
 		return os.listdir(self.extracted.name)
 
 	def list_charts(self) -> list[Chart]:
 		charts: list[Chart] = []
-		# with self.zipfs.open('word/document.xml') as doc:
-		# 	with self.zipfs.open('word/_rels/document.xml.rels') as rels:
 		with open(os.path.join(self.extracted.name, 'word/document.xml')) as doc:
 			with open(os.path.join(self.extracted.name, 'word/_rels/document.xml.rels')) as rels:
 				doc_dom = minidom.parse(doc)
 				rels_dom = minidom.parse(rels)
 				for node in doc_dom.getElementsByTagName('c:chart'):
 					relationship_id = node.getAttribute('r:id')
 					relationship = [rel for rel in rels_dom.getElementsByTagName('Relationship') if rel.getAttribute('Id') == relationship_id][0]
 					path = os.path.join(self.extracted.name, 'word', relationship.getAttribute('Target'))
 					name = node.parentNode.parentNode.parentNode.getElementsByTagName('wp:docPr')[0].getAttribute('name')
 					charts.append(Chart(path, name))
 		return charts
 
 	def find_charts_by_name(self, name: str) -> list[Chart]:
 		return [chart for chart in self.list_charts() if chart.name == name]
-
-
-
-if __name__ == '__main__':
-	doc = Document('files/test/yeet2.docx')
-	print(doc.list_contents())
-
-	for chart in doc.list_charts():
-		print(f'\n\n{chart}')
-		pprint(chart.data())
```

