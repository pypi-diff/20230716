# Comparing `tmp/indipydriver-0.0.7.tar.gz` & `tmp/indipydriver-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipydriver-0.0.7.tar", last modified: Fri Jul 14 22:05:16 2023, max compression
+gzip compressed data, was "indipydriver-1.0.0.tar", last modified: Sun Jul 16 14:57:36 2023, max compression
```

## Comparing `indipydriver-0.0.7.tar` & `indipydriver-1.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-0.0.7/LICENSE
--rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-0.0.7/README.md
--rw-r--r--   0        0        0      573 2023-07-14 21:34:04.000000 indipydriver-0.0.7/indipydriver/__init__.py
--rw-r--r--   0        0        0    17081 2023-07-09 09:46:38.000000 indipydriver-0.0.7/indipydriver/comms.py
--rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-0.0.7/indipydriver/events.py
--rw-r--r--   0        0        0    21510 2023-07-13 19:40:55.000000 indipydriver-0.0.7/indipydriver/ipydriver.py
--rw-r--r--   0        0        0    10816 2023-07-13 20:27:03.000000 indipydriver-0.0.7/indipydriver/ipyserver.py
--rw-r--r--   0        0        0    11759 2023-07-09 08:25:23.000000 indipydriver-0.0.7/indipydriver/propertymembers.py
--rw-r--r--   0        0        0    42713 2023-07-08 21:53:53.000000 indipydriver-0.0.7/indipydriver/propertyvectors.py
--rw-r--r--   0        0        0      814 2023-07-14 21:33:48.000000 indipydriver-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-04 20:13:36.000000 indipydriver-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2411 2023-07-11 05:27:01.000000 indipydriver-1.0.0/README.md
+-rw-r--r--   0        0        0      573 2023-07-16 14:51:11.000000 indipydriver-1.0.0/indipydriver/__init__.py
+-rw-r--r--   0        0        0    17081 2023-07-09 09:46:38.000000 indipydriver-1.0.0/indipydriver/comms.py
+-rw-r--r--   0        0        0    21067 2023-07-09 10:33:24.000000 indipydriver-1.0.0/indipydriver/events.py
+-rw-r--r--   0        0        0    21510 2023-07-13 19:40:55.000000 indipydriver-1.0.0/indipydriver/ipydriver.py
+-rw-r--r--   0        0        0    10816 2023-07-13 20:27:03.000000 indipydriver-1.0.0/indipydriver/ipyserver.py
+-rw-r--r--   0        0        0    11759 2023-07-09 08:25:23.000000 indipydriver-1.0.0/indipydriver/propertymembers.py
+-rw-r--r--   0        0        0    42713 2023-07-08 21:53:53.000000 indipydriver-1.0.0/indipydriver/propertyvectors.py
+-rw-r--r--   0        0        0      814 2023-07-16 14:50:33.000000 indipydriver-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3124 1970-01-01 00:00:00.000000 indipydriver-1.0.0/PKG-INFO
```

### Comparing `indipydriver-0.0.7/LICENSE` & `indipydriver-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.7/README.md` & `indipydriver-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.7/indipydriver/__init__.py` & `indipydriver-1.0.0/indipydriver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,8 +2,8 @@
 
 from .ipydriver import IPyDriver, Device
 from .propertyvectors import SwitchVector, LightVector, TextVector, BLOBVector, NumberVector
 from .propertymembers import SwitchMember, LightMember, TextMember, BLOBMember, NumberMember
 from .events import getProperties, enableBLOB, newSwitchVector, newTextVector, newNumberVector, newBLOBVector, Message, delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector, setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector
 from .ipyserver import IPyServer
 
-version = "0.0.7"
+version = "1.0.0"
```

### Comparing `indipydriver-0.0.7/indipydriver/comms.py` & `indipydriver-1.0.0/indipydriver/comms.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.7/indipydriver/events.py` & `indipydriver-1.0.0/indipydriver/events.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.7/indipydriver/ipydriver.py` & `indipydriver-1.0.0/indipydriver/ipydriver.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.7/indipydriver/ipyserver.py` & `indipydriver-1.0.0/indipydriver/ipyserver.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.7/indipydriver/propertymembers.py` & `indipydriver-1.0.0/indipydriver/propertymembers.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.7/indipydriver/propertyvectors.py` & `indipydriver-1.0.0/indipydriver/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipydriver-0.0.7/pyproject.toml` & `indipydriver-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipydriver"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.7"
+version = "1.0.0"
 description="Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'driver', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipydriver.readthedocs.io"
```

### Comparing `indipydriver-0.0.7/PKG-INFO` & `indipydriver-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipydriver
-Version: 0.0.7
+Version: 1.0.0
 Summary: Pure python package, with no dependencies, providing a set of classes which can be used to create an INDI driver.
 Keywords: indi,driver,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

