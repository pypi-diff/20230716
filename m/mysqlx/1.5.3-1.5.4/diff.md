# Comparing `tmp/mysqlx-1.5.3.tar.gz` & `tmp/mysqlx-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.5.3.tar", last modified: Sat Jul 15 04:33:41 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.5.4.tar", last modified: Sun Jul 16 06:59:38 2023, max compression
```

## Comparing `mysqlx-1.5.3.tar` & `mysqlx-1.5.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 04:33:41.000000 mysqlx-1.5.3/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.5.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx/
--rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.5.3/mysqlx/constant.py
--rw-rw-rw-   0        0        0    19185 2023-07-14 16:59:37.000000 mysqlx-1.5.3/mysqlx/db.py
--rw-rw-rw-   0        0        0    13298 2023-07-14 21:56:44.000000 mysqlx-1.5.3/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.3/mysqlx/log_support.py
--rw-rw-rw-   0        0        0    37131 2023-07-14 23:52:54.000000 mysqlx-1.5.3/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.3/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.3/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6349 2023-07-13 04:01:58.000000 mysqlx-1.5.3/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.3/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 04:06:39.000000 mysqlx-1.5.3/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4327 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      365 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4327 2023-07-15 04:33:41.000000 mysqlx-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-07-15 04:33:38.000000 mysqlx-1.5.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-15 04:33:41.000000 mysqlx-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-07-15 04:33:38.000000 mysqlx-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:38.000000 mysqlx-1.5.4/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.5.4/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx/
+-rw-rw-rw-   0        0        0      693 2023-07-15 12:20:26.000000 mysqlx-1.5.4/mysqlx/constant.py
+-rw-rw-rw-   0        0        0    19264 2023-07-15 12:24:01.000000 mysqlx-1.5.4/mysqlx/db.py
+-rw-rw-rw-   0        0        0    13298 2023-07-14 21:56:44.000000 mysqlx-1.5.4/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.4/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0    37397 2023-07-16 02:08:48.000000 mysqlx-1.5.4/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.4/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.4/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6416 2023-07-15 12:25:21.000000 mysqlx-1.5.4/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.4/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 04:06:39.000000 mysqlx-1.5.4/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4329 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      365 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 06:59:38.000000 mysqlx-1.5.4/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4329 2023-07-16 06:59:38.000000 mysqlx-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3804 2023-07-16 02:24:38.000000 mysqlx-1.5.4/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-16 06:59:38.000000 mysqlx-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-07-16 06:59:10.000000 mysqlx-1.5.4/setup.py
```

### Comparing `mysqlx-1.5.3/LICENSE` & `mysqlx-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.3/mysqlx/constant.py` & `mysqlx-1.5.4/mysqlx/constant.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+CACHE_SIZE = 'cache_size'
+
+CONFIG_DICT = dict({CACHE_SIZE: 128})
+
 LIMIT_1 = 1
 
 NO_LIMIT = 0
 
 NAMED_REGEX = r':[\w|\d]*'
 
 DYNAMIC_REGEX = '{%|{{|}}|%}'
```

### Comparing `mysqlx-1.5.3/mysqlx/db.py` & `mysqlx-1.5.4/mysqlx/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import functools
 from typing import Sequence
-from .constant import LIMIT_1, MAPPER_PATH, PK_SQL
+from .constant import LIMIT_1, MAPPER_PATH, PK_SQL, CONFIG_DICT, CACHE_SIZE
 from .log_support import logger, sql_log, page_log, insert_log, do_sql_log, do_page_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, get_named_sql, get_named_args, DBError, \
     DB_LOCK, get_batch_args
 
 _DB_CTX = None
 _SHOW_SQL = False
 
@@ -18,37 +18,44 @@
         use_mysql_connector = True
     except ImportError:
         try:
             from pymysql import connect
         except ImportError:
             raise DBError("Please install MySQL driver, mysql-connector-python >= 8.0.13, PyMySQL >= 0.9.0.")
 
+    _SHOW_SQL = show_sql
+    kwargs['user'] = user
+    kwargs['password'] = password
+    kwargs['database'] = database
+    kwargs['host'] = host
+    kwargs['port'] = port
+    kwargs['use_unicode'] = use_unicode
+
     if 'debug' in kwargs:
         if kwargs.pop('debug'):
             from logging import DEBUG
             logger.setLevel(DEBUG)
 
+    if CACHE_SIZE in kwargs:
+        CONFIG_DICT[CACHE_SIZE] = kwargs.pop(CACHE_SIZE)
+
     is_pool = use_mysql_connector and pool_size >= 1
+    if is_pool:
+        kwargs['pool_size'] = pool_size
+        if 'pool_name' not in kwargs:
+            kwargs['pool_name'] = "{}_pool".format(database)
+
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
-        _SHOW_SQL = show_sql
+
         if MAPPER_PATH in kwargs:
             from .dbx import load_mapper
             load_mapper(kwargs.pop(MAPPER_PATH))
-        if is_pool:
-            kwargs['pool_size'] = pool_size
-            if 'pool_name' not in kwargs:
-                kwargs['pool_name'] = "{}_pool".format(database)
-        kwargs['user'] = user
-        kwargs['password'] = password
-        kwargs['database'] = database
-        kwargs['host'] = host
-        kwargs['port'] = port
-        kwargs['use_unicode'] = use_unicode
+
         _DB_CTX = DBCtx(connect=lambda: connect(**kwargs), use_mysql_connector=use_mysql_connector)
     if is_pool:
         logger.info('Init db engine <%s> ok with connection pool size: %d.' % (hex(id(_DB_CTX)), pool_size))
     else:
         logger.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
```

### Comparing `mysqlx-1.5.3/mysqlx/dbx.py` & `mysqlx-1.5.4/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.3/mysqlx/log_support.py` & `mysqlx-1.5.4/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.3/mysqlx/orm.py` & `mysqlx-1.5.4/mysqlx/orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
 from .support import DBError, simple_sql
 from typing import Sequence, Union, List, Tuple
 from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, SYMBOLS, BETWEEN, LIKE, IN, PK, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY, \
-    COLUMN_SQL
+    COLUMN_SQL, CONFIG_DICT, CACHE_SIZE
 from .db import do_get_limit, do_query, do_query_one_limit, do_execute, insert, save, do_select, do_select_one_limit, transaction, batch_insert, \
     do_query_page, do_select_page, do_get
 from .log_support import logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log, orm_find_by_id_log, \
     orm_logical_delete_by_ids_log, orm_count_log, orm_find_log, orm_find_by_ids_log
 
 
 class DelFlag(IntEnum):
@@ -132,15 +132,15 @@
             if not fields:
                 fields, _ = zip(*kv.items())
             m = self.query_by_id(_id, *fields)
             if m:
                 self.__dict__.update(m)
                 return self
             else:
-                msg = "Exec func 'mysqlx.orm.Model.%s' load none, Class: '%s', %s=%d." % ('load', self.__class__.__name__, self._get_pk(), _id)
+                msg = "Exec func 'mysqlx.orm.Model.%s' load none, Class: '%s', %s=%d." % ('load', self.__class__.__name__, pk, _id)
                 logger.error(msg)
                 raise DBError(msg)
         else:
             raise KeyError("Not primary key.")
 
     def logical_delete(self):
         """
@@ -225,15 +225,15 @@
         :return: Instance object
         """
         orm_insert_log('create', cls.__name__, **kwargs)
         pk = cls._get_pk()
         _id = cls.save(**kwargs)
         if pk not in kwargs:
             kwargs[pk] = _id
-        return cls._dict2obj(kwargs)
+        return cls.to_obj(**kwargs)
 
     @classmethod
     def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = User.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
@@ -312,33 +312,44 @@
         pk, table = cls._get_pk_and_table()
         sql = 'DELETE FROM `%s` WHERE `%s`=? limit ?' % (table, pk)
         return do_execute(sql, _id, LIMIT_1)
 
     @classmethod
     def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
-        Physical delete
+        Batch physical delete, they will be executed in batches if there are too many
         rowcount = User.delete_by_ids(id=[1,2])
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', ids: %s, batch_size: %s" % ('delete_by_ids', cls.__name__, ids, batch_size))
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
-
         if ids_size == 1:
             return cls.delete_by_id(ids[0])
         elif ids_size <= batch_size:
-            return cls._delete_by_ids(ids)
+            return cls.do_delete_by_ids(ids)
         else:
             split_ids = _split_ids(ids, batch_size)
             with transaction():
-                results = list(map(cls._delete_by_ids, split_ids))
+                results = list(map(cls.do_delete_by_ids, split_ids))
             return sum(results)
 
     @classmethod
+    def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
+        """
+        Batch physical delete, please use delete_by_ids if there are too many
+        rowcount = Person.do_delete_by_ids(id=[1,2])
+        return: Effect rowcount
+        """
+        ids_size = len(ids)
+        pk, table = cls._get_pk_and_table()
+        sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
+        return do_execute(sql, *ids)
+
+    @classmethod
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = User.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
@@ -400,80 +411,80 @@
     def find(cls, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('find', cls.__name__, *fields, **kwargs)
-        return [cls._dict2obj(d) for d in cls.query(*fields, **kwargs)]
+        return [cls.to_obj(**d) for d in cls.query(*fields, **kwargs)]
 
     @classmethod
     def find_one(cls, *fields, **kwargs):
         """
         Return unique result(object) or None if no result.
         user = User.find_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('find_one', cls.__name__, *fields, **kwargs)
         result = cls.query_one(*fields, **kwargs)
-        return cls._dict2obj(result) if result else None
+        return cls.to_obj(**result) if result else None
 
     @classmethod
     def find_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = User.find_by('where name=?', '李四')
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
-        return [cls._dict2obj(d) for d in cls.query_by(where, *args, **kwargs)]
+        return [cls.to_obj(**d) for d in cls.query_by(where, *args, **kwargs)]
 
     @classmethod
     def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         users = User.find_page(1, 10, 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
         orm_page_log('find_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         result = cls.query_page(page_num, page_size, *fields, **kwargs)
-        return [cls._dict2obj(d) for d in result]
+        return [cls.to_obj(**d) for d in result]
 
     @classmethod
     def find_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = User.find_by_page(1, 10, 'where name=?', '李四')
         """
         orm_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        return [cls._dict2obj(d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
+        return [cls.to_obj(**d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
 
     @classmethod
     def find_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one class object or None if no result.
         user = User.find_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_id_log('find_by_id', cls.__name__, _id, *fields)
         result = cls.query_by_id(_id, *fields)
-        return cls._dict2obj(result) if result else None
+        return cls.to_obj(**result) if result else None
 
     @classmethod
     def find_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(class object) or empty list if no result.
         users = User.find_by_ids([1,2], 'id', 'name', 'age')
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_ids_log('find_by_ids', cls.__name__, ids, *fields)
-        return [cls._dict2obj(d) for d in cls.query_by_ids(ids, *fields)]
+        return [cls.to_obj(**d) for d in cls.query_by_ids(ids, *fields)]
 
     @classmethod
     def query(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         users = User.query('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
@@ -665,14 +676,20 @@
         assert ids_size > 0, 'ids must not be empty.'
 
         pk, table = cls._get_pk_and_table()
         where = 'WHERE `{}` in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return do_select(sql, *ids, ids_size)
 
+    @classmethod
+    def to_obj(cls, **kwargs):
+        model = cls.__new__(cls)
+        model.__dict__.update(**kwargs)
+        return model
+
     # ------------------------------------------------Private class method------------------------------------------------------------------
     @classmethod
     def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         pk, table = cls._get_pk_and_table()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
 
@@ -720,21 +737,14 @@
         else:
             sql, update_time_arg = cls._update_sql(where, del_flag_field)
             if update_time_arg:
                 return do_execute(sql, del_status.value, update_time_arg, *ids, ids_size)
             return do_execute(sql, del_status.value, *ids, ids_size)
 
     @classmethod
-    def _delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
-        ids_size = len(ids)
-        pk, table = cls._get_pk_and_table()
-        sql = 'DELETE FROM `{}` WHERE `{}` in ({}) limit ?'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
-        return do_execute(sql, *ids, ids_size)
-
-    @classmethod
     def _get_pk(cls):
         if hasattr(cls, PK):
             return cls.__pk__
         logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
         return DEFAULT_PK_FIELD
 
     @classmethod
@@ -751,20 +761,14 @@
     @classmethod
     def _get_pk_strategy(cls):
         if hasattr(cls, PK_STRATEGY):
             return cls.__pk_strategy__
         return None
 
     @classmethod
-    def _dict2obj(cls, dictionary):
-        m = cls.__new__(cls)
-        m.__dict__.update(dictionary)
-        return m
-
-    @classmethod
     def _get_update_by_field(cls):
         if hasattr(cls, UPDATE_BY):
             return cls.__update_by__
         return None
 
     @classmethod
     def _get_update_time_field(cls):
@@ -814,15 +818,15 @@
             return 'SELECT {} FROM `{}` {} limit ?,?'.format(fields, table, where)
         else:
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
         return 'SELECT {} FROM `{}` {}'.format(fields, table, where)
 
 
-@lru_cache(maxsize=128)
+@lru_cache(maxsize=CONFIG_DICT[CACHE_SIZE])
 def _get_table_columns(table: str):
     return do_get_limit(COLUMN_SQL, table, LIMIT_1)
 
 
 def _get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
         return "`{}`=?".format(k[:-4]), v
```

### Comparing `mysqlx-1.5.3/mysqlx/snowflake.py` & `mysqlx-1.5.4/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.3/mysqlx/sql_mapper.py` & `mysqlx-1.5.4/mysqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.3/mysqlx/support.py` & `mysqlx-1.5.4/mysqlx/support.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 import threading
 from enum import Enum
 from jinja2 import Template
 from functools import lru_cache
 from .log_support import logger
 from typing import Sequence, List
-from .constant import NAMED_REGEX, DYNAMIC_REGEX
+from .constant import NAMED_REGEX, DYNAMIC_REGEX, CONFIG_DICT, CACHE_SIZE
 
 DB_LOCK = threading.RLock()
 
 
 def get_batch_args(*args):
     return args[0] if isinstance(args, tuple) and len(args) == 1 and isinstance(args[0], Sequence) else args
 
@@ -42,15 +42,15 @@
     return get_named_sql_args(sql, **kwargs)
 
 
 def is_dynamic_sql(sql: str):
     return re.search(DYNAMIC_REGEX, sql)
 
 
-@lru_cache(maxsize=256)
+@lru_cache(maxsize=2*CONFIG_DICT[CACHE_SIZE])
 def _get_sql_type(sql: str):
     """
     :return: 0: placeholder, 1: dynamic, 2: named mapping
     """
     if is_dynamic_sql(sql):
         return 1
     if ':' in sql:
@@ -59,15 +59,15 @@
 
 
 def get_named_sql_args(sql: str, **kwargs):
     args = get_named_args(sql, **kwargs)
     return get_named_sql(sql), args
 
 
-@lru_cache(maxsize=256)
+@lru_cache(maxsize=CONFIG_DICT[CACHE_SIZE])
 def get_named_sql(sql: str):
     return re.sub(NAMED_REGEX, '?', sql)
 
 
 def get_named_args(sql: str, **kwargs):
     return [kwargs[r[1:]] for r in re.findall(NAMED_REGEX, sql)]
```

### Comparing `mysqlx-1.5.3/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.5.4/mysqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.3
+Version: 1.5.4
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -143,10 +143,10 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, please use PgSqlx: https://pypi.org/project/pgsqlx/
+If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx/
```

### Comparing `mysqlx-1.5.3/PKG-INFO` & `mysqlx-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.3
+Version: 1.5.4
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -143,10 +143,10 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, please use PgSqlx: https://pypi.org/project/pgsqlx/
+If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx/
```

### Comparing `mysqlx-1.5.3/README.rst` & `mysqlx-1.5.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -129,8 +129,8 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, please use PgSqlx: https://pypi.org/project/pgsqlx/
+If you want to operate PostgreSQL database, you may need PgSqlx: https://pypi.org/project/pgsqlx/
```

### Comparing `mysqlx-1.5.3/setup.py` & `mysqlx-1.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.5.3',
+    version='1.5.4',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

