# Comparing `tmp/apache-airflow-providers-http-4.5.0.tar.gz` & `tmp/apache-airflow-providers-http-4.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-http-4.5.0.tar", last modified: Wed Jul 12 19:10:17 2023, max compression
+gzip compressed data, was "apache-airflow-providers-http-4.5.0rc1.tar", last modified: Wed Jul 12 19:13:29 2023, max compression
```

## Comparing `apache-airflow-providers-http-4.5.0.tar` & `apache-airflow-providers-http-4.5.0rc1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:17.020773 apache-airflow-providers-http-4.5.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:10:15.000000 apache-airflow-providers-http-4.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.5.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4474 2023-07-12 19:10:17.021283 apache-airflow-providers-http-4.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2847 2023-07-12 19:10:15.000000 apache-airflow-providers-http-4.5.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:16.936243 apache-airflow-providers-http-4.5.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:16.937334 apache-airflow-providers-http-4.5.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:16.972260 apache-airflow-providers-http-4.5.0/airflow/providers/http/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-12 19:08:31.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3320 2023-07-12 19:10:15.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:16.977838 apache-airflow-providers-http-4.5.0/airflow/providers/http/hooks/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16172 2023-07-09 14:40:47.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/hooks/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:16.983623 apache-airflow-providers-http-4.5.0/airflow/providers/http/operators/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7470 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/operators/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:16.989238 apache-airflow-providers-http-4.5.0/airflow/providers/http/sensors/
--rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5864 2023-07-05 07:19:39.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/sensors/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:16.994838 apache-airflow-providers-http-4.5.0/airflow/providers/http/triggers/
--rw-r--r--   0 root         (0) root         (0)      787 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/triggers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4988 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0/airflow/providers/http/triggers/http.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:17.018149 apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4474 2023-07-12 19:10:16.000000 apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      852 2023-07-12 19:10:16.000000 apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:10:16.000000 apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-12 19:10:16.000000 apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:10:16.000000 apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       73 2023-07-12 19:10:16.000000 apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:10:16.000000 apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-http-4.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1958 2023-07-12 19:10:17.023128 apache-airflow-providers-http-4.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1626 2023-07-12 19:10:15.000000 apache-airflow-providers-http-4.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.266460 apache-airflow-providers-http-4.5.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.5.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:28.000000 apache-airflow-providers-http-4.5.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-http-4.5.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4480 2023-07-12 19:13:29.267642 apache-airflow-providers-http-4.5.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2850 2023-07-12 19:13:28.000000 apache-airflow-providers-http-4.5.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.180504 apache-airflow-providers-http-4.5.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.181594 apache-airflow-providers-http-4.5.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.215986 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-12 19:08:31.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3320 2023-07-12 19:13:28.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.221668 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16172 2023-07-09 14:40:47.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.227193 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7470 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.232834 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-06-01 06:14:28.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5864 2023-07-05 07:19:39.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.238574 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/triggers/
+-rw-r--r--   0 root         (0) root         (0)      787 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/triggers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-07-10 18:20:09.000000 apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/triggers/http.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:29.262194 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4480 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      852 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:29.000000 apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-http-4.5.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-07-12 19:13:29.269949 apache-airflow-providers-http-4.5.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1626 2023-07-12 19:13:27.000000 apache-airflow-providers-http-4.5.0rc1/setup.py
```

### Comparing `apache-airflow-providers-http-4.5.0/LICENSE` & `apache-airflow-providers-http-4.5.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/MANIFEST.in` & `apache-airflow-providers-http-4.5.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/PKG-INFO` & `apache-airflow-providers-http-4.5.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.5.0
+Version: 4.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.5.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.5.0``
+Release: ``4.5.0rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.5.0/README.rst` & `apache-airflow-providers-http-4.5.0rc1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.5.0``
+Release: ``4.5.0rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/get_provider_info.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/hooks/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/hooks/http.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/hooks/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/operators/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/operators/http.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/operators/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/sensors/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/sensors/http.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/sensors/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/triggers/__init__.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/triggers/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/airflow/providers/http/triggers/http.py` & `apache-airflow-providers-http-4.5.0rc1/airflow/providers/http/triggers/http.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/PKG-INFO` & `apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-http
-Version: 4.5.0
+Version: 4.5.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-http package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-http/4.5.0/
@@ -66,15 +66,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-http``
 
-Release: ``4.5.0``
+Release: ``4.5.0rc1``
 
 
 `Hypertext Transfer Protocol (HTTP) <https://www.w3.org/Protocols/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-http-4.5.0/apache_airflow_providers_http.egg-info/SOURCES.txt` & `apache-airflow-providers-http-4.5.0rc1/apache_airflow_providers_http.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/pyproject.toml` & `apache-airflow-providers-http-4.5.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-http-4.5.0/setup.cfg` & `apache-airflow-providers-http-4.5.0rc1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -44,23 +44,23 @@
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
 	aiohttp
-	apache-airflow>=2.4.0
+	apache-airflow>=2.4.0.dev0
 	asgiref
 	requests>=2.26.0
 	requests_toolbelt
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.http.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.http
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-http-4.5.0/setup.py` & `apache-airflow-providers-http-4.5.0rc1/setup.py`

 * *Files identical despite different names*

