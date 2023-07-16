# Comparing `tmp/django-pdr-1.2.8.tar.gz` & `tmp/django-pdr-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pdr-1.2.8.tar", last modified: Fri Dec 23 12:31:33 2022, max compression
+gzip compressed data, was "django-pdr-1.2.9.tar", last modified: Fri Dec 23 12:57:48 2022, max compression
```

## Comparing `django-pdr-1.2.8.tar` & `django-pdr-1.2.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.216888 django-pdr-1.2.8/
--rw-rw-rw-   0        0        0    11542 2021-06-26 08:06:44.000000 django-pdr-1.2.8/LICENSE
--rw-rw-rw-   0        0        0      218 2021-06-26 08:06:44.000000 django-pdr-1.2.8/MANIFEST.in
--rw-rw-rw-   0        0        0     8816 2022-12-23 12:31:33.217884 django-pdr-1.2.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.137091 django-pdr-1.2.8/django_pdr/
--rw-rw-rw-   0        0        0        0 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/__init__.py
--rw-rw-rw-   0        0        0     5323 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/admin.py
--rw-rw-rw-   0        0        0      154 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/apps.py
--rw-rw-rw-   0        0        0     2540 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/datasources.py
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.175879 django-pdr-1.2.8/django_pdr/js/
--rw-rw-rw-   0        0        0      823 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/js/README.MD
--rw-rw-rw-   0        0        0     1973 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/js/bind-connection-tables.js
--rw-rw-rw-   0        0        0     2643 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/js/get-reflection-template.js
--rw-rw-rw-   0        0        0     1052 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/js/list_config.js
--rw-rw-rw-   0        0        0     1866 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/js/list_db_tables.js
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.176883 django-pdr-1.2.8/django_pdr/management/
--rw-rw-rw-   0        0        0        0 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/management/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.183882 django-pdr-1.2.8/django_pdr/management/commands/
--rw-rw-rw-   0        0        0        0 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/management/commands/__init__.py
--rw-rw-rw-   0        0        0     4755 2022-12-23 12:30:15.000000 django-pdr-1.2.8/django_pdr/management/commands/export.py
--rw-rw-rw-   0        0        0     4231 2022-12-23 12:30:47.000000 django-pdr-1.2.8/django_pdr/management/commands/import.py
--rw-rw-rw-   0        0        0     1893 2022-11-18 09:56:36.000000 django-pdr-1.2.8/django_pdr/management/commands/pdr-reflect.py
--rw-rw-rw-   0        0        0     1546 2021-07-18 15:18:24.000000 django-pdr-1.2.8/django_pdr/methods.py
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.185883 django-pdr-1.2.8/django_pdr/migrations/
--rw-rw-rw-   0        0        0        0 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/migrations/__init__.py
--rw-rw-rw-   0        0        0    40656 2022-11-20 13:31:17.000000 django-pdr-1.2.8/django_pdr/models.py
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.190882 django-pdr-1.2.8/django_pdr/sql/
--rw-rw-rw-   0        0        0     2615 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/README.MD
--rw-rw-rw-   0        0        0      582 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/get_pk.sql
--rw-rw-rw-   0        0        0      101 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/list_tables.sql
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.193883 django-pdr-1.2.8/django_pdr/sql/mssql+pymssql/
--rw-rw-rw-   0        0        0     1235 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/mssql+pymssql/create_event_listener.sql
--rw-rw-rw-   0        0        0      138 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/mssql+pymssql/delete_event_listener.sql
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.196884 django-pdr-1.2.8/django_pdr/sql/mysql+mysqldb/
--rw-rw-rw-   0        0        0     1053 2022-11-13 15:07:40.000000 django-pdr-1.2.8/django_pdr/sql/mysql+mysqldb/create_event_listener.sql
--rw-rw-rw-   0        0        0      236 2022-11-13 15:08:00.000000 django-pdr-1.2.8/django_pdr/sql/mysql+mysqldb/delete_event_listener.sql
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.200886 django-pdr-1.2.8/django_pdr/sql/postgresql/
--rw-rw-rw-   0        0        0     1665 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/postgresql/create_event_listener.sql
--rw-rw-rw-   0        0        0      416 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/postgresql/delete_event_listener.sql
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.206881 django-pdr-1.2.8/django_pdr/sql/sqlite+pysqlite/
--rw-rw-rw-   0        0        0     1077 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/sqlite+pysqlite/create_event_listener.sql
--rw-rw-rw-   0        0        0      226 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/sqlite+pysqlite/delete_event_listener.sql
--rw-rw-rw-   0        0        0       61 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/sql/sqlite+pysqlite/list_tables.sql
--rw-rw-rw-   0        0        0       63 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/tests.py
--rw-rw-rw-   0        0        0     1552 2021-06-26 08:06:44.000000 django-pdr-1.2.8/django_pdr/views.py
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.165891 django-pdr-1.2.8/django_pdr.egg-info/
--rw-rw-rw-   0        0        0     8816 2022-12-23 12:31:33.000000 django-pdr-1.2.8/django_pdr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1454 2022-12-23 12:31:33.000000 django-pdr-1.2.8/django_pdr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-23 12:31:33.000000 django-pdr-1.2.8/django_pdr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      136 2022-12-23 12:31:33.000000 django-pdr-1.2.8/django_pdr.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-12-23 12:31:33.000000 django-pdr-1.2.8/django_pdr.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.114091 django-pdr-1.2.8/docs/
-drwxrwxrwx   0        0        0        0 2022-12-23 12:31:33.213882 django-pdr-1.2.8/docs/images/
--rw-rw-rw-   0        0        0    24316 2021-06-26 08:06:44.000000 django-pdr-1.2.8/docs/images/add_db.png
--rw-rw-rw-   0        0        0    41399 2021-06-26 08:06:44.000000 django-pdr-1.2.8/docs/images/add_reflection.png
--rw-rw-rw-   0        0        0    26994 2021-06-26 08:06:44.000000 django-pdr-1.2.8/docs/images/add_source.png
--rw-rw-rw-   0        0        0     4745 2021-06-26 08:06:44.000000 django-pdr-1.2.8/docs/images/models.png
--rw-rw-rw-   0        0        0     1214 2022-12-23 12:31:33.220883 django-pdr-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-06-26 08:06:44.000000 django-pdr-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.515522 django-pdr-1.2.9/
+-rw-rw-rw-   0        0        0    11542 2021-06-26 08:06:44.000000 django-pdr-1.2.9/LICENSE
+-rw-rw-rw-   0        0        0      218 2021-06-26 08:06:44.000000 django-pdr-1.2.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     8816 2022-12-23 12:57:48.516521 django-pdr-1.2.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.441521 django-pdr-1.2.9/django_pdr/
+-rw-rw-rw-   0        0        0        0 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/__init__.py
+-rw-rw-rw-   0        0        0     5323 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/admin.py
+-rw-rw-rw-   0        0        0      154 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/apps.py
+-rw-rw-rw-   0        0        0     2540 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/datasources.py
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.470515 django-pdr-1.2.9/django_pdr/js/
+-rw-rw-rw-   0        0        0      823 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/js/README.MD
+-rw-rw-rw-   0        0        0     1973 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/js/bind-connection-tables.js
+-rw-rw-rw-   0        0        0     2643 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/js/get-reflection-template.js
+-rw-rw-rw-   0        0        0     1052 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/js/list_config.js
+-rw-rw-rw-   0        0        0     1866 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/js/list_db_tables.js
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.471518 django-pdr-1.2.9/django_pdr/management/
+-rw-rw-rw-   0        0        0        0 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/management/__init__.py
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.478518 django-pdr-1.2.9/django_pdr/management/commands/
+-rw-rw-rw-   0        0        0        0 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/management/commands/__init__.py
+-rw-rw-rw-   0        0        0     4736 2022-12-23 12:57:36.000000 django-pdr-1.2.9/django_pdr/management/commands/export.py
+-rw-rw-rw-   0        0        0     4234 2022-12-23 12:42:02.000000 django-pdr-1.2.9/django_pdr/management/commands/import.py
+-rw-rw-rw-   0        0        0     1893 2022-11-18 09:56:36.000000 django-pdr-1.2.9/django_pdr/management/commands/pdr-reflect.py
+-rw-rw-rw-   0        0        0     1546 2021-07-18 15:18:24.000000 django-pdr-1.2.9/django_pdr/methods.py
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.479518 django-pdr-1.2.9/django_pdr/migrations/
+-rw-rw-rw-   0        0        0        0 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/migrations/__init__.py
+-rw-rw-rw-   0        0        0    40656 2022-11-20 13:31:17.000000 django-pdr-1.2.9/django_pdr/models.py
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.485527 django-pdr-1.2.9/django_pdr/sql/
+-rw-rw-rw-   0        0        0     2615 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/README.MD
+-rw-rw-rw-   0        0        0      582 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/get_pk.sql
+-rw-rw-rw-   0        0        0      101 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/list_tables.sql
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.489526 django-pdr-1.2.9/django_pdr/sql/mssql+pymssql/
+-rw-rw-rw-   0        0        0     1235 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/mssql+pymssql/create_event_listener.sql
+-rw-rw-rw-   0        0        0      138 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/mssql+pymssql/delete_event_listener.sql
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.494522 django-pdr-1.2.9/django_pdr/sql/mysql+mysqldb/
+-rw-rw-rw-   0        0        0     1053 2022-11-13 15:07:40.000000 django-pdr-1.2.9/django_pdr/sql/mysql+mysqldb/create_event_listener.sql
+-rw-rw-rw-   0        0        0      236 2022-11-13 15:08:00.000000 django-pdr-1.2.9/django_pdr/sql/mysql+mysqldb/delete_event_listener.sql
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.498520 django-pdr-1.2.9/django_pdr/sql/postgresql/
+-rw-rw-rw-   0        0        0     1665 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/postgresql/create_event_listener.sql
+-rw-rw-rw-   0        0        0      416 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/postgresql/delete_event_listener.sql
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.505520 django-pdr-1.2.9/django_pdr/sql/sqlite+pysqlite/
+-rw-rw-rw-   0        0        0     1077 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/sqlite+pysqlite/create_event_listener.sql
+-rw-rw-rw-   0        0        0      226 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/sqlite+pysqlite/delete_event_listener.sql
+-rw-rw-rw-   0        0        0       61 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/sql/sqlite+pysqlite/list_tables.sql
+-rw-rw-rw-   0        0        0       63 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/tests.py
+-rw-rw-rw-   0        0        0     1552 2021-06-26 08:06:44.000000 django-pdr-1.2.9/django_pdr/views.py
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.461519 django-pdr-1.2.9/django_pdr.egg-info/
+-rw-rw-rw-   0        0        0     8816 2022-12-23 12:57:48.000000 django-pdr-1.2.9/django_pdr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1454 2022-12-23 12:57:48.000000 django-pdr-1.2.9/django_pdr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-23 12:57:48.000000 django-pdr-1.2.9/django_pdr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      136 2022-12-23 12:57:48.000000 django-pdr-1.2.9/django_pdr.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-12-23 12:57:48.000000 django-pdr-1.2.9/django_pdr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.420516 django-pdr-1.2.9/docs/
+drwxrwxrwx   0        0        0        0 2022-12-23 12:57:48.513522 django-pdr-1.2.9/docs/images/
+-rw-rw-rw-   0        0        0    24316 2021-06-26 08:06:44.000000 django-pdr-1.2.9/docs/images/add_db.png
+-rw-rw-rw-   0        0        0    41399 2021-06-26 08:06:44.000000 django-pdr-1.2.9/docs/images/add_reflection.png
+-rw-rw-rw-   0        0        0    26994 2021-06-26 08:06:44.000000 django-pdr-1.2.9/docs/images/add_source.png
+-rw-rw-rw-   0        0        0     4745 2021-06-26 08:06:44.000000 django-pdr-1.2.9/docs/images/models.png
+-rw-rw-rw-   0        0        0     1214 2022-12-23 12:57:48.519522 django-pdr-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2021-06-26 08:06:44.000000 django-pdr-1.2.9/setup.py
```

### Comparing `django-pdr-1.2.8/LICENSE` & `django-pdr-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/PKG-INFO` & `django-pdr-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pdr
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Django app to create and manage live replications of SQL database tables.
 Home-page: https://github.com/meena-erian/pdr
 Author: Meena (Menas) Erian
 Author-email: hi@menas.pro
 License: Apache V2 License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-pdr Version: 1.2.8 Summary: A Django app to
+Metadata-Version: 2.1 Name: django-pdr Version: 1.2.9 Summary: A Django app to
 create and manage live replications of SQL database tables. Home-page: https://
 github.com/meena-erian/pdr Author: Meena (Menas) Erian Author-email:
 hi@menas.pro License: Apache V2 License Platform: UNKNOWN Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
 Framework :: Django :: 3.1 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

### Comparing `django-pdr-1.2.8/django_pdr/admin.py` & `django-pdr-1.2.9/django_pdr/admin.py`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/datasources.py` & `django-pdr-1.2.9/django_pdr/datasources.py`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/js/README.MD` & `django-pdr-1.2.9/django_pdr/js/README.MD`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/js/bind-connection-tables.js` & `django-pdr-1.2.9/django_pdr/js/bind-connection-tables.js`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/js/get-reflection-template.js` & `django-pdr-1.2.9/django_pdr/js/get-reflection-template.js`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/js/list_config.js` & `django-pdr-1.2.9/django_pdr/js/list_config.js`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/js/list_db_tables.js` & `django-pdr-1.2.9/django_pdr/js/list_db_tables.js`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/management/commands/export.py` & `django-pdr-1.2.9/django_pdr/management/commands/export.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         pwd = os.path.join(pwd, 'exported_pdr_data')
         os.mkdir(pwd)
         logging.info(f"Created Export Directory {pwd}")
         databases_dir = os.path.join(pwd, "databases")
         os.mkdir(databases_dir)
         logging.info(f"Created Databases Directory {databases_dir}")
         for database in Database.objects.all():
-            logging.info("Exporting Database {database}")
+            logging.info(f"Exporting Database {database}")
             db_dir = os.path.join(pwd, "databases", database.handle)
             os.mkdir(db_dir)
             db_meta = {
                 "source": database.source,
                 "description": database.description,
                 "pk": database.pk
             }
@@ -49,29 +49,29 @@
                 file.write(json.dumps(db_meta, indent=4))
             with open(os.path.join(db_dir, "config.json"), "w") as file:
                 file.write(json.dumps(db_config, indent=4))
         source_tables_dir = os.path.join(pwd, "source_tables")
         os.mkdir(source_tables_dir)
         logging.info(f"Created SourceTables Directory {source_tables_dir}")
         for source in SourceTable.objects.all():
-            logging.info("Exporting SourceTabe {source}")
+            logging.info(f"Exporting SourceTabe {source}")
             source_dir = os.path.join(pwd, "source_tables", str(source.pk))
             os.mkdir(source_dir)
             source_meta = {
                 "database": source.source_database.pk,
                 "table": source.source_table,
                 "description": source.description,
             }
             with open(os.path.join(source_dir, "meta.json"), "w") as file:
                 file.write(json.dumps(source_meta, indent=4))
         reflections_dir = os.path.join(pwd, "reflections")
         os.mkdir(reflections_dir)
         logging.info(f"Created Reflections Directory {reflections_dir}")
         for reflection in Reflection.objects.all():
-            logging.info("Exporting Reflection {reflection}")
+            logging.info(f"Exporting Reflection {reflection}")
             reflection_dir = os.path.join(
                 pwd,
                 "reflections",
                 str(reflection.pk)
             )
             os.mkdir(reflection_dir)
             reflection_meta = {
@@ -102,8 +102,8 @@
                     ), "w") as file:
                 file.write(json.dumps(destination_fields, indent=4))
             with open(
                     os.path.join(
                         reflection_dir,
                         "reflection_statment.sql"
                     ), "w") as file:
-                file.write(json.dumps(reflection_statment, indent=4))
+                file.write(reflection_statment)
```

### Comparing `django-pdr-1.2.8/django_pdr/management/commands/import.py` & `django-pdr-1.2.9/django_pdr/management/commands/import.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,29 +39,29 @@
             database = Database(
                 handle=db_handle,
                 source=db_meta["source"],
                 description=db_meta["description"],
                 pk=db_meta["pk"],
                 config=db_config
             )
-            logging.info("Importing Database {database}")
+            logging.info(f"Importing Database {database}")
             database.clean()
             database.save()
         source_tables = os.listdir(os.path.join(pwd, "source_tables"))
         for pk in source_tables:
             source_dir = os.path.join(pwd, "source_tables", pk)
             with open(os.path.join(source_dir, "meta.json")) as file:
                 source_meta = json.load(file)
             source = SourceTable(
                 pk=int(pk),
                 source_database=source_meta["database"],
                 source_table=source_meta["table"],
                 description=source_meta["description"]
             )
-            logging.info("Importing SourceTable {source}")
+            logging.info(f"Importing SourceTable {source}")
             source.clean()
             source.save()
         reflections = os.listdir(os.path.join(pwd, "reflections"))
         for pk in reflections:
             reflection_dir = os.path.join(pwd, "reflections", pk)
             with open(os.path.join(reflection_dir, "meta.json")) as file:
                 reflection_meta = json.load(file)
@@ -93,10 +93,10 @@
                 # last_updated=reflection_meta["last_updated"],
                 active=reflection_meta["active"],
                 ignore_delete_events=reflection_meta["ignore_delete_events"],
                 source_fields=source_fields,
                 destination_fields=destination_fields,
                 reflection_statment=reflection_statment
             )
-            logging.info("Importing Reflection {reflection}")
+            logging.info(f"Importing Reflection {reflection}")
             reflection.clean()
             reflection.save()
```

### Comparing `django-pdr-1.2.8/django_pdr/management/commands/pdr-reflect.py` & `django-pdr-1.2.9/django_pdr/management/commands/pdr-reflect.py`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/methods.py` & `django-pdr-1.2.9/django_pdr/methods.py`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/models.py` & `django-pdr-1.2.9/django_pdr/models.py`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/sql/README.MD` & `django-pdr-1.2.9/django_pdr/sql/README.MD`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/sql/get_pk.sql` & `django-pdr-1.2.9/django_pdr/sql/get_pk.sql`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/sql/mssql+pymssql/create_event_listener.sql` & `django-pdr-1.2.9/django_pdr/sql/mssql+pymssql/create_event_listener.sql`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/sql/mysql+mysqldb/create_event_listener.sql` & `django-pdr-1.2.9/django_pdr/sql/mysql+mysqldb/create_event_listener.sql`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/sql/postgresql/create_event_listener.sql` & `django-pdr-1.2.9/django_pdr/sql/postgresql/create_event_listener.sql`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/sql/sqlite+pysqlite/create_event_listener.sql` & `django-pdr-1.2.9/django_pdr/sql/sqlite+pysqlite/create_event_listener.sql`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr/views.py` & `django-pdr-1.2.9/django_pdr/views.py`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/django_pdr.egg-info/PKG-INFO` & `django-pdr-1.2.9/django_pdr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pdr
-Version: 1.2.8
+Version: 1.2.9
 Summary: A Django app to create and manage live replications of SQL database tables.
 Home-page: https://github.com/meena-erian/pdr
 Author: Meena (Menas) Erian
 Author-email: hi@menas.pro
 License: Apache V2 License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-pdr Version: 1.2.8 Summary: A Django app to
+Metadata-Version: 2.1 Name: django-pdr Version: 1.2.9 Summary: A Django app to
 create and manage live replications of SQL database tables. Home-page: https://
 github.com/meena-erian/pdr Author: Meena (Menas) Erian Author-email:
 hi@menas.pro License: Apache V2 License Platform: UNKNOWN Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
 Framework :: Django :: 3.1 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

### Comparing `django-pdr-1.2.8/django_pdr.egg-info/SOURCES.txt` & `django-pdr-1.2.9/django_pdr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/docs/images/add_db.png` & `django-pdr-1.2.9/docs/images/add_db.png`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/docs/images/add_reflection.png` & `django-pdr-1.2.9/docs/images/add_reflection.png`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/docs/images/add_source.png` & `django-pdr-1.2.9/docs/images/add_source.png`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/docs/images/models.png` & `django-pdr-1.2.9/docs/images/models.png`

 * *Files identical despite different names*

### Comparing `django-pdr-1.2.8/setup.cfg` & `django-pdr-1.2.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a61 6e67 6f2d 7064 720d 0a76   = django-pdr..v
-00000020: 6572 7369 6f6e 203d 2031 2e32 2e38 0d0a  ersion = 1.2.8..
+00000020: 6572 7369 6f6e 203d 2031 2e32 2e39 0d0a  ersion = 1.2.9..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
 00000040: 446a 616e 676f 2061 7070 2074 6f20 6372  Django app to cr
 00000050: 6561 7465 2061 6e64 206d 616e 6167 6520  eate and manage 
 00000060: 6c69 7665 2072 6570 6c69 6361 7469 6f6e  live replication
 00000070: 7320 6f66 2053 514c 2064 6174 6162 6173  s of SQL databas
 00000080: 6520 7461 626c 6573 2e0d 0a6c 6f6e 675f  e tables...long_
 00000090: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
```

