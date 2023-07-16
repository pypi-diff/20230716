# Comparing `tmp/foursight_cgap-3.5.0.2b9.tar.gz` & `tmp/foursight_cgap-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foursight_cgap-3.5.0.2b9.tar", max compression
+gzip compressed data, was "foursight_cgap-3.6.0.tar", max compression
```

## Comparing `foursight_cgap-3.5.0.2b9.tar` & `foursight_cgap-3.6.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.5.0.2b9/LICENSE.txt
--rw-r--r--   0        0        0        0 2023-06-09 17:29:40.788939 foursight_cgap-3.5.0.2b9/chalicelib_cgap/__init__.py
--rw-r--r--   0        0        0     1038 2023-06-09 17:29:40.789199 foursight_cgap-3.5.0.2b9/chalicelib_cgap/app_utils.py
--rw-r--r--   0        0        0      952 2023-06-09 17:29:40.789412 foursight_cgap-3.5.0.2b9/chalicelib_cgap/buckets.py
--rw-r--r--   0        0        0     4805 2023-07-07 22:28:47.480273 foursight_cgap-3.5.0.2b9/chalicelib_cgap/check_schedules.py
--rw-r--r--   0        0        0    17006 2023-06-17 14:10:51.489200 foursight_cgap-3.5.0.2b9/chalicelib_cgap/check_setup.json
--rw-r--r--   0        0        0     9278 2023-06-09 17:29:40.790018 foursight_cgap-3.5.0.2b9/chalicelib_cgap/check_setup.json-local
--rw-r--r--   0        0        0      249 2023-06-09 17:29:40.790103 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/__init__.py
--rw-r--r--   0        0        0     9636 2023-06-09 17:29:40.790318 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/audit_checks.py
--rw-r--r--   0        0        0    11502 2023-06-09 17:29:40.790849 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/deployment_checks.py
--rw-r--r--   0        0        0     2874 2023-06-09 17:29:40.791248 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/ecs_checks.py
--rw-r--r--   0        0        0     3919 2023-06-09 17:29:40.791502 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/es_checks.py
--rw-r--r--   0        0        0    11577 2023-06-09 17:29:40.791624 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/clone_utils.py
--rw-r--r--   0        0        0      262 2023-06-09 17:29:40.791685 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/confchecks.py
--rw-r--r--   0        0        0      333 2023-06-09 17:29:40.791742 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/constants.py
--rw-r--r--   0        0        0    13110 2023-06-09 17:29:40.791986 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/lifecycle_utils.py
--rw-r--r--   0        0        0     8518 2023-06-09 17:29:40.792053 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/linecount_dicts.py
--rw-r--r--   0        0        0     4014 2023-06-09 17:29:40.792137 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/utils.py
--rw-r--r--   0        0        0    39030 2023-06-09 17:29:40.792368 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/wfr_utils.py
--rw-r--r--   0        0        0     2571 2023-06-09 17:29:40.792453 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/wfrset_utils.py
--rw-r--r--   0        0        0     7577 2023-06-09 17:29:40.792770 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/lifecycle_checks.py
--rw-r--r--   0        0        0    26338 2023-06-09 17:29:40.793201 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/system_checks.py
--rw-r--r--   0        0        0    58825 2023-06-09 17:29:40.793706 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/wfr_checks.py
--rw-r--r--   0        0        0    58234 2023-07-07 22:28:47.481409 foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/wrangler_checks.py
--rw-r--r--   0        0        0      772 2023-06-09 17:29:40.794456 foursight_cgap-3.5.0.2b9/chalicelib_cgap/deploy.py
--rw-r--r--   0        0        0      616 2023-06-09 17:29:40.794522 foursight_cgap-3.5.0.2b9/chalicelib_cgap/package.py
--rw-r--r--   0        0        0      315 2023-06-09 17:29:40.794978 foursight_cgap-3.5.0.2b9/chalicelib_cgap/vars.py
--rw-r--r--   0        0        0     1174 2023-07-13 21:23:24.241416 foursight_cgap-3.5.0.2b9/pyproject.toml
--rw-r--r--   0        0        0     1293 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.2b9/setup.py
--rw-r--r--   0        0        0      981 1970-01-01 00:00:00.000000 foursight_cgap-3.5.0.2b9/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-07 10:09:15.330430 foursight_cgap-3.6.0/LICENSE.txt
+-rw-r--r--   0        0        0        0 2023-06-09 17:29:40.788939 foursight_cgap-3.6.0/chalicelib_cgap/__init__.py
+-rw-r--r--   0        0        0     1071 2023-07-16 13:30:43.380566 foursight_cgap-3.6.0/chalicelib_cgap/app_utils.py
+-rw-r--r--   0        0        0      952 2023-06-09 17:29:40.789412 foursight_cgap-3.6.0/chalicelib_cgap/buckets.py
+-rw-r--r--   0        0        0     4805 2023-07-16 13:30:43.381482 foursight_cgap-3.6.0/chalicelib_cgap/check_schedules.py
+-rw-r--r--   0        0        0    17006 2023-06-17 14:10:51.489200 foursight_cgap-3.6.0/chalicelib_cgap/check_setup.json
+-rw-r--r--   0        0        0     9278 2023-06-09 17:29:40.790018 foursight_cgap-3.6.0/chalicelib_cgap/check_setup.json-local
+-rw-r--r--   0        0        0      249 2023-06-09 17:29:40.790103 foursight_cgap-3.6.0/chalicelib_cgap/checks/__init__.py
+-rw-r--r--   0        0        0     9636 2023-06-09 17:29:40.790318 foursight_cgap-3.6.0/chalicelib_cgap/checks/audit_checks.py
+-rw-r--r--   0        0        0    11502 2023-06-09 17:29:40.790849 foursight_cgap-3.6.0/chalicelib_cgap/checks/deployment_checks.py
+-rw-r--r--   0        0        0     2874 2023-06-09 17:29:40.791248 foursight_cgap-3.6.0/chalicelib_cgap/checks/ecs_checks.py
+-rw-r--r--   0        0        0     3919 2023-06-09 17:29:40.791502 foursight_cgap-3.6.0/chalicelib_cgap/checks/es_checks.py
+-rw-r--r--   0        0        0    11577 2023-06-09 17:29:40.791624 foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/clone_utils.py
+-rw-r--r--   0        0        0      262 2023-06-09 17:29:40.791685 foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/confchecks.py
+-rw-r--r--   0        0        0      333 2023-06-09 17:29:40.791742 foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/constants.py
+-rw-r--r--   0        0        0    13110 2023-06-09 17:29:40.791986 foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/lifecycle_utils.py
+-rw-r--r--   0        0        0     8518 2023-06-09 17:29:40.792053 foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/linecount_dicts.py
+-rw-r--r--   0        0        0     4014 2023-06-09 17:29:40.792137 foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/utils.py
+-rw-r--r--   0        0        0    39030 2023-06-09 17:29:40.792368 foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/wfr_utils.py
+-rw-r--r--   0        0        0     2571 2023-06-09 17:29:40.792453 foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/wfrset_utils.py
+-rw-r--r--   0        0        0     7577 2023-06-09 17:29:40.792770 foursight_cgap-3.6.0/chalicelib_cgap/checks/lifecycle_checks.py
+-rw-r--r--   0        0        0    26338 2023-07-16 12:57:18.590153 foursight_cgap-3.6.0/chalicelib_cgap/checks/system_checks.py
+-rw-r--r--   0        0        0    58825 2023-06-09 17:29:40.793706 foursight_cgap-3.6.0/chalicelib_cgap/checks/wfr_checks.py
+-rw-r--r--   0        0        0    58234 2023-07-16 13:30:43.383060 foursight_cgap-3.6.0/chalicelib_cgap/checks/wrangler_checks.py
+-rw-r--r--   0        0        0      772 2023-06-09 17:29:40.794456 foursight_cgap-3.6.0/chalicelib_cgap/deploy.py
+-rw-r--r--   0        0        0      616 2023-06-09 17:29:40.794522 foursight_cgap-3.6.0/chalicelib_cgap/package.py
+-rw-r--r--   0        0        0      315 2023-06-09 17:29:40.794978 foursight_cgap-3.6.0/chalicelib_cgap/vars.py
+-rw-r--r--   0        0        0     1135 2023-07-16 13:33:27.623113 foursight_cgap-3.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1284 1970-01-01 00:00:00.000000 foursight_cgap-3.6.0/setup.py
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 foursight_cgap-3.6.0/PKG-INFO
```

### Comparing `foursight_cgap-3.5.0.2b9/LICENSE.txt` & `foursight_cgap-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/app_utils.py` & `foursight_cgap-3.6.0/chalicelib_cgap/app_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     apply_identity_globally()
 
     # Overridden from subclass.
     APP_PACKAGE_NAME = "foursight-cgap"
 
     # Note that this is set in the new (as of August 2022) apply_identity code;
     # see foursight-core/foursight_core/{app_utils.py,identity.py}.
-    es_host = os.environ.get("ES_HOST")
+    es_host = os.environ.get("ES_HOST_LOCAL", os.environ.get("ES_HOST"))
     if not es_host:
         raise Exception("Foursight ES_HOST environment variable not set!")
     HOST = es_host
 
     # overwriting parent class
     prefix = FOURSIGHT_PREFIX
     FAVICON = 'https://cgap-dbmi.hms.harvard.edu/favicon.ico'
```

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/buckets.py` & `foursight_cgap-3.6.0/chalicelib_cgap/buckets.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/check_schedules.py` & `foursight_cgap-3.6.0/chalicelib_cgap/check_schedules.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/check_setup.json` & `foursight_cgap-3.6.0/chalicelib_cgap/check_setup.json`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/check_setup.json-local` & `foursight_cgap-3.6.0/chalicelib_cgap/check_setup.json-local`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/audit_checks.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/audit_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/deployment_checks.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/deployment_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/ecs_checks.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/ecs_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/es_checks.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/es_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/clone_utils.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/clone_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/lifecycle_utils.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/lifecycle_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/linecount_dicts.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/linecount_dicts.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/utils.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/wfr_utils.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/wfr_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/helpers/wfrset_utils.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/helpers/wfrset_utils.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/lifecycle_checks.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/lifecycle_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/system_checks.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/system_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/wfr_checks.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/wfr_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/checks/wrangler_checks.py` & `foursight_cgap-3.6.0/chalicelib_cgap/checks/wrangler_checks.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/deploy.py` & `foursight_cgap-3.6.0/chalicelib_cgap/deploy.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/chalicelib_cgap/package.py` & `foursight_cgap-3.6.0/chalicelib_cgap/package.py`

 * *Files identical despite different names*

### Comparing `foursight_cgap-3.5.0.2b9/pyproject.toml` & `foursight_cgap-3.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "foursight-cgap"
-version = "3.5.0.2b9"
+version = "3.6.0"
 description = "Serverless Chalice Application for Monitoring"
 authors = ["4DN-DCIC Team <support@4dnucleome.org>"]
 license = "MIT"
 packages = [
   { include = "chalicelib_cgap" }
 ]
 
@@ -21,16 +21,15 @@
 elasticsearch = "^7.13.4"
 elasticsearch-dsl = "^7.0.0"
 gitpython = "^3.1.2"
 pytz = "^2020.1"
 magma-suite = "^1.2.2"
 tibanna-ff = "^1.3.0"
 MarkupSafe = "1.1.1"
-#foursight-core = "4.3.0.2b6"
-foursight-core = "4.3.0.1b54"
+foursight-core = "4.4.0"
 # use below for tests but not for deployment
 #foursight-core = { git = "https://github.com/4dn-dcic/foursight-core.git", branch="core2" }
 cgap-pipeline-utils = "23.0"
 pytest = "5.1.2"
 
 [tool.poetry.dev-dependencies]
 chalice = "^1.21.6"
```

### Comparing `foursight_cgap-3.5.0.2b9/setup.py` & `foursight_cgap-3.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
  'MarkupSafe==1.1.1',
  'PyJWT>=2.5.0,<3.0.0',
  'cgap-pipeline-utils==23.0',
  'click>=7.1.2,<8.0.0',
  'dcicutils==7.6.0.1b4',
  'elasticsearch-dsl>=7.0.0,<8.0.0',
  'elasticsearch>=7.13.4,<8.0.0',
- 'foursight-core==4.3.0.1b54',
+ 'foursight-core==4.4.0',
  'geocoder==1.38.1',
  'gitpython>=3.1.2,<4.0.0',
  'google-api-python-client>=1.12.5,<2.0.0',
  'magma-suite>=1.2.2,<2.0.0',
  'pytest==5.1.2',
  'pytz>=2020.1,<2021.0',
  'tibanna-ff>=1.3.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['publish-to-pypi = '
                      'dcicutils.scripts.publish_to_pypi:main']}
 
 setup_kwargs = {
     'name': 'foursight-cgap',
-    'version': '3.5.0.2b9',
+    'version': '3.6.0',
     'description': 'Serverless Chalice Application for Monitoring',
     'long_description': 'None',
     'author': '4DN-DCIC Team',
     'author_email': 'support@4dnucleome.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `foursight_cgap-3.5.0.2b9/PKG-INFO` & `foursight_cgap-3.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foursight-cgap
-Version: 3.5.0.2b9
+Version: 3.6.0
 Summary: Serverless Chalice Application for Monitoring
 License: MIT
 Author: 4DN-DCIC Team
 Author-email: support@4dnucleome.org
 Requires-Python: >=3.7.1,<3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Requires-Dist: MarkupSafe (==1.1.1)
 Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
 Requires-Dist: cgap-pipeline-utils (==23.0)
 Requires-Dist: click (>=7.1.2,<8.0.0)
 Requires-Dist: dcicutils (==7.6.0.1b4)
 Requires-Dist: elasticsearch (>=7.13.4,<8.0.0)
 Requires-Dist: elasticsearch-dsl (>=7.0.0,<8.0.0)
-Requires-Dist: foursight-core (==4.3.0.1b54)
+Requires-Dist: foursight-core (==4.4.0)
 Requires-Dist: geocoder (==1.38.1)
 Requires-Dist: gitpython (>=3.1.2,<4.0.0)
 Requires-Dist: google-api-python-client (>=1.12.5,<2.0.0)
 Requires-Dist: magma-suite (>=1.2.2,<2.0.0)
 Requires-Dist: pytest (==5.1.2)
 Requires-Dist: pytz (>=2020.1,<2021.0)
 Requires-Dist: tibanna-ff (>=1.3.0,<2.0.0)
```

