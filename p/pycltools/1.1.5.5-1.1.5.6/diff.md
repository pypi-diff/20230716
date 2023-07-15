# Comparing `tmp/pycltools-1.1.5.5.tar.gz` & `tmp/pycltools-1.1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycltools-1.1.5.5.tar", last modified: Tue Jul 11 15:33:56 2023, max compression
+gzip compressed data, was "pycltools-1.1.5.6.tar", last modified: Sat Jul 15 14:51:58 2023, max compression
```

## Comparing `pycltools-1.1.5.5.tar` & `pycltools-1.1.5.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:33:56.334192 pycltools-1.1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:33:56.330192 pycltools-1.1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:33:56.330192 pycltools-1.1.5.5/pycltools/
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/pycltools/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    46778 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/pycltools/pycltools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:33:56.330192 pycltools-1.1.5.5/pycltools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 15:33:56.000000 pycltools-1.1.5.5/pycltools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:33:56.334192 pycltools-1.1.5.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-11 15:33:44.000000 pycltools-1.1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:58.033962 pycltools-1.1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-15 14:51:47.000000 pycltools-1.1.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-15 14:51:58.033962 pycltools-1.1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-15 14:51:47.000000 pycltools-1.1.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:58.033962 pycltools-1.1.5.6/pycltools/
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-15 14:51:47.000000 pycltools-1.1.5.6/pycltools/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49270 2023-07-15 14:51:47.000000 pycltools-1.1.5.6/pycltools/pycltools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:51:58.033962 pycltools-1.1.5.6/pycltools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-15 14:51:57.000000 pycltools-1.1.5.6/pycltools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-15 14:51:57.000000 pycltools-1.1.5.6/pycltools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:51:57.000000 pycltools-1.1.5.6/pycltools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-15 14:51:57.000000 pycltools-1.1.5.6/pycltools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-15 14:51:57.000000 pycltools-1.1.5.6/pycltools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:51:58.033962 pycltools-1.1.5.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      130 2023-07-15 14:51:47.000000 pycltools-1.1.5.6/setup.py
```

### Comparing `pycltools-1.1.5.5/LICENSE` & `pycltools-1.1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.5/PKG-INFO` & `pycltools-1.1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.5
+Version: 1.1.5.6
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `pycltools-1.1.5.5/README.md` & `pycltools-1.1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `pycltools-1.1.5.5/pycltools/__init__.py` & `pycltools-1.1.5.6/pycltools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 # Define self package variable
-__version__ = "1.1.5.5"
+__version__ = "1.1.5.6"
 __all__ = ["pycltools"]
 __author__ = "Adrien Leger"
 __email__ = "adrien.leger@nanoporetech.com"
 __url__ = "https://github.com/a-slide/pycltools"
 __licence__ = "GPLv3"
 __classifiers__ = [
     "Development Status :: 3 - Alpha",
```

### Comparing `pycltools-1.1.5.5/pycltools/pycltools.py` & `pycltools-1.1.5.6/pycltools/pycltools.py`

 * *Files 4% similar despite different names*

```diff
@@ -340,14 +340,51 @@
     """
     try:
         os.remove(fp)
     except OSError as E:
         if exception_if_exist:
             raise E
 
+def super_iglob (pathname, recursive=False, regex_list=[]):
+    """ Same as iglob but pass multiple path regex instead of one. does not store anything in memory"""
+    if type(pathname) == str:
+        pathname = [pathname]
+
+    if type(pathname) in [list, tuple, set]:
+        for paths in pathname:
+            for path in iglob(pathname=paths, recursive=recursive):
+                if os.path.isdir(path) and regex_list:
+                    for regex in regex_list:
+                        regex_paths = os.path.join(path, regex)
+                        for regex_path in iglob(pathname=regex_paths, recursive=recursive):
+                            yield regex_path
+                elif os.path.isfile(path):
+                    yield path
+    else:
+        raise ValueError ("Invalid file type")
+
+def fastq_merge (src_dir, dest_fn, progress=True):
+    """
+    Concatenate a list of scr files in a single output file. Handle gziped files (mixed input and output)
+    """ 
+    if is_gziped(dest_fn):
+        open_fun_dest, open_mode_dest = gzip.open, "wt"
+    else:
+        open_fun_dest, open_mode_dest = open, "w"
+    
+    with open_fun_dest(dest_fn, open_mode_dest) as dest_fp, tqdm(desc="Files processed ", unit=" files", disable= not progress) as pb:
+        for src in super_iglob (src_dir, regex_list=["*.fastq","*.fq","*.fastq.gz","*.fq.gz"]):
+            if is_gziped(src):
+                open_fun_src, open_mode_src = gzip.open, "rt"
+            else:
+                open_fun_src, open_mode_src = open, "r"
+            with open_fun_src(src, open_mode_src) as src_fp:
+                shutil.copyfileobj(src_fp, dest_fp)
+                pb.update(1)
+
 # ~~~~~~~ FILE INFORMATION/PARSING ~~~~~~~#
 
 def linerange(fp, range_list=[], line_numbering=True, max_char_line=150, **kwargs):
     """
     Print a range of lines in a file according to a list of start end lists. Handle gziped files
     * fp
         Path to the file to be parsed
@@ -606,14 +643,32 @@
             lines += buf.count("\n")
             buf = read_f(buf_size)
 
     return lines
 
 # ~~~~~~~ DIRECTORY MANIPULATION ~~~~~~~#
 
+def super_iglob (pathname, recursive=False, regex_list=[]):
+    """ Same as iglob but pass multiple path regex instead of one. does not store anything in memory"""
+    if type(pathname) == str:
+        pathname = [pathname]
+
+    if type(pathname) in [list, tuple, set]:
+        for paths in pathname:
+            for path in iglob(pathname=paths, recursive=recursive):
+                if os.path.isdir(path) and regex_list:
+                    for regex in regex_list:
+                        regex_paths = os.path.join(path, regex)
+                        for regex_path in iglob(pathname=regex_paths, recursive=recursive):
+                            yield regex_path
+                elif os.path.isfile(path):
+                    yield path
+    else:
+        raise ValueError ("Invalid file type")
+
 def mkdir(
     fp,
     error_if_existing=False,
     delete_existing=False,
     verbose=False,
     **kwargs,
 ):
@@ -1521,8 +1576,9 @@
                 if self.verbose:
                     print(f"Seed {seed} already known. Incrementing")
                 while seed in self.previous_seeds:
                     seed += 1
             self.previous_seeds.add(seed)
 
         random.seed(seed)
-        self.seed = seed
+        self.seed = seed
+        return self.seed
```

### Comparing `pycltools-1.1.5.5/pycltools.egg-info/PKG-INFO` & `pycltools-1.1.5.6/pycltools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycltools
-Version: 1.1.5.5
+Version: 1.1.5.6
 Summary: pycltools is a package written in python3 containing a collection of generic functions and classes for file parsing, manipulation...
 Home-page: https://github.com/a-slide/pycltools
 Author: Adrien Leger
 Author-email: adrien.leger@nanoporetech.com
 License: GPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

