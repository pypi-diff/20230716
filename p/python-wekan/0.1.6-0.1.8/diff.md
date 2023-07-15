# Comparing `tmp/python-wekan-0.1.6.tar.gz` & `tmp/python-wekan-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-wekan-0.1.6.tar", last modified: Sat Jul 15 20:57:43 2023, max compression
+gzip compressed data, was "python-wekan-0.1.8.tar", last modified: Sat Jul 15 22:08:09 2023, max compression
```

## Comparing `python-wekan-0.1.6.tar` & `python-wekan-0.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:43.397710 python-wekan-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-15 20:57:28.000000 python-wekan-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-15 20:57:43.397710 python-wekan-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-15 20:57:28.000000 python-wekan-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:43.393710 python-wekan-0.1.6/python_wekan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:57:43.397710 python-wekan-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-15 20:57:28.000000 python-wekan-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:43.393710 python-wekan-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:28.000000 python-wekan-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-15 20:57:28.000000 python-wekan-0.1.6/tests/test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:43.397710 python-wekan-0.1.6/wekan/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/board.py
--rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/card_checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/card_checklist_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/card_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/customfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/swimlane.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/wekan_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/wekan_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:08:09.227110 python-wekan-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-15 22:07:57.000000 python-wekan-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-15 22:08:09.227110 python-wekan-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-15 22:07:57.000000 python-wekan-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:08:09.227110 python-wekan-0.1.8/python_wekan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-15 22:08:09.000000 python-wekan-0.1.8/python_wekan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-15 22:08:09.000000 python-wekan-0.1.8/python_wekan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:08:09.000000 python-wekan-0.1.8/python_wekan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 22:08:09.000000 python-wekan-0.1.8/python_wekan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 22:08:09.000000 python-wekan-0.1.8/python_wekan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 22:08:09.227110 python-wekan-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-15 22:07:57.000000 python-wekan-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:08:09.227110 python-wekan-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 22:07:57.000000 python-wekan-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-15 22:07:57.000000 python-wekan-0.1.8/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:08:09.227110 python-wekan-0.1.8/wekan/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15921 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/card_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/card_checklist_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/card_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/customfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/swimlane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/wekan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-15 22:07:57.000000 python-wekan-0.1.8/wekan/wekan_list.py
```

### Comparing `python-wekan-0.1.6/LICENSE` & `python-wekan-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/PKG-INFO` & `python-wekan-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-wekan
-Version: 0.1.6
+Version: 0.1.8
 Summary: This is a python client for interacting with the WeKan® REST-API
 Home-page: https://github.com/bastianwenske/python-wekan
 Download-URL: https://github.com/bastianwenske/python-wekan
 Author: Bastian Wenske
 Author-email: 
 License: BSD 3-Clause License
 Keywords: python
```

### Comparing `python-wekan-0.1.6/README.md` & `python-wekan-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/python_wekan.egg-info/PKG-INFO` & `python-wekan-0.1.8/python_wekan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-wekan
-Version: 0.1.6
+Version: 0.1.8
 Summary: This is a python client for interacting with the WeKan® REST-API
 Home-page: https://github.com/bastianwenske/python-wekan
 Download-URL: https://github.com/bastianwenske/python-wekan
 Author: Bastian Wenske
 Author-email: 
 License: BSD 3-Clause License
 Keywords: python
```

### Comparing `python-wekan-0.1.6/setup.py` & `python-wekan-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='python-wekan',
-    version='0.1.6',
+    version='0.1.8',
     packages=['tests', 'wekan'],
     url='https://github.com/bastianwenske/python-wekan',
     download_url='https://github.com/bastianwenske/python-wekan',
     license='BSD 3-Clause License',
     author='Bastian Wenske',
     author_email='',
     description='This is a python client for interacting with the WeKan® REST-API',
```

### Comparing `python-wekan-0.1.6/tests/test_cases.py` & `python-wekan-0.1.8/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/board.py` & `python-wekan-0.1.8/wekan/board.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.allows_show_lists = self.__raw_data.get('allowsShowLists', None)
         self.allows_assigned_by = self.__raw_data['allowsAssignedBy']
         self.allows_received_date = self.__raw_data['allowsReceivedDate']
         self.allows_start_date = self.__raw_data['allowsStartDate']
         self.allows_end_date = self.__raw_data['allowsEndDate']
         self.allows_due_date = self.__raw_data['allowsDueDate']
         self.present_parent_task = self.__raw_data.get('presentParentTask', None)
-        self.is_overtime = self.__raw_data['isOvertime']
+        self.is_overtime = self.__raw_data.get('isOvertime', None)
         self.type = self.__raw_data['type']
         self.sort = self.__raw_data['sort']
 
 
     def __repr__(self) -> str:
         return f"<Board (id: {self.id}, title: {self.title})>"
```

### Comparing `python-wekan-0.1.6/wekan/card.py` & `python-wekan-0.1.8/wekan/card.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/card_checklist.py` & `python-wekan-0.1.8/wekan/card_checklist.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/card_checklist_item.py` & `python-wekan-0.1.8/wekan/card_checklist_item.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/card_comment.py` & `python-wekan-0.1.8/wekan/card_comment.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/customfield.py` & `python-wekan-0.1.8/wekan/customfield.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/integration.py` & `python-wekan-0.1.8/wekan/integration.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/label.py` & `python-wekan-0.1.8/wekan/label.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/swimlane.py` & `python-wekan-0.1.8/wekan/swimlane.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/user.py` & `python-wekan-0.1.8/wekan/user.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/wekan_client.py` & `python-wekan-0.1.8/wekan/wekan_client.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.6/wekan/wekan_list.py` & `python-wekan-0.1.8/wekan/wekan_list.py`

 * *Files identical despite different names*

