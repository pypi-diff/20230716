# Comparing `tmp/hedgesql-1.3.tar.gz` & `tmp/hedgesql-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hedgesql-1.3.tar", last modified: Fri Jun 23 19:28:46 2023, max compression
+gzip compressed data, was "hedgesql-1.3.1.tar", last modified: Sun Jul 16 09:00:00 2023, max compression
```

## Comparing `hedgesql-1.3.tar` & `hedgesql-1.3.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-23 19:28:46.659167 hedgesql-1.3/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.3/LICENSE
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-23 19:28:46.659167 hedgesql-1.3/PKG-INFO
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-23 19:28:46.659167 hedgesql-1.3/hedgesql/
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.3/hedgesql/__init__.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     5214 2023-06-23 17:25:05.000000 hedgesql-1.3/hedgesql/datatypes.py
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9584 2023-06-23 19:28:05.000000 hedgesql-1.3/hedgesql/hedge_sql.py
-drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-06-23 19:28:46.659167 hedgesql-1.3/hedgesql.egg-info/
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      614 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/PKG-INFO
--rw-rw-r--   0 frevod    (1000) frevod    (1000)      240 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/SOURCES.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/dependency_links.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/requires.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-06-23 19:28:46.000000 hedgesql-1.3/hedgesql.egg-info/top_level.txt
--rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-06-23 19:28:46.659167 hedgesql-1.3/setup.cfg
--rwxrwxrwx   0 frevod    (1000) frevod    (1000)      759 2023-06-23 19:28:19.000000 hedgesql-1.3/setup.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-16 09:00:00.248837 hedgesql-1.3.1/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)    35149 2023-06-10 20:40:52.000000 hedgesql-1.3.1/LICENSE
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-07-16 09:00:00.248837 hedgesql-1.3.1/PKG-INFO
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-16 09:00:00.248837 hedgesql-1.3.1/hedgesql/
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)       96 2023-06-18 17:46:31.000000 hedgesql-1.3.1/hedgesql/__init__.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     5214 2023-06-23 17:25:05.000000 hedgesql-1.3.1/hedgesql/datatypes.py
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)     9711 2023-07-16 08:59:16.000000 hedgesql-1.3.1/hedgesql/hedge_sql.py
+drwxrwxr-x   0 frevod    (1000) frevod    (1000)        0 2023-07-16 09:00:00.248837 hedgesql-1.3.1/hedgesql.egg-info/
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      616 2023-07-16 08:59:59.000000 hedgesql-1.3.1/hedgesql.egg-info/PKG-INFO
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)      240 2023-07-16 09:00:00.000000 hedgesql-1.3.1/hedgesql.egg-info/SOURCES.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        1 2023-07-16 08:59:59.000000 hedgesql-1.3.1/hedgesql.egg-info/dependency_links.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       10 2023-07-16 08:59:59.000000 hedgesql-1.3.1/hedgesql.egg-info/requires.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)        9 2023-07-16 08:59:59.000000 hedgesql-1.3.1/hedgesql.egg-info/top_level.txt
+-rw-rw-r--   0 frevod    (1000) frevod    (1000)       38 2023-07-16 09:00:00.248837 hedgesql-1.3.1/setup.cfg
+-rwxrwxrwx   0 frevod    (1000) frevod    (1000)      761 2023-07-16 08:59:34.000000 hedgesql-1.3.1/setup.py
```

### Comparing `hedgesql-1.3/LICENSE` & `hedgesql-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hedgesql-1.3/PKG-INFO` & `hedgesql-1.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.3
+Version: 1.3.1
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.3/hedgesql/datatypes.py` & `hedgesql-1.3.1/hedgesql/datatypes.py`

 * *Files identical despite different names*

### Comparing `hedgesql-1.3/hedgesql/hedge_sql.py` & `hedgesql-1.3.1/hedgesql/hedge_sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,18 +106,18 @@
 
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
         self.__cursor.execute(query, tuple(values))
         self.__conn.commit()
 
     def delete_data(self,
                     table_name: str,
-                    where: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
+                    where: Optional[List[Dict[str, Union[str, int, float]]]] = None) -> None:
         if where:
-            where_clause = 'WHERE ' + ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(where.values())
+            where_clause = ' WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
+            values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
         self.__cursor.execute(query, values)
         self.__conn.commit()
 
@@ -230,18 +230,18 @@
 
         query = f"UPDATE {table_name} SET {set_clause} {where_clause}"
         await self.__cursor.execute(query, tuple(values))
         await self.__conn.commit()
 
     async def delete_data(self,
                           table_name: str,
-                          where: Optional[Dict[str, Union[str, int, float]]] = None) -> None:
+                          where: Optional[List[Dict[str, Union[str, int, float]]]] = None) -> None:
         if where:
-            where_clause = 'WHERE' + ' AND '.join([f'{col}=?' for col in where.keys()])
-            values = tuple(where.values())
+            where_clause = ' WHERE ' + ' OR '.join([' AND '.join([f'{col}=?' for col in d.keys()]) for d in where])
+            values = tuple(value for d in where for value in d.values())
         else:
             where_clause = ''
             values = ()
         query = f"DELETE FROM {table_name} {where_clause}"
         await self.__cursor.execute(query, values)
         await self.__conn.commit()
```

### Comparing `hedgesql-1.3/hedgesql.egg-info/PKG-INFO` & `hedgesql-1.3.1/hedgesql.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hedgesql
-Version: 1.3
+Version: 1.3.1
 Summary: Convenient work with sqlite3 and aiosqlite
 Home-page: https://github.com/I-HedgeDev/litesqlite
 Author: HedgeDev
 Author-email: hedge_dev@mail.ru
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `hedgesql-1.3/setup.py` & `hedgesql-1.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='hedgesql',
-    version='1.3',
+    version='1.3.1',
     description='Convenient work with sqlite3 and aiosqlite',
     url='https://github.com/I-HedgeDev/litesqlite',
     author='HedgeDev',
     author_email='hedge_dev@mail.ru',
     packages=['hedgesql'],
     install_requires=[
         'aiosqlite'
```

