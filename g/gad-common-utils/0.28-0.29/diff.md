# Comparing `tmp/gad_common_utils-0.28.tar.gz` & `tmp/gad_common_utils-0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gad_common_utils-0.28.tar", last modified: Thu Jul  6 12:10:53 2023, max compression
+gzip compressed data, was "gad_common_utils-0.29.tar", last modified: Sun Jul 16 12:02:44 2023, max compression
```

## Comparing `gad_common_utils-0.28.tar` & `gad_common_utils-0.29.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:53.604667 gad_common_utils-0.28/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:53.600667 gad_common_utils-0.28/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:53.600667 gad_common_utils-0.28/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-06 12:10:38.000000 gad_common_utils-0.28/.github/workflows/black-format-checker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-06 12:10:38.000000 gad_common_utils-0.28/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-06 12:10:38.000000 gad_common_utils-0.28/.github/workflows/pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-06 12:10:38.000000 gad_common_utils-0.28/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-06 12:10:38.000000 gad_common_utils-0.28/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 12:10:53.604667 gad_common_utils-0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-06 12:10:38.000000 gad_common_utils-0.28/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:53.604667 gad_common_utils-0.28/common_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-06 12:10:53.000000 gad_common_utils-0.28/common_utils/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/data_loading_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/data_type_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/date_time_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/dynamodb_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/dynamodb_ray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/files_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)    29208 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/gad_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/gad_utils_additionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/json_schema_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/run_athena_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/s3_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/sql_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-06 12:10:38.000000 gad_common_utils-0.28/common_utils/string_transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:53.604667 gad_common_utils-0.28/gad_common_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-06 12:10:53.000000 gad_common_utils-0.28/gad_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-06 12:10:53.000000 gad_common_utils-0.28/gad_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:10:53.000000 gad_common_utils-0.28/gad_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-06 12:10:53.000000 gad_common_utils-0.28/gad_common_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-06 12:10:53.000000 gad_common_utils-0.28/gad_common_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-06 12:10:38.000000 gad_common_utils-0.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:10:53.604667 gad_common_utils-0.28/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:53.604667 gad_common_utils-0.28/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:10:38.000000 gad_common_utils-0.28/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-06 12:10:38.000000 gad_common_utils-0.28/tests/test_json_schema_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.948770 gad_common_utils-0.29/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.944769 gad_common_utils-0.29/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.944769 gad_common_utils-0.29/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.github/workflows/black-format-checker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.github/workflows/pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-16 12:02:35.000000 gad_common_utils-0.29/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-16 12:02:44.948770 gad_common_utils-0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-16 12:02:35.000000 gad_common_utils-0.29/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.944769 gad_common_utils-0.29/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-16 12:02:44.000000 gad_common_utils-0.29/common_utils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/data_loading_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/data_type_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/date_time_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/dynamodb_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/dynamodb_ray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/files_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29472 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/gad_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      895 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/gad_utils_additionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/json_schema_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/run_athena_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/s3_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/sql_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-16 12:02:35.000000 gad_common_utils-0.29/common_utils/string_transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.948770 gad_common_utils-0.29/gad_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-16 12:02:44.000000 gad_common_utils-0.29/gad_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-16 12:02:35.000000 gad_common_utils-0.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 12:02:44.948770 gad_common_utils-0.29/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:44.948770 gad_common_utils-0.29/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 12:02:35.000000 gad_common_utils-0.29/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-16 12:02:35.000000 gad_common_utils-0.29/tests/test_json_schema_methods.py
```

### Comparing `gad_common_utils-0.28/.github/workflows/black-format-checker.yml` & `gad_common_utils-0.29/.github/workflows/black-format-checker.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/.github/workflows/publish-to-pypi.yml` & `gad_common_utils-0.29/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/.github/workflows/pytest.yml` & `gad_common_utils-0.29/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/PKG-INFO` & `gad_common_utils-0.29/gad_common_utils.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gad_common_utils
-Version: 0.28
+Name: gad-common-utils
+Version: 0.29
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.28/common_utils/data_loading_management.py` & `gad_common_utils-0.29/common_utils/data_loading_management.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/data_type_conversion.py` & `gad_common_utils-0.29/common_utils/data_type_conversion.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/date_time_methods.py` & `gad_common_utils-0.29/common_utils/date_time_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/dynamodb_methods.py` & `gad_common_utils-0.29/common_utils/dynamodb_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/files_methods.py` & `gad_common_utils-0.29/common_utils/files_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/gad_utils.py` & `gad_common_utils-0.29/common_utils/gad_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """
     WORK_DIR = "/opt/aiola/projects"
     SUB_FOLDER = os.environ.get("DEPLOYMENT_DIR", content_path)
     PROJECT_DIR = f"{WORK_DIR}/{SUB_FOLDER}/{project}"
     DBT_OUTPUT_DIR = "/opt/airflow/logs"
     PYTHON_DIR = f"{PROJECT_DIR}/python"
     DBT_DIR = f"{PROJECT_DIR}/dbt"
-    GX_DIR = f"{PROJECT_DIR}/gx/checkpoints_executions"
+    GX_DIR = f"{PROJECT_DIR}/gx"
     CONFIG_DIR = f"{PROJECT_DIR}/configuration"
 
     paths = {
         "WORK_DIR": WORK_DIR,
         "SUB_FOLDER": SUB_FOLDER,
         "PROJECT_DIR": PROJECT_DIR,
         "DBT_DIR": DBT_DIR,
@@ -189,15 +189,18 @@
         'executable' key of the task_dict.
         """
         if task_dict["task_type"] == "dbt":
             return ["dbt", task_dict["executable"]]
         elif task_dict["task_type"] == "python":
             return ["python", f"{paths['PYTHON_DIR']}/{task_dict['executable']}.py"]
         elif task_dict["task_type"] == "gx":
-            return ["python", f"{paths['GX_DIR']}/{task_dict['executable']}.py"]
+            return [
+                "python",
+                f"{paths['GX_DIR']}/checkpoints_executions/{task_dict['executable']}.py",
+            ]
 
     def return_command_args(task_dict: dict, xcom_pull_task_id: str) -> list:
         """Returns a list of command-line arguments based on task_dict and configs.
 
         Args:
         task_dict: dict
         A dictionary containing information about the task to be executed.
@@ -705,18 +708,24 @@
             slack_api_token_secret = Secret(
                 deploy_type="env",
                 deploy_target="api_token",
                 secret="gad-slack-api-token",
                 key="api_token",
             )
 
+            env_vars_to_pod = []
+            if task["task_type"] == "gx":
+                env_vars_to_pod.append(
+                    {"name": "GX_ROOT_DIR", "value": paths["GX_DIR"]}
+                )
+
             kubernetes_task = KubernetesPodOperator(
                 volumes=volumes,
                 volume_mounts=volumes_mounts,
-                env_vars=[],
+                env_vars=env_vars_to_pod,
                 env_from=[envConfigMap],
                 namespace="default",
                 labels={"Task": task["task_type"]},
                 image_pull_policy="Never",
                 name=task["task_id"],
                 task_id=task["task_id"],
                 is_delete_operator_pod=True,
```

### Comparing `gad_common_utils-0.28/common_utils/gad_utils_additionals.py` & `gad_common_utils-0.29/common_utils/gad_utils_additionals.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/json_schema_methods.py` & `gad_common_utils-0.29/common_utils/json_schema_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/run_athena_query.py` & `gad_common_utils-0.29/common_utils/run_athena_query.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/s3_methods.py` & `gad_common_utils-0.29/common_utils/s3_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/sql_methods.py` & `gad_common_utils-0.29/common_utils/sql_methods.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/common_utils/string_transformations.py` & `gad_common_utils-0.29/common_utils/string_transformations.py`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/gad_common_utils.egg-info/PKG-INFO` & `gad_common_utils-0.29/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gad-common-utils
-Version: 0.28
+Name: gad_common_utils
+Version: 0.29
 Summary: gad utility
 Project-URL: Homepage, http://gad-co.ml
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `gad_common_utils-0.28/gad_common_utils.egg-info/SOURCES.txt` & `gad_common_utils-0.29/gad_common_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/pyproject.toml` & `gad_common_utils-0.29/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gad_common_utils-0.28/tests/test_json_schema_methods.py` & `gad_common_utils-0.29/tests/test_json_schema_methods.py`

 * *Files identical despite different names*

