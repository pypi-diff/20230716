# Comparing `tmp/symlib-1.3.7.tar.gz` & `tmp/symlib-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.7.tar", last modified: Tue Jun 27 17:16:38 2023, max compression
+gzip compressed data, was "symlib-1.3.8.tar", last modified: Sun Jul 16 21:24:19 2023, max compression
```

## Comparing `symlib-1.3.7.tar` & `symlib-1.3.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-27 17:16:38.680738 symlib-1.3.7/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.7/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-27 17:16:38.680622 symlib-1.3.7/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.7/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.7/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-06-27 17:16:38.680773 symlib-1.3.7/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-06-27 17:16:32.000000 symlib-1.3.7/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-27 17:16:38.679675 symlib-1.3.7/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.7/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.7/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    53792 2023-06-23 23:11:21.000000 symlib-1.3.7/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.7/symlib/match.py
--rw-r--r--   0 phil       (501) staff       (20)    36177 2023-06-27 17:16:14.000000 symlib-1.3.7/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     9876 2023-06-14 22:30:07.000000 symlib-1.3.7/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-06-27 17:16:38.680472 symlib-1.3.7/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      303 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-06-27 17:16:38.000000 symlib-1.3.7/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 21:24:19.007568 symlib-1.3.8/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.8/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-07-16 21:24:19.007409 symlib-1.3.8/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.8/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.8/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-07-16 21:24:19.007626 symlib-1.3.8/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-07-16 21:07:47.000000 symlib-1.3.8/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 21:24:19.006618 symlib-1.3.8/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.8/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.8/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    53792 2023-07-15 01:24:54.000000 symlib-1.3.8/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.8/symlib/match.py
+-rw-r--r--   0 phil       (501) staff       (20)    36177 2023-06-27 17:16:14.000000 symlib-1.3.8/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     9979 2023-07-15 01:24:54.000000 symlib-1.3.8/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 21:24:19.007215 symlib-1.3.8/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      303 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.7/LICENSE` & `symlib-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.7/PKG-INFO` & `symlib-1.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.7
+Version: 1.3.8
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.7/setup.py` & `symlib-1.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.7"
+version = "1.3.8"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.7/symlib/__init__.py` & `symlib-1.3.8/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.7/symlib/file_management.py` & `symlib-1.3.8/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.7/symlib/lib.py` & `symlib-1.3.8/symlib/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -800,15 +800,15 @@
 
 def read_tree(dir_name, var_names):
     """ read_tree reads variables from the halo directory halo_dir in
     depth-first order. var_names is a list of variables to be read (see
     TREE_COL_NAMES). A list of arrays is returned. Use the branches and merger
     files to identify main branches and important haloes, respectively.
     """
-    tree_files = sorted(glob.glob(path.join(dir_name, "halos", "tree_*.dat")))
+    tree_files = sorted(glob.glob(path.join(dir_name, "trees", "tree_*.dat")))
     tree_files = [fname for fname in tree_files if
                   path.basename(fname) != "tree_header.dat"]
 
     out = []
     for i in range(len(var_names)):
         var = []
         for j in range(len(tree_files)):
```

### Comparing `symlib-1.3.7/symlib/match.py` & `symlib-1.3.8/symlib/match.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.7/symlib/star_tagging.py` & `symlib-1.3.8/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.7/symlib/util.py` & `symlib-1.3.8/symlib/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,11 +191,11 @@
     """
     
     if len(suite_name) > 2 and suite_name[-2:] == "LR":
         suite_dir = suite_name[:-2]
     else:
         suite_dir = suite_name
 
-    if isinstance(halo_name, int):
+    if isinstance(halo_name, int) or isinstance(halo_name, np.int) or isinstance(halo_name, np.int64) or isinstance(halo_name, np.int32):
         halo_name = DEFAULT_HALO_NAMES[suite_name][halo_name]
 
     return path.join(base_dir, suite_dir, halo_name)
```

### Comparing `symlib-1.3.7/symlib.egg-info/PKG-INFO` & `symlib-1.3.8/symlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.7
+Version: 1.3.8
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

