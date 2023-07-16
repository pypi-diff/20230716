# Comparing `tmp/ez0th-0.1.4.tar.gz` & `tmp/ez0th-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez0th-0.1.4.tar", last modified: Fri Jul  7 05:46:59 2023, max compression
+gzip compressed data, was "ez0th-0.1.5.tar", last modified: Sun Jul 16 02:47:17 2023, max compression
```

## Comparing `ez0th-0.1.4.tar` & `ez0th-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-07 05:46:59.029437 ez0th-0.1.4/
--rw-rw-rw-   0        0        0    14297 2023-07-07 05:46:59.029437 ez0th-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0    11755 2023-07-07 05:46:02.000000 ez0th-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-07 05:46:59.016482 ez0th-0.1.4/ez0th/
--rw-rw-rw-   0        0        0    10983 2023-07-07 05:41:40.000000 ez0th-0.1.4/ez0th/__init__.py
--rw-rw-rw-   0        0        0     3484 2023-07-07 05:42:55.000000 ez0th-0.1.4/ez0th/test.py
-drwxrwxrwx   0        0        0        0 2023-07-07 05:46:59.028439 ez0th-0.1.4/ez0th.egg-info/
--rw-rw-rw-   0        0        0    14297 2023-07-07 05:46:58.000000 ez0th-0.1.4/ez0th.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      194 2023-07-07 05:46:58.000000 ez0th-0.1.4/ez0th.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-07 05:46:58.000000 ez0th-0.1.4/ez0th.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-07 05:46:58.000000 ez0th-0.1.4/ez0th.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-07 05:46:58.000000 ez0th-0.1.4/ez0th.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-07 05:46:59.029437 ez0th-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      801 2023-07-07 05:46:55.000000 ez0th-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:47:17.565664 ez0th-0.1.5/
+-rw-rw-rw-   0        0        0    14838 2023-07-16 02:47:17.564651 ez0th-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0    12168 2023-07-16 02:46:44.000000 ez0th-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 02:47:17.548444 ez0th-0.1.5/ez0th/
+-rw-rw-rw-   0        0        0    10983 2023-07-07 05:41:40.000000 ez0th-0.1.5/ez0th/__init__.py
+-rw-rw-rw-   0        0        0     3687 2023-07-16 02:42:45.000000 ez0th-0.1.5/ez0th/test.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:47:17.563686 ez0th-0.1.5/ez0th.egg-info/
+-rw-rw-rw-   0        0        0    14838 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-16 02:47:17.000000 ez0th-0.1.5/ez0th.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 02:47:17.565664 ez0th-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      801 2023-07-16 02:47:13.000000 ez0th-0.1.5/setup.py
```

### Comparing `ez0th-0.1.4/PKG-INFO` & `ez0th-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
         
@@ -75,14 +75,22 @@
             send_func = send_func,  # Mail sending function etc. (argument: sess_token (for creating confirmation URL))
             db = db,    # Database
             timeout = 1 # Timeout period (in hours; infinite if specified as inf)
         )
         # Result confirmation
         print(sent_flag)
         
+        # Account existence verification [ez0th]
+        flag = ez0th.exists(
+            u_id = "WhiteDog",  # Login id (any registered id is acceptable)
+            db = db,    # Database
+        )
+        # Check the result
+        print(flag)
+        
         # Password change [ez0th]
         success_flag = ez0th.change_pw(
             sess_token = sess_token,    # Session token
             password = "abc123456", # New password
             db = db,    # Database
         )
         # Check result
@@ -207,14 +215,22 @@
             send_func = send_func,  # メール送信等の関数 (引数: sess_token (確認URL作成用))
             db = db,    # データベース
             timeout = 1 # タイムアウト時間 (時間単位; inf指定で無限大)
         )
         # 結果確認
         print(sent_flag)
         
+        # アカウント存在確認 [ez0th]
+        flag = ez0th.exists(
+            u_id = "WhiteDog",  # ログインid (登録されたいずれのidも可)
+            db = db,    # データベース
+        )
+        # 結果確認
+        print(flag)
+        
         # パスワード変更 [ez0th]
         success_flag = ez0th.change_pw(
             sess_token = sess_token,    # セッショントークン
             password = "abc123456", # 変更後のパスワード
             db = db,    # データベース
         )
         # 結果確認
```

### Comparing `ez0th-0.1.4/README.md` & `ez0th-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,22 @@
     send_func = send_func,  # Mail sending function etc. (argument: sess_token (for creating confirmation URL))
     db = db,    # Database
     timeout = 1 # Timeout period (in hours; infinite if specified as inf)
 )
 # Result confirmation
 print(sent_flag)
 
+# Account existence verification [ez0th]
+flag = ez0th.exists(
+    u_id = "WhiteDog",  # Login id (any registered id is acceptable)
+    db = db,    # Database
+)
+# Check the result
+print(flag)
+
 # Password change [ez0th]
 success_flag = ez0th.change_pw(
     sess_token = sess_token,    # Session token
     password = "abc123456", # New password
     db = db,    # Database
 )
 # Check result
@@ -199,14 +207,22 @@
     send_func = send_func,  # メール送信等の関数 (引数: sess_token (確認URL作成用))
     db = db,    # データベース
     timeout = 1 # タイムアウト時間 (時間単位; inf指定で無限大)
 )
 # 結果確認
 print(sent_flag)
 
+# アカウント存在確認 [ez0th]
+flag = ez0th.exists(
+    u_id = "WhiteDog",  # ログインid (登録されたいずれのidも可)
+    db = db,    # データベース
+)
+# 結果確認
+print(flag)
+
 # パスワード変更 [ez0th]
 success_flag = ez0th.change_pw(
     sess_token = sess_token,    # セッショントークン
     password = "abc123456", # 変更後のパスワード
     db = db,    # データベース
 )
 # 結果確認
```

### Comparing `ez0th-0.1.4/ez0th/__init__.py` & `ez0th-0.1.5/ez0th/__init__.py`

 * *Files identical despite different names*

### Comparing `ez0th-0.1.4/ez0th/test.py` & `ez0th-0.1.5/ez0th/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,22 @@
 	send_func = send_func,	# メール送信等の関数 (引数: sess_token (確認URL作成用))
 	db = db,	# データベース
 	timeout = 1	# タイムアウト時間 (時間単位; inf指定で無限大)
 )
 # 結果確認
 print(sent_flag)
 
+# アカウント存在確認 [ez0th]
+flag = ez0th.exists(
+	u_id = "WhiteDog",	# ログインid (登録されたいずれのidも可)
+	db = db,	# データベース
+)
+# 結果確認
+print(flag)
+
 # パスワード変更 [ez0th]
 success_flag = ez0th.change_pw(
 	sess_token = sess_token,	# セッショントークン
 	password = "abc123456",	# 変更後のパスワード
 	db = db,	# データベース
 )
 # 結果確認
```

### Comparing `ez0th-0.1.4/ez0th.egg-info/PKG-INFO` & `ez0th-0.1.5/ez0th.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez0th
-Version: 0.1.4
+Version: 0.1.5
 Summary: Python Library for Easy Authentication and Authorization
 Home-page: https://github.co.jp/
 Author: bib_inf
 Author-email: contact.bibinf@gmail.com
 License: CC0 v1.0
 Description: # ez0th - Python Library for Easy Authentication and Authorization
         
@@ -75,14 +75,22 @@
             send_func = send_func,  # Mail sending function etc. (argument: sess_token (for creating confirmation URL))
             db = db,    # Database
             timeout = 1 # Timeout period (in hours; infinite if specified as inf)
         )
         # Result confirmation
         print(sent_flag)
         
+        # Account existence verification [ez0th]
+        flag = ez0th.exists(
+            u_id = "WhiteDog",  # Login id (any registered id is acceptable)
+            db = db,    # Database
+        )
+        # Check the result
+        print(flag)
+        
         # Password change [ez0th]
         success_flag = ez0th.change_pw(
             sess_token = sess_token,    # Session token
             password = "abc123456", # New password
             db = db,    # Database
         )
         # Check result
@@ -207,14 +215,22 @@
             send_func = send_func,  # メール送信等の関数 (引数: sess_token (確認URL作成用))
             db = db,    # データベース
             timeout = 1 # タイムアウト時間 (時間単位; inf指定で無限大)
         )
         # 結果確認
         print(sent_flag)
         
+        # アカウント存在確認 [ez0th]
+        flag = ez0th.exists(
+            u_id = "WhiteDog",  # ログインid (登録されたいずれのidも可)
+            db = db,    # データベース
+        )
+        # 結果確認
+        print(flag)
+        
         # パスワード変更 [ez0th]
         success_flag = ez0th.change_pw(
             sess_token = sess_token,    # セッショントークン
             password = "abc123456", # 変更後のパスワード
             db = db,    # データベース
         )
         # 結果確認
```

### Comparing `ez0th-0.1.4/setup.py` & `ez0th-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 00000080: 205b 657a 7069 705d 0d0a 7769 7468 2065   [ezpip]..with e
 00000090: 7a70 6970 2e70 6163 6b61 6765 7228 6465  zpip.packager(de
 000000a0: 7665 6c6f 705f 6469 7220 3d20 222e 2f5f  velop_dir = "./_
 000000b0: 6465 7665 6c6f 705f 657a 3074 682f 2229  develop_ez0th/")
 000000c0: 2061 7320 703a 0d0a 0973 6574 7570 280d   as p:...setup(.
 000000d0: 0a09 096e 616d 6520 3d20 2265 7a30 7468  ...name = "ez0th
 000000e0: 222c 0d0a 0909 7665 7273 696f 6e20 3d20  ",....version = 
-000000f0: 2230 2e31 2e34 222c 0d0a 0909 6465 7363  "0.1.4",....desc
+000000f0: 2230 2e31 2e35 222c 0d0a 0909 6465 7363  "0.1.5",....desc
 00000100: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
 00000110: 6e20 4c69 6272 6172 7920 666f 7220 4561  n Library for Ea
 00000120: 7379 2041 7574 6865 6e74 6963 6174 696f  sy Authenticatio
 00000130: 6e20 616e 6420 4175 7468 6f72 697a 6174  n and Authorizat
 00000140: 696f 6e22 2c0d 0a09 0961 7574 686f 7220  ion",....author 
 00000150: 3d20 2262 6962 5f69 6e66 222c 0d0a 0909  = "bib_inf",....
 00000160: 6175 7468 6f72 5f65 6d61 696c 203d 2022  author_email = "
```

