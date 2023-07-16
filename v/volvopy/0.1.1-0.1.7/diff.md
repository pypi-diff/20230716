# Comparing `tmp/volvopy-0.1.1.tar.gz` & `tmp/volvopy-0.1.7.tar.gz`

## Comparing `volvopy-0.1.1.tar` & `volvopy-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,23 @@
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 volvopy-0.1.1/BUILDING.md
--rwxr-xr-x   0        0        0     2157 2020-02-02 00:00:00.000000 volvopy-0.1.1/mkbld
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 volvopy-0.1.1/tox.ini
--rw-r--r--   0        0        0    18390 2020-02-02 00:00:00.000000 volvopy-0.1.1/docs/energy-api-specification.json
--rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 volvopy-0.1.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 volvopy-0.1.1/LICENSE
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 volvopy-0.1.1/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 volvopy-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 volvopy-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0      214 2020-02-02 00:00:00.000000 volvopy-0.1.7/.editorconfig
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 volvopy-0.1.7/BUILDING.md
+-rwxr-xr-x   0        0        0     2157 2020-02-02 00:00:00.000000 volvopy-0.1.7/mkbld
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 volvopy-0.1.7/requirements.txt
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 volvopy-0.1.7/tox.ini
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 volvopy-0.1.7/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     1867 2020-02-02 00:00:00.000000 volvopy-0.1.7/examples/demo.py
+-rwxr-xr-x   0        0        0    18668 2020-02-02 00:00:00.000000 volvopy-0.1.7/examples/omed.py
+-rwxr-xr-x   0        0        0     1800 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/__constants__.py
+-rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/connected.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/energy.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/extended.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/location.py
+-rw-r--r--   0        0        0   377649 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/specification/connected-vehicle-c3-specification.v1.json
+-rw-r--r--   0        0        0    56534 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/specification/energy-api-specification.v1.json
+-rw-r--r--   0        0        0    23483 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/specification/extended-vehicle-c3-specification.v1.json
+-rw-r--r--   0        0        0    11391 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/specification/location-specification.v1.json
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 volvopy-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 volvopy-0.1.7/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 volvopy-0.1.7/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 volvopy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 volvopy-0.1.7/PKG-INFO
```

### Comparing `volvopy-0.1.1/BUILDING.md` & `volvopy-0.1.7/BUILDING.md`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.1/mkbld` & `volvopy-0.1.7/mkbld`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.1/tox.ini` & `volvopy-0.1.7/tox.ini`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.1/.gitignore` & `volvopy-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.1/LICENSE` & `volvopy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.1/pyproject.toml` & `volvopy-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "volvopy"
 description = "Connect to the Volvo API using Python."
 # version = "0.1.1"  # latest/current distribution version
-version = "0.1.1"  # latest test version
+version = "0.1.7"  # latest test version
 dependencies = []
 license = "MIT"
 authors = [
   { name="Mausy5043" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
```

