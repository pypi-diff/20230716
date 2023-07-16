# Comparing `tmp/crateman-1.0.1.tar.gz` & `tmp/crateman-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crateman-1.0.1.tar", last modified: Sat Jul 15 19:30:53 2023, max compression
+gzip compressed data, was "crateman-1.0.2.tar", last modified: Sun Jul 16 09:13:02 2023, max compression
```

## Comparing `crateman-1.0.1.tar` & `crateman-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lch361    (1000) lch361    (1000)        0 2023-07-15 19:30:53.373479 crateman-1.0.1/
--rw-r--r--   0 lch361    (1000) lch361    (1000)     2167 2023-07-15 19:30:53.373479 crateman-1.0.1/PKG-INFO
--rw-r--r--   0 lch361    (1000) lch361    (1000)     1653 2023-07-15 13:07:46.000000 crateman-1.0.1/README.md
-drwxr-xr-x   0 lch361    (1000) lch361    (1000)        0 2023-07-15 19:30:53.373479 crateman-1.0.1/crateman/
--rw-r--r--   0 lch361    (1000) lch361    (1000)      622 2023-07-12 21:11:13.000000 crateman-1.0.1/crateman/__init__.py
--rw-r--r--   0 lch361    (1000) lch361    (1000)     3925 2023-07-15 18:34:11.000000 crateman-1.0.1/crateman/cli.py
--rw-r--r--   0 lch361    (1000) lch361    (1000)    13503 2023-07-15 10:35:55.000000 crateman-1.0.1/crateman/config.py
--rw-r--r--   0 lch361    (1000) lch361    (1000)     8620 2023-07-15 18:31:16.000000 crateman-1.0.1/crateman/crate.py
--rw-r--r--   0 lch361    (1000) lch361    (1000)      502 2023-07-13 12:11:24.000000 crateman-1.0.1/crateman/exception.py
--rw-r--r--   0 lch361    (1000) lch361    (1000)     2185 2023-07-15 08:30:50.000000 crateman-1.0.1/crateman/log.py
--rw-r--r--   0 lch361    (1000) lch361    (1000)    10772 2023-07-15 17:14:11.000000 crateman-1.0.1/crateman/resolver.py
-drwxr-xr-x   0 lch361    (1000) lch361    (1000)        0 2023-07-15 19:30:53.373479 crateman-1.0.1/crateman.egg-info/
--rw-r--r--   0 lch361    (1000) lch361    (1000)     2167 2023-07-15 19:30:53.000000 crateman-1.0.1/crateman.egg-info/PKG-INFO
--rw-r--r--   0 lch361    (1000) lch361    (1000)      351 2023-07-15 19:30:53.000000 crateman-1.0.1/crateman.egg-info/SOURCES.txt
--rw-r--r--   0 lch361    (1000) lch361    (1000)        1 2023-07-15 19:30:53.000000 crateman-1.0.1/crateman.egg-info/dependency_links.txt
--rw-r--r--   0 lch361    (1000) lch361    (1000)       57 2023-07-15 19:30:53.000000 crateman-1.0.1/crateman.egg-info/entry_points.txt
--rw-r--r--   0 lch361    (1000) lch361    (1000)        5 2023-07-15 19:30:53.000000 crateman-1.0.1/crateman.egg-info/requires.txt
--rw-r--r--   0 lch361    (1000) lch361    (1000)        9 2023-07-15 19:30:53.000000 crateman-1.0.1/crateman.egg-info/top_level.txt
--rw-r--r--   0 lch361    (1000) lch361    (1000)      749 2023-07-15 19:30:37.000000 crateman-1.0.1/pyproject.toml
--rw-r--r--   0 lch361    (1000) lch361    (1000)       38 2023-07-15 19:30:53.373479 crateman-1.0.1/setup.cfg
+drwxr-xr-x   0 lch361    (1000) lch361    (1000)        0 2023-07-16 09:13:02.208130 crateman-1.0.2/
+-rw-r--r--   0 lch361    (1000) lch361    (1000)     2225 2023-07-16 09:13:02.208130 crateman-1.0.2/PKG-INFO
+-rw-r--r--   0 lch361    (1000) lch361    (1000)     1653 2023-07-15 13:07:46.000000 crateman-1.0.2/README.md
+drwxr-xr-x   0 lch361    (1000) lch361    (1000)        0 2023-07-16 09:13:02.208130 crateman-1.0.2/crateman/
+-rw-r--r--   0 lch361    (1000) lch361    (1000)      622 2023-07-12 21:11:13.000000 crateman-1.0.2/crateman/__init__.py
+-rw-r--r--   0 lch361    (1000) lch361    (1000)     3955 2023-07-15 22:34:47.000000 crateman-1.0.2/crateman/cli.py
+-rw-r--r--   0 lch361    (1000) lch361    (1000)    13503 2023-07-15 10:35:55.000000 crateman-1.0.2/crateman/config.py
+-rw-r--r--   0 lch361    (1000) lch361    (1000)     8620 2023-07-15 18:31:16.000000 crateman-1.0.2/crateman/crate.py
+-rw-r--r--   0 lch361    (1000) lch361    (1000)      502 2023-07-13 12:11:24.000000 crateman-1.0.2/crateman/exception.py
+-rw-r--r--   0 lch361    (1000) lch361    (1000)     2185 2023-07-15 08:30:50.000000 crateman-1.0.2/crateman/log.py
+-rw-r--r--   0 lch361    (1000) lch361    (1000)    10815 2023-07-16 08:41:24.000000 crateman-1.0.2/crateman/resolver.py
+drwxr-xr-x   0 lch361    (1000) lch361    (1000)        0 2023-07-16 09:13:02.208130 crateman-1.0.2/crateman.egg-info/
+-rw-r--r--   0 lch361    (1000) lch361    (1000)     2225 2023-07-16 09:13:02.000000 crateman-1.0.2/crateman.egg-info/PKG-INFO
+-rw-r--r--   0 lch361    (1000) lch361    (1000)      351 2023-07-16 09:13:02.000000 crateman-1.0.2/crateman.egg-info/SOURCES.txt
+-rw-r--r--   0 lch361    (1000) lch361    (1000)        1 2023-07-16 09:13:02.000000 crateman-1.0.2/crateman.egg-info/dependency_links.txt
+-rw-r--r--   0 lch361    (1000) lch361    (1000)       57 2023-07-16 09:13:02.000000 crateman-1.0.2/crateman.egg-info/entry_points.txt
+-rw-r--r--   0 lch361    (1000) lch361    (1000)        5 2023-07-16 09:13:02.000000 crateman-1.0.2/crateman.egg-info/requires.txt
+-rw-r--r--   0 lch361    (1000) lch361    (1000)        9 2023-07-16 09:13:02.000000 crateman-1.0.2/crateman.egg-info/top_level.txt
+-rw-r--r--   0 lch361    (1000) lch361    (1000)      815 2023-07-16 09:12:35.000000 crateman-1.0.2/pyproject.toml
+-rw-r--r--   0 lch361    (1000) lch361    (1000)       38 2023-07-16 09:13:02.208130 crateman-1.0.2/setup.cfg
```

### Comparing `crateman-1.0.1/PKG-INFO` & `crateman-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: crateman
-Version: 1.0.1
+Version: 1.0.2
 Summary: Build system focused on resolving and building dependencies.
 Author-email: lch361 <surperior64@gmail.com>
 License: GPL-3.0
+Project-URL: Homepage, https://gitlab.com/lch361/crateman
 Keywords: build,system,dependency,package,manager,development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `crateman-1.0.1/README.md` & `crateman-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `crateman-1.0.1/crateman/__init__.py` & `crateman-1.0.2/crateman/__init__.py`

 * *Files identical despite different names*

### Comparing `crateman-1.0.1/crateman/cli.py` & `crateman-1.0.2/crateman/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         if self.colors is not None:
             if self.colors:
                 log.colors_enable()
             else:
                 log.colors_disable()
 
         if self.deps_only:
+            global BUILD_FUNC
             BUILD_FUNC = Crate.build_deps
 
         if self.help:
             log.info(Args.USAGE_MSG)
             return False
 
         return True
```

### Comparing `crateman-1.0.1/crateman/config.py` & `crateman-1.0.2/crateman/config.py`

 * *Files identical despite different names*

### Comparing `crateman-1.0.1/crateman/crate.py` & `crateman-1.0.2/crateman/crate.py`

 * *Files identical despite different names*

### Comparing `crateman-1.0.1/crateman/log.py` & `crateman-1.0.2/crateman/log.py`

 * *Files identical despite different names*

### Comparing `crateman-1.0.1/crateman/resolver.py` & `crateman-1.0.2/crateman/resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,16 @@
         crate_info = self.crate_infos.get(crate_name)
         if crate_info is None or crate_info.state < State.PROCESSED:
             raise InvalidCrateExtract(crate_name)
 
         crate = Crate(crate_name, crate_info.version,
                       crate_info.build_cmd, crate_info.path)
         crate.env = {i: ' '.join(v) for i, v in crate_info.env.items()}
-        crate.env['PROFILE'] = self.profile
+        if 'PROFILE' not in crate.env:
+            crate.env['PROFILE'] = self.profile
 
         cache[crate_name] = crate
         for i in crate_info.deps:
             version_req = crate_info.required_versions.get(i)
             if version_req is None:
                 version_req = RE_EVERY_VERSION
```

### Comparing `crateman-1.0.1/crateman.egg-info/PKG-INFO` & `crateman-1.0.2/crateman.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.1
 Name: crateman
-Version: 1.0.1
+Version: 1.0.2
 Summary: Build system focused on resolving and building dependencies.
 Author-email: lch361 <surperior64@gmail.com>
 License: GPL-3.0
+Project-URL: Homepage, https://gitlab.com/lch361/crateman
 Keywords: build,system,dependency,package,manager,development
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Utilities
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `crateman-1.0.1/pyproject.toml` & `crateman-1.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "crateman"
-version = "1.0.1"
+version = "1.0.2"
 description = "Build system focused on resolving and building dependencies."
 license = {text = "GPL-3.0"}
 authors = [
     {name = "lch361", email = "surperior64@gmail.com"}
 ]
 dependencies = ["toml"]
 readme = "README.md"
@@ -17,12 +17,15 @@
     "Topic :: Software Development :: Build Tools",
     "Topic :: Utilities",
     "Operating System :: POSIX :: Linux",
 	"Programming Language :: Python :: 3",
     "Intended Audience :: Developers"
 ]
 
+[project.urls]
+"Homepage" = "https://gitlab.com/lch361/crateman"
+
 [project.scripts]
 crateman = "crateman.cli:crateman_entry"
 
 [tool.setuptools]
 packages = ["crateman"]
```

