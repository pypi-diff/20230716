# Comparing `tmp/talkytimes_package-0.1.9.tar.gz` & `tmp/talkytimes_package-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.1.9.tar", last modified: Sun Jul 16 08:05:14 2023, max compression
+gzip compressed data, was "talkytimes_package-0.2.0.tar", last modified: Sun Jul 16 08:12:18 2023, max compression
```

## Comparing `talkytimes_package-0.1.9.tar` & `talkytimes_package-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:05:14.430913 talkytimes_package-0.1.9/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.9/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 08:05:14.430913 talkytimes_package-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.9/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 08:05:14.431913 talkytimes_package-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:05:14.405911 talkytimes_package-0.1.9/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 08:05:14.413916 talkytimes_package-0.1.9/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.9/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.9/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2325 2023-07-16 08:04:06.000000 talkytimes_package-0.1.9/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:05:14.415915 talkytimes_package-0.1.9/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 08:05:07.000000 talkytimes_package-0.1.9/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.9/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     4430 2023-07-16 07:54:40.000000 talkytimes_package-0.1.9/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:05:14.429915 talkytimes_package-0.1.9/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 08:05:14.000000 talkytimes_package-0.1.9/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 08:05:14.000000 talkytimes_package-0.1.9/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:05:14.000000 talkytimes_package-0.1.9/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 08:05:14.000000 talkytimes_package-0.1.9/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 08:05:14.000000 talkytimes_package-0.1.9/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.247465 talkytimes_package-0.2.0/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:12:18.247465 talkytimes_package-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.0/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 08:12:18.249469 talkytimes_package-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.224459 talkytimes_package-0.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.232463 talkytimes_package-0.2.0/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.0/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.0/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2325 2023-07-16 08:04:06.000000 talkytimes_package-0.2.0/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.235460 talkytimes_package-0.2.0/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 08:11:50.000000 talkytimes_package-0.2.0/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.0/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     4405 2023-07-16 08:11:37.000000 talkytimes_package-0.2.0/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:12:18.246467 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 08:12:18.000000 talkytimes_package-0.2.0/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.1.9/LICENSE` & `talkytimes_package-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.9/src/dynamodb/dynamodb.py` & `talkytimes_package-0.2.0/src/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.9/src/talkytimes/base.py` & `talkytimes_package-0.2.0/src/talkytimes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 from selenium import webdriver
 from selenium.webdriver.chrome.service import Service
 
 from dynamodb.dynamodb import DynamoDB
 
 
 class AbstractAutomation(abc.ABC):
-    table: str
 
-    def __init__(self, url: str):
+    def __init__(self, url: str, table: str):
         self.url = url
         self.driver = self.__get_driver()
-        self.db = DynamoDB(table=self.table)
+        self.db = DynamoDB(table=table)
 
     def __get_driver(self) -> webdriver.Chrome:
         options = webdriver.ChromeOptions()
         service = Service(executable_path='/opt/chromedriver')
         options.binary_location = '/opt/chrome/chrome'
         options.add_argument('--headless')
         options.add_argument('--no-sandbox')
```

### Comparing `talkytimes_package-0.1.9/src/talkytimes/talkytimes.py` & `talkytimes_package-0.2.0/src/talkytimes/talkytimes.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from selenium.webdriver.common.by import By
 
 from talkytimes.base import AbstractAutomation
 
 
 class TalkyTimesAutomation(AbstractAutomation):
-    table = "users_info"
 
     def login_task(self, *, user: str, pw: str) -> None:
         user_input = "/html/body/div[1]/div/div[1]/main/div/div/div/div/div[1]/div/div[1]/form/div/div[1]/div/input"
         pw_input = "/html/body/div[1]/div/div[1]/main/div/div/div/div/div[1]/div/div[1]/form/div/div[2]/div/input"
         login_button = "/html/body/div[1]/div/div[1]/main/div/div/div/div/div[1]/div/div[2]/button"
         self.driver.get(f"{self.url}/auth/login")
         time.sleep(2)
```

