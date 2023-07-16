# Comparing `tmp/talkytimes_package-0.2.3.tar.gz` & `tmp/talkytimes_package-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.2.3.tar", last modified: Sun Jul 16 08:46:28 2023, max compression
+gzip compressed data, was "talkytimes_package-0.2.4.tar", last modified: Sun Jul 16 08:50:36 2023, max compression
```

## Comparing `talkytimes_package-0.2.3.tar` & `talkytimes_package-0.2.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.471886 talkytimes_package-0.2.3/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.3/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 08:46:28.472886 talkytimes_package-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.3/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.3/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 08:46:28.473886 talkytimes_package-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.443880 talkytimes_package-0.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.451882 talkytimes_package-0.2.3/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.3/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.3/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2343 2023-07-16 08:42:54.000000 talkytimes_package-0.2.3/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.453880 talkytimes_package-0.2.3/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 08:46:22.000000 talkytimes_package-0.2.3/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.3/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3956 2023-07-16 08:32:47.000000 talkytimes_package-0.2.3/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:46:28.470881 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 08:46:28.000000 talkytimes_package-0.2.3/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.211445 talkytimes_package-0.2.4/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:50:36.211445 talkytimes_package-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.4/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 08:50:36.212445 talkytimes_package-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.189445 talkytimes_package-0.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.197445 talkytimes_package-0.2.4/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.4/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.4/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2343 2023-07-16 08:42:54.000000 talkytimes_package-0.2.4/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.200446 talkytimes_package-0.2.4/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 08:50:33.000000 talkytimes_package-0.2.4/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.4/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3960 2023-07-16 08:50:22.000000 talkytimes_package-0.2.4/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:50:36.210447 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 08:50:36.000000 talkytimes_package-0.2.4/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.2.3/LICENSE` & `talkytimes_package-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.3/src/dynamodb/dynamodb.py` & `talkytimes_package-0.2.4/src/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.3/src/talkytimes/base.py` & `talkytimes_package-0.2.4/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.3/src/talkytimes/talkytimes.py` & `talkytimes_package-0.2.4/src/talkytimes/talkytimes.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 print("Error get users page", page_count, e)
                 break
 
     def save_user_chat(self):
         users = self.db.get_users()
         for user in users:
             external_id = user.get("external_id")
-            others = json.loads(user.get("value"))
+            others = json.loads(user.get("user_info"))
             status = others.get("status")
             url = f"{self.url}/user/id/{external_id}"
             self.driver.get(url)
             time.sleep(3)
             button_chat = "/html/body/div[1]/div/div[1]/main/div[2]/div/div[1]/div[2]/div[2]/div[1]/div[3]/div[1]/button"
             button_chat = self.driver.find_element(by=By.XPATH, value=button_chat)
             if not button_chat.text == "Change to mail":
```

