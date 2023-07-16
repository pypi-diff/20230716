# Comparing `tmp/optumi-api-3.16.1.tar.gz` & `tmp/optumi-api-3.16.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optumi-api-3.16.1.tar", last modified: Sat Jul  8 17:49:37 2023, max compression
+gzip compressed data, was "optumi-api-3.16.2.tar", last modified: Sat Jul 15 22:49:31 2023, max compression
```

## Comparing `optumi-api-3.16.1.tar` & `optumi-api-3.16.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-08 17:49:37.116498 optumi-api-3.16.1/
--rw-rw-r--   0 denis     (1001) denis     (1001)      281 2023-07-07 15:36:36.000000 optumi-api-3.16.1/LICENSE
--rw-rw-r--   0 denis     (1001) denis     (1001)       58 2023-07-07 15:36:36.000000 optumi-api-3.16.1/MANIFEST.in
--rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-07-08 17:49:37.116498 optumi-api-3.16.1/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-07-07 15:36:36.000000 optumi-api-3.16.1/README.md
--rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-07-08 17:49:36.000000 optumi-api-3.16.1/core_version.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-08 17:49:37.112498 optumi-api-3.16.1/optumi_api/
--rw-rw-r--   0 denis     (1001) denis     (1001)     2839 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/CloudFile.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3663 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/CloudFileVersion.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5135 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/CloudStorage.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4044 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Colab.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5371 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Container.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4353 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/ContainerRegistry.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4179 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/EnvironmentVariables.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6589 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Executable.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      976 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/HoldoverTime.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3070 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/LocalFile.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2398 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/LocalStorage.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1505 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Log.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6281 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/LoginServer.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6734 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Machine.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1957 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Machines.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      723 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Notebook.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     6795 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/NotebookConfig.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     2487 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Notifications.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      819 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Packages.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1609 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Program.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     5284 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Provider.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1299 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Providers.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4038 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Resource.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      696 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Script.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     4168 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Server.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1958 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Summary.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    20543 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Workload.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3110 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/Workloads.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      838 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/__init__.py
--rw-rw-r--   0 denis     (1001) denis     (1001)      323 2023-07-07 22:06:45.000000 optumi-api-3.16.1/optumi_api/_version.py
--rw-rw-r--   0 denis     (1001) denis     (1001)    11502 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/api.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     1418 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/cli.py
--rw-rw-r--   0 denis     (1001) denis     (1001)     3806 2023-07-07 15:36:36.000000 optumi-api-3.16.1/optumi_api/utils.py
-drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-08 17:49:37.116498 optumi-api-3.16.1/optumi_api.egg-info/
--rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-07-08 17:49:37.000000 optumi-api-3.16.1/optumi_api.egg-info/PKG-INFO
--rw-rw-r--   0 denis     (1001) denis     (1001)     1086 2023-07-08 17:49:37.000000 optumi-api-3.16.1/optumi_api.egg-info/SOURCES.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-07-08 17:49:37.000000 optumi-api-3.16.1/optumi_api.egg-info/dependency_links.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       47 2023-07-08 17:49:37.000000 optumi-api-3.16.1/optumi_api.egg-info/entry_points.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-07-08 17:49:37.000000 optumi-api-3.16.1/optumi_api.egg-info/not-zip-safe
--rw-rw-r--   0 denis     (1001) denis     (1001)       74 2023-07-08 17:49:37.000000 optumi-api-3.16.1/optumi_api.egg-info/requires.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       11 2023-07-08 17:49:37.000000 optumi-api-3.16.1/optumi_api.egg-info/top_level.txt
--rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-07-08 17:49:37.116498 optumi-api-3.16.1/setup.cfg
--rwxrwxr-x   0 denis     (1001) denis     (1001)     2644 2023-07-07 15:36:36.000000 optumi-api-3.16.1/setup.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-15 22:49:31.550059 optumi-api-3.16.2/
+-rw-rw-r--   0 denis     (1001) denis     (1001)      281 2023-07-15 16:47:20.000000 optumi-api-3.16.2/LICENSE
+-rw-rw-r--   0 denis     (1001) denis     (1001)       58 2023-07-15 16:47:20.000000 optumi-api-3.16.2/MANIFEST.in
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-07-15 22:49:31.550059 optumi-api-3.16.2/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)      422 2023-07-15 16:47:20.000000 optumi-api-3.16.2/README.md
+-rw-rw-r--   0 denis     (1001) denis     (1001)      322 2023-07-15 22:49:31.000000 optumi-api-3.16.2/core_version.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-15 22:49:31.546059 optumi-api-3.16.2/optumi_api/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2839 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/CloudFile.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3663 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/CloudFileVersion.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5135 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/CloudStorage.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4044 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Colab.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5371 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Container.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4353 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/ContainerRegistry.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4179 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/EnvironmentVariables.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6589 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Executable.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      976 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/HoldoverTime.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3070 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/LocalFile.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2398 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/LocalStorage.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1505 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Log.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6281 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/LoginServer.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     8473 2023-07-15 16:49:30.000000 optumi-api-3.16.2/optumi_api/Machine.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1957 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Machines.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      723 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Notebook.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     7280 2023-07-15 16:49:30.000000 optumi-api-3.16.2/optumi_api/NotebookConfig.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     2487 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Notifications.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      819 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Packages.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1609 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Program.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     5284 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Provider.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1299 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Providers.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     6656 2023-07-15 16:49:30.000000 optumi-api-3.16.2/optumi_api/Resource.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      696 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Script.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     4168 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Server.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1958 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Summary.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    20567 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Workload.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3110 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/Workloads.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      838 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/__init__.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)      323 2023-07-15 16:49:30.000000 optumi-api-3.16.2/optumi_api/_version.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)    11393 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/api.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1418 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/cli.py
+-rw-rw-r--   0 denis     (1001) denis     (1001)     3806 2023-07-15 16:47:20.000000 optumi-api-3.16.2/optumi_api/utils.py
+drwxrwxr-x   0 denis     (1001) denis     (1001)        0 2023-07-15 22:49:31.550059 optumi-api-3.16.2/optumi_api.egg-info/
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1560 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1001) denis     (1001)     1086 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       47 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/entry_points.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)        1 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/not-zip-safe
+-rw-rw-r--   0 denis     (1001) denis     (1001)       74 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       11 2023-07-15 22:49:31.000000 optumi-api-3.16.2/optumi_api.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1001) denis     (1001)       38 2023-07-15 22:49:31.550059 optumi-api-3.16.2/setup.cfg
+-rwxrwxr-x   0 denis     (1001) denis     (1001)     2644 2023-07-15 16:47:20.000000 optumi-api-3.16.2/setup.py
```

### Comparing `optumi-api-3.16.1/PKG-INFO` & `optumi-api-3.16.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.16.1
+Version: 3.16.2
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.16.1/optumi_api/CloudFile.py` & `optumi-api-3.16.2/optumi_api/CloudFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/CloudFileVersion.py` & `optumi-api-3.16.2/optumi_api/CloudFileVersion.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/CloudStorage.py` & `optumi-api-3.16.2/optumi_api/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Colab.py` & `optumi-api-3.16.2/optumi_api/Colab.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Container.py` & `optumi-api-3.16.2/optumi_api/Container.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/ContainerRegistry.py` & `optumi-api-3.16.2/optumi_api/ContainerRegistry.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/EnvironmentVariables.py` & `optumi-api-3.16.2/optumi_api/EnvironmentVariables.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Executable.py` & `optumi-api-3.16.2/optumi_api/Executable.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/HoldoverTime.py` & `optumi-api-3.16.2/optumi_api/HoldoverTime.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/LocalFile.py` & `optumi-api-3.16.2/optumi_api/LocalFile.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/LocalStorage.py` & `optumi-api-3.16.2/optumi_api/LocalStorage.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Log.py` & `optumi-api-3.16.2/optumi_api/Log.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/LoginServer.py` & `optumi-api-3.16.2/optumi_api/LoginServer.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Machine.py` & `optumi-api-3.16.2/optumi_api/Machine.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ##
 
 import optumi_core as optumi
 from optumi_core.exceptions import OptumiException
 
 import json, time
 
+from typing import List
 
 class Machine:
     """A class for representing a machine. It has two constructors, one to be used when creating a new
     machine and another when reconstructing an existing Optumi dynamic machine.
     """
 
     status_values = ["Acquiring", "Configuring", "Busy", "Idle", "Releasing"]
@@ -23,45 +24,61 @@
         uuid: str,
         size: str,
         dns_name: str,
         rate: float,
         promo: bool,
         app: str,
         state: str = None,
+        gpus: List[str] = None,
+        vram: int = None,
+        ram: int = None,
+        num_cpus: int = None,
     ):
         """Constructor for new a Machine object.
 
         Args:
             uuid (str): The unique machine identifier associated with this machine.
             size (str): The acronym for this machine instance that identifies its capabilities.
             dns_name (str): The DNS name assigned to this machine.
             rate (float): The hourly rate for this machine in USD.
             promo (bool): Whether this machine is being given a promotional rate or not.
             app (str): The application name of the workload being executed on this machine.
             state (str): The current state of this machine, one of "Acquiring", "Configuring", "Busy", "Idle" or "Releasing"
+            gpus (list of str): The GPUs for this machine or None if this machine doesn't have any gpus.
+            vram (int): The total GPU RAM for this machine in GiB or None if this machine doesn't have any gpus.
+            ram (int): The amount of RAM in GiB for this machine.
+            num_cpus (int): The number of cpus for this machine.
         """
         self._uuid = uuid
         self._size = size
         self._dns_name = dns_name
         self._rate = rate
         self._promo = promo
         self._app = app
         self._state = state
+        self._gpus = gpus
+        self._vram = vram
+        self._ram = ram
+        self._num_cpus = num_cpus
         self._last_refresh = time.time()
 
     @classmethod
     def reconstruct(cls, machine_map):
         return (
             machine_map["uuid"],
             machine_map["name"],
             machine_map["dnsName"],
             machine_map["rate"],
             machine_map["promo"],
             machine_map["app"],
             machine_map["state"],
+            [machine_map["graphicsCardType"] * machine_map["graphicsNumCards"]],
+            round(machine_map["graphicsMemory"] / 1024**3),
+            round(machine_map["memorySize"] / 1024**3),
+            machine_map["computeCores"][1],
         )
 
     def _refresh(self):
         now = time.time()
         if now - self._last_refresh > 5:
             self._last_refresh = now
             response = json.loads(optumi.core.get_machines().text)
@@ -197,9 +214,49 @@
             "sequestration in progress",
             "sequestration completed",
         ]:
             return "Releasing"
         else:
             return ""
 
+    @property
+    def gpus(self):
+        """Obtain the gpus for this machine.
+
+        Returns:
+            list of str: The gpus for this machine instance.
+        """
+        self._refresh()
+        return self._gpus
+    
+    @property
+    def vram(self):
+        """Obtain the VRAM for this machine.
+
+        Returns:
+            int: The VRAM for this machine instance in GiB.
+        """
+        self._refresh()
+        return self._vram
+
+    @property
+    def ram(self):
+        """Obtain the RAM for this machine.
+
+        Returns:
+            int: The RAM for this machine instance in GiB.
+        """
+        self._refresh()
+        return self._ram
+
+    @property
+    def num_cpus(self):
+        """Obtain the number of cpus for this machine.
+
+        Returns:
+            int: The number of cpus for this machine instance.
+        """
+        self._refresh()
+        return self._num_cpus
+
     def __str__(self):
         return str(self._size) + " " + str(self._rate)
```

### Comparing `optumi-api-3.16.1/optumi_api/Machines.py` & `optumi-api-3.16.2/optumi_api/Machines.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Notebook.py` & `optumi-api-3.16.2/optumi_api/Notebook.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/NotebookConfig.py` & `optumi-api-3.16.2/optumi_api/NotebookConfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,15 +49,16 @@
             "required": False,
             "rating": [-1, -1, -1],
             "score": [-1, -1, -1],
             "cores": [-1, -1, -1],
             "memory": [-1, -1, -1],
             "frequency": [-1, -1, -1],
             "boardType": "U",
-            "memoryPerCard": 0,
+            "memoryPerBoard": [-1, -1, -1],
+            "memoryPerSystem": [-1, -1, -1],
             "boardCount": [-1, -1, -1],
         },
         "memory": {
             "expertise": "component",
             "required": False,
             "rating": [-1, -1, -1],
             "size": [-1, -1, -1],
@@ -70,14 +71,15 @@
             "iops": [-1, -1, -1],
             "throughput": [-1, -1, -1],
         },
         "upload": {"files": [], "requirements": ""},
         "integrations": [],
         "providers": [],
         "machineAssortment": [],
+        "maxRate": -1,
         "notifications": {
             "jobStartedSMSEnabled": False,
             "jobCompletedSMSEnabled": False,
             "jobFailedSMSEnabled": False,
             "packageReadySMSEnabled": False,
         },
         "interactive": False,
@@ -167,26 +169,34 @@
     # Plug in resource requirements
     if type(resource) is Server:
         check_providers([resource.provider])
         nb_config["machineAssortment"] = [resource.provider.name + ":" + resource.size]
     elif type(resource) is Resource:
         nb_config["machineAssortment"] = []
 
+        nb_config["compute"]["cores"] = [-1, -1, -1] if resource.num_cpus == 0 else [resource.num_cpus, -1, -1]
+
         if resource.gpu in Resource.gpu_required_values:
             nb_config["graphics"]["cores"] = [1 if resource.gpu == "required" else -1, -1, -1]
         else:
             nb_config["graphics"]["cores"] = [1, -1, -1]
             nb_config["graphics"]["boardType"] = resource.gpu
 
-        nb_config["graphics"]["memoryPerCard"] = resource.memory_per_gpu
-        nb_config["graphics"]["boardCount"] = [-1, -1, -1] if resource.num_gpus == 0 else [resource.num_gpus, resource.num_gpus, resource.num_gpus]
+        nb_config["graphics"]["memoryPerBoard"] = [resource.vram_per_gpu * 1024**3, -1, -1]
+        nb_config["graphics"]["memoryPerSystem"] = [resource.vram_per_system * 1024**3, -1, -1]
+        nb_config["graphics"]["boardCount"] = [-1, -1, -1] if resource.num_gpus == 0 else [resource.num_gpus, -1, -1]
+
+        nb_config["memory"]["size"] = [-1, -1, -1] if resource.ram == 0 else [resource.ram * 1024**3, -1, -1]
 
         check_providers(resource.providers)
         nb_config["providers"] = [provider.name for provider in resource.providers]
 
+        if resource.max_rate > 0:
+            nb_config['maxRate'] = resource.max_rate / 3600 
+
     # Plug in requirements
     if notifications != None:
         nb_config["notifications"] = {
             "jobStartedSMSEnabled": notifications.job_started,
             "jobCompletedSMSEnabled": notifications.job_completed,
             "jobFailedSMSEnabled": notifications.job_failed,
             "packageReadySMSEnabled": False,
```

### Comparing `optumi-api-3.16.1/optumi_api/Notifications.py` & `optumi-api-3.16.2/optumi_api/Notifications.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Packages.py` & `optumi-api-3.16.2/optumi_api/Packages.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Program.py` & `optumi-api-3.16.2/optumi_api/Program.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Provider.py` & `optumi-api-3.16.2/optumi_api/Provider.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Providers.py` & `optumi-api-3.16.2/optumi_api/Providers.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Resource.py` & `optumi-api-3.16.2/optumi_api/Server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,96 +1,122 @@
 ##
 ## Copyright (C) Optumi Inc - All rights reserved.
 ##
 ## You may only use this code under license with Optumi Inc and any distribution or modification is strictly prohibited.
 ## To receive a copy of the licensing terms please write to contact@optumi.com or visit us at https://www.optumi.com.
 ##
 
-from .Server import Server
 from .Provider import Provider
 from .Providers import Providers
 
-from typing import Union, List
+import optumi_core as optumi
+from optumi_core.exceptions import OptumiException
 
-from optumi_core.exceptions import (
-    OptumiException,
-)
+import json
 
+_machines = None
+_gpus = None
 
-class Resource:
-    """A class for creating resource specifications to be used when running scripts, notebooks or containers."""
 
-    gpu_required_values = ["required", "optional"]
+def _update_inventory_info():
+    global _machines, _gpus
 
-    def __init__(self, providers: Union[List[str], List[Provider]] = [], gpu: str = "required", memory_per_gpu: int = 0, num_gpus: int = 0):
-        """Constructor for the Resource class.
+    user_information = json.loads(optumi.core.get_user_information(True).text)
 
-        Args:
-            providers (list of str or list of Provider): The providers that can be used. Defaults to [], which means any provider can be used.
-            gpu (str): This argument specifies the type of graphics card to use. It can be set to "required" to permit any graphics card, "optional" to permit cpu only machines, or a particular value from the options in gpus(). The default option is "required".
-            memory_per_gpu (int): Memory allocated per graphics card. Default is 0.
-            num_gpus (int): The number of gpu cards. Defaults 1 gpu is specified, otherwise 0.
+    _machines = []
+    _gpus = []
 
-        Raises:
-            OptumiException: Raised if an unsupported GPU card is specified.
-        """
-        if not type(gpu) is str:
-            raise OptumiException("Unexpected GPU type '" + str(gpu) + "', expected one of " + str(Resource.gpu_required_values + Server.gpus()))
-        elif not gpu.lower() in Resource.gpu_required_values + [x.lower() for x in Server.gpus()]:
-            gpus = Server.gpus()
-            if len(gpus) == 0:
-                if len([p for p in Providers.list() if p.is_activated()]) == 0:
-                    raise OptumiException("No activated providers. Contact Optumi for more information.")
-                if len(Server.inventory()) == 0:
-                    raise OptumiException("Machine inventory is empty. Contact Optumi for more information.")
-                raise OptumiException("No GPU machines in inventory.")
-            raise OptumiException("Unexpected GPU type '" + str(gpu) + "', expected one of " + str(Resource.gpu_required_values + gpus))
-
-        self._providers = []
-        for provider in providers:
-            if type(provider) is Provider:
-                self._providers.append(provider)
-            else:
-                self._providers.append(Provider(provider))
-
-        self._gpu = gpu
-        self._memory_per_gpu = memory_per_gpu
-        self._num_gpus = 1 if num_gpus == 0 and gpu != "optional" else num_gpus
+    for machine in user_information["machines"]:
+        name = machine["name"]
+        provider = name.split(":")[0]
+        gpu = machine["graphicsCardType"]
 
-    @property
-    def providers(self):
-        """Obtain the list of the providers that can be used.
+        if not machine in _machines:
+            _machines.append(name)
+
+        if not gpu in _gpus:
+            _gpus.append(gpu)
+
+    _machines.sort()
+    _gpus.sort()
+
+
+# Support embedding the provider in the machine string, have no default provider argument
+class Server:
+    """A class specifying a server with specific machine capabilities from a given cloud provider."""
+
+    @classmethod
+    def inventory(cls):
+        """Obtain a list of all cloud machines.
 
         Returns:
-            list of Provider: The list of providers that can be used. Defaults to [], which means any provider.
+            list of string: A list of machine sizes as strings.
         """
-        return self._providers
+        if _machines is None:
+            _update_inventory_info()
 
-    @property
-    def gpu(self):
-        """Obtain the type of graphics card to be used, either True for any, or a specific string value representing one of the types in gpus()
+        return _machines
+
+    @classmethod
+    def gpus(cls):
+        """Obtain a list of all graphics cards in cloud machines.
 
         Returns:
-            str: The type of graphics card to be used, "required" to permit any graphics card, "optional" to permit cpu only machines, or a specific string value representing one of the types in gpus()
+            list of string: A list of graphics cards as strings.
         """
-        return self._gpu
+        if _gpus is None:
+            _update_inventory_info()
+
+        return _gpus
+
+    def __init__(self, size: str = "Standard_NC4as_T4_v3", provider: str = "Azure"):
+        """Constructor for the Server object.
+
+        Args:
+            size (str, optional): The machine size, e.g., 'Standard_NC4as_T4_v3'. If the size string contains a colon (':'), then the first part of the string is treated as the provider name and the second part of the string is treated as the size name. Available sizes can be listed using machines(). Defaults to "Standard_NC4as_T4_v3".
+            provider (str, optional): The name of the provider for the server, e.g., 'Azure'. Defaults to "Azure".
+
+        Raises:
+            OptumiException: Raised if an unexpected provider or size is specified.
+        """
+        if ":" in size:
+            s = size.split(":")
+            self._provider = Provider(s[0].lower())
+            self._size = s[1].lower()
+        else:
+            self._provider = Provider(provider.lower())
+            self._size = size.lower()
+
+        inventory = Server.inventory()
+        if not self._provider.name.lower() + ":" + self._size in [x.lower() for x in inventory]:
+            if len(inventory) == 0:
+                if len([p for p in Providers.list() if not p.is_activated()]) == 0:
+                    raise OptumiException("No activated providers. Contact Optumi for more information.")
+                raise OptumiException("Machine inventory is empty. Contact Optumi for more information.")
+            raise OptumiException("Unexpected machine size '" + self._provider + ":" + self._size + "', expected one of " + str(inventory))
+
+        if not self._provider.is_enabled():
+            raise OptumiException("Provider " + str(provider) + " is not enabled. Use Provider.enable() prior to launching.")
+
+        if not self._provider.is_activated():
+            raise OptumiException("Provider " + str(provider) + " is not activated by Optumi. Contact Optumi for more information.")
 
     @property
-    def memory_per_gpu(self):
-        """Obtain the memory required per graphics card.
+    def provider(self):
+        """Obtain the cloud provider name.
 
         Returns:
-            int: The memory required per graphics card, specified in GB.
+            str: The name of the cloud provider for the allocated machine.
         """
-        return self._memory_per_gpu
+        return self._provider
 
     @property
-    def num_gpus(self):
-        """Obtain the number of gpu cards.
+    def size(self):
+        """Obtain the server size.
 
         Returns:
-            int: The number of gpu cards.
+            str: The size of the allocated machine.
         """
-        return self._num_gpus
+        return self._size
 
     def __str__(self):
-        return "gpu=" + str(self.gpu)
+        return str(self.provider) + ":" + str(self.size)
```

### Comparing `optumi-api-3.16.1/optumi_api/Script.py` & `optumi-api-3.16.2/optumi_api/Script.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Summary.py` & `optumi-api-3.16.2/optumi_api/Summary.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/Workload.py` & `optumi-api-3.16.2/optumi_api/Workload.py`

 * *Files 0% similar despite different names*

```diff
@@ -557,11 +557,12 @@
     @property
     def machine(self):
         """Obtain the machine this workload is or was running on.
 
         Returns:
             Machine: The Machine object representing the machine that the workload is or was running on.
         """
+        self._refresh()
         return self._machine
 
     def __str__(self):
         return str(self.name)
```

### Comparing `optumi-api-3.16.1/optumi_api/Workloads.py` & `optumi-api-3.16.2/optumi_api/Workloads.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/__init__.py` & `optumi-api-3.16.2/optumi_api/__init__.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/api.py` & `optumi-api-3.16.2/optumi_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,17 +226,16 @@
 
 def get_holdover_time():
     """Obtain the current holdover time.
 
     The holdover time is the period of time that machines are retained (provisioned) after a workload finishes. Holdover time is global and applies to all workloads.
 
     Returns:
-        The holdover time as an integer representing minutes.
+        The holdover time as an HoldoverTime object.
     """
-    res = optumi.core.get_user_information(False)
     return HoldoverTime(int(json.loads(optumi.core.get_user_information(False).text)["userHoldoverTime"]) // 60)  # Convert to minutes
 
 
 def set_holdover_time(holdover_time: Union[int, HoldoverTime]):
     """Configure the holdover time.
 
     The holdover time is the period of time that machines are retained (provisioned) after a workload finishes. Holdover time is global and applies to all workloads.
@@ -294,9 +293,8 @@
     """Obtain the current workload limit.
 
     The workload limit is the maximum number of workloads that can be running in parallel.
 
     Returns:
         The workload limit as an integer.
     """
-    res = optumi.core.get_user_information(False)
     return int(json.loads(optumi.core.get_user_information(False).text)["maxJobs"])
```

### Comparing `optumi-api-3.16.1/optumi_api/cli.py` & `optumi-api-3.16.2/optumi_api/cli.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api/utils.py` & `optumi-api-3.16.2/optumi_api/utils.py`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/optumi_api.egg-info/PKG-INFO` & `optumi-api-3.16.2/optumi_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optumi-api
-Version: 3.16.1
+Version: 3.16.2
 Summary: Optumi api library
 Home-page: https://optumi.com
 Author: Optumi Inc Authors
 Author-email: cs@optumi.com
 Keywords: Optumi
 Platform: Linux
 Platform: Mac OS X
```

### Comparing `optumi-api-3.16.1/optumi_api.egg-info/SOURCES.txt` & `optumi-api-3.16.2/optumi_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optumi-api-3.16.1/setup.py` & `optumi-api-3.16.2/setup.py`

 * *Files identical despite different names*

