# Comparing `tmp/ibdx-0.3.0.tar.gz` & `tmp/ibdx-0.3.1.tar.gz`

## Comparing `ibdx-0.3.0.tar` & `ibdx-0.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ibdx-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ibdx-0.3.0/demo.env
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/__main__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/cli.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/configs.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/deps.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/ibd_backup.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/ibd_restore.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/mysql_db_quick.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 ibdx-0.3.0/ibdx/tools.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 ibdx-0.3.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ibdx-0.3.0/LICENSE
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 ibdx-0.3.0/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ibdx-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ibdx-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ibdx-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ibdx-0.3.1/demo.env
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/__main__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/cli.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/configs.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/deps.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/ibd_backup.py
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/ibd_restore.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/mysql_db_quick.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/tools.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 ibdx-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ibdx-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 ibdx-0.3.1/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ibdx-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ibdx-0.3.1/PKG-INFO
```

### Comparing `ibdx-0.3.0/ibdx/cli.py` & `ibdx-0.3.1/ibdx/cli.py`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.0/ibdx/ibd_backup.py` & `ibdx-0.3.1/ibdx/ibd_backup.py`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.0/ibdx/ibd_restore.py` & `ibdx-0.3.1/ibdx/ibd_restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,20 +33,22 @@
             f'{tables_pattern}.ibd',
         )
         target_sql_files = fnmatch.filter(
             zip_file.namelist(),
             f'{tables_pattern}.sql',
         )
 
+
         for sql_file in target_sql_files:
             table = sql_file.rsplit('.')[0]
             print(f"executing sql: {table}")
 
-            sql_create = zip_file.read(sql_file)
-            db.query(sql_create)
+            with suppress(Exception):
+                sql_create = zip_file.read(sql_file)
+                db.query(sql_create)
 
         for ibd_file in target_ibd_files:
             table = ibd_file.rsplit('.')[0]
             print(f"importing tablespace: {table}")
 
             try:
                 db.query(f'alter table `{table}` discard tablespace')
```

### Comparing `ibdx-0.3.0/ibdx/mysql_db_quick.py` & `ibdx-0.3.1/ibdx/mysql_db_quick.py`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.0/.gitignore` & `ibdx-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.0/LICENSE` & `ibdx-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.0/README.md` & `ibdx-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.0/pyproject.toml` & `ibdx-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.0/PKG-INFO` & `ibdx-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibdx
-Version: 0.3.0
+Version: 0.3.1
 Summary: yet another backup/restore program for mysql InnoDB tables
 Project-URL: homepage, https://github.com/Grvzard/ibdx
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: pymysql==1.0.2
 Requires-Dist: python-dotenv==0.21.0
 Requires-Dist: typer<1.0.0,>=0.7.0
```

