# Comparing `tmp/talkytimes_package-0.1.7.tar.gz` & `tmp/talkytimes_package-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.1.7.tar", last modified: Sun Jul 16 07:37:01 2023, max compression
+gzip compressed data, was "talkytimes_package-0.1.8.tar", last modified: Sun Jul 16 07:54:58 2023, max compression
```

## Comparing `talkytimes_package-0.1.7.tar` & `talkytimes_package-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:37:01.030808 talkytimes_package-0.1.7/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.7/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.7/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 07:37:01.030808 talkytimes_package-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.7/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 07:37:01.031805 talkytimes_package-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:37:01.006805 talkytimes_package-0.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 07:37:01.014810 talkytimes_package-0.1.7/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.7/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.7/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     1407 2023-07-16 07:10:19.000000 talkytimes_package-0.1.7/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:37:01.017806 talkytimes_package-0.1.7/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 07:36:59.000000 talkytimes_package-0.1.7/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.7/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     4208 2023-07-16 07:36:47.000000 talkytimes_package-0.1.7/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:37:01.029806 talkytimes_package-0.1.7/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 07:37:00.000000 talkytimes_package-0.1.7/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 07:37:00.000000 talkytimes_package-0.1.7/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:37:00.000000 talkytimes_package-0.1.7/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 07:37:00.000000 talkytimes_package-0.1.7/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 07:37:00.000000 talkytimes_package-0.1.7/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 07:54:58.519725 talkytimes_package-0.1.8/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 07:54:58.520723 talkytimes_package-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.8/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 07:54:58.521724 talkytimes_package-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:54:58.497699 talkytimes_package-0.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 07:54:58.505697 talkytimes_package-0.1.8/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.8/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.8/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2146 2023-07-16 07:53:00.000000 talkytimes_package-0.1.8/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:54:58.507724 talkytimes_package-0.1.8/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 07:53:23.000000 talkytimes_package-0.1.8/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.8/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     4430 2023-07-16 07:54:40.000000 talkytimes_package-0.1.8/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:54:58.519725 talkytimes_package-0.1.8/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 07:54:58.000000 talkytimes_package-0.1.8/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 07:54:58.000000 talkytimes_package-0.1.8/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 07:54:58.000000 talkytimes_package-0.1.8/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 07:54:58.000000 talkytimes_package-0.1.8/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 07:54:58.000000 talkytimes_package-0.1.8/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.1.7/LICENSE` & `talkytimes_package-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.7/src/talkytimes/base.py` & `talkytimes_package-0.1.8/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.7/src/talkytimes/talkytimes.py` & `talkytimes_package-0.1.8/src/talkytimes/talkytimes.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,14 +48,15 @@
                 print("Error get users page", page_count, e)
                 break
 
     def save_user_chat(self):
         users = self.db.get_users()
         for user in users:
             external_id = user.get("external_id")
+            status = user.get("status")
             url = f"{self.url}/user/id/{external_id}"
             self.driver.get(url)
             time.sleep(3)
             button_chat = "/html/body/div[1]/div/div[1]/main/div[2]/div/div[1]/div[2]/div[2]/div[1]/div[3]/div[1]/button"
             button_chat = self.driver.find_element(by=By.XPATH, value=button_chat)
             print(button_chat.text)
             if not button_chat.text == "Change to mail":
@@ -85,8 +86,13 @@
                         print(f"messages: 0")
                         messages = "0"
                     else:
                         print(f"messages: {user_pop_array[3]}")
                         messages = user_pop_array[3]
                     print(f"mails: {user_pop_array[0]}")
                     mails = user_pop_array[0]
-
+            self.db.update_user(
+                external_id=external_id,
+                status=status,
+                messages=messages,
+                emails=mails
+            )
```

