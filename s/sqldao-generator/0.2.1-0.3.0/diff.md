# Comparing `tmp/sqldao-generator-0.2.1.tar.gz` & `tmp/sqldao-generator-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldao-generator-0.2.1.tar", last modified: Sat Jul 15 07:46:25 2023, max compression
+gzip compressed data, was "sqldao-generator-0.3.0.tar", last modified: Sun Jul 16 06:59:18 2023, max compression
```

## Comparing `sqldao-generator-0.2.1.tar` & `sqldao-generator-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.126779 sqldao-generator-0.2.1/
--rw-rw-rw-   0        0        0      440 2023-07-15 07:46:25.126779 sqldao-generator-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2556 2023-07-15 06:50:28.000000 sqldao-generator-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 07:46:25.126779 sqldao-generator-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      930 2023-07-15 07:43:56.000000 sqldao-generator-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.126779 sqldao-generator-0.2.1/sqldao_generator.egg-info/
--rw-rw-rw-   0        0        0      440 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1857 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.095129 sqldao-generator-0.2.1/sqldaogenerator/
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.095129 sqldao-generator-0.2.1/sqldaogenerator/common/
--rw-rw-rw-   0        0        0      575 2023-07-15 05:33:46.000000 sqldao-generator-0.2.1/sqldaogenerator/common/Criterion.py
--rw-rw-rw-   0        0        0      263 2023-07-09 05:32:41.000000 sqldao-generator-0.2.1/sqldaogenerator/common/Database.py
--rw-rw-rw-   0        0        0     2060 2023-07-15 07:37:04.000000 sqldao-generator-0.2.1/sqldaogenerator/common/TransactionManager.py
--rw-rw-rw-   0        0        0        0 2023-07-01 05:44:52.000000 sqldao-generator-0.2.1/sqldaogenerator/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.095129 sqldao-generator-0.2.1/sqldaogenerator/entity/
--rw-rw-rw-   0        0        0      245 2023-07-04 11:14:21.000000 sqldao-generator-0.2.1/sqldaogenerator/entity/General.py
--rw-rw-rw-   0        0        0      142 2023-07-04 12:50:50.000000 sqldao-generator-0.2.1/sqldaogenerator/entity/Page.py
--rw-rw-rw-   0        0        0        0 2023-07-01 13:43:56.000000 sqldao-generator-0.2.1/sqldaogenerator/entity/__init__.py
--rw-rw-rw-   0        0        0       86 2023-06-30 13:49:06.000000 sqldao-generator-0.2.1/sqldaogenerator/entity/base.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.110138 sqldao-generator-0.2.1/sqldaogenerator/generator/
--rw-rw-rw-   0        0        0        0 2023-06-28 05:41:54.000000 sqldao-generator-0.2.1/sqldaogenerator/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.111144 sqldao-generator-0.2.1/sqldaogenerator/generator/enums/
--rw-rw-rw-   0        0        0      324 2023-07-02 06:41:27.000000 sqldao-generator-0.2.1/sqldaogenerator/generator/enums/MySqlTypeEnum.py
--rw-rw-rw-   0        0        0        0 2023-06-28 06:35:09.000000 sqldao-generator-0.2.1/sqldaogenerator/generator/enums/__init__.py
--rw-rw-rw-   0        0        0     9478 2023-07-15 07:37:04.000000 sqldao-generator-0.2.1/sqldaogenerator/generator/mysql_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.111144 sqldao-generator-0.2.1/sqldaogenerator/logger/
--rw-rw-rw-   0        0        0        0 2023-06-28 05:41:42.000000 sqldao-generator-0.2.1/sqldaogenerator/logger/__init__.py
--rw-rw-rw-   0        0        0      139 2023-07-02 12:44:00.000000 sqldao-generator-0.2.1/sqldaogenerator/logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.111144 sqldao-generator-0.2.1/sqldaogenerator/resources/
--rw-rw-rw-   0        0        0        0 2023-07-02 05:38:36.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/__init__.py
--rw-rw-rw-   0        0        0      915 2023-07-15 07:41:08.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/base_dao_template.txt
--rw-rw-rw-   0        0        0     1095 2023-07-15 05:33:47.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/criterion_template.txt
--rw-rw-rw-   0        0        0     3283 2023-07-15 07:41:38.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/dao_template.txt
--rw-rw-rw-   0        0        0      723 2023-07-15 05:28:29.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/datasource_template.txt
--rw-rw-rw-   0        0        0      361 2023-07-15 05:28:29.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/entity_template.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.258346 sqldao-generator-0.3.0/
+-rw-rw-rw-   0        0        0      440 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2558 2023-07-16 06:07:18.000000 sqldao-generator-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 06:59:18.258346 sqldao-generator-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-07-16 06:11:26.000000 sqldao-generator-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/sqldao_generator.egg-info/
+-rw-rw-rw-   0        0        0      440 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-16 06:59:18.000000 sqldao-generator-0.3.0/sqldao_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.211470 sqldao-generator-0.3.0/sqldaogenerator/
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.227096 sqldao-generator-0.3.0/sqldaogenerator/common/
+-rw-rw-rw-   0        0        0      575 2023-07-15 05:33:46.000000 sqldao-generator-0.3.0/sqldaogenerator/common/Criterion.py
+-rw-rw-rw-   0        0        0      263 2023-07-09 05:32:41.000000 sqldao-generator-0.3.0/sqldaogenerator/common/Database.py
+-rw-rw-rw-   0        0        0     2261 2023-07-16 06:42:12.000000 sqldao-generator-0.3.0/sqldaogenerator/common/TransactionManager.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 05:44:52.000000 sqldao-generator-0.3.0/sqldaogenerator/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.227096 sqldao-generator-0.3.0/sqldaogenerator/entity/
+-rw-rw-rw-   0        0        0      245 2023-07-04 11:14:21.000000 sqldao-generator-0.3.0/sqldaogenerator/entity/General.py
+-rw-rw-rw-   0        0        0      142 2023-07-04 12:50:50.000000 sqldao-generator-0.3.0/sqldaogenerator/entity/Page.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 13:43:56.000000 sqldao-generator-0.3.0/sqldaogenerator/entity/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-06-30 13:49:06.000000 sqldao-generator-0.3.0/sqldaogenerator/entity/base.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.227096 sqldao-generator-0.3.0/sqldaogenerator/generator/
+-rw-rw-rw-   0        0        0        0 2023-06-28 05:41:54.000000 sqldao-generator-0.3.0/sqldaogenerator/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/sqldaogenerator/generator/enums/
+-rw-rw-rw-   0        0        0      324 2023-07-02 06:41:27.000000 sqldao-generator-0.3.0/sqldaogenerator/generator/enums/MySqlTypeEnum.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 06:35:09.000000 sqldao-generator-0.3.0/sqldaogenerator/generator/enums/__init__.py
+-rw-rw-rw-   0        0        0     9478 2023-07-15 07:37:04.000000 sqldao-generator-0.3.0/sqldaogenerator/generator/mysql_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/sqldaogenerator/logger/
+-rw-rw-rw-   0        0        0        0 2023-06-28 05:41:42.000000 sqldao-generator-0.3.0/sqldaogenerator/logger/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-07-02 12:44:00.000000 sqldao-generator-0.3.0/sqldaogenerator/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-16 06:59:18.242719 sqldao-generator-0.3.0/sqldaogenerator/resources/
+-rw-rw-rw-   0        0        0        0 2023-07-02 05:38:36.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-07-15 07:41:08.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/base_dao_template.txt
+-rw-rw-rw-   0        0        0     1095 2023-07-15 05:33:47.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/criterion_template.txt
+-rw-rw-rw-   0        0        0     3018 2023-07-16 06:07:37.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/dao_template.txt
+-rw-rw-rw-   0        0        0      723 2023-07-15 05:28:29.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/datasource_template.txt
+-rw-rw-rw-   0        0        0      361 2023-07-15 05:28:29.000000 sqldao-generator-0.3.0/sqldaogenerator/resources/entity_template.txt
```

### Comparing `sqldao-generator-0.2.1/README.md` & `sqldao-generator-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,13 +97,13 @@
 
 - Execute in the same transaction
 
 ```python
 from sqldaogenerator.common.TransactionManager import transactional
 
 
-@transactional
+@transactional()
 def test_transactional(self):
     insert...
     update...
     delete...
 ```
```

### Comparing `sqldao-generator-0.2.1/setup.py` & `sqldao-generator-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sqldao-generator',
-    version='0.2.1',
+    version='0.3.0',
     author='Daniel Hsu',
     description='SqlAlchemy DAO generator',
     long_description_content_type='text/markdown',
     url='https://github.com/davidhsusl/sqldao-generator',
     keywords='SQLAlchemy, mysql',
     python_requires='>=3.10, <4',
     py_modules=['sqldaogenerator'],  # Name of the python package
```

### Comparing `sqldao-generator-0.2.1/sqldao_generator.egg-info/SOURCES.txt` & `sqldao-generator-0.3.0/sqldao_generator.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -20,28 +20,8 @@
 ./sqldaogenerator/resources/dao_template.txt
 ./sqldaogenerator/resources/datasource_template.txt
 ./sqldaogenerator/resources/entity_template.txt
 sqldao_generator.egg-info/PKG-INFO
 sqldao_generator.egg-info/SOURCES.txt
 sqldao_generator.egg-info/dependency_links.txt
 sqldao_generator.egg-info/requires.txt
-sqldao_generator.egg-info/top_level.txt
-sqldaogenerator/common/Criterion.py
-sqldaogenerator/common/Database.py
-sqldaogenerator/common/TransactionManager.py
-sqldaogenerator/common/__init__.py
-sqldaogenerator/entity/General.py
-sqldaogenerator/entity/Page.py
-sqldaogenerator/entity/__init__.py
-sqldaogenerator/entity/base.py
-sqldaogenerator/generator/__init__.py
-sqldaogenerator/generator/mysql_generator.py
-sqldaogenerator/generator/enums/MySqlTypeEnum.py
-sqldaogenerator/generator/enums/__init__.py
-sqldaogenerator/logger/__init__.py
-sqldaogenerator/logger/logger.py
-sqldaogenerator/resources/__init__.py
-sqldaogenerator/resources/base_dao_template.txt
-sqldaogenerator/resources/criterion_template.txt
-sqldaogenerator/resources/dao_template.txt
-sqldaogenerator/resources/datasource_template.txt
-sqldaogenerator/resources/entity_template.txt
+sqldao_generator.egg-info/top_level.txt
```

### Comparing `sqldao-generator-0.2.1/sqldaogenerator/common/Criterion.py` & `sqldao-generator-0.3.0/sqldaogenerator/common/Criterion.py`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.2.1/sqldaogenerator/common/TransactionManager.py` & `sqldao-generator-0.3.0/sqldaogenerator/common/TransactionManager.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,33 +5,14 @@
 
 from sqldaogenerator.logger.logger import info
 
 default_name = 'default'
 transaction_managers = {}
 
 
-def register_transaction_manager(name: str, transaction_manager):
-    transaction_managers.update({name: transaction_manager})
-
-
-def transactional(func):
-    def wrapper(*args, **kwargs):
-        if transaction_managers[default_name].is_exists():
-            info('Participating in an existing transaction.')
-            result = func(*args, **kwargs)
-        else:
-            info('Creating a new transaction.')
-            with transaction_managers[default_name] as session:
-                result = func(*args, **kwargs)
-                session.commit()
-        return result
-
-    return wrapper
-
-
 class TransactionManager:
     name: str
     session_maker: sessionmaker
     transaction_thread = threading.local()
 
     def __new__(cls, name: str, datasource):
         instance = super(TransactionManager, cls).__new__(cls)
@@ -59,7 +40,31 @@
         if self.is_exists():
             return self.transaction_thread.session
         else:
             raise LookupError('No existing transaction.')
 
     def new_transaction(self):
         return self.session_maker()
+
+
+def register_transaction_manager(name: str,
+                                 transaction_manager: TransactionManager):
+    transaction_managers.update({name: transaction_manager})
+
+
+def transactional(auto_commit=True):
+    def decorator(func):
+        def wrapper(*args, **kwargs):
+            if transaction_managers[default_name].is_exists():
+                info('Participating in an existing transaction.')
+                result = func(*args, **kwargs)
+            else:
+                info('Creating a new transaction.')
+                with transaction_managers[default_name] as session:
+                    result = func(*args, **kwargs)
+                    if auto_commit:
+                        session.commit()
+            return result
+
+        return wrapper
+
+    return decorator
```

### Comparing `sqldao-generator-0.2.1/sqldaogenerator/generator/mysql_generator.py` & `sqldao-generator-0.3.0/sqldaogenerator/generator/mysql_generator.py`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.2.1/sqldaogenerator/resources/base_dao_template.txt` & `sqldao-generator-0.3.0/sqldaogenerator/resources/base_dao_template.txt`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.2.1/sqldaogenerator/resources/criterion_template.txt` & `sqldao-generator-0.3.0/sqldaogenerator/resources/criterion_template.txt`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.2.1/sqldaogenerator/resources/dao_template.txt` & `sqldao-generator-0.3.0/sqldaogenerator/resources/dao_template.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,64 +6,57 @@
 from {entity_package}.{entity_name} import {entity_name}
 from sqldaogenerator.common.Criterion import Criterion
 from sqldaogenerator.common.TransactionManager import transactional
 
 
 class {entity_name}Dao({base_dao_name}):
 
+    @transactional(auto_commit=False)
     def select(self, criterion: Criterion) -> tuple[list[{entity_name}], int]:
         criterion_list = criterion.to_list()
         assert self.is_in_modules(criterion_list, {entity_name}), \
             'The expressions must be created by the {entity_name} entity.'
-        is_transaction_exists = self.is_transaction_exists()
-        if is_transaction_exists:
-            session = self.get_transaction()
-        else:
-            session = self.new_transaction()
-        try:
-            page = criterion.page
-            orders = page.order_by.split(' ')
-            query = session.query({entity_name}).filter(*criterion_list) \
-                .order_by(eval(f"{entity_name}.{{orders[0]}}.{{orders[1]}}()"))
-            total = None
-            if page.page_no is not None and page.page_size is not None:
-                query = query.offset((page.page_no - 1) * page.page_size) \
-                    .limit(page.page_size)
-                total = session.query({entity_name}).filter(*criterion_list).count()
-            entities = query.all()
-        finally:
-            if not is_transaction_exists:
-                session.close()
+        session = self.get_transaction()
+        page = criterion.page
+        orders = page.order_by.split(' ')
+        query = session.query({entity_name}).filter(*criterion_list) \
+            .order_by(eval(f"{entity_name}.{{orders[0]}}.{{orders[1]}}()"))
+        total = None
+        if page.page_no is not None and page.page_size is not None:
+            query = query.offset((page.page_no - 1) * page.page_size) \
+                .limit(page.page_size)
+            total = session.query({entity_name}).filter(*criterion_list).count()
+        entities = query.all()
         return entities, total or len(entities)
 
-    @transactional
+    @transactional()
     def insert(self, criterion: Criterion):
         session = self.get_transaction()
         entity = {entity_name}(**criterion.values)
         session.add(entity)
         session.flush()
         session.refresh(entity)
         session.expunge(entity)
         return entity
 
-    @transactional
+    @transactional()
     def update(self, criterion: Criterion):
         criterion_list = criterion.to_list()
         assert criterion_list is not None and len(criterion_list) > 0, \
             'Must have at least one condition in the update.'
         assert self.is_in_modules(criterion_list, {entity_name}), \
             'The expressions must be created by the {entity_name} entity.'
         session = self.get_transaction()
         entities = session.query({entity_name}).filter(*criterion_list).all()
         for entity in entities:
             for key, value in criterion.items():
                 setattr(entity, key, value)
         return len(entities)
 
-    @transactional
+    @transactional()
     def delete(self, criterion: Criterion):
         criterion_list = criterion.to_list()
         assert criterion_list is not None and len(criterion_list) > 0, \
             'Must have at least one condition in the delete.'
         assert self.is_in_modules(criterion_list, {entity_name}), \
             'The expressions must be created by the {entity_name} entity.'
         session = self.get_transaction()
```

### Comparing `sqldao-generator-0.2.1/sqldaogenerator/resources/datasource_template.txt` & `sqldao-generator-0.3.0/sqldaogenerator/resources/datasource_template.txt`

 * *Files identical despite different names*

