# Comparing `tmp/spark_quality_rules_tools-0.7.5.tar.gz` & `tmp/spark_quality_rules_tools-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_quality_rules_tools-0.7.5.tar", last modified: Sat Jul 15 23:03:14 2023, max compression
+gzip compressed data, was "spark_quality_rules_tools-0.8.0.tar", last modified: Sun Jul 16 01:08:14 2023, max compression
```

## Comparing `spark_quality_rules_tools-0.7.5.tar` & `spark_quality_rules_tools-0.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.052348 spark_quality_rules_tools-0.7.5/
--rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.5/LICENSE
--rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.7.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4041 2023-07-15 23:03:14.052348 spark_quality_rules_tools-0.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.7.5/README.md
--rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.7.5/pyproject.toml
--rw-rw-rw-   0        0        0       86 2023-07-15 23:03:14.057344 spark_quality_rules_tools-0.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1210 2023-07-15 23:03:09.000000 spark_quality_rules_tools-0.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.022058 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/
--rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.046841 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/functions/
--rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/functions/__init__.py
--rw-rw-rw-   0        0        0    62117 2023-07-15 23:03:09.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/functions/generator.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.046841 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/
--rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/color.py
--rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resolve.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.046841 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/
--rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf
--rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
--rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/rules.json
--rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/rules.py
-drwxrwxrwx   0        0        0        0 2023-07-15 23:03:14.045387 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/
--rw-rw-rw-   0        0        0     4041 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      205 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-07-15 23:03:13.000000 spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 01:08:14.946178 spark_quality_rules_tools-0.8.0/
+-rw-rw-rw-   0        0        0     1092 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0       50 2023-06-14 13:33:57.000000 spark_quality_rules_tools-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4041 2023-07-16 01:08:14.946178 spark_quality_rules_tools-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3242 2023-06-14 13:39:58.000000 spark_quality_rules_tools-0.8.0/README.md
+-rw-rw-rw-   0        0        0      685 2023-07-06 02:24:33.000000 spark_quality_rules_tools-0.8.0/pyproject.toml
+-rw-rw-rw-   0        0        0       86 2023-07-16 01:08:14.946178 spark_quality_rules_tools-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1210 2023-07-16 01:08:12.000000 spark_quality_rules_tools-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:08:14.896061 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/
+-rw-rw-rw-   0        0        0     2790 2023-07-06 07:26:52.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:08:14.917814 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/functions/
+-rw-rw-rw-   0        0        0        0 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/functions/__init__.py
+-rw-rw-rw-   0        0        0    62025 2023-07-16 01:08:12.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/functions/generator.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:08:14.938160 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/
+-rw-rw-rw-   0        0        0       75 2022-12-01 18:37:15.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/__init__.py
+-rw-rw-rw-   0        0        0      416 2023-04-12 03:25:49.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/color.py
+-rw-rw-rw-   0        0        0     2138 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resolve.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:08:14.946178 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resource/
+-rw-rw-rw-   0        0        0      532 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf
+-rw-rw-rw-   0        0        0      742 2023-06-30 23:04:24.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf
+-rw-rw-rw-   0        0        0    25810 2023-07-14 13:19:59.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resource/rules.json
+-rw-rw-rw-   0        0        0     3920 2023-07-14 13:01:54.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/rules.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:08:14.916813 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools.egg-info/
+-rw-rw-rw-   0        0        0     4041 2023-07-16 01:08:14.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2023-07-16 01:08:14.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 01:08:14.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      205 2023-07-16 01:08:14.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-07-16 01:08:14.000000 spark_quality_rules_tools-0.8.0/spark_quality_rules_tools.egg-info/top_level.txt
```

### Comparing `spark_quality_rules_tools-0.7.5/LICENSE` & `spark_quality_rules_tools-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/PKG-INFO` & `spark_quality_rules_tools-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark_quality_rules_tools
-Version: 0.7.5
+Version: 0.8.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.7.5/README.md` & `spark_quality_rules_tools-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/pyproject.toml` & `spark_quality_rules_tools-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/setup.py` & `spark_quality_rules_tools-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 setuppath = os.path.dirname(os.path.abspath(__file__))
 
 setup(
     name='spark_quality_rules_tools',
     packages=find_packages(),
-    version='0.7.5',
+    version='0.8.0',
     description='spark_quality_rules_tools',
     long_description=open(os.path.join(setuppath, 'README.md')).read(),
     long_description_content_type="text/markdown",
     author='Jonathan Quiza',
     author_email='jony327@gmail.com',
     url='https://github.com/jonaqp/spark_quality_rules_tools/',
     download_url='https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip',
```

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/__init__.py` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/functions/generator.py` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/functions/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                         rules_value = dict(type="", paths="")
                     else:
                         rules_value = rule_dtype[2]
                     rs_dict[rule_name] = rules_value
                 if static_id:
                     rs_dict["id"] = static_id
                 else:
+                    rule_id = str(rule_id).replace("-1", "").replace("-2", "").strip()
                     rs_dict["id"] = f"PE_{category_rule}_{table_name}_{rule_id}_{sequence}"
                 hamu_dict["class"] = rules_class
                 hamu_dict["config"] = rs_dict
     return hamu_dict, id_key_dict
 
 
 def dq_convert_url_bitbucket_artifactory(url_conf=None):
@@ -1095,18 +1096,18 @@
         StructField("SUBPARTITION_ONE", StringType(), True),
         StructField("SUBPARTITION_TWO", StringType(), True),
         StructField("VERSION", StringType(), True),
         StructField("PERIODICITY", StringType(), True),
         StructField("STATIC_ID", StringType(), True)
     ])
     df = spark.createDataFrame(df, schema=schema)
-    df = df.orderBy("TABLE", "FIELD", "SUBPARTITION_ONE", "SUBPARTITION_TWO", "VERSION")
+    df = df.orderBy("TABLE", "FIELD", "VERSION")
     df = df.withColumn('ORDEN', func.row_number().over(Window.partitionBy(func.lit('1')).orderBy(func.lit('1'))))
-    windowSpec = Window.partitionBy("TABLE", "FIELD", "SUBPARTITION_ONE", "SUBPARTITION_TWO", "VERSION").orderBy("ORDEN")
-    df = df.withColumn("SEQUENCE", func.row_number().over(windowSpec)).orderBy("ORDEN")
+    window_spec = Window.partitionBy("TABLE", "VERSION").orderBy("ORDEN")
+    df = df.withColumn("SEQUENCE", func.row_number().over(window_spec)).orderBy("ORDEN")
     table_dict = dict()
     table_list = list()
 
     for row in df.collect():
         table_name = str(row["TABLE"]).strip().lower()
         field_name = str(row["FIELD"]).strip().lower()
         subpartition_one = row["SUBPARTITION_ONE"]
@@ -1144,20 +1145,18 @@
                 table_dict[table_name]["hammurabi"]["dataFrameInfo"]["subset"] = "cutoff_date='${?CUTOFF_DATE}' and " \
                                                                                  f"{subpartition_one}=" + "'${?SUBPATITION_ONE}' and " \
                                                                                                           f"{subpartition_two}=" + "'${?SUBPATITION_TWO}'"
             table_dict[table_name]["hammurabi"]["dataFrameInfo"]["uuaa"] = uuaa_name
             table_dict[table_name]["hammurabi"]["Input"] = dict()
             table_dict[table_name]["hammurabi"]["Input"]["options"] = dict(includeMetadataAndDeleted=True, overrideSchema=True)
             table_dict[table_name]["hammurabi"]["Input"]["paths"] = [f"/data/master/{uuaa_name}/data/{table_name}"]
-            table_dict[table_name]["hammurabi"]["Input"]["type"] = "parquet"
             table_dict[table_name]["hammurabi"]["Input"]["schema"] = dict(path="${ARTIFACTORY_UNIQUE_CACHE}/artifactory/${SCHEMAS_REPOSITORY}"
                                                                                f"/schemas/pe/{uuaa_name}"
-                                                                               f"/master/{uuaa_tag}/latest/{uuaa_tag}.output.schema",
-                                                                          type="parquet")
-
+                                                                               f"/master/{uuaa_tag}/latest/{uuaa_tag}.output.schema")
+            table_dict[table_name]["hammurabi"]["Input"]["type"] = "parquet"
             table_dict[table_name]["hammurabi"]["rules"] = list()
         table_dict[table_name]["hammurabi"]["rules"].append(hamu_dict)
         table_list.append(table_name)
 
     table_unique_list = list(set(table_list))
 
     for table in table_unique_list:
```

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resolve.py` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resolve.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/resolve_edge.conf` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resource/resolve_edge.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resource/resolve_sandbox.conf`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/resource/rules.json` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/resource/rules.json`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools/utils/rules.py` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools/utils/rules.py`

 * *Files identical despite different names*

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/PKG-INFO` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spark-quality-rules-tools
-Version: 0.7.5
+Version: 0.8.0
 Summary: spark_quality_rules_tools
 Home-page: https://github.com/jonaqp/spark_quality_rules_tools/
 Author: Jonathan Quiza
 Author-email: jony327@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/jonaqp/spark_quality_rules_tools/archive/main.zip
 Keywords: spark,dq,rules,hammurabies
```

### Comparing `spark_quality_rules_tools-0.7.5/spark_quality_rules_tools.egg-info/SOURCES.txt` & `spark_quality_rules_tools-0.8.0/spark_quality_rules_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

