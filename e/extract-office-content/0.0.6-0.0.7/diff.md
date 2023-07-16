# Comparing `tmp/extract_office_content-0.0.6-py3-none-any.whl.zip` & `tmp/extract_office_content-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 10734 bytes, number of entries: 11
--rw-r--r--  2.0 unx      227 b- defN 23-Jul-02 10:31 extract_office_content/__init__.py
--rw-r--r--  2.0 unx     4444 b- defN 23-Jul-02 10:31 extract_office_content/extract_excel.py
--rw-r--r--  2.0 unx     4174 b- defN 23-Jul-02 10:31 extract_office_content/extract_ppt.py
--rw-r--r--  2.0 unx     6717 b- defN 23-Jul-02 10:31 extract_office_content/extract_word.py
--rw-r--r--  2.0 unx     2275 b- defN 23-Jul-02 10:31 extract_office_content/main.py
--rw-r--r--  2.0 unx      969 b- defN 23-Jul-02 10:31 extract_office_content/utils.py
--rw-r--r--  2.0 unx     5315 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      245 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1018 b- defN 23-Jul-02 10:31 extract_office_content-0.0.6.dist-info/RECORD
-11 files, 25499 bytes uncompressed, 8972 bytes compressed:  64.8%
+Zip file size: 10742 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      227 b- defN 23-Jul-16 14:19 extract_office_content/__init__.py
+-rw-r--r--  2.0 unx     4444 b- defN 23-Jul-16 14:19 extract_office_content/extract_excel.py
+-rw-r--r--  2.0 unx     4174 b- defN 23-Jul-16 14:19 extract_office_content/extract_ppt.py
+-rw-r--r--  2.0 unx     6717 b- defN 23-Jul-16 14:19 extract_office_content/extract_word.py
+-rw-r--r--  2.0 unx     2275 b- defN 23-Jul-16 14:19 extract_office_content/main.py
+-rw-r--r--  2.0 unx      969 b- defN 23-Jul-16 14:19 extract_office_content/utils.py
+-rw-r--r--  2.0 unx     5364 b- defN 23-Jul-16 14:19 extract_office_content-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 14:19 extract_office_content-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      245 b- defN 23-Jul-16 14:19 extract_office_content-0.0.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-Jul-16 14:19 extract_office_content-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1018 b- defN 23-Jul-16 14:19 extract_office_content-0.0.7.dist-info/RECORD
+11 files, 25548 bytes uncompressed, 8980 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: extract_office_content/main.py
 Comment: 
 
 Filename: extract_office_content/utils.py
 Comment: 
 
-Filename: extract_office_content-0.0.6.dist-info/METADATA
+Filename: extract_office_content-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: extract_office_content-0.0.6.dist-info/WHEEL
+Filename: extract_office_content-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: extract_office_content-0.0.6.dist-info/entry_points.txt
+Filename: extract_office_content-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: extract_office_content-0.0.6.dist-info/top_level.txt
+Filename: extract_office_content-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: extract_office_content-0.0.6.dist-info/RECORD
+Filename: extract_office_content-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `extract_office_content-0.0.6.dist-info/METADATA` & `extract_office_content-0.0.7.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: extract-office-content
-Version: 0.0.6
+Version: 0.0.7
 Summary: Tool for extracting content from office files.
 Home-page: https://github.com/SWHL/ExtractOfficeText.git
 Author: SWHL
 Author-email: liekkaskono@163.com
 License: Apache-2.0
 Keywords: extract,office,text,content
 Platform: Any
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6,<=3.11
+Requires-Python: >=3.6,<3.12
 Description-Content-Type: text/markdown
 Requires-Dist: lxml (>=4.9.1)
 Requires-Dist: openpyxl (>=3.1.2)
 Requires-Dist: pandas (>=1.3.5)
 Requires-Dist: pytest (>=7.1.2)
 Requires-Dist: python-docx (>=0.8.11)
 Requires-Dist: python-pptx (>=0.6.21)
```

### html2text {}

```diff
@@ -1,19 +1,20 @@
-Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.6 Summary: Tool
+Metadata-Version: 2.1 Name: extract-office-content Version: 0.0.7 Summary: Tool
 for extracting content from office files. Home-page: https://github.com/SWHL/
 ExtractOfficeText.git Author: SWHL Author-email: liekkaskono@163.com License:
 Apache-2.0 Keywords: extract,office,text,content Platform: Any Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Python: >=3.6,<=3.11 Description-Content-Type: text/
-markdown Requires-Dist: lxml (>=4.9.1) Requires-Dist: openpyxl (>=3.1.2)
-Requires-Dist: pandas (>=1.3.5) Requires-Dist: pytest (>=7.1.2) Requires-Dist:
-python-docx (>=0.8.11) Requires-Dist: python-pptx (>=0.6.21) Requires-Dist:
-tabulate Requires-Dist: filetype ## extract_office_content
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Python: >=3.6,<3.12 Description-Content-Type: text/markdown Requires-Dist: lxml
+(>=4.9.1) Requires-Dist: openpyxl (>=3.1.2) Requires-Dist: pandas (>=1.3.5)
+Requires-Dist: pytest (>=7.1.2) Requires-Dist: python-docx (>=0.8.11) Requires-
+Dist: python-pptx (>=0.6.21) Requires-Dist: tabulate Requires-Dist: filetype ##
+extract_office_content
 [https://img.shields.io/badge/Python->=3.7,<=3.10-aff.svg] [https://
 img.shields.io/badge/OS-Linux%2C%20Win%2C%20Mac-pink.svg] [PyPI] [https://
 static.pepy.tech/personalized-badge/
 extract_office_content?period=total&units=abbreviation&left_color=grey&right_color=blue&left_text=Downloads]
 ### Use 1. Install`extract_office_content` ```bash $ pip install
 extract_office_content ``` 2. Run by CLI. - Extract All office file's content.
 ```bash $ extract_office_content -h usage: extract_office_content [-h] [-
```

## Comparing `extract_office_content-0.0.6.dist-info/RECORD` & `extract_office_content-0.0.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 extract_office_content/__init__.py,sha256=Ge-pxaPmMXWiBzju-OCsdUwYXM8GLvY56qktBKTO3Xw,227
 extract_office_content/extract_excel.py,sha256=OpaS3EewiWwSJTrpwZVk9sVRgA8nMU51LnJjt3EI3kk,4444
 extract_office_content/extract_ppt.py,sha256=wmQzIgvCFK4N1fOhEv3LKzfZ86zqdp_KNMYUfYjxb2U,4174
 extract_office_content/extract_word.py,sha256=q_mNYLnfQNIT9LGvKhFU-iwn1HYjEhW2xe5Pl5hpdBE,6717
 extract_office_content/main.py,sha256=gcmeuhNQsZvNYfWOB-9nxxenQzkMyl_Wnr2UoyD8s3U,2275
 extract_office_content/utils.py,sha256=qPiuHyITVAScykQOrXEQz7U8W8OvwRdZhN-m5gyf7VU,969
-extract_office_content-0.0.6.dist-info/METADATA,sha256=qmYJjJ99ygwyjwpNUWsoiZZcjHQZ0OgcpDQC3y6J5F0,5315
-extract_office_content-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-extract_office_content-0.0.6.dist-info/entry_points.txt,sha256=JXiZmmPdeFuKjf78O0nnnTigzul8d99FV6YuamdcI6Y,245
-extract_office_content-0.0.6.dist-info/top_level.txt,sha256=quDoGD7DEfkl_J2tdoeRUbk5H4oKd5-dWIOLRaLB_mc,23
-extract_office_content-0.0.6.dist-info/RECORD,,
+extract_office_content-0.0.7.dist-info/METADATA,sha256=V3cQW-K27WQaOVAC3Bd-CSqdSpNHKon6MVcePAcm9bQ,5364
+extract_office_content-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+extract_office_content-0.0.7.dist-info/entry_points.txt,sha256=JXiZmmPdeFuKjf78O0nnnTigzul8d99FV6YuamdcI6Y,245
+extract_office_content-0.0.7.dist-info/top_level.txt,sha256=quDoGD7DEfkl_J2tdoeRUbk5H4oKd5-dWIOLRaLB_mc,23
+extract_office_content-0.0.7.dist-info/RECORD,,
```

