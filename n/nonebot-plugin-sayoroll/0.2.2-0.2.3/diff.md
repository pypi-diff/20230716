# Comparing `tmp/nonebot-plugin-sayoroll-0.2.2.tar.gz` & `tmp/nonebot-plugin-sayoroll-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sayoroll-0.2.2.tar", last modified: Sun Jul 16 12:19:12 2023, max compression
+gzip compressed data, was "nonebot-plugin-sayoroll-0.2.3.tar", last modified: Sun Jul 16 12:29:01 2023, max compression
```

## Comparing `nonebot-plugin-sayoroll-0.2.2.tar` & `nonebot-plugin-sayoroll-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 12:19:12.280673 nonebot-plugin-sayoroll-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-16 12:19:04.000000 nonebot-plugin-sayoroll-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-16 12:19:12.280673 nonebot-plugin-sayoroll-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-16 12:19:04.000000 nonebot-plugin-sayoroll-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 12:19:12.280673 nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll/
--rw-r--r--   0 runner    (1001) docker     (122)     2549 2023-07-16 12:19:04.000000 nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 12:19:12.280673 nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-16 12:19:12.000000 nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-16 12:19:12.000000 nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-16 12:19:12.000000 nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-16 12:19:12.000000 nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-16 12:19:12.000000 nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-16 12:19:12.280673 nonebot-plugin-sayoroll-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-16 12:19:04.000000 nonebot-plugin-sayoroll-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 12:29:01.353905 nonebot-plugin-sayoroll-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (122)    34523 2023-07-16 12:28:51.000000 nonebot-plugin-sayoroll-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-16 12:29:01.353905 nonebot-plugin-sayoroll-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3101 2023-07-16 12:28:51.000000 nonebot-plugin-sayoroll-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 12:29:01.349904 nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll/
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-07-16 12:28:51.000000 nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-16 12:29:01.353905 nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3573 2023-07-16 12:29:01.000000 nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      296 2023-07-16 12:29:01.000000 nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-16 12:29:01.000000 nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-07-16 12:29:01.000000 nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-07-16 12:29:01.000000 nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-16 12:29:01.353905 nonebot-plugin-sayoroll-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-07-16 12:28:51.000000 nonebot-plugin-sayoroll-0.2.3/setup.py
```

### Comparing `nonebot-plugin-sayoroll-0.2.2/LICENSE` & `nonebot-plugin-sayoroll-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-0.2.2/PKG-INFO` & `nonebot-plugin-sayoroll-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 0.2.2
+Version: 0.2.3
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.2.3 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                              [NoneBotPluginLogo]
```

### Comparing `nonebot-plugin-sayoroll-0.2.2/README.md` & `nonebot-plugin-sayoroll-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll/__init__.py` & `nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,23 +43,23 @@
     elif len(args.split(' ')) > 1 and not re.search('([\u4E00-\u9FA5]+)还是([\u4E00-\u9FA5]+)', args):
         options = args.split(' ')
         msg = '我觉得{}会比较好'.format(random.choice(options))
         await roll.finish(
             message=MessageSegment.reply(event.message_id) + msg
         )
 
-    elif re.search('([\u4E00-\u9FA5])([\u4E00-\u9FA5])\\1(.*?)', args):
+    elif re.search('([\u4E00-\u9FA5])([\u4E00-\u9FA5])\\1(.*?)', args) and not re.search('^([\u4E00-\u9FA5]+)还是([\u4E00-\u9FA5]+)$', args):
         result = re.search('([\u4E00-\u9FA5])([\u4E00-\u9FA5])\\1(.*?)', args)
         options = [result.group()[:1], result.group()[1:]]
         msg = '我觉得' + args[:result.span()[0]].replace('我', '你').replace('你', '我') + random.choice(options) + args[result.span()[1]:]
         await roll.finish(
             message=MessageSegment.reply(event.message_id) + msg
         )
-    elif re.search('([\u4E00-\u9FA5]+)还是([\u4E00-\u9FA5]+)', args):
-        result = re.search('([\u4E00-\u9FA5]+)还是([\u4E00-\u9FA5]+)', args)
+    elif re.search('^([\u4E00-\u9FA5]+)还是([\u4E00-\u9FA5]+)$', args):
+        result = re.search('^([\u4E00-\u9FA5]+)还是([\u4E00-\u9FA5]+)$', args)
         options = [args[:result.span()[0]] + result.group(1) + args[result.span()[1]:], args[:result.span()[0]] + result.group(2) + args[result.span()[1]:]]
         msg = '我觉得' + args[:result.span()[0]].replace('我', '你').replace('你', '我') + random.choice(options) + '会比较好'
         await roll.finish(
             message=MessageSegment.reply(event.message_id) + msg
         )
     else:
         await roll.finish(
```

### Comparing `nonebot-plugin-sayoroll-0.2.2/nonebot_plugin_sayoroll.egg-info/PKG-INFO` & `nonebot-plugin-sayoroll-0.2.3/nonebot_plugin_sayoroll.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sayoroll
-Version: 0.2.2
+Version: 0.2.3
 Summary: 基于NoneBot的高仿以前小夜bot的roll功能
 Home-page: https://github.com/mas-alone/nonebot-plugin-sayoroll
 Author: A M D
 Author-email: mas_alone@qq.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.2.2 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-sayoroll Version: 0.2.3 Summary:
 åºäºNoneBotçé«ä»¿ä»¥åå°å¤botçrollåè½ Home-page: https://
 github.com/mas-alone/nonebot-plugin-sayoroll Author: A M D Author-email:
 mas_alone@qq.com Classifier: Programming Language :: Python :: 3.8 Classifier:
 License :: OSI Approved :: GNU Affero General Public License v3 Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE
                              [NoneBotPluginLogo]
```

### Comparing `nonebot-plugin-sayoroll-0.2.2/setup.py` & `nonebot-plugin-sayoroll-0.2.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="nonebot-plugin-sayoroll",  # 项目名称，保证它的唯一性，不要跟已存在的包名冲突即可
-    version="0.2.2",  # 程序版本
+    version="0.2.3",  # 程序版本
     author="A M D",  # 项目作者
     author_email="mas_alone@qq.com",  # 作者邮件
     description="基于NoneBot的高仿以前小夜bot的roll功能",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述？
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://github.com/mas-alone/nonebot-plugin-sayoroll",  # 项目地址
     packages=setuptools.find_packages(),  # 无需修改
```

