# Comparing `tmp/py40kie-0.1.0.tar.gz` & `tmp/py40kie-0.1.1.tar.gz`

## Comparing `py40kie-0.1.0.tar` & `py40kie-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 py40kie-0.1.0/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 py40kie-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py40kie-0.1.0/src/__init__.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 py40kie-0.1.0/src/py40kie.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py40kie-0.1.0/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 py40kie-0.1.0/LICENSE
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 py40kie-0.1.0/README.md
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 py40kie-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 py40kie-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 py40kie-0.1.1/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 py40kie-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py40kie-0.1.1/src/__init__.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 py40kie-0.1.1/src/py40kie.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 py40kie-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 py40kie-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 py40kie-0.1.1/README.md
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 py40kie-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 py40kie-0.1.1/PKG-INFO
```

### Comparing `py40kie-0.1.0/.github/workflows/publish-to-test-pypi.yml` & `py40kie-0.1.1/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.0/.github/workflows/python-publish.yml` & `py40kie-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.0/src/py40kie.py` & `py40kie-0.1.1/src/py40kie.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,56 +20,67 @@
                              '(army rules and wargear included automatically')
 
     # Optional arguments
     parser.add_argument('-o', dest='output_pdf', default="my army list", type=str,
                         help='file to save the extracted cards to - '
                              'can be in a folder (default: "%(default)s")')
 
+    parser.add_argument('-e', dest='enhancements', action='store_true',
+                        help='flag to extract enhancements')
+
+    parser.add_argument('-nw', dest='wargear', action='store_false',
+                        help='flag to not extract wargear')
+
     parser.add_argument('-a', '--army_rules_pages', default=[1, 2, 3, 4], type=int, nargs='+',
                         help='override army rule pages - use if the army rules are not on pages 1,2,3,4 '
                              '(default: 1 2 3 4)')
 
     parser.add_argument('-v', dest='override_pages', action='store_true',
                         help='flag to override functionality - only page numbers specified will be extracted')
     return parser.parse_args()
 
-def main(index_pdf, pages, output_file_name="my army list", army_rules_pages=[1, 2, 3, 4], override_pages=False):
+def main(index_pdf, pages, output_file_name="my army list", army_rules_pages=[1, 2, 3, 4], enhancements=False, wargear=True, override_pages=False):
     reader = PdfReader(index_pdf)
     reader_pages = []
     if override_pages:
         # only extract the specified page numbers
         for page in pages:
             if page.isdigit():
                 reader_pages.append(int(page) - 1)
     else:
         # extract the army rules pages
         for page in army_rules_pages:
             if not int(page) - 1 in reader_pages:
                 reader_pages.append(int(page) - 1)
+        if enhancements:
+            if not 4 in reader_pages:
+                reader_pages.append(4)
 
         for page in pages:
             if page.isdigit():
                 # extract the specified page numbers and following page (their wargear)
                 if not int(page) - 1 in reader_pages:
                     reader_pages.append(int(page) - 1)
-                if not int(page) in reader_pages:
-                    reader_pages.append(int(page))
+                if wargear:
+                    if not int(page) in reader_pages:
+                        reader_pages.append(int(page))
             else:
                 # extract the specified pages by unit title (must be exact match)
                 # not tested thoroughly so may miss some things
                 # additionally this functionality may break in future if pypdf changes or index.pdf is reformatted
                 # if it doesn't work - use page numbers
                 i = 0
                 for i in range(len(reader.pages)):
                     text = reader.pages[i].extract_text()
                     if text.split('\n')[0].lower() == page.lower():
                         if not i in reader_pages:
                             reader_pages.append(i)
-                        if not i + 1 in reader_pages:
-                            reader_pages.append(i + 1)
+                        if wargear:
+                            if not i + 1 in reader_pages:
+                                reader_pages.append(i + 1)
                         break
 
     writer = PdfWriter()
 
     for page in reader_pages:
         writer.add_page(reader.pages[page])
     
@@ -82,11 +93,13 @@
 
 def console_entry():
     args = parse_args()
     main(index_pdf=args.index_pdf,
          pages=args.pages,
          output_file_name=args.output_pdf,
          army_rules_pages=args.army_rules_pages,
+         enhancements=args.enhancements,
+         wargear=args.wargear,
          override_pages=args.override_pages)
 
 if __name__ == "__main__":
     console_entry()
```

### Comparing `py40kie-0.1.0/.gitignore` & `py40kie-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.0/LICENSE` & `py40kie-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.0/README.md` & `py40kie-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `py40kie-0.1.0/pyproject.toml` & `py40kie-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py40kie"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Chris Austin", email="dragons.ire.oce@gmail.com" },
 ]
 description = "Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size."
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `py40kie-0.1.0/PKG-INFO` & `py40kie-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py40kie
-Version: 0.1.0
+Version: 0.1.1
 Summary: Command line Python program to extract army rules and unit cards from 10th edition Warhammer 40k indexes to create army list specific pdfs with reduced file size.
 Project-URL: Homepage, https://github.com/Dragons-Ire/40k-index-pdf-extractor
 Project-URL: Bug Tracker, https://github.com/Dragons-Ire/40k-index-pdf-extractor/issues
 Author-email: Chris Austin <dragons.ire.oce@gmail.com>
 License-File: LICENSE
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

