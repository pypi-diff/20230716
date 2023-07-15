# Comparing `tmp/gungnir-0.2.0.tar.gz` & `tmp/gungnir-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gungnir-0.2.0.tar", last modified: Wed Jun 21 18:44:40 2023, max compression
+gzip compressed data, was "gungnir-0.2.1.tar", last modified: Sat Jul 15 22:21:28 2023, max compression
```

## Comparing `gungnir-0.2.0.tar` & `gungnir-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,19 @@
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-06-21 18:44:40.682538 gungnir-0.2.0/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     1078 2023-06-08 18:54:16.000000 gungnir-0.2.0/LICENSE
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     3032 2023-06-21 18:44:40.682538 gungnir-0.2.0/PKG-INFO
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     2341 2023-06-17 19:09:42.000000 gungnir-0.2.0/README.md
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-06-21 18:44:40.682538 gungnir-0.2.0/gungnir/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      737 2023-06-21 18:42:16.000000 gungnir-0.2.0/gungnir/__init__.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     2343 2023-06-21 18:35:28.000000 gungnir-0.2.0/gungnir/__main__.py
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-06-21 18:44:40.682538 gungnir-0.2.0/gungnir/dependencytrack/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)        0 2023-06-20 16:44:34.000000 gungnir-0.2.0/gungnir/dependencytrack/__init__.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     1448 2023-06-20 18:45:24.000000 gungnir-0.2.0/gungnir/dependencytrack/api.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     3642 2023-06-20 19:10:39.000000 gungnir-0.2.0/gungnir/dependencytrack/project.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     3367 2023-06-21 18:24:55.000000 gungnir-0.2.0/gungnir/gungnir.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      921 2023-06-21 18:29:40.000000 gungnir-0.2.0/gungnir/project.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     1696 2023-06-09 00:37:58.000000 gungnir-0.2.0/gungnir/syft.py
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-06-21 18:44:40.682538 gungnir-0.2.0/gungnir.egg-info/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)     3032 2023-06-21 18:44:40.000000 gungnir-0.2.0/gungnir.egg-info/PKG-INFO
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      427 2023-06-21 18:44:40.000000 gungnir-0.2.0/gungnir.egg-info/SOURCES.txt
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)        1 2023-06-21 18:44:40.000000 gungnir-0.2.0/gungnir.egg-info/dependency_links.txt
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      140 2023-06-21 18:44:40.000000 gungnir-0.2.0/gungnir.egg-info/requires.txt
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)        8 2023-06-21 18:44:40.000000 gungnir-0.2.0/gungnir.egg-info/top_level.txt
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      959 2023-06-21 18:42:10.000000 gungnir-0.2.0/pyproject.toml
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)       38 2023-06-21 18:44:40.682538 gungnir-0.2.0/setup.cfg
-drwxrwxr-x   0 geekmasher  (1000) geekmasher  (1000)        0 2023-06-21 18:44:40.682538 gungnir-0.2.0/tests/
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      173 2023-06-19 22:17:22.000000 gungnir-0.2.0/tests/test_deptrack.py
--rw-rw-r--   0 geekmasher  (1000) geekmasher  (1000)      435 2023-06-20 16:43:56.000000 gungnir-0.2.0/tests/test_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 22:21:02.000000 gungnir-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-15 22:21:28.000786 gungnir-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2491 2023-07-15 22:21:02.000000 gungnir-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/gungnir/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/gungnir/dependencytrack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:02.000000 gungnir-0.2.1/gungnir/dependencytrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-07-15 22:21:02.000000 gungnir-0.2.1/gungnir/dependencytrack/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-07-15 22:21:02.000000 gungnir-0.2.1/gungnir/dependencytrack/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/gungnir/gungnir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 22:21:27.000000 gungnir-0.2.1/gungnir/gungnir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-15 22:21:02.000000 gungnir-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 22:21:28.000786 gungnir-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:21:28.000786 gungnir-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-15 22:21:02.000000 gungnir-0.2.1/tests/test_project.py
```

### Comparing `gungnir-0.2.0/LICENSE` & `gungnir-0.2.1/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 MIT License
 
-Copyright (c) <year> <copyright holders>
+Copyright (c) 2023 Mathew Payne
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `gungnir-0.2.0/PKG-INFO` & `gungnir-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gungnir
-Version: 0.2.0
+Version: 0.2.1
 Summary: Homelab Automation Bot to Guard your very own Asgard
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/gungnir
 Project-URL: Bug Tracker, https://github.com/GeekMasher/gungnir/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,41 +29,52 @@
 
 </div>
 
 ## Overview
 
 Gungnir is a Homelab Automation Bot to Guard your very own Asgard from the dangerous world of out of date components.
 
+## Example
+
+![DependencyTrack Example](./assets/dependency-track-example.png)
+
 ## Usage
 
 ### CLI
 
 **Requirements:**
 
 - Python 3.9+
 - [Syft](https://github.com/anchore/syft) (generate bill of materials)
 
+**Install (pip):**
+
+```bash
+pip install gungnir
+```
 
 **Help:**
 
 ```bash
 python -m gungnir --help
 ```
 
 ```
-Gungnir - Homelab Automation Bot to Guard your very own Asgard
+Gungnir - Homelab Automation Tool to Guard your very own Asgard
 
 options:
   -h, --help            show this help message and exit
   --debug               Enable Debug mode
   --banner              Show banner
   --version             Show version
   --container           Enable container mode
   --disable-banner      Disable banner
   --hostname HOSTNAME   Hostname (mainly for containers)
+
+DependencyTrack:
   -t TOKEN, --token TOKEN
                         DependencyTrack Token
   -i INSTANCE, --instance INSTANCE
                         DependencyTrack Instance
 ```
 
 ### Docker-Compose
```

### Comparing `gungnir-0.2.0/README.md` & `gungnir-0.2.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,41 +11,52 @@
 
 </div>
 
 ## Overview
 
 Gungnir is a Homelab Automation Bot to Guard your very own Asgard from the dangerous world of out of date components.
 
+## Example
+
+![DependencyTrack Example](./assets/dependency-track-example.png)
+
 ## Usage
 
 ### CLI
 
 **Requirements:**
 
 - Python 3.9+
 - [Syft](https://github.com/anchore/syft) (generate bill of materials)
 
+**Install (pip):**
+
+```bash
+pip install gungnir
+```
 
 **Help:**
 
 ```bash
 python -m gungnir --help
 ```
 
 ```
-Gungnir - Homelab Automation Bot to Guard your very own Asgard
+Gungnir - Homelab Automation Tool to Guard your very own Asgard
 
 options:
   -h, --help            show this help message and exit
   --debug               Enable Debug mode
   --banner              Show banner
   --version             Show version
   --container           Enable container mode
   --disable-banner      Disable banner
   --hostname HOSTNAME   Hostname (mainly for containers)
+
+DependencyTrack:
   -t TOKEN, --token TOKEN
                         DependencyTrack Token
   -i INSTANCE, --instance INSTANCE
                         DependencyTrack Instance
 ```
 
 ### Docker-Compose
```

### Comparing `gungnir-0.2.0/gungnir/dependencytrack/api.py` & `gungnir-0.2.1/gungnir/dependencytrack/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,36 @@
+"""Dependency Track module."""
 import logging
-from typing import Dict, List, Optional
-
-from requests import Session
-import requests
+from typing import Dict, List
+from requests import Session, Response
 
 
 logger = logging.getLogger("gungnir.dependencytrack")
 
 KNOWN_ERRORS = {304: ""}
 
 
 class DependencyTrack:
+    """Dependency Track API class."""
+
     base: str
+    """Full base URL"""
     instance: str = "http://localhost:8080"
+    """Instance"""
     token: str = ""
+    """Token"""
     version: str = "v1"
+    """Version number"""
 
     session: Session
+    """Requests Session"""
 
     @staticmethod
     def init(instance: str, token: str) -> None:
+        """Initialise Dependency Track API."""
         DependencyTrack.instance = instance
         DependencyTrack.version = "v1"
 
         DependencyTrack.session = Session()
         DependencyTrack.session.headers = {
             "Accepts": "application/json",
             "X-Api-Key": token,
@@ -31,21 +38,23 @@
 
         DependencyTrack.base = (
             f"{DependencyTrack.instance}/api/{DependencyTrack.version}"
         )
 
     @staticmethod
     def getVersion() -> str:
+        """Get Version."""
         resp = DependencyTrack.session.get(f"{DependencyTrack.instance}/api/version")
         return resp.json().get("version", "NA")
 
 
 def checkResponse(
-    resp: requests.Response, expected: int = 200, is_json: bool = True
+    resp: Response, expected: int = 200, is_json: bool = True
 ) -> Dict | List[Dict]:
+    """Check Response."""
     if resp.status_code == expected:
         if is_json:
             return resp.json()
         return {}
 
     err = KNOWN_ERRORS.get(resp.status_code)
     if err:
```

### Comparing `gungnir-0.2.0/gungnir/dependencytrack/project.py` & `gungnir-0.2.1/gungnir/dependencytrack/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+"""Dependency Track Project."""
 import json
 import base64
 import logging
 
 from gungnir.dependencytrack.api import DependencyTrack, checkResponse
 from gungnir.project import Container, OperatingSystem
 
 logger = logging.getLogger("gungnir.dependencytrack")
 
 
 class Project:
+    """Dependency Track Project."""
+
     @staticmethod
     def lookup(project: OperatingSystem | Container):
-        """Lookup project based on name"""
+        """Lookup project based on name."""
 
         if isinstance(project, Container):
             # get all the children
             uuid = project.parent.uuid
             url = f"{DependencyTrack.base}/project/{uuid}/children"
         else:
             url = f"{DependencyTrack.base}/project"
@@ -33,15 +36,15 @@
                 continue
 
             project.__dict__.update(result)
             project.active = True
 
     @staticmethod
     def create(project: OperatingSystem | Container):
-        """Create a new Project in DependencyTrack
+        """Create a new Project in DependencyTrack.
 
         Required access to `PORTFOLIO_MANAGEMENT` permission todo this
         """
         logger.info(f"Creating new project (version: {project.version})")
 
         parent = None
         if project.parent:
@@ -61,15 +64,15 @@
         data = checkResponse(resp, 201)
         if not isinstance(data, dict):
             return
         project.__dict__.update(**data)
 
     @staticmethod
     def update(project: OperatingSystem | Container):
-        """Update Project in Dependency Track"""
+        """Update Project in Dependency Track."""
         logger.debug(f"Updating project :: {project.uuid}")
 
         parent = None
         if project.parent:
             parent = {"uuid": project.parent.uuid}
 
         payload = {
@@ -85,15 +88,15 @@
         )
 
         checkResponse(resp)
         logger.info("Successfully updated remote Project")
 
     @staticmethod
     def getChildren(project: OperatingSystem):
-        """Get Project children"""
+        """Get Project children."""
         logger.debug(f"Get Children for :: {project.uuid}")
         resp = DependencyTrack.session.get(
             f"{DependencyTrack.base}/project/{project.uuid}/children"
         )
         data = checkResponse(resp)
 
         for child in data:
@@ -106,12 +109,13 @@
                     parent=project,
                     active=bool(child.get("active", False)),
                 )
             )
 
     @staticmethod
     def uploadSbom(project: Container, bom: dict):
+        """Upload SBOM to Dependency Track API."""
         b64 = base64.b64encode(json.dumps(bom).encode())
         payload = {"project": project.uuid, "bom": b64.decode()}
         resp = DependencyTrack.session.put(f"{DependencyTrack.base}/bom", json=payload)
 
         checkResponse(resp)
```

### Comparing `gungnir-0.2.0/gungnir.egg-info/PKG-INFO` & `gungnir-0.2.1/gungnir/gungnir.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gungnir
-Version: 0.2.0
+Version: 0.2.1
 Summary: Homelab Automation Bot to Guard your very own Asgard
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/gungnir
 Project-URL: Bug Tracker, https://github.com/GeekMasher/gungnir/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -29,41 +29,52 @@
 
 </div>
 
 ## Overview
 
 Gungnir is a Homelab Automation Bot to Guard your very own Asgard from the dangerous world of out of date components.
 
+## Example
+
+![DependencyTrack Example](./assets/dependency-track-example.png)
+
 ## Usage
 
 ### CLI
 
 **Requirements:**
 
 - Python 3.9+
 - [Syft](https://github.com/anchore/syft) (generate bill of materials)
 
+**Install (pip):**
+
+```bash
+pip install gungnir
+```
 
 **Help:**
 
 ```bash
 python -m gungnir --help
 ```
 
 ```
-Gungnir - Homelab Automation Bot to Guard your very own Asgard
+Gungnir - Homelab Automation Tool to Guard your very own Asgard
 
 options:
   -h, --help            show this help message and exit
   --debug               Enable Debug mode
   --banner              Show banner
   --version             Show version
   --container           Enable container mode
   --disable-banner      Disable banner
   --hostname HOSTNAME   Hostname (mainly for containers)
+
+DependencyTrack:
   -t TOKEN, --token TOKEN
                         DependencyTrack Token
   -i INSTANCE, --instance INSTANCE
                         DependencyTrack Instance
 ```
 
 ### Docker-Compose
```

### Comparing `gungnir-0.2.0/pyproject.toml` & `gungnir-0.2.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 [project]
 name = "gungnir"
-version = "0.2.0"
-authors = [
-  { name="GeekMasher" },
-]
+version = "0.2.1"
+authors = [{ name = "GeekMasher" }]
 description = "Homelab Automation Bot to Guard your very own Asgard"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "certifi==2023.5.7",
-    "charset-normalizer==3.1.0",
+    "charset-normalizer==3.2.0",
     "docker==6.1.3",
     "idna==3.4",
     "packaging==23.1",
     "requests==2.31.0",
     "urllib3==2.0.3",
-    "websocket-client==1.5.2"
+    "websocket-client==1.6.1",
 ]
 
+[tool.setuptools.packages.find]
+where = ["gungnir"]
+
 [project.urls]
 "Homepage" = "https://github.com/GeekMasher/gungnir"
 "Bug Tracker" = "https://github.com/GeekMasher/gungnir/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
-
```

