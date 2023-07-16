# Comparing `tmp/volvopy-0.1.7.tar.gz` & `tmp/volvopy-0.1.8.tar.gz`

## Comparing `volvopy-0.1.7.tar` & `volvopy-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rwxr-xr-x   0        0        0      214 2020-02-02 00:00:00.000000 volvopy-0.1.7/.editorconfig
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 volvopy-0.1.7/BUILDING.md
--rwxr-xr-x   0        0        0     2157 2020-02-02 00:00:00.000000 volvopy-0.1.7/mkbld
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 volvopy-0.1.7/requirements.txt
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 volvopy-0.1.7/tox.ini
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 volvopy-0.1.7/.github/dependabot.yml
--rwxr-xr-x   0        0        0     1867 2020-02-02 00:00:00.000000 volvopy-0.1.7/examples/demo.py
--rwxr-xr-x   0        0        0    18668 2020-02-02 00:00:00.000000 volvopy-0.1.7/examples/omed.py
--rwxr-xr-x   0        0        0     1800 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/__constants__.py
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/connected.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/energy.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/extended.py
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/location.py
--rw-r--r--   0        0        0   377649 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/specification/connected-vehicle-c3-specification.v1.json
--rw-r--r--   0        0        0    56534 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/specification/energy-api-specification.v1.json
--rw-r--r--   0        0        0    23483 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/specification/extended-vehicle-c3-specification.v1.json
--rw-r--r--   0        0        0    11391 2020-02-02 00:00:00.000000 volvopy-0.1.7/src/volvopy/specification/location-specification.v1.json
--rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 volvopy-0.1.7/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 volvopy-0.1.7/LICENSE
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 volvopy-0.1.7/README.md
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 volvopy-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 volvopy-0.1.7/PKG-INFO
+-rwxr-xr-x   0        0        0      214 2020-02-02 00:00:00.000000 volvopy-0.1.8/.editorconfig
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 volvopy-0.1.8/BUILDING.md
+-rwxr-xr-x   0        0        0     2157 2020-02-02 00:00:00.000000 volvopy-0.1.8/mkbld
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 volvopy-0.1.8/requirements.txt
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 volvopy-0.1.8/tox.ini
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 volvopy-0.1.8/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     1867 2020-02-02 00:00:00.000000 volvopy-0.1.8/examples/demo.py
+-rwxr-xr-x   0        0        0    18668 2020-02-02 00:00:00.000000 volvopy-0.1.8/examples/omed.py
+-rwxr-xr-x   0        0        0     1800 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/__constants__.py
+-rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/__init__.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/connected.py
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/energy.py
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/extended.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/location.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/volvo_api.py
+-rw-r--r--   0        0        0   377649 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/specification/connected-vehicle-c3-specification.v1.json
+-rw-r--r--   0        0        0    56534 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/specification/energy-api-specification.v1.json
+-rw-r--r--   0        0        0    23483 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/specification/extended-vehicle-c3-specification.v1.json
+-rw-r--r--   0        0        0    11391 2020-02-02 00:00:00.000000 volvopy-0.1.8/src/volvopy/specification/location-specification.v1.json
+-rwxr-xr-x   0        0        0     1906 2020-02-02 00:00:00.000000 volvopy-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 volvopy-0.1.8/LICENSE
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 volvopy-0.1.8/README.md
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 volvopy-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 volvopy-0.1.8/PKG-INFO
```

### Comparing `volvopy-0.1.7/BUILDING.md` & `volvopy-0.1.8/BUILDING.md`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/mkbld` & `volvopy-0.1.8/mkbld`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/tox.ini` & `volvopy-0.1.8/tox.ini`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/examples/demo.py` & `volvopy-0.1.8/examples/demo.py`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/examples/omed.py` & `volvopy-0.1.8/examples/omed.py`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/src/volvopy/__constants__.py` & `volvopy-0.1.8/src/volvopy/__constants__.py`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/src/volvopy/location.py` & `volvopy-0.1.8/src/volvopy/location.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 #!/usr/bin/env python3
 
 import __constants__ as vc
+from volvo_api import VolvoAPI
 import os
-import syslog
 
 import mausy5043_common.funfile as mf
 DEBUG = False
 HERE = os.path.realpath(__file__).split("/")
-# runlist id :
 MYID = HERE[-1]
 
 
-class Location():
+class Location(VolvoAPI):
     """Class to connect and interact with the Volvo Location API.
 
     ref.: https://developer.volvocars.com/apis/location/v1/specification/
     """
-    def __init__(self):
-        self.api_primary_key = vc.API_KEY[0]
-        self.api_secondary_key = vc.API_KEY[1]
-        self.api_token = vc.API_TOKEN
-        self.vin = vc.API_VIN
-        vin = self.vin  # noqa
+    def __init__(self, debug=False):
+        super().__init__(debug=debug)
+
         api = 'location'
         self.base_url = f"{vc.API_SPECIFICATIONS[api]['servers'][0]['url']}"
-        self.call_urls = []
+        vin = self.vin  # noqa
         for path in vc.API_SPECIFICATIONS[api]['paths']:
             url_path = eval(f"f'{path}'")
             self.call_urls.append(f"{self.base_url}{url_path}")
         print(f"Number of URLs: {len(self.call_urls)}")
         for item in self.call_urls:
             mf.syslog_trace(item, False, DEBUG)
 
 
 if __name__ == "__main__":
     DEBUG = True
-    a = Location()
+    a = Location(debug=DEBUG)
+    a.get()
```

### Comparing `volvopy-0.1.7/src/volvopy/specification/connected-vehicle-c3-specification.v1.json` & `volvopy-0.1.8/src/volvopy/specification/connected-vehicle-c3-specification.v1.json`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/src/volvopy/specification/energy-api-specification.v1.json` & `volvopy-0.1.8/src/volvopy/specification/energy-api-specification.v1.json`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/src/volvopy/specification/extended-vehicle-c3-specification.v1.json` & `volvopy-0.1.8/src/volvopy/specification/extended-vehicle-c3-specification.v1.json`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/src/volvopy/specification/location-specification.v1.json` & `volvopy-0.1.8/src/volvopy/specification/location-specification.v1.json`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/.gitignore` & `volvopy-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/LICENSE` & `volvopy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/README.md` & `volvopy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `volvopy-0.1.7/pyproject.toml` & `volvopy-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "volvopy"
 description = "Connect to the Volvo API using Python."
 # version = "0.1.1"  # latest/current distribution version
-version = "0.1.7"  # latest test version
+version = "0.1.8"  # latest test version
 dependencies = []
 license = "MIT"
 authors = [
   { name="Mausy5043" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `volvopy-0.1.7/PKG-INFO` & `volvopy-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volvopy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Connect to the Volvo API using Python.
 Project-URL: Homepage, https://github.com/Mausy5043/volvopy
 Project-URL: Bug Tracker, https://github.com/Mausy5043/volvopy/issues
 Author: Mausy5043
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
```

