# Comparing `tmp/pgsqlx-1.0.0.tar.gz` & `tmp/pgsqlx-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.0.0.tar", last modified: Sat Jul 15 04:29:07 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.0.1.tar", last modified: Sun Jul 16 06:57:58 2023, max compression
```

## Comparing `pgsqlx-1.0.0.tar` & `pgsqlx-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/
--rw-rw-rw-   0        0        0    11558 2023-07-14 14:50:12.000000 pgsqlx-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/pgsqlx/
--rw-rw-rw-   0        0        0      604 2023-07-15 00:05:25.000000 pgsqlx-1.0.0/pgsqlx/constant.py
--rw-rw-rw-   0        0        0    19197 2023-07-15 04:20:36.000000 pgsqlx-1.0.0/pgsqlx/db.py
--rw-rw-rw-   0        0        0    13886 2023-07-15 04:16:12.000000 pgsqlx-1.0.0/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.0/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0    37465 2023-07-15 00:10:02.000000 pgsqlx-1.0.0/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 pgsqlx-1.0.0/pgsqlx/snowflake.py
--rw-rw-rw-   0        0        0     5119 2023-07-14 23:31:12.000000 pgsqlx-1.0.0/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6375 2023-07-14 22:05:14.000000 pgsqlx-1.0.0/pgsqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.0/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4292 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       30 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      365 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4292 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     3758 2023-07-15 04:27:50.000000 pgsqlx-1.0.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-15 04:29:07.000000 pgsqlx-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1204 2023-07-15 04:28:57.000000 pgsqlx-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-07-14 14:50:12.000000 pgsqlx-1.0.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx/
+-rw-rw-rw-   0        0        0      678 2023-07-15 12:19:37.000000 pgsqlx-1.0.1/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0    19259 2023-07-15 12:23:23.000000 pgsqlx-1.0.1/pgsqlx/db.py
+-rw-rw-rw-   0        0        0    13886 2023-07-15 04:16:12.000000 pgsqlx-1.0.1/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 pgsqlx-1.0.1/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0    37094 2023-07-16 02:08:15.000000 pgsqlx-1.0.1/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 pgsqlx-1.0.1/pgsqlx/snowflake.py
+-rw-rw-rw-   0        0        0     5119 2023-07-14 23:31:12.000000 pgsqlx-1.0.1/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6442 2023-07-15 12:25:53.000000 pgsqlx-1.0.1/pgsqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 pgsqlx-1.0.1/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-15 04:29:07.000000 pgsqlx-1.0.1/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4292 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       30 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      365 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4292 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3758 2023-07-16 02:24:38.000000 pgsqlx-1.0.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-16 06:57:58.000000 pgsqlx-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1204 2023-07-16 06:57:53.000000 pgsqlx-1.0.1/setup.py
```

### Comparing `pgsqlx-1.0.0/LICENSE` & `pgsqlx-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.0/pgsqlx/constant.py` & `pgsqlx-1.0.1/pgsqlx/constant.py`

 * *Files 23% similar despite different names*

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
@@ -15,7 +19,9 @@
 BETWEEN, LIKE, IN = 'between', 'like', 'in'
 
 PK, PK_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, PK_STRATEGY = '__pk__', '__pk_seq__', '__table__', '__update_by__', '__update_time__', \
     '__del_flag__', '__pk_strategy__'
 
 COLUMN_SQL = '''SELECT array_to_string(array_agg(column_name),',') as column_name FROM information_schema.columns 
                  WHERE table_schema='public' and table_name = ? LIMIT ?'''
+
+
```

### Comparing `pgsqlx-1.0.0/pgsqlx/db.py` & `pgsqlx-1.0.1/pgsqlx/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 import functools
 from typing import Sequence
-from .constant import LIMIT_1, MAPPER_PATH
+from .constant import LIMIT_1, MAPPER_PATH, CONFIG_DICT, CACHE_SIZE
 from .log_support import logger, sql_log, page_log, insert_log, do_sql_log, do_page_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, dynamic_sql, get_named_sql, get_named_args, DBError, \
     DB_LOCK, get_batch_args
 
 _DB_CTX = None
 _SHOW_SQL = False
 
 
 def init_db(user='root', password='', database='test', host='127.0.0.1', port=3306, show_sql=False, **kwargs):
     global _DB_CTX
     global _SHOW_SQL
     from psycopg2  import connect
 
+    _SHOW_SQL = show_sql
+    kwargs['user'] = user
+    kwargs['password'] = password
+    kwargs['database'] = database
+    kwargs['host'] = host
+    kwargs['port'] = port
+
     if 'debug' in kwargs:
         if kwargs.pop('debug'):
             from logging import DEBUG
             logger.setLevel(DEBUG)
 
+    if CACHE_SIZE in kwargs:
+        CONFIG_DICT[CACHE_SIZE] = kwargs.pop(CACHE_SIZE)
+
     with DB_LOCK:
         if _DB_CTX is not None:
             raise DBError('DB is already initialized.')
-        _SHOW_SQL = show_sql
+
         if MAPPER_PATH in kwargs:
             from .dbx import load_mapper
-            load_mapper(kwargs[MAPPER_PATH])
-            del kwargs[MAPPER_PATH]
+            load_mapper(kwargs.pop(MAPPER_PATH))
 
-        kwargs['user'] = user
-        kwargs['password'] = password
-        kwargs['database'] = database
-        kwargs['host'] = host
-        kwargs['port'] = port
         _DB_CTX = DBCtx(connect=lambda: connect(**kwargs), is_pool=False)
         logger.info('Init db engine <%s> ok without connection pool.' % hex(id(_DB_CTX)))
 
 
 def connection():
     """
     Return _ConnectionCtx object that can be used by 'with' statement:
```

### Comparing `pgsqlx-1.0.0/pgsqlx/dbx.py` & `pgsqlx-1.0.1/pgsqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.0/pgsqlx/log_support.py` & `pgsqlx-1.0.1/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.0/pgsqlx/orm.py` & `pgsqlx-1.0.1/pgsqlx/orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from .snowflake import get_id
 from enum import Enum, IntEnum
 from functools import lru_cache
 from .support import DBError, simple_sql
 from typing import Sequence, Union, List, Tuple
 from .constant import LIMIT_1, NO_LIMIT, DEFAULT_PK_FIELD, SYMBOLS, BETWEEN, LIKE, IN, PK, PK_SEQ, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, \
-    PK_STRATEGY, COLUMN_SQL
+    PK_STRATEGY, COLUMN_SQL, CONFIG_DICT, CACHE_SIZE
 from .db import do_get_limit, do_query, do_query_one_limit, do_execute, insert, save, do_select, do_select_one_limit, transaction, batch_insert, \
     do_query_page, do_select_page, do_get
 from .log_support import logger, orm_page_log, orm_insert_log, orm_by_log, orm_delete_by_id_log, orm_by_page_log, orm_inst_log, orm_find_by_id_log, \
     orm_logical_delete_by_ids_log, orm_count_log, orm_find_log, orm_find_by_ids_log
 
 
 class DelFlag(IntEnum):
@@ -61,21 +61,21 @@
     """
 
     def __str__(self):
         return str({k: v for k, v in self.__dict__.items() if not k.startswith("__")})
 
     def __getattr__(self, name):
         if PK == name:
-            return self._get_pk()
+            return _get_pk(self.__class__)
         elif TABLE == name:
-            return self._get_table()
+            return _get_table(self.__class__)
         elif UPDATE_BY == name:
-            return self._get_update_by_field()
+            return _get_update_by_field(self.__class__)
         elif UPDATE_TIME == name:
-            return self._get_update_time_field()
+            return _get_update_time_field(self.__class__)
         else:
             return None
 
     def persist(self):
         """
         person = Person(name='张三', age=55)
         effect_rowcount = person.persist()
@@ -89,28 +89,28 @@
         """
         person = Person(name='张三', age=55)
         id = person.save()
         :return: Primary key
         """
         orm_inst_log('inst_save', self.__class__.__name__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
-        pk = self._get_pk()
+        pk = _get_pk(self.__class__)
         _id = self.save(**kv)
         if pk not in kv:
             self.__dict__.update({pk: _id})
         return _id
 
     def update(self):
         """
         person = Person(id=1, name='李四', age=66)
         rowcount = person.update()
         :return: Effect rowcount
         """
         orm_inst_log('update', self.__class__.__name__)
-        pk, table = self._get_pk_and_table()
+        pk, table = _get_pk_and_table(self.__class__)
         kv = {k: v for k, v in self.__dict__.items() if v is not None}
         if pk not in kv:
             raise KeyError("Not primary key.")
 
         update_kv = {k: v for k, v in kv.items() if k != pk}
         if update_kv:
             return self.update_by_id(kv[pk], **update_kv)
@@ -122,371 +122,382 @@
         """
         Return new object from database and update itself.
         :param fields: Default select all fields if not set. like: ('id', 'name', 'age')
         person = Person(id=1)
         person2 = person.load()
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s', Class: '%s', fields: %s" % ('load', self.__class__.__name__, fields))
-        pk = self._get_pk()
+        pk = _get_pk(self.__class__)
         kv = self.__dict__
         _id = kv.get(pk)
         if _id is not None:
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
         Logic delete only update the del flag
         person = Person(id=1)
         rowcount = person.logical_delete()
         """
         orm_inst_log('logical_delete', self.__class__.__name__)
-        pk = self._get_pk()
+        pk = _get_pk(self.__class__)
         _id = self.__dict__.get(pk)
-        update_by = self.__dict__.get(self._get_update_by_field())
+        update_by = self.__dict__.get(_get_update_by_field(self.__class__))
         if _id is None:
             raise KeyError("Not primary key.")
 
         return self.logical_delete_by_id(_id, update_by)
 
     def un_logical_delete(self):
         """
         Logic un delete only update the del flag
         person = Person(id=1)
         rowcount = person.un_logical_delete()
         """
         orm_inst_log('un_logical_delete', self.__class__.__name__)
-        pk = self._get_pk()
+        pk = _get_pk(self.__class__)
         _id = self.__dict__.get(pk)
         update_by = self.__dict__.get(self._get_update_by_field())
         if _id is None:
             raise KeyError("Not primary key.")
         return self.un_logical_delete_by_id(_id, update_by)
 
     def delete(self):
         """
         Physical delete
         person = Person(id=1)
         rowcount = person.delete()
         """
         orm_inst_log('delete', self.__class__.__name__)
-        pk = self._get_pk()
+        pk = _get_pk(self.__class__)
         _id = self.__dict__.get(pk)
         if _id is None:
             raise KeyError("Not primary key.")
         return self.delete_by_id(_id)
 
     # ----------------------------------------------------------Class method------------------------------------------------------------------
     @classmethod
     def insert(cls, **kwargs):
         """
         rowcount = Person.insert(name='张三', age=20)
         return: Effect rowcount
         """
         orm_insert_log('insert', cls.__name__, **kwargs)
-        pk, table = cls._get_pk_and_table()
-        pk_strategy = cls._get_pk_strategy()
+        pk, table = _get_pk_and_table(cls)
+        pk_strategy = _get_pk_strategy(cls)
         if pk_strategy == PkStrategy.SNOWFLAKE and pk not in kwargs:
             kwargs[pk] = get_id()
         return insert(table, **kwargs)
 
     @classmethod
     def save(cls, **kwargs):
         """
         id = Person.save(name='张三', age=20)
         :return: Primary key
         """
         orm_insert_log('save', cls.__name__, **kwargs)
-        pk, table = cls._get_pk_and_table()
-        pk_strategy = cls._get_pk_strategy()
+        pk, table = _get_pk_and_table(cls)
+        pk_strategy = _get_pk_strategy(cls)
         if pk_strategy == PkStrategy.SNOWFLAKE:
             if pk in kwargs:
                 _id = kwargs[pk]
             else:
                 _id = get_id()
                 kwargs[pk] = _id
             insert(table, **kwargs)
         else:
-            kwargs['pk_seq'] = cls._get_pk_seq()
+            kwargs['pk_seq'] = _get_pk_seq(cls)
             _id = save(table, **kwargs)
         return _id
 
     @classmethod
     def create(cls, **kwargs):
         """
         person = Person.create(name='张三', age=20)
         :return: Instance object
         """
         orm_insert_log('create', cls.__name__, **kwargs)
-        pk = cls._get_pk()
+        pk = _get_pk(cls)
         _id = cls.save(**kwargs)
         if pk not in kwargs:
             kwargs[pk] = _id
-        return cls._dict2obj(kwargs)
+        return cls.to_obj(**kwargs)
 
     @classmethod
     def update_by_id(cls, _id: Union[int, str], **kwargs):
         """
         rowcount = Person.update_by_id(id=1, name='王五')
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', id: %d, kwargs: %s" % ('update_by_id', cls.__name__, _id, kwargs))
         assert kwargs, 'Must set update kv'
-        pk = cls._get_pk()
+        pk = _get_pk(cls)
         where = '%s=?' % pk
         cols, args = zip(*kwargs.items())
-        sql, update_time_arg = cls._update_sql(where, *cols)
+        sql, update_time_arg = _update_sql(cls, where, *cols)
         if update_time_arg:
             args = [*args, update_time_arg]
         return do_execute(sql, *args, _id)
 
     @classmethod
     def logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = Person.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
-        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
+        return _logical_delete_by_id_op(cls, _id, update_by, DelFlag.DELETED)
 
     @classmethod
     def un_logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
         rowcount = Person.un_logical_delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         orm_delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
-        return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
+        return _logical_delete_by_id_op(cls, _id, update_by, DelFlag.UN_DELETE)
 
     @classmethod
     def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = Person.logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         orm_logical_delete_by_ids_log('logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
-        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
+        return _logical_delete_by_ids_op(cls, ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
 
     @classmethod
     def un_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = Person.un_logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         orm_logical_delete_by_ids_log('un_logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
-        return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
+        return _logical_delete_by_ids_op(cls, ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
 
     @classmethod
     def delete_by(cls, where: str, *args, **kwargs):
         """
         Physical delete
         rowcount = Person.delete_by('where name=? and age=?', '张三', 55)
         return: Effect rowcount
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'WHERE' in the where parameter."
-        table = cls._get_table()
+        table = _get_table(cls)
         sql = 'DELETE FROM %s %s' % (table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_execute(sql, *args)
 
     @classmethod
     def delete_by_id(cls, _id: Union[int, str]):
         """
         Physical delete
         rowcount = Person.delete_by_id(id=1)
         return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', id: %d" % ('delete_by_id', cls.__name__, _id))
-        pk, table = cls._get_pk_and_table()
+        pk, table = _get_pk_and_table(cls)
         sql = 'DELETE FROM %s WHERE %s=?' % (table, pk)
         return do_execute(sql, _id)
 
     @classmethod
     def delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], batch_size=128):
         """
-        Physical delete
+        Batch physical delete, they will be executed in batches if there are too many
         rowcount = Person.delete_by_ids(id=[1,2])
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
+        pk, table = _get_pk_and_table(cls)
+        sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
+        return do_execute(sql, *ids)
+
+    @classmethod
     def batch_insert(cls, *args):
         """
         Batch insert
         rowcount = Person.batch_insert([{'name': '张三', 'age': 55},{'name': '李四', 'age': 66}])
         :param args: All number must have same key.
         :return: Effect rowcount
         """
         logger.debug("Exec func 'mysqlx.orm.Model.%s' \n\t Class: '%s', args: %s" % ('batch_insert', cls.__name__, args))
         assert len(args) > 0, 'args must not be empty.'
-        pk, table = cls._get_pk_and_table()
-        pk_strategy = cls._get_pk_strategy()
+        pk, table = _get_pk_and_table(cls)
+        pk_strategy = _get_pk_strategy(cls)
         if pk_strategy == PkStrategy.SNOWFLAKE:
             for arg in args:
                 if pk not in arg:
                     arg[pk] = get_id()
 
         return batch_insert(table, *args)
 
     # ------------------------------------------------Class query method--------------------------------------------------------
     @classmethod
     def count(cls, **kwargs):
         """
         count = Person.count(name='张三', age=55)
         """
         orm_count_log('count', cls.__name__, **kwargs)
-        table = cls._get_table()
+        table = _get_table(cls)
         where, args, _ = _get_where_arg_limit(**kwargs)
         fields = 'count(1)'
         sql = _select_sql(table, where, LIMIT_1, fields)
         return do_get_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = Person.count_by('where name=?', '李四')
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
-        table = cls._get_table()
+        table = _get_table(cls)
         sql = "SELECT count(1) FROM {} {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_get(sql, *args)
 
     @classmethod
     def exists(cls, **kwargs):
         orm_count_log('exists', cls.__name__, **kwargs)
-        table = cls._get_table()
+        table = _get_table(cls)
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = "SELECT 1 FROM {} {} limit ?".format(table, where)
         return do_get_limit(sql, *args, LIMIT_1) == 1
 
     @classmethod
     def exists_by(cls, where: str, *args, **kwargs):
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
-        table = cls._get_table()
+        table = _get_table(cls)
         sql = "SELECT 1 FROM {} {}".format(table, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_get(sql, *args) == 1
 
     @classmethod
     def find(cls, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         persons = Person.find('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('find', cls.__name__, *fields, **kwargs)
-        return [cls._dict2obj(d) for d in cls.query(*fields, **kwargs)]
+        return [cls.to_obj(**d) for d in cls.query(*fields, **kwargs)]
 
     @classmethod
     def find_one(cls, *fields, **kwargs):
         """
         Return unique result(object) or None if no result.
         person = Person.find_one('id', 'name', 'age', name='张三', age=55)
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
         rows = Person.find_by('where name=?', '李四')
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
-        return [cls._dict2obj(d) for d in cls.query_by(where, *args, **kwargs)]
+        return [cls.to_obj(**d) for d in cls.query_by(where, *args, **kwargs)]
 
     @classmethod
     def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         persons = Person.find_page(1, 10, 'name', 'age', name='张三', age=55)
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
         rows = Person.find_by_page(1, 10, 'where name=?', '李四')
         """
         orm_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        return [cls._dict2obj(d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
+        return [cls.to_obj(**d) for d in cls.query_page_by(page_num, page_size, where, *args, **kwargs)]
 
     @classmethod
     def find_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one class object or None if no result.
         person = Person.find_by_id(1, 'id', 'name', 'age')
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
         persons = Person.find_by_ids([1,2], 'id', 'name', 'age')
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
         persons = Person.query('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('query', cls.__name__, *fields, **kwargs)
         where, args, limit = _get_where_arg_limit(**kwargs)
-        table = cls._get_table()
+        table = _get_table(cls)
         sql = _select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
         return do_query(sql, *args)
@@ -496,65 +507,65 @@
         """
         Return unique result(dict) or None if no result.
         persons = Person.query_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('query_one', cls.__name__, *fields, **kwargs)
         where, args, _ = _get_where_arg_limit(**kwargs)
-        table = cls._get_table()
+        table = _get_table(cls)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_query_one_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.query_by('where name=?', '李四')
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
-        sql = cls._where_sql(where)
+        sql = _where_sql(cls, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_query(sql, *args)
 
     @classmethod
     def query_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         persons = Person.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
         orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        table = cls._get_table()
+        table = _get_table(cls)
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
         return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = Person.query_by_page(1, 10, 'where name=?', '李四')
         """
         orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        sql = cls._where_sql(where)
+        sql = _where_sql(cls, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         person = Person.query_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
-        pk, table = cls._get_pk_and_table()
+        pk, table = _get_pk_and_table(cls)
         where = 'WHERE {}=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_query_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
@@ -563,29 +574,29 @@
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk, table = cls._get_pk_and_table()
+        pk, table = _get_pk_and_table(cls)
         where = 'WHERE {} in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return do_query(sql, *ids, ids_size)
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('select', cls.__name__, *fields, **kwargs)
         where, args, limit = _get_where_arg_limit(**kwargs)
-        table = cls._get_table()
+        table = _get_table(cls)
         sql = _select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
         return do_select(sql, *args)
@@ -595,65 +606,65 @@
         """
         Return unique result(tuple) or None if no result.
         row = Person.select_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         orm_find_log('select_one', cls.__name__, *fields, **kwargs)
         where, args, _ = _get_where_arg_limit(**kwargs)
-        table = cls._get_table()
+        table = _get_table(cls)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_select_one_limit(sql, *args, LIMIT_1)
 
     @classmethod
     def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by('where name=?', '李四')
         """
         orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
-        sql = cls._where_sql(where)
+        sql = _where_sql(cls, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_select(sql, *args)
 
     @classmethod
     def select_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_page('id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
         orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
-        table = cls._get_table()
+        table = _get_table(cls)
         where, args, _ = _get_where_arg_limit(**kwargs)
         sql = _select_sql(table, where, NO_LIMIT, *fields)
         return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = Person.select_by_page(1, 10, 'where name=?', '李四')
         """
         orm_by_page_log(sys._getframe().f_code.co_name, page_num, page_size, cls.__name__, where, *args, **kwargs)
-        sql = cls._where_sql(where)
+        sql = _where_sql(cls, where)
         sql, args = simple_sql(sql, *args, **kwargs)
         return do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_by_id(cls, _id: Union[int, str], *fields):
         """
         Return one row(dict) or None if no result.
         row = Person.select_by_id(1, 'id', 'name', 'age')
         :param _id: pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
-        pk, table = cls._get_pk_and_table()
+        pk, table = _get_pk_and_table(cls)
         where = 'WHERE {}=?'.format(pk)
         sql = _select_sql(table, where, LIMIT_1, *fields)
         return do_select_one_limit(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
@@ -662,159 +673,151 @@
         :param ids: List of pk
         :param fields: Default select all fields if not set
         """
         orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
-        pk, table = cls._get_pk_and_table()
+        pk, table = _get_pk_and_table(cls)
         where = 'WHERE {} in ({})'.format(pk, ','.join(['?' for _ in range(ids_size)]))
         sql = _select_sql(table, where, ids_size, *fields)
         return do_select(sql, *ids, ids_size)
 
-    # ------------------------------------------------Private class method------------------------------------------------------------------
     @classmethod
-    def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
-        pk, table = cls._get_pk_and_table()
-        del_flag_field = cls._get_del_flag_field()
-        update_by_field = cls._get_update_by_field()
+    def to_obj(cls, **kwargs):
+        model = cls.__new__(cls)
+        model.__dict__.update(**kwargs)
+        return model
 
-        where = '%s=?' % pk
-        if update_by is not None and update_by_field is not None:
-            sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
-            if update_time_arg:
-                return do_execute(sql, del_status.value, update_by, update_time_arg, _id)
-            return do_execute(sql, del_status.value, update_by, _id)
-        else:
-            sql, update_time_arg = cls._update_sql(where, del_flag_field)
-            if update_time_arg:
-                return do_execute(sql, del_status.value, update_time_arg, _id)
-            return do_execute(sql, del_status.value, _id)
 
-    @classmethod
-    def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
-            del_status=DelFlag.DELETED):
-        ids_size = len(ids)
-        assert ids_size > 0, 'ids must not be empty.'
+# ------------------------------------------------Private function------------------------------------------------------------------
+def _logical_delete_by_id_op(cls, _id: Union[int, str], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
+    pk, table = _get_pk_and_table(cls)
+    del_flag_field = _get_del_flag_field(cls)
+    update_by_field = _get_update_by_field(cls)
+
+    where = '%s=?' % pk
+    if update_by is not None and update_by_field is not None:
+        sql, update_time_arg = _update_sql(cls, where, del_flag_field, update_by_field)
+        if update_time_arg:
+            return do_execute(sql, del_status.value, update_by, update_time_arg, _id)
+        return do_execute(sql, del_status.value, update_by, _id)
+    else:
+        sql, update_time_arg = _update_sql(cls, where, del_flag_field)
+        if update_time_arg:
+            return do_execute(sql, del_status.value, update_time_arg, _id)
+        return do_execute(sql, del_status.value, _id)
 
-        if ids_size == 1:
-            return cls._logical_delete_by_id_op(ids[0], update_by, del_status)
-        elif ids_size <= batch_size:
-            return cls._do_logical_delete_by_ids(ids, update_by, del_status)
-        else:
-            split_ids = _split_ids(ids, batch_size)
-            with transaction():
-                results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
-            return sum(results)
 
-    @classmethod
-    def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
-        ids_size = len(ids)
-        pk = cls._get_pk()
-        del_flag_field = cls._get_del_flag_field()
-        update_by_field = cls._get_update_by_field()
-
-        where = '%s in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
-        if update_by is not None and update_by_field is not None:
-            sql, update_time_arg = cls._update_sql(where, del_flag_field, update_by_field)
-            if update_time_arg:
-                return do_execute(sql, del_status.value, update_by, update_time_arg, *ids)
-            return do_execute(sql, del_status.value, update_by, *ids)
-        else:
-            sql, update_time_arg = cls._update_sql(where, del_flag_field)
-            if update_time_arg:
-                return do_execute(sql, del_status.value, update_time_arg, *ids)
-            return do_execute(sql, del_status.value, *ids)
+def _logical_delete_by_ids_op(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128,
+        del_status=DelFlag.DELETED):
+    ids_size = len(ids)
+    assert ids_size > 0, 'ids must not be empty.'
+
+    if ids_size == 1:
+        return _logical_delete_by_id_op(cls, ids[0], update_by, del_status)
+    elif ids_size <= batch_size:
+        return _do_logical_delete_by_ids(cls, ids, update_by, del_status)
+    else:
+        split_ids = _split_ids(ids, batch_size)
+        with transaction():
+            results = [_do_logical_delete_by_ids(cls, ids, update_by, del_status) for ids in split_ids]
+        return sum(results)
 
-    @classmethod
-    def _delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
-        ids_size = len(ids)
-        pk, table = cls._get_pk_and_table()
-        sql = 'DELETE FROM {} WHERE {} in ({})'.format(table, pk, ','.join(['?' for _ in range(ids_size)]))
-        return do_execute(sql, *ids)
 
-    @classmethod
-    def _get_pk(cls):
-        if hasattr(cls, PK):
-            return cls.__pk__
-        logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
-        return DEFAULT_PK_FIELD
+def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
+    ids_size = len(ids)
+    pk = _get_pk(cls)
+    del_flag_field = _get_del_flag_field(cls)
+    update_by_field = _get_update_by_field(cls)
+
+    where = '%s in (%s)' % (pk, ','.join(['?' for _ in range(ids_size)]))
+    if update_by is not None and update_by_field is not None:
+        sql, update_time_arg = _update_sql(cls, where, del_flag_field, update_by_field)
+        if update_time_arg:
+            return do_execute(sql, del_status.value, update_by, update_time_arg, *ids)
+        return do_execute(sql, del_status.value, update_by, *ids)
+    else:
+        sql, update_time_arg = _update_sql(cls, where, del_flag_field)
+        if update_time_arg:
+            return do_execute(sql, del_status.value, update_time_arg, *ids)
+        return do_execute(sql, del_status.value, *ids)
 
-    @classmethod
-    def _get_pk_seq(cls):
-        if hasattr(cls, PK_SEQ):
-            return cls.__pk_seq__
-        logger.warning("%s not set attribute '%s'" % (cls.__name__, PK_SEQ))
-        pk, table = cls._get_pk_and_table()
-        return "{}_{}_seq".format(table, pk)
 
-    @classmethod
-    def _get_table(cls):
-        if hasattr(cls, TABLE):
-            return cls.__table__
-        logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
-        return _get_table_name(cls.__name__)
+def _get_pk(cls):
+    if hasattr(cls, PK):
+        return cls.__pk__
+    logger.warning("%s not set attribute '%s'" % (cls.__name__, PK))
+    return DEFAULT_PK_FIELD
 
-    @classmethod
-    def _get_pk_and_table(cls):
-        return cls._get_pk(), cls._get_table()
 
-    @classmethod
-    def _get_pk_strategy(cls):
-        if hasattr(cls, PK_STRATEGY):
-            return cls.__pk_strategy__
-        return None
+def _get_pk_seq(cls):
+    if hasattr(cls, PK_SEQ):
+        return cls.__pk_seq__
+    logger.warning("%s not set attribute '%s'" % (cls.__name__, PK_SEQ))
+    pk, table = _get_pk_and_table(cls)
+    return "{}_{}_seq".format(table, pk)
 
-    @classmethod
-    def _dict2obj(cls, dictionary):
-        m = cls.__new__(cls)
-        m.__dict__.update(dictionary)
-        return m
 
-    @classmethod
-    def _get_update_by_field(cls):
-        if hasattr(cls, UPDATE_BY):
-            return cls.__update_by__
-        return None
+def _get_table(cls):
+    if hasattr(cls, TABLE):
+        return cls.__table__
+    logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
+    return _get_table_name(cls.__name__)
 
-    @classmethod
-    def _get_update_time_field(cls):
-        if hasattr(cls, UPDATE_TIME):
-            return cls.__update_time__
-        return None
 
-    @classmethod
-    def _get_del_flag_field(cls):
-        assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
-        return cls.__del_flag__
+def _get_pk_and_table(cls):
+    return _get_pk(cls), _get_table(cls)
 
-    @classmethod
-    def _update_sql(cls, where, *update_fields):
-        update_time_arg = None
-        table = cls._get_table()
-        update_time_field = cls._get_update_time_field()
-        if update_time_field is not None and update_time_field not in update_fields:
-            update_fields = [*update_fields, update_time_field]
-            update_time_arg = datetime.now()
 
-        update_fields = ','.join(['{}=?'.format(col) for col in update_fields])
-        return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
+def _get_pk_strategy(cls):
+    if hasattr(cls, PK_STRATEGY):
+        return cls.__pk_strategy__
+    return None
 
-    @classmethod
-    def _where_sql(cls, where: str):
-        low_where = where.lower()
-        if low_where.startswith('where'):
-            table = cls._get_table()
-            return _select_sql(table, where, NO_LIMIT)
-        elif low_where.startswith('select'):
-            return where
-        raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
+
+def _get_update_by_field(cls):
+    if hasattr(cls, UPDATE_BY):
+        return cls.__update_by__
+    return None
+
+
+def _get_update_time_field(cls):
+    if hasattr(cls, UPDATE_TIME):
+        return cls.__update_time__
+    return None
+
+
+def _get_del_flag_field(cls):
+    assert hasattr(cls, DEL_FLAG), "%s not set attribute '%s'" % (cls.__name__, DEL_FLAG)
+    return cls.__del_flag__
+
+
+def _update_sql(cls, where, *update_fields):
+    update_time_arg = None
+    table = _get_table(cls)
+    update_time_field = _get_update_time_field(cls)
+    if update_time_field is not None and update_time_field not in update_fields:
+        update_fields = [*update_fields, update_time_field]
+        update_time_arg = datetime.now()
+
+    update_fields = ','.join(['{}=?'.format(col) for col in update_fields])
+    return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
+
+
+def _where_sql(cls, where: str):
+    low_where = where.lower()
+    if low_where.startswith('where'):
+        table = _get_table(cls)
+        return _select_sql(table, where, NO_LIMIT)
+    elif low_where.startswith('select'):
+        return where
+    raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
 
 
-# ----------------------------------------------------------Private function------------------------------------------------------------------
 def _select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
     if fields:
         fields = ','.join([col if '(' in col else '{}'.format(col) for col in fields])
     else:
         fields = _get_table_columns(table)
 
     if limit:
@@ -824,15 +827,15 @@
             return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(fields, table, where)
         else:
             raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
     else:
         return 'SELECT {} FROM {} {}'.format(fields, table, where)
 
 
-@lru_cache(maxsize=128)
+@lru_cache(maxsize=CONFIG_DICT[CACHE_SIZE])
 def _get_table_columns(table: str):
     return do_get_limit(COLUMN_SQL, table, LIMIT_1)
 
 
 def _get_condition_arg(k: str, v: object):
     if k.endswith("__eq"):
         return "{}=?".format(k[:-4]), v
```

### Comparing `pgsqlx-1.0.0/pgsqlx/snowflake.py` & `pgsqlx-1.0.1/pgsqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.0/pgsqlx/sql_mapper.py` & `pgsqlx-1.0.1/pgsqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.0.0/pgsqlx/support.py` & `pgsqlx-1.0.1/pgsqlx/support.py`

 * *Files 2% similar despite different names*

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

### Comparing `pgsqlx-1.0.0/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.0.1/pgsqlx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.0
+Version: 1.0.1
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -142,10 +142,10 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate a MySQL database, please use MySqlx: https://pypi.org/project/mysqlx
+If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
```

### Comparing `pgsqlx-1.0.0/PKG-INFO` & `pgsqlx-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.0.0
+Version: 1.0.1
 Summary: PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
@@ -142,10 +142,10 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate a MySQL database, please use MySqlx: https://pypi.org/project/mysqlx
+If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
```

### Comparing `pgsqlx-1.0.0/README.rst` & `pgsqlx-1.0.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -128,8 +128,8 @@
 
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 
-If you want to operate a MySQL database, please use MySqlx: https://pypi.org/project/mysqlx
+If you want to operate MySQL database, you may need MySqlx: https://pypi.org/project/mysqlx
```

### Comparing `pgsqlx-1.0.0/setup.py` & `pgsqlx-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="PgSqlx is a simple python sql executor for PostgreSQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         'psycopg2>=2.7.4',
     ],
-    version='1.0.0',
+    version='1.0.1',
     url='https://gitee.com/summry/pgsqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

