# Comparing `tmp/casbin_async_sqlalchemy_adapter-1.1.1.tar.gz` & `tmp/casbin_async_sqlalchemy_adapter-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.1.1.tar", last modified: Thu Jul 13 09:32:36 2023, max compression
+gzip compressed data, was "casbin_async_sqlalchemy_adapter-1.2.0.tar", last modified: Sun Jul 16 15:29:21 2023, max compression
```

## Comparing `casbin_async_sqlalchemy_adapter-1.1.1.tar` & `casbin_async_sqlalchemy_adapter-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10919 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-13 09:32:36.000000 casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 09:32:36.938301 casbin_async_sqlalchemy_adapter-1.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-13 09:32:06.000000 casbin_async_sqlalchemy_adapter-1.1.1/tests/test_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:29:21.138502 casbin_async_sqlalchemy_adapter-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-16 15:29:21.142502 casbin_async_sqlalchemy_adapter-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:29:21.138502 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:29:21.138502 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 15:29:21.000000 casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-16 15:29:21.142502 casbin_async_sqlalchemy_adapter-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:29:21.138502 casbin_async_sqlalchemy_adapter-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-07-16 15:28:44.000000 casbin_async_sqlalchemy_adapter-1.2.0/tests/test_adapter.py
```

### Comparing `casbin_async_sqlalchemy_adapter-1.1.1/LICENSE` & `casbin_async_sqlalchemy_adapter-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.1.1/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin_async_sqlalchemy_adapter
-Version: 1.1.1
+Version: 1.2.0
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin_async_sqlalchemy_adapter-1.1.1/README.md` & `casbin_async_sqlalchemy_adapter-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/__init__.py` & `casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/__init__.py`

 * *Files identical despite different names*

### Comparing `casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter/adapter.py` & `casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter/adapter.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import warnings
 from contextlib import asynccontextmanager
+from typing import List
 
 from casbin import persist
-from sqlalchemy import Column, Integer, String
+from sqlalchemy import Column, Integer, String, delete
 from sqlalchemy import or_
 from sqlalchemy.ext.asyncio import create_async_engine, AsyncSession
 from sqlalchemy.future import select
 from sqlalchemy.orm import declarative_base, sessionmaker
 
 Base = declarative_base()
 
@@ -113,42 +114,41 @@
 
     def is_filtered(self):
         return self._filtered
 
     async def load_filtered_policy(self, model, filter) -> None:
         """loads all policy rules from the storage."""
         async with self._session_scope() as session:
-            query = select(self._db_class)
-            filters = self.filter_query(query, filter)
-            filters = await session.execute(filters)
-
-            for line in filters.scalars():
+            stmt = select(self._db_class)
+            stmt = self.filter_query(stmt, filter)
+            result = await session.execute(stmt)
+            for line in result.scalars():
                 persist.load_policy_line(str(line), model)
             self._filtered = True
-
-    def filter_query(self, querydb, filter):
+    
+    def filter_query(self, stmt, filter):
         for attr in ("ptype", "v0", "v1", "v2", "v3", "v4", "v5"):
             if len(getattr(filter, attr)) > 0:
-                querydb = querydb.filter(
+                stmt = stmt.where(
                     getattr(self._db_class, attr).in_(getattr(filter, attr))
                 )
-        return querydb.order_by(self._db_class.id)
+        return stmt.order_by(self._db_class.id)
 
     async def _save_policy_line(self, ptype, rule):
         async with self._session_scope() as session:
             line = self._db_class(ptype=ptype)
             for i, v in enumerate(rule):
                 setattr(line, "v{}".format(i), v)
             session.add(line)
 
     async def save_policy(self, model):
         """saves all policy rules to the storage."""
         async with self._session_scope() as session:
-            query = select(self._db_class)
-            await session.execute(query.delete())
+            stmt = delete(self._db_class)
+            await session.execute(stmt)
             for sec in ["p", "g"]:
                 if sec not in model.model.keys():
                     continue
                 for ptype, ast in model.model[sec].items():
                     for rule in ast.policy:
                         await self._save_policy_line(ptype, rule)
         return True
@@ -161,126 +161,126 @@
         """adds a policy rules to the storage."""
         for rule in rules:
             await self._save_policy_line(ptype, rule)
 
     async def remove_policy(self, sec, ptype, rule):
         """removes a policy rule from the storage."""
         async with self._session_scope() as session:
-            query = session.query(self._db_class)
-            query = query.filter(self._db_class.ptype == ptype)
+            stmt = delete(self._db_class).where(self._db_class.ptype == ptype)
             for i, v in enumerate(rule):
-                query = query.filter(getattr(self._db_class, "v{}".format(i)) == v)
-            r = await query.delete()
+                stmt = stmt.where(getattr(self._db_class, "v{}".format(i)) == v)
+            r = await session.execute(stmt)
 
-        return True if r > 0 else False
+        return True if r.rowcount > 0 else False
 
     async def remove_policies(self, sec, ptype, rules):
         """remove policy rules from the storage."""
         if not rules:
             return
         async with self._session_scope() as session:
-            query = session.query(self._db_class)
-            query = query.filter(self._db_class.ptype == ptype)
+            stmt = delete(self._db_class).where(self._db_class.ptype == ptype)
             rules = zip(*rules)
             for i, rule in enumerate(rules):
-                query = query.filter(
+                stmt = stmt.where(
                     or_(getattr(self._db_class, "v{}".format(i)) == v for v in rule)
                 )
-            await query.delete()
+            await session.execute(stmt)
 
     async def remove_filtered_policy(self, sec, ptype, field_index, *field_values):
         """removes policy rules that match the filter from the storage.
         This is part of the Auto-Save feature.
         """
         async with self._session_scope() as session:
-            query = session.query(self._db_class).filter(self._db_class.ptype == ptype)
+            stmt = delete(self._db_class).where(self._db_class.ptype == ptype)
 
             if not (0 <= field_index <= 5):
                 return False
             if not (1 <= field_index + len(field_values) <= 6):
                 return False
             for i, v in enumerate(field_values):
                 if v != "":
                     v_value = getattr(self._db_class, "v{}".format(field_index + i))
-                    query = query.filter(v_value == v)
-            r = await query.delete()
+                    stmt = stmt.where(v_value == v)
+            r = await session.execute(stmt)
 
-        return True if r > 0 else False
+        return True if r.rowcount > 0 else False
 
-    async def update_policy(self, sec: str, ptype: str, old_rule: [str], new_rule: [str]) -> None:
+    async def update_policy(self, sec: str, ptype: str, old_rule: List[str], new_rule: List[str]) -> None:
         """
         Update the old_rule with the new_rule in the database (storage).
 
         :param sec: section type
         :param ptype: policy type
         :param old_rule: the old rule that needs to be modified
         :param new_rule: the new rule to replace the old rule
 
         :return: None
         """
 
         async with self._session_scope() as session:
-            query = session.query(self._db_class).filter(self._db_class.ptype == ptype)
+            stmt = select(self._db_class).where(self._db_class.ptype == ptype)
 
             # locate the old rule
             for index, value in enumerate(old_rule):
                 v_value = getattr(self._db_class, "v{}".format(index))
-                query = query.filter(v_value == value)
+                stmt = stmt.where(v_value == value)
 
             # need the length of the longest_rule to perform overwrite
             longest_rule = old_rule if len(old_rule) > len(new_rule) else new_rule
-            old_rule_line = await query.one()
+            result = await session.execute(stmt)
+            old_rule_line = result.scalar_one()
 
             # overwrite the old rule with the new rule
             for index in range(len(longest_rule)):
                 if index < len(new_rule):
                     setattr(old_rule_line, "v{}".format(index), new_rule[index])
                 else:
                     setattr(old_rule_line, "v{}".format(index), None)
 
-    async def update_policies(self, sec: str, ptype: str, old_rules: [[str], ], new_rules: [[str], ]) -> None:
+    async def update_policies(self, sec: str, ptype: str, old_rules: List[List[str]], new_rules: List[List[str]]) -> None:
         """
         Update the old_rules with the new_rules in the database (storage).
 
         :param sec: section type
         :param ptype: policy type
         :param old_rules: the old rules that need to be modified
         :param new_rules: the new rules to replace the old rules
 
         :return: None
         """
         for i in range(len(old_rules)):
             await self.update_policy(sec, ptype, old_rules[i], new_rules[i])
 
-    async def update_filtered_policies(self, sec, ptype, new_rules: [[str]], field_index, *field_values) -> [[str]]:
+    async def update_filtered_policies(self, sec, ptype, new_rules: List[List[str]], field_index, *field_values) -> List[List[str]]:
         """update_filtered_policies updates all the policies on the basis of the filter."""
 
         filter = Filter()
         filter.ptype = ptype
 
         # Creating Filter from the field_index & field_values provided
         for i in range(len(field_values)):
             if field_index <= i and i < field_index + len(field_values):
                 setattr(filter, f"v{i}", field_values[i - field_index])
             else:
                 break
 
         return await self._update_filtered_policies(new_rules, filter)
 
-    async def _update_filtered_policies(self, new_rules, filter) -> [[str]]:
+    async def _update_filtered_policies(self, new_rules, filter) -> List[List[str]]:
         """_update_filtered_policies updates all the policies on the basis of the filter."""
 
         async with self._session_scope() as session:
             # Load old policies
 
-            query = session.query(self._db_class).filter(
+            stmt = select(self._db_class).where(
                 self._db_class.ptype == filter.ptype
             )
-            filtered_query = self.filter_query(query, filter)
-            old_rules = await filtered_query.all()
+            filtered_stmt = self.filter_query(stmt, filter)
+            result = await session.execute(filtered_stmt)
+            old_rules = result.scalars().all()
 
             # Delete old policies
 
             await self.remove_policies("p", filter.ptype, old_rules)
 
             # Insert new policies
```

### Comparing `casbin_async_sqlalchemy_adapter-1.1.1/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO` & `casbin_async_sqlalchemy_adapter-1.2.0/casbin_async_sqlalchemy_adapter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: casbin-async-sqlalchemy-adapter
-Version: 1.1.1
+Version: 1.2.0
 Summary: Asynchronous SQLAlchemy Adapter for PyCasbin
 Home-page: https://github.com/pycasbin/async-sqlalchemy-adapter
 Author: wrapping-2000
 Author-email: wenpengchen@njust.edu.cn
 License: Apache 2.0
 Keywords: asynccasbin,SQLAlchemy,casbin-adapter,rbac,access control,abac,acl,permission
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `casbin_async_sqlalchemy_adapter-1.1.1/setup.py` & `casbin_async_sqlalchemy_adapter-1.2.0/setup.py`

 * *Files identical despite different names*

