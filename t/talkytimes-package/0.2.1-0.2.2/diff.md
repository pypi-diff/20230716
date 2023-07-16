# Comparing `tmp/talkytimes_package-0.2.1.tar.gz` & `tmp/talkytimes_package-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.2.1.tar", last modified: Sun Jul 16 08:22:20 2023, max compression
+gzip compressed data, was "talkytimes_package-0.2.2.tar", last modified: Sun Jul 16 08:33:41 2023, max compression
```

## Comparing `talkytimes_package-0.2.1.tar` & `talkytimes_package-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.613515 talkytimes_package-0.2.1/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 08:22:20.613515 talkytimes_package-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.1/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 08:22:20.615516 talkytimes_package-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.589415 talkytimes_package-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.596514 talkytimes_package-0.2.1/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.1/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.1/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     2325 2023-07-16 08:04:06.000000 talkytimes_package-0.2.1/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.599513 talkytimes_package-0.2.1/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 08:22:18.000000 talkytimes_package-0.2.1/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.1/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     4471 2023-07-16 08:20:56.000000 talkytimes_package-0.2.1/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 08:22:20.612515 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 08:22:20.000000 talkytimes_package-0.2.1/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:33:41.002037 talkytimes_package-0.2.2/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:33:41.002037 talkytimes_package-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.2.2/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 08:33:41.003041 talkytimes_package-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:33:40.980038 talkytimes_package-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 08:33:40.988040 talkytimes_package-0.2.2/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.2.2/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.2.2/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     2321 2023-07-16 08:28:00.000000 talkytimes_package-0.2.2/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:33:40.990038 talkytimes_package-0.2.2/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 08:33:08.000000 talkytimes_package-0.2.2/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1236 2023-07-16 08:11:24.000000 talkytimes_package-0.2.2/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     3956 2023-07-16 08:32:47.000000 talkytimes_package-0.2.2/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:33:41.001037 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 08:33:40.000000 talkytimes_package-0.2.2/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.2.1/LICENSE` & `talkytimes_package-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.1/src/dynamodb/dynamodb.py` & `talkytimes_package-0.2.2/src/dynamodb/dynamodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         external_id: str,
         status: str,
         messages: Optional[str] = "0",
         emails: Optional[str] = "0"
     ) -> Any:
         data = dict(
             external_id=external_id,
-            others=json.dumps(
+            value=json.dumps(
                 dict(
                     status=status,
                     messages=messages,
                     emails=emails
                 )
             )
         )
@@ -52,17 +52,17 @@
                 status=status,
                 messages=messages,
                 emails=emails
             )
         )
         self.table.update_item(
             Key=dict(external_id=external_id),
-            UpdateExpression="set others=:others",
+            UpdateExpression="set value=:value",
             ExpressionAttributeValues={
-                ':others': others,
+                ':value': others,
             },
             ReturnValues="UPDATED_NEW"
         )
 
     def create_or_update(
         self,
         *,
```

### Comparing `talkytimes_package-0.2.1/src/talkytimes/base.py` & `talkytimes_package-0.2.2/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.2.1/src/talkytimes/talkytimes.py` & `talkytimes_package-0.2.2/src/talkytimes/talkytimes.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,52 +48,40 @@
                 print("Error get users page", page_count, e)
                 break
 
     def save_user_chat(self):
         users = self.db.get_users()
         for user in users:
             external_id = user.get("external_id")
-            others = json.loads(user.get("others"))
+            others = json.loads(user.get("value"))
             status = others.get("status")
             url = f"{self.url}/user/id/{external_id}"
             self.driver.get(url)
             time.sleep(3)
             button_chat = "/html/body/div[1]/div/div[1]/main/div[2]/div/div[1]/div[2]/div[2]/div[1]/div[3]/div[1]/button"
             button_chat = self.driver.find_element(by=By.XPATH, value=button_chat)
-            print(button_chat.text)
             if not button_chat.text == "Change to mail":
                 button_chat.click()
                 time.sleep(3)
             user_pop = self.driver.find_element(
                 by=By.CLASS_NAME,
                 value="scroll-button__text"
             ).text
 
-            print(user_pop)
             user_pop_array = user_pop.split(" ")
             messages = "0"
             mails = "0"
             if not user_pop == "You can’t message inactive users":
                 if (user_pop_array[1] == "message") | (user_pop_array[1] == "messages"):
-                    print(f"messages: {user_pop_array[0]}")
                     messages = user_pop_array[0]
-                    if user_pop_array[3] == "no":
-                        print(f"mails: 0")
-                        mails = "0"
-                    else:
-                        print(f"mails: {user_pop_array[3]}")
+                    if not user_pop_array[3] == "no":
                         mails = user_pop_array[3]
                 else:
-                    if user_pop_array[3] == "no":
-                        print(f"messages: 0")
-                        messages = "0"
-                    else:
-                        print(f"messages: {user_pop_array[3]}")
+                    if not user_pop_array[3] == "no":
                         messages = user_pop_array[3]
-                    print(f"mails: {user_pop_array[0]}")
                     mails = user_pop_array[0]
             self.db.update_user(
                 external_id=external_id,
                 status=status,
                 messages=messages,
                 emails=mails
             )
```

