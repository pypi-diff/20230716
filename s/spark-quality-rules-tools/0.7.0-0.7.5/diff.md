# Comparing `tmp/spark_quality_rules_tools-0.7.0.tar.gz` & `tmp/spark_quality_rules_tools-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.7.0.tar", last modified: Sat Jul 15 03:33:30 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.7.5.tar", last modified: Sat Jul 15 23:03:14 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.7.0.tar` & `spark_quality_rules_tools-0.7.5.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.179382 spark_quality_rules_tools-0.7.0/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.0/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-15 03:33:30.180382 spark_quality_rules_tools-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.7.0/README.md
--rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.7.0/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-15 03:33:30.181383 spark_quality_rules_tools-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-14 14:04:42.000000 spark_quality_rules_tools-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.130616 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.152103 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    56640 2023-07-14 14:06:25.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.169740 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.178382 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-15 03:33:30.151103 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-15 03:33:30.000000 spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.052348 spark_quality_rules_tools-0.7.5/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.5/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.7.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-15 23:03:14.052348 spark_quality_rules_tools-0.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.7.5/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.7.5/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-15 23:03:14.057344 spark_quality_rules_tools-0.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-15 23:03:09.000000 spark_quality_rules_tools-0.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.022058 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.046841 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    62117 2023-07-15 23:03:09.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.046841 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.046841 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.045387 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.7.0/LICENSE` & `spark_quality_rules_tools-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/PKG-INFO` & `spark_quality_rules_tools-0.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.7.0
+Version: 0.7.5
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.7.0/README.md` & `spark_quality_rules_tools-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/pyproject.toml` & `spark_quality_rules_tools-0.7.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/setup.py` & `spark_quality_rules_tools-0.7.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.7.0',
+    version='0.7.5',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/functions/generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,32 @@
                 else:
                     rs_dict["id"] = f"PE_{category_rule}_{table_name}_{rule_id}_{sequence}"
                 hamu_dict["class"] = rules_class
                 hamu_dict["config"] = rs_dict
     return hamu_dict, id_key_dict
 
 
+def dq_convert_url_bitbucket_artifactory(url_conf=None):
+    url = url_conf
+    url_conf_name = str(str(url).split("/")[-3])
+    url_conf_name = f"{url_conf_name}"
+    url_conf_zone = str(str(url).split("/")[-2])
+    uuaa_name = str(str(url).split("/")[-4])
+    url_conf = f"http://artifactory-gdt.central-02.nextgen.igrupobbva/" \
+               f"artifactory/gl-datio-generic-local/" \
+               f"dq/" \
+               f"pe/" \
+               f"{uuaa_name.lower()}/" \
+               f"{url_conf_zone.lower()}/" \
+               f"{url_conf_name.lower()}/" \
+               f"0.1.0/" \
+               f"{url_conf_name.lower()}-01.conf"
+    return url_conf
+
+
 def dq_creating_directory_hdfs(spark=None, path=None):
     from spark_quality_rules_tools import get_color, get_color_b
 
     sc = spark.sparkContext
     fs = spark._jvm.org.apache.hadoop.fs.FileSystem.get(spark._jsc.hadoopConfiguration())
     if path in ("", None):
         raise Exception(f'required variable path')
@@ -1155,7 +1173,115 @@
         conf2 = ConfigFactory.parse_string(json_file2)
         hocons_file2 = HOCONConverter.convert(conf2, "hocon")
 
         with open(dir_hocons_filename, "w") as f:
             f.write(hocons_file2)
 
         print(f"{get_color('HOCON CREATE:')} {get_color_b(dir_hocons_filename)}")
+
+
+def dq_extract_parameters_file_malla(file_conf=None, uuaa=None):
+    import os
+    import sys
+    import re
+    import json
+    from spark_quality_rules_tools import get_color, get_color_b
+
+    is_windows = sys.platform.startswith('win')
+    dir_confs_name = os.getenv('pj_dq_dir_confs_name')
+    if file_conf in ("", None):
+        raise Exception(f'required variable url_conf')
+    if dir_confs_name is None:
+        raise Exception(f'required environment: pj_dq_dir_confs_name')
+
+    url_conf_name = str(str(file_conf).split(".")[0])
+    uuaa_name = str(uuaa).upper()
+    dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
+    dir_confs_env_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS_ENV.json")
+
+    if is_windows:
+        dir_confs_filename = dir_confs_filename.replace("\\", "/")
+        dir_confs_env_parameters = dir_confs_env_parameters.replace("\\", "/")
+    os.makedirs(os.path.dirname(dir_confs_filename), exist_ok=True)
+
+    with open(file_conf) as file:
+        hammurabi_conf = file.read()
+    with open(dir_confs_filename, 'w') as file:
+        file.write(hammurabi_conf)
+    with open(dir_confs_filename) as f:
+        hammurabi_conf = f.read()
+    variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_list = list(set(variables_1 + variables_2))
+    variables_dict = {variables: "" for variables in variables_list if
+                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY", "TEST_PATH")}
+    env_variables = {key: f"%%PARM{i + 1}" for i, key in enumerate(variables_dict)}
+    env_controlm = {"CONTROLM_JOB_ID": "%%JOBNAME", "CONTROLM_JOB_FLOW": "%%SCHEDTAB"}
+    env_dict = dict()
+    env_dict["env"] = dict()
+    env_dict["env"].update(env_variables)
+    env_dict["env"].update(env_controlm)
+    with open(f"{dir_confs_env_parameters}", "w") as f:
+        json.dump(env_dict, f)
+
+    with open(f"{dir_confs_env_parameters}") as f:
+        parameter_conf = f.read()
+
+    print(f"{get_color('ENV:')} {get_color_b(parameter_conf)}")
+
+
+def dq_extract_parameters_bitbucket_malla(url_conf=None):
+    import os
+    import sys
+    import re
+    import json
+    import requests
+    from spark_quality_rules_tools import get_color, get_color_b
+
+    is_windows = sys.platform.startswith('win')
+    dir_confs_name = os.getenv('pj_dq_dir_confs_name')
+    if url_conf in ("", None):
+        raise Exception(f'required variable url_conf')
+    if dir_confs_name is None:
+        raise Exception(f'required environment: pj_dq_dir_confs_name')
+
+    url = dq_convert_url_bitbucket_artifactory(url_conf=url_conf)
+    url_conf_extension = str(str(url).split("/")[-1]).replace("-", "_").upper().strip()
+    url_conf_name = str(str(url_conf_extension).split(".")[0])
+    uuaa_name = str(str(url).split("/")[-2]).upper()
+    if not len(uuaa_name) == 4:
+        uuaa_name = str(str(url).split("/")[-5]).upper()
+    dir_confs_filename = os.path.join(dir_confs_name, uuaa_name, f"{url_conf_name}.txt")
+    dir_confs_env_parameters = os.path.join(dir_confs_name, uuaa_name, f"PARAMS_ENV.json")
+
+    if is_windows:
+        dir_confs_filename = dir_confs_filename.replace("\\", "/")
+        dir_confs_env_parameters = dir_confs_env_parameters.replace("\\", "/")
+    os.makedirs(os.path.dirname(dir_confs_filename), exist_ok=True)
+
+    with requests.get(url, stream=True, verify=True) as r:
+        r.raise_for_status()
+        with open(dir_confs_filename, 'wb+') as f:
+            for chunk in r.iter_content(chunk_size=8192):
+                f.write(chunk)
+    with open(dir_confs_filename) as f:
+        hammurabi_conf = f.read()
+    variables_1 = sorted(list(set(re.findall(r'{([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_2 = sorted(list(set(re.findall(r'{?([a-zA-Z_.-]+)}', hammurabi_conf))))
+    variables_list = list(set(variables_1 + variables_2))
+    variables_dict = {variables: "" for variables in variables_list if
+                      variables not in ("ARTIFACTORY_UNIQUE_CACHE", "SCHEMAS_REPOSITORY", "TEST_PATH")}
+
+    env_variables = {key: f"%%PARM{i + 1}" for i, key in enumerate(variables_dict)}
+    env_controlm = {"CONTROLM_JOB_ID": "%%JOBNAME", "CONTROLM_JOB_FLOW": "%%SCHEDTAB"}
+    env_dict = dict()
+    env_dict["env"] = dict()
+    env_dict["env"].update(env_variables)
+    env_dict["env"].update(env_controlm)
+
+    with open(f"{dir_confs_env_parameters}", "w") as f:
+        json.dump(env_dict, f)
+
+    with open(f"{dir_confs_env_parameters}") as f:
+        parameter_conf = f.read()
+
+    print(f"{get_color('ENV:')} {get_color_b(parameter_conf)}")
```

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.7.0
+Version: 0.7.5
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.7.0/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

