# Comparing `tmp/ibdx-0.3.1.tar.gz` & `tmp/ibdx-0.3.2.tar.gz`

## Comparing `ibdx-0.3.1.tar` & `ibdx-0.3.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ibdx-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ibdx-0.3.1/demo.env
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/__main__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/cli.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/configs.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/deps.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/ibd_backup.py
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/ibd_restore.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/mysql_db_quick.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 ibdx-0.3.1/ibdx/tools.py
--rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 ibdx-0.3.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ibdx-0.3.1/LICENSE
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 ibdx-0.3.1/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ibdx-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ibdx-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ibdx-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ibdx-0.3.2/demo.env
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/__main__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/cli.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/configs.py
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/deps.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/ibd_backup.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/ibd_restore.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/mysql_db_quick.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 ibdx-0.3.2/ibdx/tools.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 ibdx-0.3.2/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 ibdx-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 ibdx-0.3.2/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 ibdx-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 ibdx-0.3.2/PKG-INFO
```

### Comparing `ibdx-0.3.1/ibdx/cli.py` & `ibdx-0.3.2/ibdx/cli.py`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.1/ibdx/ibd_backup.py` & `ibdx-0.3.2/ibdx/ibd_backup.py`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.1/ibdx/ibd_restore.py` & `ibdx-0.3.2/ibdx/ibd_restore.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,20 +48,24 @@
 
         for ibd_file in target_ibd_files:
             table = ibd_file.rsplit('.')[0]
             print(f"importing tablespace: {table}")
 
             try:
                 db.query(f'alter table `{table}` discard tablespace')
+                print(f'. alter table `{table}` discard tablespace')
 
                 zip_file.extract(f'{table}.ibd', db_path)
+                print(f'.. extract {table}.ibd')
                 with suppress(Exception):
                     zip_file.extract(f'{table}.cfg', db_path)
+                    print(f'.. extract {table}.cfg')
 
                 db.query(f'alter table `{table}` import tablespace')
+                print(f'... alter table `{table}` import tablespace')
 
             except Exception as e:
                 (db_path / f'{table}.ibd').unlink(missing_ok=True)
                 (db_path / f'{table}.cfg').unlink(missing_ok=True)
 
                 # db.query(f'drop table if exists `{table}`;')
```

### Comparing `ibdx-0.3.1/ibdx/mysql_db_quick.py` & `ibdx-0.3.2/ibdx/mysql_db_quick.py`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.1/.gitignore` & `ibdx-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.1/LICENSE` & `ibdx-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.1/README.md` & `ibdx-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.1/pyproject.toml` & `ibdx-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ibdx-0.3.1/PKG-INFO` & `ibdx-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ibdx
-Version: 0.3.1
+Version: 0.3.2
 Summary: yet another backup/restore program for mysql InnoDB tables
 Project-URL: homepage, https://github.com/Grvzard/ibdx
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: pymysql==1.0.2
 Requires-Dist: python-dotenv==0.21.0
 Requires-Dist: typer<1.0.0,>=0.7.0
```

