# Comparing `tmp/bb_dirtree-0.4.0.tar.gz` & `tmp/bb_dirtree-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb_dirtree-0.4.0.tar", max compression
+gzip compressed data, was "bb_dirtree-0.4.1.tar", max compression
```

## Comparing `bb_dirtree-0.4.0.tar` & `bb_dirtree-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.4.0/LICENSE
--rw-r--r--   0        0        0     5582 2023-07-16 12:00:26.428041 bb_dirtree-0.4.0/README.md
--rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.4.0/bbdirtree/COLORS.py
--rw-r--r--   0        0        0      125 2023-07-16 10:04:23.941243 bb_dirtree-0.4.0/bbdirtree/__init__.py
--rw-r--r--   0        0        0    33551 2023-07-16 11:59:35.901374 bb_dirtree-0.4.0/bbdirtree/__main__.py
--rw-r--r--   0        0        0     2236 2023-07-16 08:24:42.264463 bb_dirtree-0.4.0/bbdirtree/unixvolumeinfo.py
--rw-r--r--   0        0        0     3528 2023-07-16 03:57:58.694161 bb_dirtree-0.4.0/bbdirtree/winvolumeinfo.py
--rw-r--r--   0        0        0      577 2023-07-16 10:04:26.731243 bb_dirtree-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 bb_dirtree-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-30 20:03:10.000000 bb_dirtree-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5655 2023-07-16 12:06:24.024715 bb_dirtree-0.4.1/README.md
+-rw-r--r--   0        0        0     3804 2022-08-14 02:50:32.000000 bb_dirtree-0.4.1/bbdirtree/COLORS.py
+-rw-r--r--   0        0        0      125 2023-07-16 12:06:36.014715 bb_dirtree-0.4.1/bbdirtree/__init__.py
+-rw-r--r--   0        0        0    33570 2023-07-16 12:07:12.428049 bb_dirtree-0.4.1/bbdirtree/__main__.py
+-rw-r--r--   0        0        0     2236 2023-07-16 08:24:42.264463 bb_dirtree-0.4.1/bbdirtree/unixvolumeinfo.py
+-rw-r--r--   0        0        0     3528 2023-07-16 03:57:58.694161 bb_dirtree-0.4.1/bbdirtree/winvolumeinfo.py
+-rw-r--r--   0        0        0      577 2023-07-16 12:06:30.058048 bb_dirtree-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6224 1970-01-01 00:00:00.000000 bb_dirtree-0.4.1/PKG-INFO
```

### Comparing `bb_dirtree-0.4.0/LICENSE` & `bb_dirtree-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.4.0/README.md` & `bb_dirtree-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -187,7 +187,11 @@
 - added winvolumeinfo module
 - added unixvolumeinfo module
 - added option to print version info
 - adjusted output for when base directory is a link
 - changed html colors to hex values and adjusted
 - changed tty colors to rgb values
 - changed some option arguments
+
+#### v0.4.1 - 7-16-2023
+
+- changed base directory to show absolute path
```

#### html2text {}

```diff
@@ -76,8 +76,9 @@
 colored recursive directory links red - moved formatting code to class
 instances #### v0.3.4 - 7-15-2023 - fixed hidden file detection in windows -
 added more title methods #### v0.4.0 - 7-16-2023 - updated bb_appdirs - changed
 some log messages - added more title methods - added a fancy title header -
 added winvolumeinfo module - added unixvolumeinfo module - added option to
 print version info - adjusted output for when base directory is a link -
 changed html colors to hex values and adjusted - changed tty colors to rgb
-values - changed some option arguments
+values - changed some option arguments #### v0.4.1 - 7-16-2023 - changed base
+directory to show absolute path
```

### Comparing `bb_dirtree-0.4.0/bbdirtree/COLORS.py` & `bb_dirtree-0.4.1/bbdirtree/COLORS.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.4.0/bbdirtree/__main__.py` & `bb_dirtree-0.4.1/bbdirtree/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         elif not isdir( directory ):
             try:
                 assert isdir( join( os.getcwd(), directory ))
                 directory = join( os.getcwd(), directory )
             except:
                 directory = os.getcwd()
 
-        self.base_dir      = directory
+        self.base_dir      = os.path.abspath( directory )
         self.depth         = depth
         self.dotfiles      = dotfiles
         self.ignore_errors = ignore_errors
         self.follow_links  = follow_links
         self.regex_ex      = regex_ex
         self.regex_in      = regex_in
         self.exclude_dirs  = exclude_dirs
```

### Comparing `bb_dirtree-0.4.0/bbdirtree/unixvolumeinfo.py` & `bb_dirtree-0.4.1/bbdirtree/unixvolumeinfo.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.4.0/bbdirtree/winvolumeinfo.py` & `bb_dirtree-0.4.1/bbdirtree/winvolumeinfo.py`

 * *Files identical despite different names*

### Comparing `bb_dirtree-0.4.0/pyproject.toml` & `bb_dirtree-0.4.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BB-DirTree"
-version = "0.4.0"
+version = "0.4.1"
 description = "Create a nice looking directory tree with options"
 authors = ["Erik Beebe <beebeapps_feedback@tuta.io>"]
 license = "MIT"
 packages = [ { include = 'bbdirtree' } ]
 readme = "README.md"
 
 keywords = [ "script", "qt", "files" ]
```

### Comparing `bb_dirtree-0.4.0/PKG-INFO` & `bb_dirtree-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-dirtree
-Version: 0.4.0
+Version: 0.4.1
 Summary: Create a nice looking directory tree with options
 License: MIT
 Keywords: script,qt,files
 Author: Erik Beebe
 Author-email: beebeapps_feedback@tuta.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -205,7 +205,11 @@
 - added unixvolumeinfo module
 - added option to print version info
 - adjusted output for when base directory is a link
 - changed html colors to hex values and adjusted
 - changed tty colors to rgb values
 - changed some option arguments
 
+#### v0.4.1 - 7-16-2023
+
+- changed base directory to show absolute path
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bb-dirtree Version: 0.4.0 Summary: Create a nice
+Metadata-Version: 2.1 Name: bb-dirtree Version: 0.4.1 Summary: Create a nice
 looking directory tree with options License: MIT Keywords: script,qt,files
 Author: Erik Beebe Author-email: beebeapps_feedback@tuta.io Requires-Python:
 >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: bb-
 apputils (>=0.4.0,<0.5.0) Requires-Dist: tabulate (>=0.8.9,<0.9.0) Description-
 Content-Type: text/markdown
@@ -84,8 +84,9 @@
 colored recursive directory links red - moved formatting code to class
 instances #### v0.3.4 - 7-15-2023 - fixed hidden file detection in windows -
 added more title methods #### v0.4.0 - 7-16-2023 - updated bb_appdirs - changed
 some log messages - added more title methods - added a fancy title header -
 added winvolumeinfo module - added unixvolumeinfo module - added option to
 print version info - adjusted output for when base directory is a link -
 changed html colors to hex values and adjusted - changed tty colors to rgb
-values - changed some option arguments
+values - changed some option arguments #### v0.4.1 - 7-16-2023 - changed base
+directory to show absolute path
```

