# Comparing `tmp/pyjava-0.6.4.tar.gz` & `tmp/pyjava-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjava-0.6.4.tar", last modified: Sun Jun 25 04:12:49 2023, max compression
+gzip compressed data, was "pyjava-0.6.5.tar", last modified: Sun Jul 16 03:10:50 2023, max compression
```

## Comparing `pyjava-0.6.4.tar` & `pyjava-0.6.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-25 04:12:49.884317 pyjava-0.6.4/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      448 2023-04-11 04:53:45.000000 pyjava-0.6.4/README.md
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/pyjava/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2612 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/pyjava/api/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      688 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/api/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16024 2023-05-26 04:03:49.000000 pyjava-0.6.4/pyjava/api/mlsql.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4524 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/api/serve.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/pyjava/cache/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/cache/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      489 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/cache/code_cache.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42222 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/cloudpickle.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7048 2023-04-17 05:24:46.000000 pyjava-0.6.4/pyjava/daemon.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/pyjava/data/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/data/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1185 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/data/datasource.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/pyjava/datatype/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/datatype/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    64554 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/datatype/types.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2190 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/rayfix.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30195 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/serializers.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/pyjava/storage/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.4/pyjava/storage/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2825 2023-04-24 06:01:20.000000 pyjava-0.6.4/pyjava/storage/streaming_tar.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/pyjava/udf/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6260 2023-06-25 03:46:27.000000 pyjava-0.6.4/pyjava/udf/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1555 2023-06-24 13:03:57.000000 pyjava-0.6.4/pyjava/udf/store.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3990 2023-06-23 13:03:45.000000 pyjava-0.6.4/pyjava/utils.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      828 2023-06-25 04:12:06.000000 pyjava-0.6.4/pyjava/version.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6457 2023-04-18 03:10:44.000000 pyjava-0.6.4/pyjava/worker.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-25 04:12:49.884317 pyjava-0.6.4/pyjava.egg-info/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-06-25 04:12:49.000000 pyjava-0.6.4/pyjava.egg-info/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      616 2023-06-25 04:12:49.000000 pyjava-0.6.4/pyjava.egg-info/SOURCES.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-06-25 04:12:49.000000 pyjava-0.6.4/pyjava.egg-info/dependency_links.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        7 2023-06-25 04:12:49.000000 pyjava-0.6.4/pyjava.egg-info/top_level.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       79 2023-06-25 04:12:49.884317 pyjava-0.6.4/setup.cfg
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2955 2023-04-11 04:53:45.000000 pyjava-0.6.4/setup.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.294583 pyjava-0.6.5/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-07-16 03:10:50.294583 pyjava-0.6.5/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      448 2023-04-11 04:53:45.000000 pyjava-0.6.5/README.md
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.290583 pyjava-0.6.5/pyjava/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2612 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.294583 pyjava-0.6.5/pyjava/api/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      688 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/api/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16024 2023-05-26 04:03:49.000000 pyjava-0.6.5/pyjava/api/mlsql.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4524 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/api/serve.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.294583 pyjava-0.6.5/pyjava/cache/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/cache/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      489 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/cache/code_cache.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42222 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/cloudpickle.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7048 2023-04-17 05:24:46.000000 pyjava-0.6.5/pyjava/daemon.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.294583 pyjava-0.6.5/pyjava/data/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/data/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1185 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/data/datasource.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.294583 pyjava-0.6.5/pyjava/datatype/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/datatype/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    64554 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/datatype/types.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2190 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/rayfix.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30195 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/serializers.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.294583 pyjava-0.6.5/pyjava/storage/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-11 04:53:45.000000 pyjava-0.6.5/pyjava/storage/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2825 2023-04-24 06:01:20.000000 pyjava-0.6.5/pyjava/storage/streaming_tar.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.294583 pyjava-0.6.5/pyjava/udf/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6368 2023-07-16 01:46:23.000000 pyjava-0.6.5/pyjava/udf/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1555 2023-06-24 13:03:57.000000 pyjava-0.6.5/pyjava/udf/store.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3990 2023-06-23 13:03:45.000000 pyjava-0.6.5/pyjava/utils.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      828 2023-07-16 03:10:34.000000 pyjava-0.6.5/pyjava/version.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6457 2023-04-18 03:10:44.000000 pyjava-0.6.5/pyjava/worker.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-16 03:10:50.290583 pyjava-0.6.5/pyjava.egg-info/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      597 2023-07-16 03:10:50.000000 pyjava-0.6.5/pyjava.egg-info/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      616 2023-07-16 03:10:50.000000 pyjava-0.6.5/pyjava.egg-info/SOURCES.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-07-16 03:10:50.000000 pyjava-0.6.5/pyjava.egg-info/dependency_links.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        7 2023-07-16 03:10:50.000000 pyjava-0.6.5/pyjava.egg-info/top_level.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       79 2023-07-16 03:10:50.294583 pyjava-0.6.5/setup.cfg
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2955 2023-04-11 04:53:45.000000 pyjava-0.6.5/setup.py
```

### Comparing `pyjava-0.6.4/PKG-INFO` & `pyjava-0.6.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjava
-Version: 0.6.4
+Version: 0.6.5
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyjava-0.6.4/pyjava/__init__.py` & `pyjava-0.6.5/pyjava/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/api/__init__.py` & `pyjava-0.6.5/pyjava/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/api/mlsql.py` & `pyjava-0.6.5/pyjava/api/mlsql.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/api/serve.py` & `pyjava-0.6.5/pyjava/api/serve.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/cloudpickle.py` & `pyjava-0.6.5/pyjava/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/daemon.py` & `pyjava-0.6.5/pyjava/daemon.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/data/datasource.py` & `pyjava-0.6.5/pyjava/data/datasource.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/datatype/types.py` & `pyjava-0.6.5/pyjava/datatype/types.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/rayfix.py` & `pyjava-0.6.5/pyjava/rayfix.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/serializers.py` & `pyjava-0.6.5/pyjava/serializers.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/storage/streaming_tar.py` & `pyjava-0.6.5/pyjava/storage/streaming_tar.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/udf/__init__.py` & `pyjava-0.6.5/pyjava/udf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     
     def create_workers(self, conf):
         udf_worker_conf = {}
 
         if "num_cpus" in conf:
             udf_worker_conf["num_cpus"] = float(conf["num_cpus"])
 
-        if "num_gpus" in conf:
+        infer_backend =  conf.get("infer_backend", "transformers")
+        if "num_gpus" in conf and not infer_backend.startswith("ray/"):
             udf_worker_conf["num_gpus"] = float(conf["num_gpus"])
 
         custom_resources = [(key.split("resource.")[1], float(conf[key])) for key in
                             conf.keys() if
                             key.startswith("resource.")]
 
         if len(custom_resources) > 0:
```

### Comparing `pyjava-0.6.4/pyjava/udf/store.py` & `pyjava-0.6.5/pyjava/udf/store.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/utils.py` & `pyjava-0.6.5/pyjava/utils.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava/version.py` & `pyjava-0.6.5/pyjava/version.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.6.4"
+__version__ = "0.6.5"
```

### Comparing `pyjava-0.6.4/pyjava/worker.py` & `pyjava-0.6.5/pyjava/worker.py`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/pyjava.egg-info/PKG-INFO` & `pyjava-0.6.5/pyjava.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjava
-Version: 0.6.4
+Version: 0.6.5
 Summary: PyJava Python API
 Home-page: https://github.com/allwefantasy/pyjava
 Author: allwefantasy
 Author-email: allwefantasy@gmail.com
 License: http://www.apache.org/licenses/LICENSE-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyjava-0.6.4/pyjava.egg-info/SOURCES.txt` & `pyjava-0.6.5/pyjava.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyjava-0.6.4/setup.py` & `pyjava-0.6.5/setup.py`

 * *Files identical despite different names*

