# Comparing `tmp/spark_quality_rules_tools-0.8.5.tar.gz` & `tmp/spark_quality_rules_tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.8.5.tar", last modified: Sun Jul 16 01:29:30 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.9.0.tar", last modified: Sun Jul 16 03:49:17 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.8.5.tar` & `spark_quality_rules_tools-0.9.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:29:30.255872 spark_quality_rules_tools-0.8.5/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.8.5/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.8.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-16 01:29:30.256873 spark_quality_rules_tools-0.8.5/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.8.5/README.md
--rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.8.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-16 01:29:30.256873 spark_quality_rules_tools-0.8.5/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-16 01:29:29.000000 spark_quality_rules_tools-0.8.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:29:30.238347 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     3068 2023-07-16 01:29:29.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:29:30.251871 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    62025 2023-07-16 01:08:12.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:29:30.253872 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:29:30.255872 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:29:30.250871 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-16 01:29:30.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-16 01:29:30.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:29:30.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-16 01:29:30.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-16 01:29:30.000000 spark_quality_rules_tools-0.8.5/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.105161 spark_quality_rules_tools-0.9.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-16 03:49:17.105161 spark_quality_rules_tools-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.9.0/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-16 03:49:17.106161 spark_quality_rules_tools-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-16 03:48:50.000000 spark_quality_rules_tools-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.083156 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     3068 2023-07-16 01:29:29.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.100160 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    62025 2023-07-16 03:48:50.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.103160 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.104160 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:49:17.098159 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-16 03:49:17.000000 spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.8.5/LICENSE` & `spark_quality_rules_tools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/PKG-INFO` & `spark_quality_rules_tools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.8.5
+Version: 0.9.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.8.5/README.md` & `spark_quality_rules_tools-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/pyproject.toml` & `spark_quality_rules_tools-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/setup.py` & `spark_quality_rules_tools-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.8.5',
+    version='0.9.0',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/functions/generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,21 +55,21 @@
     url = url_conf
     url_conf_name = str(str(url).split("/")[-3])
     url_conf_name = f"{url_conf_name}"
     url_conf_zone = str(str(url).split("/")[-2])
     uuaa_name = str(str(url).split("/")[-4])
     url_conf = f"http://artifactory-gdt.central-02.nextgen.igrupobbva/" \
                f"artifactory/gl-datio-generic-local/" \
-               f"dq/" \
+               f"kirby/" \
                f"pe/" \
                f"{uuaa_name.lower()}/" \
                f"{url_conf_zone.lower()}/" \
                f"{url_conf_name.lower()}/" \
                f"0.1.0/" \
-               f"{url_conf_name.lower()}-01.conf"
+               f"{url_conf_name.lower()}.conf"
     return url_conf
 
 
 def dq_creating_directory_hdfs(spark=None, path=None):
     from spark_quality_rules_tools import get_color, get_color_b
 
     sc = spark.sparkContext
```

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.8.5
+Version: 0.9.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.8.5/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.9.0/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

