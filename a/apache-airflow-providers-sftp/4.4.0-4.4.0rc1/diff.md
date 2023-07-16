# Comparing `tmp/apache-airflow-providers-sftp-4.4.0.tar.gz` & `tmp/apache-airflow-providers-sftp-4.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apache-airflow-providers-sftp-4.4.0.tar", last modified: Wed Jul 12 19:10:21 2023, max compression
+gzip compressed data, was "apache-airflow-providers-sftp-4.4.0rc1.tar", last modified: Wed Jul 12 19:13:33 2023, max compression
```

## Comparing `apache-airflow-providers-sftp-4.4.0.tar` & `apache-airflow-providers-sftp-4.4.0rc1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.395039 apache-airflow-providers-sftp-4.4.0/
--rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:10:20.000000 apache-airflow-providers-sftp-4.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.4.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     5466 2023-07-12 19:10:21.395601 apache-airflow-providers-sftp-4.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3819 2023-07-12 19:10:20.000000 apache-airflow-providers-sftp-4.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.303724 apache-airflow-providers-sftp-4.4.0/airflow/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.304814 apache-airflow-providers-sftp-4.4.0/airflow/providers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.340243 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/
--rw-r--r--   0 root         (0) root         (0)     1529 2023-07-12 19:08:31.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.343202 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/decorators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.348941 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/decorators/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/decorators/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2862 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/decorators/sensors/sftp.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-07-12 19:10:20.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/get_provider_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.355424 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/hooks/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/hooks/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14745 2023-06-05 12:50:36.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/hooks/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.361778 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/operators/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/operators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8458 2023-07-06 04:42:33.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/operators/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.368209 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/sensors/
--rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/sensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4410 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/sensors/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:10:21.392679 apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5466 2023-07-12 19:10:21.000000 apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      918 2023-07-12 19:10:21.000000 apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:10:21.000000 apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      101 2023-07-12 19:10:21.000000 apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:10:21.000000 apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       94 2023-07-12 19:10:21.000000 apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:10:21.000000 apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-sftp-4.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1940 2023-07-12 19:10:21.397496 apache-airflow-providers-sftp-4.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1665 2023-07-12 19:10:20.000000 apache-airflow-providers-sftp-4.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.597969 apache-airflow-providers-sftp-4.4.0rc1/
+-rw-r--r--   0 root         (0) root         (0)    10850 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.4.0rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      240 2023-06-01 06:14:29.000000 apache-airflow-providers-sftp-4.4.0rc1/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-07-12 19:13:33.598522 apache-airflow-providers-sftp-4.4.0rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3822 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.504568 apache-airflow-providers-sftp-4.4.0rc1/airflow/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.505728 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.546449 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/
+-rw-r--r--   0 root         (0) root         (0)     1529 2023-07-12 19:08:31.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.549508 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.555289 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/get_provider_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.560953 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14745 2023-06-05 12:50:36.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.566531 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8458 2023-07-06 04:42:33.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.572295 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 06:14:28.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-07-10 18:20:09.000000 apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-12 19:13:33.595702 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      918 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      101 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      104 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-12 19:13:33.000000 apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     5424 2023-06-24 10:23:12.000000 apache-airflow-providers-sftp-4.4.0rc1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1953 2023-07-12 19:13:33.600765 apache-airflow-providers-sftp-4.4.0rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1665 2023-07-12 19:13:32.000000 apache-airflow-providers-sftp-4.4.0rc1/setup.py
```

### Comparing `apache-airflow-providers-sftp-4.4.0/LICENSE` & `apache-airflow-providers-sftp-4.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/MANIFEST.in` & `apache-airflow-providers-sftp-4.4.0rc1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/PKG-INFO` & `apache-airflow-providers-sftp-4.4.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sftp
-Version: 4.4.0
+Version: 4.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.4.0``
+Release: ``4.4.0rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-sftp-4.4.0/README.rst` & `apache-airflow-providers-sftp-4.4.0rc1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.4.0``
+Release: ``4.4.0rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/decorators/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/decorators/sensors/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/decorators/sensors/sftp.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/decorators/sensors/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/get_provider_info.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/get_provider_info.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/hooks/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/hooks/sftp.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/hooks/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/operators/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/operators/sftp.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/operators/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/sensors/__init__.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/__init__.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/airflow/providers/sftp/sensors/sftp.py` & `apache-airflow-providers-sftp-4.4.0rc1/airflow/providers/sftp/sensors/sftp.py`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/PKG-INFO` & `apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apache-airflow-providers-sftp
-Version: 4.4.0
+Version: 4.4.0rc1
 Summary: Provider for Apache Airflow. Implements apache-airflow-providers-sftp package
 Home-page: https://airflow.apache.org/
 Download-URL: https://archive.apache.org/dist/airflow/providers
 Author: Apache Software Foundation
 Author-email: dev@airflow.apache.org
 License: Apache License 2.0
 Project-URL: Documentation, https://airflow.apache.org/docs/apache-airflow-providers-sftp/4.4.0/
@@ -67,15 +67,15 @@
     KIND, either express or implied.  See the License for the
     specific language governing permissions and limitations
     under the License.
 
 
 Package ``apache-airflow-providers-sftp``
 
-Release: ``4.4.0``
+Release: ``4.4.0rc1``
 
 
 `SSH File Transfer Protocol (SFTP) <https://tools.ietf.org/wg/secsh/draft-ietf-secsh-filexfer/>`__
 
 
 Provider package
 ----------------
```

### Comparing `apache-airflow-providers-sftp-4.4.0/apache_airflow_providers_sftp.egg-info/SOURCES.txt` & `apache-airflow-providers-sftp-4.4.0rc1/apache_airflow_providers_sftp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/pyproject.toml` & `apache-airflow-providers-sftp-4.4.0rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `apache-airflow-providers-sftp-4.4.0/setup.cfg` & `apache-airflow-providers-sftp-4.4.0rc1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -43,21 +43,21 @@
 include_package_data = True
 python_requires = ~=3.8
 packages = find:
 setup_requires = 
 	setuptools
 	wheel
 install_requires = 
-	apache-airflow-providers-ssh>=2.1.0
-	apache-airflow>=2.4.0
+	apache-airflow-providers-ssh>=2.1.0.dev0
+	apache-airflow>=2.4.0.dev0
 
 [options.entry_points]
 apache_airflow_provider = 
 	provider_info=airflow.providers.sftp.get_provider_info:get_provider_info
 
 [files]
 packages = airflow.providers.sftp
 
 [egg_info]
-tag_build = 
+tag_build = rc1
 tag_date = 0
```

### Comparing `apache-airflow-providers-sftp-4.4.0/setup.py` & `apache-airflow-providers-sftp-4.4.0rc1/setup.py`

 * *Files identical despite different names*

