# Comparing `tmp/talkytimes_package-0.1.3.tar.gz` & `tmp/talkytimes_package-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talkytimes_package-0.1.3.tar", last modified: Sun Jul 16 07:06:37 2023, max compression
+gzip compressed data, was "talkytimes_package-0.1.4.tar", last modified: Sun Jul 16 07:14:41 2023, max compression
```

## Comparing `talkytimes_package-0.1.3.tar` & `talkytimes_package-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 07:06:37.010245 talkytimes_package-0.1.3/
--rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0      265 2023-07-16 07:06:37.011244 talkytimes_package-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.3/README.md
--rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      121 2023-07-16 07:06:37.012244 talkytimes_package-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:06:36.988242 talkytimes_package-0.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-16 07:06:36.996242 talkytimes_package-0.1.3/src/dynamodb/
--rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.3/src/dynamodb/__init__.py
--rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.3/src/dynamodb/base.py
--rw-rw-rw-   0        0        0     1409 2023-07-16 07:03:47.000000 talkytimes_package-0.1.3/src/dynamodb/dynamodb.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:06:36.999244 talkytimes_package-0.1.3/src/talkytimes/
--rw-rw-rw-   0        0        0       49 2023-07-16 07:06:35.000000 talkytimes_package-0.1.3/src/talkytimes/__init__.py
--rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.3/src/talkytimes/base.py
--rw-rw-rw-   0        0        0     3820 2023-07-16 07:05:25.000000 talkytimes_package-0.1.3/src/talkytimes/talkytimes.py
-drwxrwxrwx   0        0        0        0 2023-07-16 07:06:37.010245 talkytimes_package-0.1.3/src/talkytimes_package.egg-info/
--rw-rw-rw-   0        0        0      265 2023-07-16 07:06:36.000000 talkytimes_package-0.1.3/src/talkytimes_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-07-16 07:06:36.000000 talkytimes_package-0.1.3/src/talkytimes_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 07:06:36.000000 talkytimes_package-0.1.3/src/talkytimes_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-16 07:06:36.000000 talkytimes_package-0.1.3/src/talkytimes_package.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-07-16 07:06:36.000000 talkytimes_package-0.1.3/src/talkytimes_package.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.825325 talkytimes_package-0.1.4/
+-rw-rw-rw-   0        0        0     1079 2023-07-16 06:08:25.000000 talkytimes_package-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       85 2023-07-16 06:08:25.000000 talkytimes_package-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      265 2023-07-16 07:14:41.825325 talkytimes_package-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-16 06:14:12.000000 talkytimes_package-0.1.4/README.md
+-rw-rw-rw-   0        0        0       98 2023-07-16 06:08:25.000000 talkytimes_package-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-07-16 07:14:41.827326 talkytimes_package-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-07-16 06:43:16.000000 talkytimes_package-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.801325 talkytimes_package-0.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.810325 talkytimes_package-0.1.4/src/dynamodb/
+-rw-rw-rw-   0        0        0        0 2023-07-16 06:22:05.000000 talkytimes_package-0.1.4/src/dynamodb/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-07-16 06:20:33.000000 talkytimes_package-0.1.4/src/dynamodb/base.py
+-rw-rw-rw-   0        0        0     1407 2023-07-16 07:10:19.000000 talkytimes_package-0.1.4/src/dynamodb/dynamodb.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.813329 talkytimes_package-0.1.4/src/talkytimes/
+-rw-rw-rw-   0        0        0       49 2023-07-16 07:14:39.000000 talkytimes_package-0.1.4/src/talkytimes/__init__.py
+-rw-rw-rw-   0        0        0     1244 2023-07-16 06:26:27.000000 talkytimes_package-0.1.4/src/talkytimes/base.py
+-rw-rw-rw-   0        0        0     4174 2023-07-16 07:14:10.000000 talkytimes_package-0.1.4/src/talkytimes/talkytimes.py
+drwxrwxrwx   0        0        0        0 2023-07-16 07:14:41.824326 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-07-16 07:14:41.000000 talkytimes_package-0.1.4/src/talkytimes_package.egg-info/top_level.txt
```

### Comparing `talkytimes_package-0.1.3/LICENSE` & `talkytimes_package-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.3/src/dynamodb/dynamodb.py` & `talkytimes_package-0.1.4/src/dynamodb/dynamodb.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def get_user(self, *, external_id: str) -> Any:
         data = dict(external_id=external_id)
         return self.get_item(key=data)
 
     def get_users(self) -> dict[str, Any]:
         response = self.table.scan()
         print(response)
-        data = response.get("'Items'")
+        data = response.get("Items")
 
         while 'LastEvaluatedKey' in response:
             response = self.table.scan(ExclusiveStartKey=response['LastEvaluatedKey'])
             data.extend(response['Items'])
         return data
 
     def create_user(self, *, external_id: str, status: str) -> Any:
```

### Comparing `talkytimes_package-0.1.3/src/talkytimes/base.py` & `talkytimes_package-0.1.4/src/talkytimes/base.py`

 * *Files identical despite different names*

### Comparing `talkytimes_package-0.1.3/src/talkytimes/talkytimes.py` & `talkytimes_package-0.1.4/src/talkytimes/talkytimes.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,41 +45,47 @@
                 self.driver.find_element(by=By.XPATH, value=next_button).click()
                 element_button = self.driver.find_element(by=By.CLASS_NAME, value='next')
             except Exception as e:
                 print("Error get users page", page_count, e)
                 break
 
     def save_user_chat(self):
-        button_chat = "/html/body/div[1]/div/div[1]/main/div[2]/div/div[1]/div[2]/div[2]/div[1]/div[3]/div[1]/button"
-        button_chat = self.driver.find_element(by=By.XPATH, value=button_chat)
-        if not button_chat.text == " Change to mail ":
-            button_chat.click()
-            time.sleep(1)
-        user_pop = self.driver.find_element(
-            by=By.CLASS_NAME,
-            value="scroll-button__text"
-        ).text
+        users = self.db.get_users()
+        for user in users:
+            external_id = user.get("external_id")
+            url = f"{self.url}/user/id/{external_id}"
+            self.driver.get(url)
+            time.sleep(2)
+            button_chat = "/html/body/div[1]/div/div[1]/main/div[2]/div/div[1]/div[2]/div[2]/div[1]/div[3]/div[1]/button"
+            button_chat = self.driver.find_element(by=By.XPATH, value=button_chat)
+            if not button_chat.text == " Change to mail ":
+                button_chat.click()
+                time.sleep(1)
+            user_pop = self.driver.find_element(
+                by=By.CLASS_NAME,
+                value="scroll-button__text"
+            ).text
 
-        print(user_pop)
-        user_pop_array = user_pop.split(" ")
-        messages = "0"
-        mails = "0"
-        if not user_pop == "You can’t message inactive users":
-            if (user_pop_array[1] == "message") | (user_pop_array[1] == "messages"):
-                print(f"messages: {user_pop_array[0]}")
-                messages = user_pop_array[0]
-                if user_pop_array[3] == "no":
-                    print(f"mails: 0")
-                    mails = "0"
+            print(user_pop)
+            user_pop_array = user_pop.split(" ")
+            messages = "0"
+            mails = "0"
+            if not user_pop == "You can’t message inactive users":
+                if (user_pop_array[1] == "message") | (user_pop_array[1] == "messages"):
+                    print(f"messages: {user_pop_array[0]}")
+                    messages = user_pop_array[0]
+                    if user_pop_array[3] == "no":
+                        print(f"mails: 0")
+                        mails = "0"
+                    else:
+                        print(f"mails: {user_pop_array[3]}")
+                        mails = user_pop_array[3]
                 else:
-                    print(f"mails: {user_pop_array[3]}")
-                    mails = user_pop_array[3]
-            else:
-                if user_pop_array[3] == "no":
-                    print(f"messages: 0")
-                    messages = "0"
-                else:
-                    print(f"messages: {user_pop_array[3]}")
-                    messages = user_pop_array[3]
-                print(f"mails: {user_pop_array[0]}")
-                mails = user_pop_array[0]
+                    if user_pop_array[3] == "no":
+                        print(f"messages: 0")
+                        messages = "0"
+                    else:
+                        print(f"messages: {user_pop_array[3]}")
+                        messages = user_pop_array[3]
+                    print(f"mails: {user_pop_array[0]}")
+                    mails = user_pop_array[0]
```

