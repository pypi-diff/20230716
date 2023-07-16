# Comparing `tmp/nonebot_plugin_cp_broadcast-1.1.0.tar.gz` & `tmp/nonebot_plugin_cp_broadcast-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_cp_broadcast-1.1.0.tar", max compression
+gzip compressed data, was "nonebot_plugin_cp_broadcast-1.1.1.tar", max compression
```

## Comparing `nonebot_plugin_cp_broadcast-1.1.0.tar` & `nonebot_plugin_cp_broadcast-1.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-07-15 16:52:19.077491 nonebot_plugin_cp_broadcast-1.1.0/LICENSE
--rw-r--r--   0        0        0     5432 2023-07-15 16:52:19.077491 nonebot_plugin_cp_broadcast-1.1.0/README.md
--rw-r--r--   0        0        0     8511 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/__init__.py
--rw-r--r--   0        0        0     2699 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/atcoder.py
--rw-r--r--   0        0        0     3665 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/codeforces.py
--rw-r--r--   0        0        0      589 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/config.py
--rw-r--r--   0        0        0     2416 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/nowcoder.py
--rw-r--r--   0        0        0     7803 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/sqlite3.py
--rw-r--r--   0        0        0      732 2023-07-15 16:52:19.085492 nonebot_plugin_cp_broadcast-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6389 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-16 02:14:37.191455 nonebot_plugin_cp_broadcast-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5432 2023-07-16 02:14:37.191455 nonebot_plugin_cp_broadcast-1.1.1/README.md
+-rw-r--r--   0        0        0     8511 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/__init__.py
+-rw-r--r--   0        0        0     2699 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/atcoder.py
+-rw-r--r--   0        0        0     3665 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/codeforces.py
+-rw-r--r--   0        0        0      589 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/config.py
+-rw-r--r--   0        0        0     2416 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/nowcoder.py
+-rw-r--r--   0        0        0     7803 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/sqlite3.py
+-rw-r--r--   0        0        0      732 2023-07-16 02:14:37.203454 nonebot_plugin_cp_broadcast-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     6389 1970-01-01 00:00:00.000000 nonebot_plugin_cp_broadcast-1.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/LICENSE` & `nonebot_plugin_cp_broadcast-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/README.md` & `nonebot_plugin_cp_broadcast-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/__init__.py` & `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/atcoder.py` & `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/atcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/codeforces.py` & `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/codeforces.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/config.py` & `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/nowcoder.py` & `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/nowcoder.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/nonebot_plugin_cp_broadcast/sqlite3.py` & `nonebot_plugin_cp_broadcast-1.1.1/nonebot_plugin_cp_broadcast/sqlite3.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     outputlist = []
     Users = await updateUser()
 
     global cursor, conn
     for user in Users:
         output=f"当前时间：{time.strftime('%Y-%m-%d %H:%M:%S', time.localtime())}\n"
         cursor.execute('SELECT now_rating,last_rating,QQ FROM CF_User WHERE id = ?', (user.id,))
-        row = cursor.fetchall()
+        row = cursor.fetchone()
         now_rating, last_rating, QQ = row
         if last_rating != now_rating:
             change = now_rating - last_rating
             output += f"cf用户 {user.id} 分数发生变化，从 {last_rating} → {now_rating}，变动了{change}分！\n"
             outputlist.append({'QQ':QQ,'output':output})
 
     return outputlist
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/pyproject.toml` & `nonebot_plugin_cp_broadcast-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-cp-broadcast"
-version = "1.1.0"
+version = "1.1.1"
 description = "Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备"
 authors = ["HuParry <huparry@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nonebot_plugin_cp_broadcast"}]
 homepage = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
 repository = "https://github.com/HuParry/nonebot-plugin-cp-broadcast"
```

### Comparing `nonebot_plugin_cp_broadcast-1.1.0/PKG-INFO` & `nonebot_plugin_cp_broadcast-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-cp-broadcast
-Version: 1.1.0
+Version: 1.1.1
 Summary: Codeforces、牛客、AtCoder平台比赛查询，ACMer 必备
 Home-page: https://github.com/HuParry/nonebot-plugin-cp-broadcast
 License: MIT
 Author: HuParry
 Author-email: huparry@outlook.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 1.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-cp-broadcast Version: 1.1.1 Summary:
 Codeforcesãçå®¢ãAtCoderå¹³å°æ¯èµæ¥è¯¢ï¼ACMer å¿å¤ Home-page:
 https://github.com/HuParry/nonebot-plugin-cp-broadcast License: MIT Author:
 HuParry Author-email: huparry@outlook.com Requires-Python: >=3.8 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
```

