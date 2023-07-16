# Comparing `tmp/talkytimes_package-0.1.4.tar.gz` & `tmp/talkytimes_package-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.1.4.tar", last modified: Sun Jul 16 07:14:41 2023, max compression
+gzip compressed data, was "talkytimes_package-0.1.5.tar", last modified: Sun Jul 16 07:22:36 2023, max compression
```

## Comparing `talkytimes_package-0.1.4.tar` & `talkytimes_package-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.825325 talkytimes_package-0.1.4/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 07:14:41.825325 talkytimes_package-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.4/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 07:14:41.827326 talkytimes_package-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.801325 talkytimes_package-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.810325 talkytimes_package-0.1.4/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.4/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.4/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     1407 2023-07-16 07:10:19.000000 talkytimes_package-0.1.4/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.813329 talkytimes_package-0.1.4/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 07:14:39.000000 talkytimes_package-0.1.4/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.4/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     4174 2023-07-16 07:14:10.000000 talkytimes_package-0.1.4/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.824326 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 07:22:36.315733 talkytimes_package-0.1.5/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 07:22:36.315733 talkytimes_package-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.5/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 07:22:36.316733 talkytimes_package-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:22:36.289734 talkytimes_package-0.1.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 07:22:36.297736 talkytimes_package-0.1.5/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.5/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.5/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     1407 2023-07-16 07:10:19.000000 talkytimes_package-0.1.5/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:22:36.300737 talkytimes_package-0.1.5/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 07:22:32.000000 talkytimes_package-0.1.5/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.5/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     4174 2023-07-16 07:21:25.000000 talkytimes_package-0.1.5/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:22:36.314736 talkytimes_package-0.1.5/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 07:22:36.000000 talkytimes_package-0.1.5/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 07:22:36.000000 talkytimes_package-0.1.5/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 07:22:36.000000 talkytimes_package-0.1.5/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 07:22:36.000000 talkytimes_package-0.1.5/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 07:22:36.000000 talkytimes_package-0.1.5/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.1.4/LICENSE` & `talkytimes_package-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.4/src/dynamodb/dynamodb.py` & `talkytimes_package-0.1.5/src/dynamodb/dynamodb.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.4/src/talkytimes/base.py` & `talkytimes_package-0.1.5/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.4/src/talkytimes/talkytimes.py` & `talkytimes_package-0.1.5/src/talkytimes/talkytimes.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,20 +50,20 @@
 
     def save_user_chat(self):
         users = self.db.get_users()
         for user in users:
             external_id = user.get("external_id")
             url = f"{self.url}/user/id/{external_id}"
             self.driver.get(url)
-            time.sleep(2)
+            time.sleep(3)
             button_chat = "/html/body/div[1]/div/div[1]/main/div[2]/div/div[1]/div[2]/div[2]/div[1]/div[3]/div[1]/button"
             button_chat = self.driver.find_element(by=By.XPATH, value=button_chat)
             if not button_chat.text == " Change to mail ":
                 button_chat.click()
-                time.sleep(1)
+                time.sleep(3)
             user_pop = self.driver.find_element(
                 by=By.CLASS_NAME,
                 value="scroll-button__text"
             ).text
 
             print(user_pop)
             user_pop_array = user_pop.split(" ")
```

