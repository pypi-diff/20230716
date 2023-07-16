# Comparing `tmp/nillip-1.31.tar.gz` & `tmp/nillip-1.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nillip-1.31.tar", last modified: Sun Jul 16 19:42:14 2023, max compression
+gzip compressed data, was "dist/nillip-1.36.tar", last modified: Sun Jul 16 20:02:40 2023, max compression
```

## Comparing `nillip-1.31.tar` & `nillip-1.36.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 19:42:14.000000 nillip-1.31/
--rw-r--r--   0 phil       (501) staff       (20)      463 2023-07-16 19:42:14.000000 nillip-1.31/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)        0 2023-07-14 00:42:39.000000 nillip-1.31/README.md
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 19:42:14.000000 nillip-1.31/nillip/
--rw-r--r--   0 phil       (501) staff       (20)       19 2023-07-15 01:09:26.000000 nillip-1.31/nillip/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)    40513 2023-07-16 19:38:48.000000 nillip-1.31/nillip/nil.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      463 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      229 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-14 05:14:31.000000 nillip-1.31/nillip.egg-info/not-zip-safe
--rw-r--r--   0 phil       (501) staff       (20)      134 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-07-16 19:42:14.000000 nillip-1.31/nillip.egg-info/top_level.txt
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-07-16 19:42:14.000000 nillip-1.31/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)     1646 2023-07-16 19:42:01.000000 nillip-1.31/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 20:02:40.000000 nillip-1.36/
+-rw-r--r--   0 phil       (501) staff       (20)      463 2023-07-16 20:02:40.000000 nillip-1.36/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-07-14 00:42:39.000000 nillip-1.36/README.md
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 20:02:40.000000 nillip-1.36/nillip/
+-rw-r--r--   0 phil       (501) staff       (20)       18 2023-07-16 19:56:54.000000 nillip-1.36/nillip/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)    40513 2023-07-16 19:38:48.000000 nillip-1.36/nillip/nil.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 20:02:40.000000 nillip-1.36/nillip/test/
+-rw-r--r--   0 phil       (501) staff       (20)        0 2023-07-16 19:53:18.000000 nillip-1.36/nillip/test/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)       50 2023-07-16 20:02:17.000000 nillip-1.36/nillip/test/test_1.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 20:02:40.000000 nillip-1.36/nillip.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      463 2023-07-16 20:02:40.000000 nillip-1.36/nillip.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      275 2023-07-16 20:02:40.000000 nillip-1.36/nillip.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-16 20:02:40.000000 nillip-1.36/nillip.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-14 05:14:31.000000 nillip-1.36/nillip.egg-info/not-zip-safe
+-rw-r--r--   0 phil       (501) staff       (20)      134 2023-07-16 20:02:40.000000 nillip-1.36/nillip.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-07-16 20:02:40.000000 nillip-1.36/nillip.egg-info/top_level.txt
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-07-16 20:02:40.000000 nillip-1.36/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)     1646 2023-07-16 20:02:35.000000 nillip-1.36/setup.py
```

### Comparing `nillip-1.31/nillip/nil.py` & `nillip-1.36/nillip/nil.py`

 * *Files identical despite different names*

### Comparing `nillip-1.31/setup.py` & `nillip-1.36/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
                'final_model/extra_LGBM_models']
 include_files = list(nil.lister_it(include_files, remove_string=remove_list))
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(name='nillip',
-      version='1.31',
+      version='1.36',
       author="Phillip Maire",
       license='MIT',
       description='custom utils package for me, but feel free to use it if you want',
       packages=find_packages(),
       author_email='phillip.maire@gmail.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
```

