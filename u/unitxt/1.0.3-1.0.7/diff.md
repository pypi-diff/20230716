# Comparing `tmp/unitxt-1.0.3.tar.gz` & `tmp/unitxt-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitxt-1.0.3.tar", last modified: Thu Jul 13 12:56:46 2023, max compression
+gzip compressed data, was "unitxt-1.0.7.tar", last modified: Sun Jul 16 11:51:23 2023, max compression
```

## Comparing `unitxt-1.0.3.tar` & `unitxt-1.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-13 12:56:46.970772 unitxt-1.0.3/
--rw-rw-r--   0 elron    (605371) tslm      (3127)    11357 2023-07-11 12:24:16.000000 unitxt-1.0.3/LICENSE
--rw-rw-r--   0 elron    (605371) tslm      (3127)       33 2023-07-11 12:24:16.000000 unitxt-1.0.3/MANIFEST.in
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2437 2023-07-13 12:56:46.970439 unitxt-1.0.3/PKG-INFO
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2005 2023-07-13 09:36:28.000000 unitxt-1.0.3/README.md
--rw-rw-r--   0 elron    (605371) tslm      (3127)      118 2023-07-12 07:33:22.000000 unitxt-1.0.3/pyproject.toml
--rw-rw-r--   0 elron    (605371) tslm      (3127)       38 2023-07-13 12:56:46.970882 unitxt-1.0.3/setup.cfg
--rw-rw-r--   0 elron    (605371) tslm      (3127)      811 2023-07-13 12:56:06.000000 unitxt-1.0.3/setup.py
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-13 12:56:46.953632 unitxt-1.0.3/src/
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-13 12:56:46.967549 unitxt-1.0.3/src/unitxt/
--rw-rw-r--   0 elron    (605371) tslm      (3127)      129 2023-07-12 10:12:58.000000 unitxt-1.0.3/src/unitxt/__init__.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6331 2023-07-13 09:36:28.000000 unitxt-1.0.3/src/unitxt/artifact.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      944 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/blocks.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      535 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/card.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     3240 2023-07-13 11:06:45.000000 unitxt-1.0.3/src/unitxt/catalog.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/collections.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2948 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/common.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     3868 2023-07-13 09:38:45.000000 unitxt-1.0.3/src/unitxt/dataclass.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2905 2023-07-13 12:49:32.000000 unitxt-1.0.3/src/unitxt/dataset.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      945 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/file_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      398 2023-07-12 10:44:35.000000 unitxt-1.0.3/src/unitxt/fusion.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1686 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/generator_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      656 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/instructions.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      407 2023-07-13 09:36:28.000000 unitxt-1.0.3/src/unitxt/load.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      669 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/loaders.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     4628 2023-07-13 12:49:45.000000 unitxt-1.0.3/src/unitxt/metric.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     4244 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/metrics.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      935 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/normalizers.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     8441 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/operator.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     7075 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/operators.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      201 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/processors.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      428 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/recipe.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1856 2023-07-13 11:09:36.000000 unitxt-1.0.3/src/unitxt/register.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2041 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/schema.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)    11051 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/split_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     3556 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/splitters.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6556 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/stream.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      567 2023-07-12 07:30:16.000000 unitxt-1.0.3/src/unitxt/task.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6351 2023-07-12 07:58:27.000000 unitxt-1.0.3/src/unitxt/templates.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     6768 2023-07-11 12:24:16.000000 unitxt-1.0.3/src/unitxt/text_utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)      238 2023-07-13 09:36:28.000000 unitxt-1.0.3/src/unitxt/utils.py
--rw-rw-r--   0 elron    (605371) tslm      (3127)     1327 2023-07-12 10:44:34.000000 unitxt-1.0.3/src/unitxt/validate.py
-drwxrwsr-x   0 elron    (605371) tslm      (3127)        0 2023-07-13 12:56:46.969839 unitxt-1.0.3/src/unitxt.egg-info/
--rw-rw-r--   0 elron    (605371) tslm      (3127)     2437 2023-07-13 12:56:46.967954 unitxt-1.0.3/src/unitxt.egg-info/PKG-INFO
--rw-rw-r--   0 elron    (605371) tslm      (3127)      955 2023-07-13 12:56:46.968276 unitxt-1.0.3/src/unitxt.egg-info/SOURCES.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)        1 2023-07-13 12:56:46.968791 unitxt-1.0.3/src/unitxt.egg-info/dependency_links.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)       66 2023-07-13 12:56:46.969413 unitxt-1.0.3/src/unitxt.egg-info/requires.txt
--rw-rw-r--   0 elron    (605371) tslm      (3127)        7 2023-07-13 12:56:46.969940 unitxt-1.0.3/src/unitxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:51:23.665161 unitxt-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 11:51:14.000000 unitxt-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-16 11:51:14.000000 unitxt-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-16 11:51:23.665161 unitxt-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-16 11:51:14.000000 unitxt-1.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-16 11:51:14.000000 unitxt-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 11:51:23.665161 unitxt-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-07-16 11:51:22.000000 unitxt-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:51:23.661161 unitxt-1.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:51:23.665161 unitxt-1.0.7/src/unitxt/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3868 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/fusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/generator_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/instructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4627 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/processors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/split_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-16 11:51:14.000000 unitxt-1.0.7/src/unitxt/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 11:51:23.665161 unitxt-1.0.7/src/unitxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-16 11:51:23.000000 unitxt-1.0.7/src/unitxt.egg-info/top_level.txt
```

### Comparing `unitxt-1.0.3/LICENSE` & `unitxt-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/README.md` & `unitxt-1.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,59 @@
+Metadata-Version: 2.1
+Name: unitxt
+Version: 1.0.7
+Summary: Load any mixture of text to text data in one line of code
+Home-page: https://github.com/ibm/unitxt
+Author: IBM Research
+Author-email: elron.bandel@ibm.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
     <img src="./assets/banner.png" alt="Image Description" width="100%" />
 </div>
 
 Unitxt is a python library for getting data fired up and set for utilization.
 In one line of code, it preps a dataset or mixtures-of-datasets into an input-output format for training and evaluation.
 We aspire to be simple, adaptable and transperant. 
 
 Unitxt builds on separation. Separation allows adding a dataset, without knowing anything about the models using it. Separation allows training without caring for preprocessing, switching models without loading the data differently and changing formats (instruction\ICL\etc.) without changing anything else. 
 
 # 
-[![version](https://img.shields.io/pypi/v/unitxt)](https://pypi.org/project/unitxt/)  ![license](https://img.shields.io/github/license/ibm/unitxt)  ![python](https://img.shields.io/badge/python-3.8%20|%203.9-blue)  ![tests](https://img.shields.io/github/actions/workflow/status/ibm/unitxt/tests.yml?branch=main&label=tests)
+[![version](https://img.shields.io/pypi/v/unitxt)](https://pypi.org/project/unitxt/)
+![license](https://img.shields.io/github/license/ibm/unitxt)
+![python](https://img.shields.io/badge/python-3.8%20|%203.9-blue)
+![tests](https://img.shields.io/github/actions/workflow/status/ibm/unitxt/tests.yml?branch=main&label=tests)
+[![codecov](https://codecov.io/gh/IBM/unitxt/branch/main/graph/badge.svg?token=mlrWq9cwz3)](https://codecov.io/gh/IBM/unitxt)
 ![Read the Docs](https://img.shields.io/readthedocs/unitxt)
 [![downloads](https://static.pepy.tech/personalized-badge/unitxt?period=total&units=international_system&left_color=grey&right_color=green&left_text=downloads)](https://pepy.tech/project/unitxt)
 
+#
 
-# Installation 🦄
-
-```bash
-  pip install unitxt
-```
-
-# Usage 🦄
-
-## Load a dataset
-
-```python
-from datasets import load_dataset
-
-dataset = load_dataset('unitxt/data', 'squad')
-```
+<div align="center">
+    <img src="./assets/unitxt_flow_light.gif" alt="Unitxt Flow" width="100%" />
+</div>
 
+# Where to start? 🦄
+[![Button](https://img.shields.io/badge/Overview-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
+[![Button](https://img.shields.io/badge/Concepts-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
+[![Button](https://img.shields.io/badge/Tutorial-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
+[![Button](https://img.shields.io/badge/Examples-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
+[![Button](https://img.shields.io/badge/Docs-pink?style=for-the-badge)](https://unitxt.readthedocs.io/)
 # Why Unitxt? 🦄
 
-Unitxt is construct in the light of the principles: (1) Simplicity (2) Adpatability (3) Transperancy
 ### 🦄 Simplicity
 Everything is unitxt is simple and designed to feel natural and self explenatory.
 ### 🦄 Adaptability
 Adding new datasets, loading recpepies, instructions and formattors is possible and encoureged!
 ### 🦄 Transperancy
 The reosurces and formators of Unitxt are stored as shared datasets and therfore can easily reviewed by the crowed. Moreover, when assembling dataset with Unitxt it is very clear to others whats in it. 
 
 #
 
+
+
```

### Comparing `unitxt-1.0.3/setup.py` & `unitxt-1.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
     
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="unitxt",
-    version="1.0.3",
+    version="1.0.7",
     author="IBM Research",
     author_email="elron.bandel@ibm.com",
     description="Load any mixture of text to text data in one line of code",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ibm/unitxt",
     packages=setuptools.find_packages('src'),
```

### Comparing `unitxt-1.0.3/src/unitxt/artifact.py` & `unitxt-1.0.7/src/unitxt/artifact.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/blocks.py` & `unitxt-1.0.7/src/unitxt/blocks.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/card.py` & `unitxt-1.0.7/src/unitxt/card.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/catalog.py` & `unitxt-1.0.7/src/unitxt/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import re
 from pathlib import Path
 import requests
 import json
 from .artifact import Artifact, Artifactory
 
 
-COLLECTION_SEPARATOR = '::'
+COLLECTION_SEPARATOR = '.'
 PATHS_SEP = ':'
 
 
 class Catalog(Artifactory):
     name: str = None
     location: str = None
 
@@ -24,15 +24,18 @@
 
 
 class LocalCatalog(Catalog):
     name: str = "local"
     location: str = default_catalog_path
 
     def path(self, artifact_identifier: str):
-        return os.path.join(self.location, *(artifact_identifier + ".json").split(COLLECTION_SEPARATOR))
+        assert artifact_identifier.strip(), 'artifact_identifier should not be an empty string.'
+        parts = artifact_identifier.split(COLLECTION_SEPARATOR)
+        parts[-1] = parts[-1] + ".json"
+        return os.path.join(self.location, *parts)
 
     def load(self, artifact_identifier: str):
         assert artifact_identifier in self, "Artifact with name {} does not exist".format(artifact_identifier)
         path = self.path(artifact_identifier)
         artifact_instance = Artifact.load(path)
         return artifact_instance
```

### Comparing `unitxt-1.0.3/src/unitxt/collections.py` & `unitxt-1.0.7/src/unitxt/collections.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/common.py` & `unitxt-1.0.7/src/unitxt/common.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/dataclass.py` & `unitxt-1.0.7/src/unitxt/dataclass.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/dataset.py` & `unitxt-1.0.7/src/unitxt/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         return None
 
 
 def parse(query: str):
     """
     Parses a query of the form 'key1=value1,key2=value2,...' into a dictionary.
     """
-    query = query.replace("@", "::")
     result = {}
     for kv in query.split(","):
         parts = kv.split("=")
         if parts[1].isdigit():
             result[parts[0]] = int(parts[1])
         elif parts[1].replace(".", "", 1).isdigit():
             result[parts[0]] = float(parts[1])
```

### Comparing `unitxt-1.0.3/src/unitxt/file_utils.py` & `unitxt-1.0.7/src/unitxt/file_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/generator_utils.py` & `unitxt-1.0.7/src/unitxt/generator_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/instructions.py` & `unitxt-1.0.7/src/unitxt/instructions.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/loaders.py` & `unitxt-1.0.7/src/unitxt/loaders.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/metric.py` & `unitxt-1.0.7/src/unitxt/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 
 class MetricRecipe(SequntialOperatorInitilizer):
     def prepare(self):
         register_all_artifacts()
         self.steps = [
             FromPredictionsAndOriginalData(),
             ApplyValueOperatorsField(
-                value_field="prediction", operators_field="processors", default_operators=["processors::to_string"]
+                value_field="prediction", operators_field="processors", default_operators=["processors.to_string"]
             ),
             SplitByValue(["group"]),
             ApplyStreamOperatorsField(
                 "metrics",
                 reversed=True,
             ),
             MultiStreamScoreMean(),
```

### Comparing `unitxt-1.0.3/src/unitxt/metrics.py` & `unitxt-1.0.7/src/unitxt/metrics.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/normalizers.py` & `unitxt-1.0.7/src/unitxt/normalizers.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/operator.py` & `unitxt-1.0.7/src/unitxt/operator.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/operators.py` & `unitxt-1.0.7/src/unitxt/operators.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/register.py` & `unitxt-1.0.7/src/unitxt/register.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/schema.py` & `unitxt-1.0.7/src/unitxt/schema.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/split_utils.py` & `unitxt-1.0.7/src/unitxt/split_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/splitters.py` & `unitxt-1.0.7/src/unitxt/splitters.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/stream.py` & `unitxt-1.0.7/src/unitxt/stream.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/task.py` & `unitxt-1.0.7/src/unitxt/task.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/templates.py` & `unitxt-1.0.7/src/unitxt/templates.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/text_utils.py` & `unitxt-1.0.7/src/unitxt/text_utils.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt/validate.py` & `unitxt-1.0.7/src/unitxt/validate.py`

 * *Files identical despite different names*

### Comparing `unitxt-1.0.3/src/unitxt.egg-info/SOURCES.txt` & `unitxt-1.0.7/src/unitxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

