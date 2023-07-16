# Comparing `tmp/py_astrolab-0.2.2.tar.gz` & `tmp/py_astrolab-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.2.2.tar", max compression
+gzip compressed data, was "py_astrolab-0.2.3.tar", max compression
```

## Comparing `py_astrolab-0.2.2.tar` & `py_astrolab-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.2.2/README.md
--rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.2.2/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    16866 2023-07-12 12:53:57.224268 py_astrolab-0.2.2/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.2.2/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    76214 2023-07-16 14:04:16.679953 py_astrolab-0.2.2/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.2.2/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.2.2/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    63098 2023-07-16 14:01:21.996365 py_astrolab-0.2.2/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.2.2/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.2.2/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.2.2/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    26385 2023-06-21 20:10:47.767169 py_astrolab-0.2.2/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.2.2/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.2.2/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.2.2/py_astrolab/report.py
--rwxr-xr-x   0        0        0     5074 2023-07-12 12:49:41.885152 py_astrolab-0.2.2/py_astrolab/types.py
--rwxr-xr-x   0        0        0     7171 2023-07-12 13:18:34.934445 py_astrolab-0.2.2/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      689 2023-07-16 14:05:22.476649 py_astrolab-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.2.3/README.md
+-rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.2.3/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    16866 2023-07-12 12:53:57.224268 py_astrolab-0.2.3/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.2.3/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    76214 2023-07-16 14:04:16.679953 py_astrolab-0.2.3/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.2.3/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.2.3/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    63098 2023-07-16 14:01:21.996365 py_astrolab-0.2.3/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.2.3/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.2.3/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.2.3/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    26831 2023-07-16 14:53:31.922402 py_astrolab-0.2.3/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.2.3/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.2.3/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.2.3/py_astrolab/report.py
+-rwxr-xr-x   0        0        0     5074 2023-07-12 12:49:41.885152 py_astrolab-0.2.3/py_astrolab/types.py
+-rwxr-xr-x   0        0        0     7171 2023-07-12 13:18:34.934445 py_astrolab-0.2.3/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      689 2023-07-16 14:54:48.137518 py_astrolab-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.2.3/PKG-INFO
```

### Comparing `py_astrolab-0.2.2/py_astrolab/__init__.py` & `py_astrolab-0.2.3/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/aspects.py` & `py_astrolab-0.2.3/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.2.3/py_astrolab/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.2.3/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.2.3/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.2.3/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.2.3/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/fetch_geonames.py` & `py_astrolab-0.2.3/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/kr.config.json` & `py_astrolab-0.2.3/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/main.py` & `py_astrolab-0.2.3/py_astrolab/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -528,14 +528,26 @@
         )
         self.mean_node = for_every_planet(
             self.mean_node, self.planets_degrees[10]
         )
         self.true_node = for_every_planet(
             self.true_node, self.planets_degrees[11]
         )
+        self.ascendant = for_every_planet(
+            self.ascendant, self.ascendant['abs_pos']
+        )
+        self.midheaven = for_every_planet(
+            self.midheaven, self.midheaven['abs_pos']
+        )
+        self.descendant = for_every_planet(
+            self.descendant, self.descendant['abs_pos']
+        )
+        self.imum_coeli = for_every_planet(
+            self.imum_coeli, self.imum_coeli['abs_pos']
+        )
 
         planets_list = [
             self.sun,
             self.moon,
             self.mercury,
             self.venus,
             self.mars,
```

### Comparing `py_astrolab-0.2.2/py_astrolab/print_all_data.py` & `py_astrolab-0.2.3/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/relationship_score.py` & `py_astrolab-0.2.3/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/report.py` & `py_astrolab-0.2.3/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/types.py` & `py_astrolab-0.2.3/py_astrolab/types.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/py_astrolab/utilities.py` & `py_astrolab-0.2.3/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.2/pyproject.toml` & `py_astrolab-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.2.2"
+version = "0.2.3"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.2.2/PKG-INFO` & `py_astrolab-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

