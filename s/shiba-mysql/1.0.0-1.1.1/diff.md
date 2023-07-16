# Comparing `tmp/shiba_mysql-1.0.0.tar.gz` & `tmp/shiba_mysql-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shiba_mysql-1.0.0.tar", last modified: Sun Jul 16 01:16:56 2023, max compression
+gzip compressed data, was "shiba_mysql-1.1.1.tar", last modified: Sun Jul 16 01:31:00 2023, max compression
```

## Comparing `shiba_mysql-1.0.0.tar` & `shiba_mysql-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:16:56.644723 shiba_mysql-1.0.0/
--rw-rw-rw-   0        0        0     1105 2023-07-14 20:43:24.000000 shiba_mysql-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     3845 2023-07-16 01:16:56.642182 shiba_mysql-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2679 2023-07-14 21:03:27.000000 shiba_mysql-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 01:16:56.645715 shiba_mysql-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      897 2023-07-16 01:16:43.000000 shiba_mysql-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:16:56.623519 shiba_mysql-1.0.0/shiba/
--rw-rw-rw-   0        0        0      662 2023-07-16 01:09:58.000000 shiba_mysql-1.0.0/shiba/__init__.py
--rw-rw-rw-   0        0        0     5111 2023-07-14 21:03:27.000000 shiba_mysql-1.0.0/shiba/database.py
--rw-rw-rw-   0        0        0     5306 2023-07-15 22:38:47.000000 shiba_mysql-1.0.0/shiba/query_builder.py
--rw-rw-rw-   0        0        0     4623 2023-07-16 01:09:58.000000 shiba_mysql-1.0.0/shiba/table_builder.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:16:56.640189 shiba_mysql-1.0.0/shiba_mysql.egg-info/
--rw-rw-rw-   0        0        0     3845 2023-07-16 01:16:56.000000 shiba_mysql-1.0.0/shiba_mysql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2023-07-16 01:16:56.000000 shiba_mysql-1.0.0/shiba_mysql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:16:56.000000 shiba_mysql-1.0.0/shiba_mysql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-07-16 01:16:56.000000 shiba_mysql-1.0.0/shiba_mysql.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-16 01:16:56.000000 shiba_mysql-1.0.0/shiba_mysql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 01:31:00.059455 shiba_mysql-1.1.1/
+-rw-rw-rw-   0        0        0     1105 2023-07-14 20:43:24.000000 shiba_mysql-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     3979 2023-07-16 01:31:00.056877 shiba_mysql-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2662 2023-07-16 01:29:04.000000 shiba_mysql-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 01:31:00.060423 shiba_mysql-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1047 2023-07-16 01:27:46.000000 shiba_mysql-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:31:00.041240 shiba_mysql-1.1.1/shiba_mysql.egg-info/
+-rw-rw-rw-   0        0        0     3979 2023-07-16 01:30:59.000000 shiba_mysql-1.1.1/shiba_mysql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-16 01:30:59.000000 shiba_mysql-1.1.1/shiba_mysql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 01:30:59.000000 shiba_mysql-1.1.1/shiba_mysql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-07-16 01:30:59.000000 shiba_mysql-1.1.1/shiba_mysql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-16 01:30:59.000000 shiba_mysql-1.1.1/shiba_mysql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 01:31:00.053878 shiba_mysql-1.1.1/shibamysql/
+-rw-rw-rw-   0        0        0      662 2023-07-16 01:09:58.000000 shiba_mysql-1.1.1/shibamysql/__init__.py
+-rw-rw-rw-   0        0        0     5111 2023-07-14 21:03:27.000000 shiba_mysql-1.1.1/shibamysql/database.py
+-rw-rw-rw-   0        0        0     5306 2023-07-15 22:38:47.000000 shiba_mysql-1.1.1/shibamysql/query_builder.py
+-rw-rw-rw-   0        0        0     4623 2023-07-16 01:09:58.000000 shiba_mysql-1.1.1/shibamysql/table_builder.py
```

### Comparing `shiba_mysql-1.0.0/LICENSE` & `shiba_mysql-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shiba_mysql-1.0.0/PKG-INFO` & `shiba_mysql-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: shiba_mysql
-Version: 1.0.0
+Version: 1.1.1
 Summary: A library to interact with MySQL
 Home-page: https://github.com/ShibaRoPinoo/Shiba-Py-Mysql
 Author: Rodrigo Pino
 Author-email: ro.pinoo18@gmail.com
 License: MIT
-Keywords: mysql
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Keywords: mysql,database,SQL,data access,ORM
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Database
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shiba-Py-Mysql
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/ShibaRoPinoo/Shiba-Py-Mysql/blob/main/LICENSE)
 
@@ -29,23 +32,23 @@
 - Retrieving data from tables with support for JSON fields.
 
 ## Installation
 
 You can install Shiba-Py-Mysql using pip:
 
 ```shell
-pip install shiba-py-mysql
+pip install shiba-mysql
 ```
 
 ```python
 
-from shiba import ShibaConnection
+import shiba as s
 
 # Create a connection to the MySQL database
-connection = ShibaConnection(host='localhost', port=3306, user='myuser', password='mypassword')
+connection = s.ShibaConnection(host='localhost', port=3306, user='myuser', password='mypassword')
 
 # Create a new database
 connection.create_database('my_database')
 
 # Select the database
 connection.use_database('my_database')
```

### Comparing `shiba_mysql-1.0.0/README.md` & `shiba_mysql-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 - Retrieving data from tables with support for JSON fields.
 
 ## Installation
 
 You can install Shiba-Py-Mysql using pip:
 
 ```shell
-pip install shiba-py-mysql
+pip install shiba-mysql
 ```
 
 ```python
 
-from shiba import ShibaConnection
+import shiba as s
 
 # Create a connection to the MySQL database
-connection = ShibaConnection(host='localhost', port=3306, user='myuser', password='mypassword')
+connection = s.ShibaConnection(host='localhost', port=3306, user='myuser', password='mypassword')
 
 # Create a new database
 connection.create_database('my_database')
 
 # Select the database
 connection.use_database('my_database')
```

### Comparing `shiba_mysql-1.0.0/shiba/__init__.py` & `shiba_mysql-1.1.1/shibamysql/__init__.py`

 * *Files identical despite different names*

### Comparing `shiba_mysql-1.0.0/shiba/database.py` & `shiba_mysql-1.1.1/shibamysql/database.py`

 * *Files identical despite different names*

### Comparing `shiba_mysql-1.0.0/shiba/query_builder.py` & `shiba_mysql-1.1.1/shibamysql/query_builder.py`

 * *Files identical despite different names*

### Comparing `shiba_mysql-1.0.0/shiba/table_builder.py` & `shiba_mysql-1.1.1/shibamysql/table_builder.py`

 * *Files identical despite different names*

### Comparing `shiba_mysql-1.0.0/shiba_mysql.egg-info/PKG-INFO` & `shiba_mysql-1.1.1/shiba_mysql.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: shiba-mysql
-Version: 1.0.0
+Version: 1.1.1
 Summary: A library to interact with MySQL
 Home-page: https://github.com/ShibaRoPinoo/Shiba-Py-Mysql
 Author: Rodrigo Pino
 Author-email: ro.pinoo18@gmail.com
 License: MIT
-Keywords: mysql
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Keywords: mysql,database,SQL,data access,ORM
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Database
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Shiba-Py-Mysql
 
 [![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](https://github.com/ShibaRoPinoo/Shiba-Py-Mysql/blob/main/LICENSE)
 
@@ -29,23 +32,23 @@
 - Retrieving data from tables with support for JSON fields.
 
 ## Installation
 
 You can install Shiba-Py-Mysql using pip:
 
 ```shell
-pip install shiba-py-mysql
+pip install shiba-mysql
 ```
 
 ```python
 
-from shiba import ShibaConnection
+import shiba as s
 
 # Create a connection to the MySQL database
-connection = ShibaConnection(host='localhost', port=3306, user='myuser', password='mypassword')
+connection = s.ShibaConnection(host='localhost', port=3306, user='myuser', password='mypassword')
 
 # Create a new database
 connection.create_database('my_database')
 
 # Select the database
 connection.use_database('my_database')
```

