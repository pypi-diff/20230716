# Comparing `tmp/redhat_qe_cloud_tools-1.0.8.tar.gz` & `tmp/redhat_qe_cloud_tools-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redhat_qe_cloud_tools-1.0.8.tar", max compression
+gzip compressed data, was "redhat_qe_cloud_tools-1.0.9.tar", max compression
```

## Comparing `redhat_qe_cloud_tools-1.0.8.tar` & `redhat_qe_cloud_tools-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11357 2023-06-29 14:06:23.151726 redhat_qe_cloud_tools-1.0.8/LICENSE
--rw-r--r--   0        0        0      852 2023-06-29 14:06:23.151726 redhat_qe_cloud_tools-1.0.8/README.md
--rw-r--r--   0        0        0        0 2023-06-29 14:06:23.151726 redhat_qe_cloud_tools-1.0.8/clouds/__init__.py
--rw-r--r--   0        0        0      787 2023-06-29 14:06:23.151726 redhat_qe_cloud_tools-1.0.8/clouds/aws/README.md
--rw-r--r--   0        0        0        0 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/__init__.py
--rw-r--r--   0        0        0     4478 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/aws_utils.py
--rw-r--r--   0        0        0     4317 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/delete_s3_velero_bucket.py
--rw-r--r--   0        0        0      455 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/roles/README.md
--rw-r--r--   0        0        0        0 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/roles/__init__.py
--rw-r--r--   0        0        0     1193 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/roles/roles.py
--rw-r--r--   0        0        0      554 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/session_clients.py
--rw-r--r--   0        0        0     8197 2023-06-29 14:06:23.152726 redhat_qe_cloud_tools-1.0.8/clouds/aws/utilities/delete_aws_resources.py
--rw-r--r--   0        0        0      815 2023-06-29 14:06:23.153726 redhat_qe_cloud_tools-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-09 18:06:16.328454 redhat_qe_cloud_tools-1.0.9/LICENSE
+-rw-r--r--   0        0        0      852 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/__init__.py
+-rw-r--r--   0        0        0      787 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/__init__.py
+-rw-r--r--   0        0        0     4565 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/aws_utils.py
+-rw-r--r--   0        0        0     4317 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/delete_s3_velero_bucket.py
+-rw-r--r--   0        0        0      455 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/roles/README.md
+-rw-r--r--   0        0        0        0 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/roles/__init__.py
+-rw-r--r--   0        0        0     1193 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/roles/roles.py
+-rw-r--r--   0        0        0      554 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/session_clients.py
+-rw-r--r--   0        0        0     8197 2023-07-09 18:06:16.329454 redhat_qe_cloud_tools-1.0.9/clouds/aws/utilities/delete_aws_resources.py
+-rw-r--r--   0        0        0      850 2023-07-09 18:06:16.330454 redhat_qe_cloud_tools-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 redhat_qe_cloud_tools-1.0.9/PKG-INFO
```

### Comparing `redhat_qe_cloud_tools-1.0.8/LICENSE` & `redhat_qe_cloud_tools-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.8/README.md` & `redhat_qe_cloud_tools-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.8/clouds/aws/README.md` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/README.md`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.8/clouds/aws/aws_utils.py` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/aws_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import os
 from configparser import ConfigParser, NoOptionError, NoSectionError
 from http import HTTPStatus
 
 from simple_logger.logger import get_logger
 
+from clouds.aws.session_clients import ec2_client
+
 LOGGER = get_logger(name=__name__)
 AWS_CONFIG_FILE = os.environ.get("AWS_CONFIG_FILE", os.path.expanduser("~/.aws/config"))
 AWS_CREDENTIALS_FILE = os.environ.get(
     "AWS_CONFIG_FILE", os.path.expanduser("~/.aws/credentials")
 )
 
 
@@ -64,14 +66,15 @@
 
 
 def set_and_verify_aws_credentials():
     set_and_verify_existing_config_in_env_vars_or_file(
         vars_list=["AWS_ACCESS_KEY_ID", "AWS_SECRET_ACCESS_KEY"],
         file_path=AWS_CREDENTIALS_FILE,
     )
+    ec2_client().describe_regions()
 
 
 def set_and_verify_aws_config():
     set_and_verify_existing_config_in_env_vars_or_file(
         vars_list=["AWS_REGION"],
         file_path=AWS_CONFIG_FILE,
     )
```

### Comparing `redhat_qe_cloud_tools-1.0.8/clouds/aws/delete_s3_velero_bucket.py` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/delete_s3_velero_bucket.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.8/clouds/aws/roles/roles.py` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/roles/roles.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.8/clouds/aws/session_clients.py` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/session_clients.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.8/clouds/aws/utilities/delete_aws_resources.py` & `redhat_qe_cloud_tools-1.0.9/clouds/aws/utilities/delete_aws_resources.py`

 * *Files identical despite different names*

### Comparing `redhat_qe_cloud_tools-1.0.8/pyproject.toml` & `redhat_qe_cloud_tools-1.0.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -14,29 +14,30 @@
 
 [tool.isort]
 line_length = 88
 profile = "black"
 
 [tool.poetry]
 name = "redhat-qe-cloud-tools"
-version = "1.0.8"
+version = "1.0.9"
 description = "Python utilities to manage cloud services, such as AWS."
 authors = ["Meni Yakove", "Ruth Netser"]
 readme = "README.md"
 repository = "https://github.com/RedHatQE/cloud-tools"
 packages = [{include = "clouds"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-colorlog = "*"
-boto3 = "*"
-click = "*"
-configparser = "*"
-python-simple-logger="*"
-openshift-python-utilities = "*"
+boto3 = "^1.28.1"
+colorlog = "^6.7.0"
+openshift-python-utilities = "^4.14.2"
+python-simple-logger = "^1.0.5"
+click = "^8.1.4"
+configparser = "^6.0.0"
+
 
 [tool.poetry.dev-dependencies]
 ipython = "*"
 ipdb = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `redhat_qe_cloud_tools-1.0.8/PKG-INFO` & `redhat_qe_cloud_tools-1.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: redhat-qe-cloud-tools
-Version: 1.0.8
+Version: 1.0.9
 Summary: Python utilities to manage cloud services, such as AWS.
 Home-page: https://github.com/RedHatQE/cloud-tools
 Author: Meni Yakove
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: boto3
-Requires-Dist: click
-Requires-Dist: colorlog
-Requires-Dist: configparser
-Requires-Dist: openshift-python-utilities
-Requires-Dist: python-simple-logger
+Requires-Dist: boto3 (>=1.28.1,<2.0.0)
+Requires-Dist: click (>=8.1.4,<9.0.0)
+Requires-Dist: colorlog (>=6.7.0,<7.0.0)
+Requires-Dist: configparser (>=6.0.0,<7.0.0)
+Requires-Dist: openshift-python-utilities (>=4.14.2,<5.0.0)
+Requires-Dist: python-simple-logger (>=1.0.5,<2.0.0)
 Project-URL: Repository, https://github.com/RedHatQE/cloud-tools
 Description-Content-Type: text/markdown
 
 # cloud-tools
 Python utilities to manage cloud services, such as AWS.
 
 ## Local run
```

