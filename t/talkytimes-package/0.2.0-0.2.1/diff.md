# Comparing `tmp/talkytimes_package-0.2.0.tar.gz` & `tmp/talkytimes_package-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.2.0.tar", last modified: Sun Jul 16 08:12:18 2023, max compression
+gzip compressed data, was "talkytimes_package-0.2.1.tar", last modified: Sun Jul 16 08:22:20 2023, max compression
```

## Comparing `talkytimes_package-0.2.0.tar` & `talkytimes_package-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.247465 talkytimes_package-0.2.0/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 08:12:18.247465 talkytimes_package-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.0/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 08:12:18.249469 talkytimes_package-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.224459 talkytimes_package-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.232463 talkytimes_package-0.2.0/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.0/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.0/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2325 2023-07-16 08:04:06.000000 talkytimes_package-0.2.0/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.235460 talkytimes_package-0.2.0/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 08:11:50.000000 talkytimes_package-0.2.0/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.0/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     4405 2023-07-16 08:11:37.000000 talkytimes_package-0.2.0/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.246467 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.613515 talkytimes_package-0.2.1/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:22:20.613515 talkytimes_package-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.1/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 08:22:20.615516 talkytimes_package-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.589415 talkytimes_package-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.596514 talkytimes_package-0.2.1/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.1/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.1/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2325 2023-07-16 08:04:06.000000 talkytimes_package-0.2.1/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.599513 talkytimes_package-0.2.1/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 08:22:18.000000 talkytimes_package-0.2.1/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.1/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     4471 2023-07-16 08:20:56.000000 talkytimes_package-0.2.1/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.612515 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.2.0/LICENSE` & `talkytimes_package-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.0/src/dynamodb/dynamodb.py` & `talkytimes_package-0.2.1/src/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.0/src/talkytimes/base.py` & `talkytimes_package-0.2.1/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.0/src/talkytimes/talkytimes.py` & `talkytimes_package-0.2.1/src/talkytimes/talkytimes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import time
 
 from selenium.webdriver.common.by import By
 
 from talkytimes.base import AbstractAutomation
 
 
@@ -47,15 +48,16 @@
                 print("Error get users page", page_count, e)
                 break
 
     def save_user_chat(self):
         users = self.db.get_users()
         for user in users:
             external_id = user.get("external_id")
-            status = user.get("status")
+            others = json.loads(user.get("others"))
+            status = others.get("status")
             url = f"{self.url}/user/id/{external_id}"
             self.driver.get(url)
             time.sleep(3)
             button_chat = "/html/body/div[1]/div/div[1]/main/div[2]/div/div[1]/div[2]/div[2]/div[1]/div[3]/div[1]/button"
             button_chat = self.driver.find_element(by=By.XPATH, value=button_chat)
             print(button_chat.text)
             if not button_chat.text == "Change to mail":
```

