# Comparing `tmp/AshCrypt-1.3.6.tar.gz` & `tmp/AshCrypt-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AshCrypt-1.3.6.tar", last modified: Wed Jul 12 12:31:29 2023, max compression
+gzip compressed data, was "AshCrypt-2.0.0.tar", last modified: Sun Jul 16 14:43:51 2023, max compression
```

## Comparing `AshCrypt-1.3.6.tar` & `AshCrypt-2.0.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.913721 AshCrypt-1.3.6/
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.858448 AshCrypt-1.3.6/AshCrypt/
--rw-rw-rw-   0        0        0     5207 2023-07-11 22:44:20.000000 AshCrypt-1.3.6/AshCrypt/Ash.py
--rw-rw-rw-   0        0        0    39423 2023-07-11 23:08:17.000000 AshCrypt-1.3.6/AshCrypt/AshCryptGUI.py
--rw-rw-rw-   0        0        0     6789 2023-07-12 12:30:45.000000 AshCrypt-1.3.6/AshCrypt/CliCrypt.py
--rw-rw-rw-   0        0        0     8993 2023-07-09 22:27:03.000000 AshCrypt-1.3.6/AshCrypt/Database.py
--rw-rw-rw-   0        0        0     4017 2023-07-11 22:47:20.000000 AshCrypt-1.3.6/AshCrypt/FileCrypt.py
--rw-rw-rw-   0        0        0      288 2023-07-11 22:11:01.000000 AshCrypt-1.3.6/AshCrypt/README.md
--rw-rw-rw-   0        0        0     1799 2023-07-11 22:47:20.000000 AshCrypt-1.3.6/AshCrypt/TextCrypt.py
--rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-1.3.6/AshCrypt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.895726 AshCrypt-1.3.6/AshCrypt/__pycache__/
--rw-rw-rw-   0        0        0     6384 2023-07-11 22:44:21.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/Ash.cpython-39.pyc
--rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
--rw-rw-rw-   0        0        0     7369 2023-07-10 11:21:27.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/Database.cpython-39.pyc
--rw-rw-rw-   0        0        0     3292 2023-07-11 22:47:20.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0     2430 2023-07-11 22:47:20.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
--rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0      738 2023-07-10 11:21:27.000000 AshCrypt-1.3.6/AshCrypt/__pycache__/qr.cpython-39.pyc
--rw-rw-rw-   0        0        0      536 2023-07-09 22:29:03.000000 AshCrypt-1.3.6/AshCrypt/qr.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.901722 AshCrypt-1.3.6/AshCrypt/unittests/
--rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-1.3.6/AshCrypt/unittests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.907719 AshCrypt-1.3.6/AshCrypt/unittests/__pycache__/
--rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-1.3.6/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5719 2023-07-11 22:42:13.000000 AshCrypt-1.3.6/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
--rw-rw-rw-   0        0        0     3348 2023-07-11 22:42:13.000000 AshCrypt-1.3.6/AshCrypt/unittests/unittestAsh.py
-drwxrwxrwx   0        0        0        0 2023-07-12 12:31:29.872127 AshCrypt-1.3.6/AshCrypt.egg-info/
--rw-rw-rw-   0        0        0     1315 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      853 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-12 12:31:29.000000 AshCrypt-1.3.6/AshCrypt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-1.3.6/LICENSE
--rw-rw-rw-   0        0        0     1315 2023-07-12 12:31:29.911726 AshCrypt-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0    21689 2023-07-11 22:57:53.000000 AshCrypt-1.3.6/README.md
--rw-rw-rw-   0        0        0       42 2023-07-12 12:31:29.913721 AshCrypt-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1660 2023-07-12 12:30:49.000000 AshCrypt-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:43:51.415449 AshCrypt-2.0.0/
+drwxrwxrwx   0        0        0        0 2023-07-16 14:43:51.374526 AshCrypt-2.0.0/AshCrypt/
+-rw-rw-rw-   0        0        0     5215 2023-07-16 14:41:51.000000 AshCrypt-2.0.0/AshCrypt/Ash.py
+-rw-rw-rw-   0        0        0    39324 2023-07-16 14:38:46.000000 AshCrypt-2.0.0/AshCrypt/AshCryptGUI.py
+-rw-rw-rw-   0        0        0     6791 2023-07-16 13:27:43.000000 AshCrypt-2.0.0/AshCrypt/CliCrypt.py
+-rw-rw-rw-   0        0        0     8954 2023-07-16 13:14:33.000000 AshCrypt-2.0.0/AshCrypt/Database.py
+-rw-rw-rw-   0        0        0     3977 2023-07-16 12:56:57.000000 AshCrypt-2.0.0/AshCrypt/FileCrypt.py
+-rw-rw-rw-   0        0        0      288 2023-07-11 22:11:01.000000 AshCrypt-2.0.0/AshCrypt/README.md
+-rw-rw-rw-   0        0        0     1797 2023-07-16 13:00:11.000000 AshCrypt-2.0.0/AshCrypt/TextCrypt.py
+-rw-rw-rw-   0        0        0       88 2023-07-03 12:24:38.000000 AshCrypt-2.0.0/AshCrypt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:43:51.404584 AshCrypt-2.0.0/AshCrypt/__pycache__/
+-rw-rw-rw-   0        0        0     6394 2023-07-16 13:27:44.000000 AshCrypt-2.0.0/AshCrypt/__pycache__/Ash.cpython-39.pyc
+-rw-rw-rw-   0        0        0    19834 2023-07-03 21:09:38.000000 AshCrypt-2.0.0/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7371 2023-07-16 13:43:19.000000 AshCrypt-2.0.0/AshCrypt/__pycache__/Database.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3285 2023-07-16 13:27:44.000000 AshCrypt-2.0.0/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2444 2023-07-16 13:27:44.000000 AshCrypt-2.0.0/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc
+-rw-rw-rw-   0        0        0      218 2023-07-03 12:24:42.000000 AshCrypt-2.0.0/AshCrypt/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0      709 2023-07-16 13:43:20.000000 AshCrypt-2.0.0/AshCrypt/__pycache__/qr.cpython-39.pyc
+-rw-rw-rw-   0        0        0      499 2023-07-16 13:09:19.000000 AshCrypt-2.0.0/AshCrypt/qr.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:43:51.407605 AshCrypt-2.0.0/AshCrypt/unittests/
+-rw-rw-rw-   0        0        0       25 2023-06-30 15:01:03.000000 AshCrypt-2.0.0/AshCrypt/unittests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:43:51.412589 AshCrypt-2.0.0/AshCrypt/unittests/__pycache__/
+-rw-rw-rw-   0        0        0      173 2023-07-02 16:55:47.000000 AshCrypt-2.0.0/AshCrypt/unittests/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5719 2023-07-11 22:42:13.000000 AshCrypt-2.0.0/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3348 2023-07-11 22:42:13.000000 AshCrypt-2.0.0/AshCrypt/unittests/unittestAsh.py
+drwxrwxrwx   0        0        0        0 2023-07-16 14:43:51.384521 AshCrypt-2.0.0/AshCrypt.egg-info/
+-rw-rw-rw-   0        0        0     1315 2023-07-16 14:43:50.000000 AshCrypt-2.0.0/AshCrypt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-07-16 14:43:51.000000 AshCrypt-2.0.0/AshCrypt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 14:43:51.000000 AshCrypt-2.0.0/AshCrypt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-07-16 14:43:51.000000 AshCrypt-2.0.0/AshCrypt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 14:43:51.000000 AshCrypt-2.0.0/AshCrypt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1091 2023-06-30 15:01:03.000000 AshCrypt-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0     1315 2023-07-16 14:43:51.414597 AshCrypt-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    21678 2023-07-16 12:52:32.000000 AshCrypt-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-16 14:43:51.415449 AshCrypt-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1660 2023-07-16 14:43:27.000000 AshCrypt-2.0.0/setup.py
```

### Comparing `AshCrypt-1.3.6/AshCrypt/Ash.py` & `AshCrypt-2.0.0/AshCrypt/Ash.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return bcrypt.kdf(
             password=mainkey.encode('UTF-8'),
             salt=salt_pepper,
             desired_key_bytes=32,
             rounds=iterations)
 
     @staticmethod
-    def genMainkey() -> str:
+    def genkey() -> str:
         return os.urandom(32).hex()
 
     def mode(self):
         return modes.CBC(self.iv)
 
     def cipher(self):
         return Cipher(
@@ -68,24 +68,24 @@
 
     def HMAC(self) -> bytes:
         h = self.hmac_key
         h = hmac.HMAC(h, hashes.SHA512())
         h.update(self.ciphertext())
         return h.finalize()
 
-    def setupIterations(self) -> bytes:
+    def setup_iterations(self) -> bytes:
         iters_bytes = struct.pack('!I', self.iterations)
         return iters_bytes
 
-    def encToBytes(self) -> bytes:
+    def enc_to_bytes(self) -> bytes:
         return self.HMAC() + self.iv + self.salt + self.pepper + \
-            self.setupIterations() + self.ciphertext()
+            self.setup_iterations() + self.ciphertext()
 
-    def encToStr(self) -> str:
-        return base64.urlsafe_b64encode(self.encToBytes()).decode('UTF-8')
+    def enc_to_str(self) -> str:
+        return base64.urlsafe_b64encode(self.enc_to_bytes()).decode('UTF-8')
 
 
 class MessageTamperingError(Exception):
     def __init__(self) -> None:
         self.display = 'HMAC mismatch ! Message has been TAMPERED with ,\n or Possible key difference'
         super().__init__(self.display)
 
@@ -140,12 +140,12 @@
         return self.cipher_decryptor().update(self.rec_ciphertext) + \
             self.cipher_decryptor().finalize()
 
     def unpadded_m(self) -> bytes:
         unpadder = padding.PKCS7(128).unpadder()
         return unpadder.update(self.pre_unpadding_dec()) + unpadder.finalize()
 
-    def decToBytes(self) -> bytes:
+    def dec_to_bytes(self) -> bytes:
         return self.unpadded_m()
 
-    def decToStr(self) -> str:
-        return (self.unpadded_m().decode('UTF-8'))
+    def dec_to_str(self) -> str:
+        return self.unpadded_m().decode('UTF-8')
```

### Comparing `AshCrypt-1.3.6/AshCrypt/AshCryptGUI.py` & `AshCrypt-2.0.0/AshCrypt/AshCryptGUI.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import AshCrypt.TextCrypt as AT
-import AshCrypt.FileCrypt as AF
-import AshCrypt.Database as AD
+import AshCrypt.TextCrypt as At
+import AshCrypt.FileCrypt as Af
+import AshCrypt.Database as Ad
 import ttkbootstrap as tk
 import AshCrypt.qr as qr
 import platform
 import secrets
 import os.path
 import string
 import atexit
 import json
 import re
 
 
 '''------------------------FRAMING STARTED-------------------'''
 
-object = tk.Window(themename='vapor')
-object.resizable(False, False)
-object.title('AshCrypt')
-object.geometry('1500x800')
+main_object = tk.Window(themename='vapor')
+main_object.resizable(False, False)
+main_object.title('AshCrypt')
+main_object.geometry('1500x800')
 
 
-databaseFrame = tk.Frame(master=object, width=500, height=800)
+databaseFrame = tk.Frame(master=main_object, width=500, height=800)
 databaseFrame.place(x=0, y=0)
 
-frameFile1 = tk.Frame(master=object, width=500, height=250)
+frameFile1 = tk.Frame(master=main_object, width=500, height=250)
 frameFile1.place(x=500, y=0)
 
-frameFile2 = tk.Frame(master=object, width=500, height=250)
+frameFile2 = tk.Frame(master=main_object, width=500, height=250)
 frameFile2.place(x=500, y=250)
 
-textFrame1 = tk.Frame(master=object, width=500, height=250)
+textFrame1 = tk.Frame(master=main_object, width=500, height=250)
 textFrame1.place(x=1000, y=0)
 
-textFrame2 = tk.Frame(master=object, width=500, height=250)
+textFrame2 = tk.Frame(master=main_object, width=500, height=250)
 textFrame2.place(x=1000, y=250)
 
-lowerFrame = tk.Frame(master=object, width=1000, height=260)
+lowerFrame = tk.Frame(master=main_object, width=1000, height=260)
 lowerFrame.place(x=500, y=540)
 
 '''---------------DATABASE FRAME STARTED-----------------------'''
 
 
-databaseFrame = tk.Frame(master=object, height=800, width=500)
+databaseFrame = tk.Frame(master=main_object, height=800, width=500)
 databaseFrame.place(rely=0, relx=0)
 
 if platform.system() == 'Windows':
     console_label = tk.Label(
         master=databaseFrame,
         text='DATABASE OUTPUT CONSOLE',
         font='Terminal 15 bold')
@@ -59,43 +59,44 @@
     db_display_text.place(relx=0.016, rely=0.105)
     db_display_text.insert(tk.END, 'Waiting to fetch..')
 else:
     console_label = tk.Label(
         master=databaseFrame,
         text='DATABASE OUTPUT CONSOLE',
         font='Calibre 15 bold')
-    console_label.place(relx=0.09, rely=0.04)
+    console_label.place(relx=0.115, rely=0.04)
 
     db_display_text = tk.Text(
         width=38,
         height=22,
         font='Calibre 13 bold',
         wrap='word')
     db_display_text.place(relx=0.015, rely=0.105)
     db_display_text.insert(tk.END, 'Waiting to fetch..')
 
+
 def show_all_content():
     global db_enable_blocker, main_db_name_var, usable_real_path, main_db_conn, db_display_text, keys_db_conn
     if db_enable_blocker != 0:
         db_display_text.delete('1.0', tk.END)
         db_display_text.insert(
             tk.END, f"Check 'output.json' in the chosen path : {usable_real_path}\n")
         json_path = os.path.join(usable_real_path, 'output.json')
         if swich_db_var.get() == 1:
             conn = keys_db_conn
         else:
             conn = main_db_conn
         try:
             with open(json_path, 'w') as f:
-                eBuffer = {}
+                buffer = {}
                 for e in conn.content():
-                    eBuffer['ID ' + e[0].__str__()] = [{'Filename': e[1]}, {
+                    buffer['ID ' + e[0].__str__()] = [{'Filename': e[1]}, {
                         'Content': e[2].__str__()}, {'KeyRef': e[3]}]
-                eJSON = json.dumps(eBuffer, indent=2)
-                f.write(eJSON)
+                json_content = json.dumps(buffer, indent=2)
+                f.write(json_content)
                 db_display_text.insert(
                     tk.END, f"\nSuccessfully written all table content in output.json\n"
                     f"\nNote that this file will be deleted when the app is closed")
         except BaseException:
             db_display_text.insert(
                 tk.END, f"Failed to write all table content in output.json\n")
 
@@ -118,36 +119,36 @@
                 elif last_id != -1:
 
                     if int(idd) in range(1, last_id):
                         db_display_text.delete('1.0', tk.END)
                         to_json_path = os.path.join(
                             usable_real_path, 'output.json')
                         with open(to_json_path, 'w') as f:
-                            eBuffer = {}
+                            buffer = {}
                             for e in conn.content_by_id(int(idd)):
-                                eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
+                                buffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
                                     'Content': e[2].__str__()}, {'KeyRef': e[3]}]
-                            eJSON = json.dumps(eBuffer, indent=2)
-                            f.write(eJSON)
+                            json_content = json.dumps(buffer, indent=2)
+                            f.write(json_content)
                         db_display_text.insert(
                             tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
                             f" chosen path :\n\n'{usable_real_path}'")
                     if int(idd) == last_id:
                         db_display_text.delete('1.0', tk.END)
                         db_display_text.insert(tk.END, 'Chosen last ID\n\n')
                         to_json_path = os.path.join(
                             usable_real_path, 'output.json')
                         try:
                             with open(to_json_path, 'w') as f:
-                                eBuffer = {}
+                                buffer = {}
                                 for e in conn.content_by_id(int(idd)):
-                                    eBuffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
+                                    buffer['ID_' + e[0].__str__()] = [{'Filename': e[1]}, {
                                         'Content': e[2].__str__()}, {'KeyRef': e[3]}]
-                                eJSON = json.dumps(eBuffer, indent=2)
-                                f.write(eJSON)
+                                json_content = json.dumps(buffer, indent=2)
+                                f.write(json_content)
                             db_display_text.insert(
                                 tk.END, f"Successful fetch !\n\nCheck the 'output.json' file in the"
                                 f" the chosen path :\n\n'{usable_real_path}'")
                         except BaseException:
                             db_display_text.delete('1.0', tk.END)
                             db_display_text.insert(
                                 tk.END, "ERROR \n\nCheck the validity of 'output.json' file"
@@ -231,18 +232,18 @@
         if len(query_var) > 0:
             try:
                 db_display_text.delete('1.0', tk.END)
                 json_file = os.path.join(usable_real_path, 'output.json')
                 with open(json_file, 'w') as f:
                     query_out = conn.query(query_var)
                     conn.addtable()
-                    eJSON = json.dumps(
+                    json_content = json.dumps(
                         {f'query {query_clicks}': query_out}, indent=2)
                     query_clicks += 1
-                    f.write(eJSON)
+                    f.write(json_content)
                 db_display_text.insert(
                     tk.END, f"Ran query {query_clicks} !\n\n")
                 db_display_text.insert(
                     tk.END, f"The result of the query is in 'output.json' file\n\n")
             except BaseException:
                 db_display_text.delete('1.0', tk.END)
                 db_display_text.insert(
@@ -257,17 +258,17 @@
 
 
 query_entry_var = tk.StringVar()
 query_entry = tk.Entry(
     master=databaseFrame,
     width=38,
     font='Calibre 13 bold',
-    textvariable=query_entry_var).place(
-        relx=0.043,
-    rely=0.742)
+    textvariable=query_entry_var)
+
+query_entry.place(relx=0.043, rely=0.742)
 
 query_button = tk.Button(
     master=databaseFrame,
     text='RUN QUERY',
     command=query,
     bootstyle='warning outline')
 query_button.place(relx=0.39, rely=0.81)
@@ -295,15 +296,15 @@
     bootstyle='warning outline')
 show_content_by_id_button.place(relx=0.562, rely=0.93)
 
 
 '''----------------------LOWER FRAME STARTED------------------'''
 
 
-lowerFrame = tk.Frame(master=object, width=1000, height=260)
+lowerFrame = tk.Frame(master=main_object, width=1000, height=260)
 lowerFrame.place(x=500, y=540)
 
 
 db_path_blocker = 0
 usable_real_path = ''
 
 
@@ -344,26 +345,26 @@
                 conn_path_db = os.path.join(usable_real_path, maindbname)
                 if os.path.isfile(
                         fullpath +
                         f'\\{maindbname}') or os.path.isfile(
                         fullpath +
                         f'/{maindbname}'):
                     db_already_exists_blocker = 1
-                    main_db_conn = AD.Database(conn_path_db)
+                    main_db_conn = Ad.Database(conn_path_db)
                     main_db_conn.addtable()
                     main_db_name_result_var.set('CONNECTED')
                     db_display_text.delete('1.0', tk.END)
                     db_display_text.insert(
                         tk.END, f'Connected to {maindbname}..\n\n')
                     success_maindb_connection_blocker = 1
                     encfiletoolbutt.state(['!disabled'])
                     decfiletoolbutt.state(['!disabled'])
                 else:
                     db_already_exists_blocker = 0
-                    main_db_conn = AD.Database(conn_path_db)
+                    main_db_conn = Ad.Database(conn_path_db)
                     main_db_conn.addtable()
                     db_display_text.delete('1.0', tk.END)
                     db_display_text.insert(
                         tk.END,
                         f"Created and Connected to '{maindbname}'.. in the directory '{fullpath}'\n\n")
                     success_maindb_connection_blocker = 1
                     encfiletoolbutt.state(['!disabled'])
@@ -377,48 +378,49 @@
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"The database might be distorted")
     else:
         main_db_name_result_var.set('NOT SET')
         main_db_name_blocker = 0
 
 
-def keyDBsetup():
+def keyd_db_setup():
     global usable_real_path,\
         success_keysdb_connection_blocker,\
         keys_db_conn
     print(usable_real_path)
     if db_path_blocker == 1 and main_db_name_blocker == 1:
         try:
             dbname = main_db_name_var.get().strip()
-            keysDB = dbname[:-3] + 'Keys.db'
-            dbnameKeysWindows = '\\' + keysDB
-            dbnameKeysUnix = '/' + keysDB
-            conn_path_keys = os.path.join(usable_real_path, keysDB)
+            keys_db = dbname[:-3] + 'Keys.db'
+            dbname_keys_win = '\\' + keys_db
+            dbname_keys_unix = '/' + keys_db
+            conn_path_keys = os.path.join(usable_real_path, keys_db)
             if db_already_exists_blocker == 1:
                 if os.path.isfile(
                         usable_real_path +
-                        dbnameKeysWindows) or os.path.isfile(
+                        dbname_keys_win) or os.path.isfile(
                         usable_real_path +
-                        dbnameKeysUnix):
-                    keys_db_conn = AD.Database(conn_path_keys)
+                        dbname_keys_unix):
+                    keys_db_conn = Ad.Database(conn_path_keys)
                     keys_db_conn.addtable()
                     db_display_text.insert(
-                        tk.END, f"Connected to '{keysDB}' ..\n\n")
+                        tk.END, f"Connected to '{keys_db}' ..\n\n")
                     success_keysdb_connection_blocker = 1
                 else:
-                    keys_db_conn = AD.Database(conn_path_keys)
+                    keys_db_conn = Ad.Database(conn_path_keys)
                     keys_db_conn.addtable()
                     db_display_text.insert(
-                        tk.END, f"'{keysDB}' NOT FOUND ! ==> Created and Connected to '{keysDB}' ..\n\n")
+                        tk.END,
+                        f"'{keys_db}' NOT FOUND ! ==> Created and Connected to '{keys_db}' ..\n\n")
                     success_keysdb_connection_blocker = 1
             else:
-                keys_db_conn = AD.Database(conn_path_keys)
+                keys_db_conn = Ad.Database(conn_path_keys)
                 keys_db_conn.addtable()
                 db_display_text.insert(
-                    tk.END, f"Created and Connected to '{keysDB}' ..\n\n")
+                    tk.END, f"Created and Connected to '{keys_db}' ..\n\n")
                 success_keysdb_connection_blocker = 1
         except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(
                 tk.END, f"The database might be distorted\n")
 
 
@@ -426,51 +428,51 @@
 success_keysdb_connection_blocker = 0
 db_enable_blocker = 0
 
 
 def path_name_wrapper():
     set_db_path()
     main_db_name()
-    keyDBsetup()
+    keyd_db_setup()
     global db_enable_blocker, success_keysdb_connection_blocker, success_keysdb_connection_blocker
     if success_keysdb_connection_blocker and success_keysdb_connection_blocker:
         db_enable_blocker = 1
         swich_db_toggle.state(['!disabled'])
     else:
         db_enable_blocker = 0
         swich_db_toggle.state(['disabled'])
 
 
 db_path_var = tk.StringVar()
 db_path_entry = tk.Entry(master=lowerFrame,
                          width=31,
                          font='Calibre 14 bold',
-                         textvariable=db_path_var).place(relx=0.03, rely=0.005)
+                         textvariable=db_path_var)
+db_path_entry.place(relx=0.03, rely=0.005)
 
 db_path_result_var = tk.StringVar(value="")
 db_path_result_entry = tk.Label(
     master=lowerFrame,
     font='Calibre 13 bold',
     bootstyle='light',
-    textvariable=db_path_result_var).place(
-        relx=0.7,
-    rely=0.022)
+    textvariable=db_path_result_var)
+db_path_result_entry.place(relx=0.7, rely=0.022)
 
 path_label = tk.Label(master=lowerFrame,
                       font='Calibre 13 bold',
                       bootstyle='light',
-                      text='DATABASES PATH').place(relx=0.47, rely=0.022)
+                      text='DATABASES PATH')
+path_label.place(relx=0.47, rely=0.022)
 
 main_database_label = tk.Label(
     master=lowerFrame,
     font='Calibre 13 bold',
     bootstyle='light',
-    text='MAIN DATABASE').place(
-        relx=0.47,
-    rely=0.205)
+    text='MAIN DATABASE')
+main_database_label.place(relx=0.47, rely=0.205)
 
 set_db_path_button = tk.Button(
     master=lowerFrame,
     text='SUBMIT PATH AND NAME',
     width=49,
     command=path_name_wrapper,
     bootstyle='info outline')
@@ -515,19 +517,19 @@
             q = conn.query('SELECT ID FROM Classified')
             idd = 0
             for e in q:
                 for k, v in e.items():
                     idd += v[-1][-1][0]
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Last inserted ID is : '{idd}'\n")
-            return (idd)
+            return idd
         except BaseException:
             db_display_text.delete('1.0', tk.END)
             db_display_text.insert(tk.END, f"Last inserted ID is : '0'\n")
-            return (-1)
+            return -1
 
 
 id_button = tk.Button(
     master=lowerFrame,
     text='LAST ID',
     width=22,
     command=checkid,
@@ -557,27 +559,25 @@
 
 
 main_db_name_var = tk.StringVar()
 main_db_name_entry = tk.Entry(
     master=lowerFrame,
     width=31,
     font='Calibre 14 bold',
-    textvariable=main_db_name_var).place(
-        relx=0.03,
-    rely=0.192)
+    textvariable=main_db_name_var)
+main_db_name_entry.place(relx=0.03, rely=0.192)
 
 
 main_db_name_result_var = tk.StringVar(value='')
 main_db_name_result_entry = tk.Label(
     master=lowerFrame,
     font='Calibre 13 bold',
     bootstyle='light',
-    textvariable=main_db_name_result_var).place(
-        relx=0.7,
-    rely=0.205)
+    textvariable=main_db_name_result_var)
+main_db_name_result_entry.place(relx=0.7, rely=0.205)
 
 current_working_db = maindbname
 
 
 def swich_db():
     global current_working_db
     if db_enable_blocker != 0:
@@ -593,15 +593,16 @@
             current_working_db = maindbname[:-3] + 'Keys.db'
 
 
 switch_db_label_var = tk.StringVar(value='SWITCH DATABASE')
 switch_db_label = tk.Label(master=lowerFrame,
                            textvariable=switch_db_label_var,
                            bootstyle='light',
-                           font='Calibre 13 bold').place(relx=0.52, rely=0.39)
+                           font='Calibre 13 bold')
+switch_db_label.place(relx=0.52, rely=0.39)
 
 
 swich_db_var = tk.IntVar(value=0)
 swich_db_toggle = tk.Checkbutton(bootstyle='light,squared-toggle',
                                  master=lowerFrame,
                                  variable=swich_db_var,
                                  offvalue=0,
@@ -614,35 +615,35 @@
 
 
 '''------------TEXT DECRYPTION/ENCRYPTION STARTED--------------'''
 
 
 def encryption():
     m = inputfield1_1.get()
-    if AF.CryptFile.keyverify(
+    if Af.CryptFile.keyverify(
             mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
         if len(m) > 200:
             outputvar1.set('Too Long')
         else:
             if inputfield1_1.get():
                 progressbar.start()
-                a = AT.Crypt(m, mainkeyvar.get())
+                a = At.Crypt(m, mainkeyvar.get())
                 b = a.encrypt()[1]
                 outputvar1.set(b.__str__())
                 if var1.get() == 1:
                     qr.tqr(b)
 
 
 def decryption():
     n = inputfield2_1.get()
-    if AF.CryptFile.keyverify(
+    if Af.CryptFile.keyverify(
             mainkeyvar.get()) == 1 and keySelectionFlag.get() == 1:
         if inputfield2_1.get():
             progressbar2.start()
-            a = AT.Crypt(n, mainkeyvar.get())
+            a = At.Crypt(n, mainkeyvar.get())
             b = a.decrypt()[1]
             outputvar2.set(b.__str__())
             if var2.get() == 1:
                 if not len(b) > 200:
                     qr.tqr(b)
 
 
@@ -660,64 +661,61 @@
         label2.config(text='QR OFF')
 
 
 button1 = tk.Button(
     master=textFrame1,
     text='ENCRYPT',
     command=encryption,
-    bootstyle='light outline').place(
-        relx=0.42,
-    rely=0.73)
+    bootstyle='light outline')
+button1.place(relx=0.42, rely=0.73)
+
 button2 = tk.Button(
     master=textFrame2,
     text='DECRYPT',
     command=decryption,
-    bootstyle='light outline').place(
-        relx=0.42,
-    rely=0.8)
+    bootstyle='light outline')
+button2.place(relx=0.42, rely=0.8)
 
 inputfield1_1 = tk.StringVar()
 textfield1_1 = tk.Entry(master=textFrame1,
                         width=20,
                         font='Calibre 11 bold',
-                        textvariable=inputfield1_1).place(relx=0.29, rely=0.30)
+                        textvariable=inputfield1_1)
+textfield1_1.place(relx=0.29, rely=0.30)
 
 inputfield2_1 = tk.StringVar(value='')
 textfield2_1 = tk.Entry(
     master=textFrame2,
     font='Calibre 11 bold',
     width=20,
-    textvariable=inputfield2_1).place(
-        relx=0.290,
-    rely=0.38)
+    textvariable=inputfield2_1)
+textfield2_1.place(relx=0.290, rely=0.38)
 
 namelabel1 = tk.Label(master=textFrame1,
                       text='TEXT ENCRYPTION',
                       font='Calibre 20 bold',
                       )
 namelabel1.place(relx=0.190, rely=0.10)
 namelabel2 = tk.Label(master=textFrame2,
                       text='TEXT DECRYPTION',
                       font='Calibre 20 bold',
-                      ).place(relx=0.190, rely=0.200)
+                      )
+namelabel2.place(relx=0.190, rely=0.200)
 
 outputvar1 = tk.StringVar(value='')
 outputlabel1 = tk.Entry(master=textFrame1,
                         textvariable=outputvar1,
-                        font='terminal 11 bold').place(relx=0.02,
-                                                       rely=0.48,
-                                                       width=480,
-                                                       height=50)
+                        font='terminal 11 bold')
+outputlabel1.place(relx=0.02, rely=0.48, width=480, height=50)
+
 outputvar2 = tk.StringVar(value='')
 outputlabel2 = tk.Entry(master=textFrame2,
                         textvariable=outputvar2,
-                        font='terminal 11 bold').place(relx=0.02,
-                                                       rely=0.55,
-                                                       width=480,
-                                                       height=50)
+                        font='terminal 11 bold')
+outputlabel2.place(relx=0.02, rely=0.55, width=480, height=50)
 
 
 label1 = tk.Label(master=textFrame1, text='QR', font=('terminal', 17))
 label1.place(relx=0.2, rely=0.75)
 var1 = tk.IntVar()
 mytoolbutt3 = tk.Checkbutton(bootstyle='success , round-toggle',
                              master=textFrame1,
@@ -766,29 +764,31 @@
                          )
 filepathlabel.place(relx=0.335, rely=0.10)
 
 if platform.system() == 'Windows':
     resultvarfile = tk.StringVar(value='                 ..........')
     resultLabelfile = tk.Label(master=frameFile1,
                                textvariable=resultvarfile,
-                               font='terminal 13 bold').place(rely=0.55)
+                               font='terminal 13 bold')
+    resultLabelfile.place(rely=0.55)
 else:
     resultvarfile = tk.StringVar(value='                    ..........')
     resultLabelfile = tk.Label(master=frameFile1,
                                textvariable=resultvarfile,
-                               font='terminal 13 bold').place(rely=0.55)
+                               font='terminal 13 bold')
+    resultLabelfile.place(rely=0.55)
 
 
-def encFile():
-    global fileaccessSemo, add_enc_to_db, main_db_conn, mainkey
+def enc_file():
+    global add_enc_to_db, main_db_conn, mainkey
     if 1:
         if keySelectionFlag.get() != 0:
             filename = filenameStringVar.get().strip()
             key = mainkey
-            target = AF.CryptFile(filename, key)
+            target = Af.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
                 filename = filename + '.crypt'
                 filenameStringVar.set(filename)
                 resultvarfile.set(
                     '      Encrypted Successfully / added .crypt')
                 if encfiletoolbuttvar.get() == 1:
@@ -834,20 +834,20 @@
                         '         ERROR : File is already encrypted')
                 elif a == 7:
                     resultvarfile.set(
                         '   ERROR : Given a directory instead of a file')
 
 
 def decfile():
-    global fileaccessSemo, add_dec_to_db, main_db_conn, mainkey
+    global add_dec_to_db, main_db_conn, mainkey
     if 1:
         if keySelectionFlag.get() != 0:
             filename = filenameStringVar.get().strip()
             key = mainkey
-            target = AF.CryptFile(filename, key)
+            target = Af.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
                 filename = os.path.splitext(filename)[0]
                 filenameStringVar.set(filename)
                 resultvarfile.set(
                     '     Decrypted Successfully + removed .crypt')
                 if decfiletoolbuttvar.get() == 1:
@@ -895,97 +895,95 @@
                     resultvarfile.set(
                         '   ERROR : Given a directory instead of a file')
 
 
 encryptionfilebutton = tk.Button(
     master=frameFile1,
     text='ENCRYPT FILE',
-    command=encFile,
-    bootstyle='warning outline').place(
-        relx=0.25,
-    rely=0.73)
+    command=enc_file,
+    bootstyle='warning outline')
+encryptionfilebutton.place(relx=0.25, rely=0.73)
+
 decryptionfilebutton = tk.Button(
     master=frameFile1,
     text='DECRYPT FILE',
     command=decfile,
-    bootstyle='warning outline').place(
-        relx=0.55,
-    rely=0.73)
+    bootstyle='warning outline')
+decryptionfilebutton.place(relx=0.55, rely=0.73)
 
 filenameStringVar = tk.StringVar(value='')
 
 filenametext = tk.Entry(
     master=frameFile1,
     width=31,
     font='Calibre 15 bold',
-    textvariable=filenameStringVar).place(
-        relx=0.05,
-    rely=0.30)
+    textvariable=filenameStringVar)
+filenametext.place(relx=0.05, rely=0.30)
 
 
 addtodbLabel = tk.Label(
     master=frameFile1,
     text='ADD TO DATABASE',
     font=(
         'Calibre',
         11),
     bootstyle='warning')
 addtodbLabel.place(relx=0.35, rely=0.908)
 
 add_enc_to_db = 0
 
 
-def encToggleButtFunc():
+def enc_toggle_func():
     global add_enc_to_db
     if encfiletoolbuttvar == 1:
         add_enc_to_db = 1
     else:
         add_enc_to_db = 0
 
 
 add_dec_to_db = 0
 
 
-def decToggleButtFunc():
+def dec_toggle_func():
     global add_dec_to_db
     if decfiletoolbuttvar == 1:
         add_dec_to_db = 1
     else:
         add_dec_to_db = 0
 
 
 encfiletoolbuttvar = tk.IntVar()
 encfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
                                  master=frameFile1,
                                  variable=encfiletoolbuttvar,
                                  offvalue=0,
                                  onvalue=1,
-                                 command=encToggleButtFunc)
+                                 command=enc_toggle_func)
 encfiletoolbutt.state(['disabled'])
 encfiletoolbutt.place(relx=0.25, rely=0.92)
 
 
 decfiletoolbuttvar = tk.IntVar()
 decfiletoolbutt = tk.Checkbutton(bootstyle='warning , round-toggle',
                                  master=frameFile1,
                                  variable=decfiletoolbuttvar,
                                  offvalue=0,
-                                 command=decToggleButtFunc)
+                                 command=dec_toggle_func)
 decfiletoolbutt.state(['disabled'])
 decfiletoolbutt.place(relx=0.717, rely=0.92)
 
 
 keySelectionFlag = tk.IntVar(value=0)
 
 
-def mainKeyWrapper():
+def main_key_wrapper():
     global success_keysdb_connection_blocker, mainkey
-    if AF.CryptFile.keyverify(mainkeyvar.get().strip()) == 1:
+    if Af.CryptFile.keyverify(mainkeyvar.get().strip()) == 1:
         mainkey = mainkeyvar.get().strip()
-        keyrefGen()
+        keyref_gen()
         keyselectionvar.set('       SELECTED')
         keySelectionFlag.set(1)
         try:
             if success_keysdb_connection_blocker and os.path.isfile(
                     filenameStringVar.get().strip()):
                 keys_db_conn.insert(
                     filenameStringVar.get().strip(),
@@ -1002,26 +1000,28 @@
         keyselectionvar.set('     NOT SELECTED')
 
 
 mainkeyLabel = tk.Label(master=frameFile2,
                         text='MAIN KEY',
                         font='Calibre 20 bold',
                         bootstyle='info',
-                        ).place(relx=0.3, rely=0.075)
+                        )
+mainkeyLabel.place(relx=0.3, rely=0.075)
 
 
 mainkeyvar = tk.StringVar()
 mainkeyEntry = tk.Entry(master=frameFile2,
                         font='Calibre 14 bold',
                         textvariable=mainkeyvar,
                         width=29
-                        ).place(relx=0.09, rely=0.29)
+                        )
+mainkeyEntry.place(relx=0.09, rely=0.29)
 
 
-def keyrefGen():
+def keyref_gen():
     ref = '#'
     for _ in range(6):
         character = secrets.choice(
             string.ascii_letters +
             string.digits +
             '$' +
             '?' +
@@ -1043,43 +1043,43 @@
         'terminal',
         12))
 keyrefLabel.place(relx=0.712, rely=0.12)
 
 keySelectButton = tk.Button(
     master=frameFile2,
     text='SELECT KEY',
-    command=mainKeyWrapper,
-    bootstyle='info outline').place(
-        relx=0.6725,
-    rely=0.5)
+    command=main_key_wrapper,
+    bootstyle='info outline')
+keySelectButton.place(relx=0.6725, rely=0.5)
 
 
 keyselectionvar = tk.StringVar(value='   KEY NOT SELECTED')
 keyselectionLabel = tk.Label(master=frameFile2,
                              textvariable=keyselectionvar,
                              bootstyle='info',
-                             font='terminal 11 bold').place(relx=0.15,
-                                                            rely=0.465,
-                                                            height=50)
+                             font='terminal 11 bold')
+keyselectionLabel.place(relx=0.15, rely=0.465, height=50)
 
 
-def genMainKey():
-    keyGenVar.set(AF.CryptFile.genkey())
+def genkey():
+    keyGenVar.set(Af.CryptFile.genkey())
 
 
 keyGenVar = tk.StringVar(value='')
 keyGenEntry = tk.Entry(master=frameFile2,
                        font='Calibre 12 bold',
                        textvariable=keyGenVar,
-                       width=23).place(relx=0.1, rely=0.69)
+                       width=23)
+keyGenEntry.place(relx=0.1, rely=0.69)
 
 keyButton = tk.Button(master=frameFile2,
                       text='GENERATE',
-                      command=genMainKey,
-                      bootstyle='success outline').place(relx=0.671, rely=0.7)
+                      command=genkey,
+                      bootstyle='success outline')
+keyButton.place(relx=0.671, rely=0.7)
 
 
 '''----------------------------STAMP STARTED ------------------------------'''
 
 
 latest_ID_key_label = tk.Label(
     master=lowerFrame,
@@ -1107,8 +1107,8 @@
     rm_json()
 
 
 atexit.register(rm_all)
 
 
 if __name__ == '__main__':
-    object.mainloop()
+    main_object.mainloop()
```

### Comparing `AshCrypt-1.3.6/AshCrypt/CliCrypt.py` & `AshCrypt-2.0.0/AshCrypt/CliCrypt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from AshCrypt import FileCrypt as AF
-from AshCrypt import TextCrypt as A
+from AshCrypt import FileCrypt as Af
+from AshCrypt import TextCrypt as At
 import os.path
 import sys
 
 
 print('Welcome to the CLI')
 
 commands = 'Commands : \n' \
@@ -24,21 +24,21 @@
     if c == 1:
         print(commands)
     if e == 1:
         file_decFlag = False
         file_encFlag = False
         decFlag = False
         encflag = True
-        enc()
+        enc_f()
     if d == 1:
         file_decFlag = False
         file_encFlag = False
         encflag = False
         decFlag = True
-        dec()
+        dec_f()
     if ef == 1:
         decFlag = False
         encflag = False
         file_decFlag = False
         file_encFlag = True
         file_enc()
     if df == 1:
@@ -47,15 +47,15 @@
         file_encFlag = False
         file_decFlag = True
         file_dec()
     else:
         pass
 
 
-def inputWrap(inp):
+def input_wrap(inp):
     inp = inp.lower()
     if inp == 'c':
         input_selection(c=1)
         return 'c'
     if inp == 'q':
         input_selection(q=1)
         return 'q'
@@ -72,83 +72,82 @@
         input_selection(df=1)
         return 'df'
     else:
         return None
 
 
 def intro():
-    intro = True
-    while intro:
+    while True:
         print('Program started running..')
         print('Press c to view commands : ')
         while True:
             n = input("Press..\n")
-            inputWrap(n)
+            input_wrap(n)
 
 
 def keysetup():
     outer = True
     inner = True
     while outer:
         global key
         key = ''
         i = input('Do you have a key ?(y/n) : ')
-        inputWrap(i)
+        input_wrap(i)
         if i.lower() == 'n':
             print("Here's your key : ")
-            key = A.Crypt.genkey()
+            key = At.Crypt.genkey()
             print(key)
             inner = False
             outer = False
         elif i.lower() == 'y':
             while inner:
                 print('insert your key here : ')
                 kk = input()
-                inputWrap(kk)
-                if A.Crypt.keyverify(kk) == 1:
+                input_wrap(kk)
+                if At.Crypt.keyverify(kk) == 1:
                     print('Key selected\n')
                     key = kk
                     inner = False
                     outer = False
                 else:
                     print('Enter a valid key !\n')
 
 
 encflag = True
 
 
-def enc():
+def enc_f():
     keysetup()
     while encflag:
         print()
         global key
         print("press c to view commands.. ")
         message = input('Encrypt a message : ')
-        inputWrap(message)
-        a = A.Crypt(message, key=key)
+        input_wrap(message)
+        a = At.Crypt(message, key=key)
         enc = a.encrypt()
         if (enc[0]) == 1:
             print("Success ! Here's the message : ")
             print('\t', enc[1], '\n')
         else:
             print('Error occurred during the encryption process\n')
 
 
 decFlag = True
 
 
-def dec():
+def dec_f():
     keysetup()
     while decFlag:
         print()
         global key
         print("press c to view commands.. ")
         message = input('Decrypt a message : ')
-        inputWrap(message)
-        a = A.Crypt(message, key=key)
+        input_wrap(message)
+        a = At.Crypt(message, key=key)
         dec = a.decrypt()
         if (dec[0]) == 1:
             print("Success ! Here's the message : ")
             print('\t', dec[1], '\n')
         else:
             print('Error occurred during the decryption process\n')
 
@@ -163,19 +162,19 @@
     keysetup()
     while file_decFlag:
         print()
         global key
         pre = input(
             "running file decryption mode , press the known commands or 'Enter' to continue.. : ")
         print()
-        inputWrap(pre)
+        input_wrap(pre)
         if pre == '':
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Decrypted : ')
-            target = AF.CryptFile(filename, key)
+            target = Af.CryptFile(filename, key)
             a = target.decrypt()
             if a == 1:
                 print('File successfully decrypted + removed .crypt extension')
                 print(f'File is now named {os.path.splitext(filename)[0]}')
             if a == 2:
                 print('Cannot decrypt the file  when it is already empty')
             if a == 3:
@@ -199,19 +198,19 @@
     keysetup()
     while file_encFlag:
         print()
         global key
         pre = input(
             "running file encryption mode, press the known commands or 'Enter' to continue.. : ")
         print()
-        inputWrap(pre)
+        input_wrap(pre)
         if pre == '':
             print("You can use the commands AFTER entering the file name.. ")
             filename = input('Enter full file name to be Encrypted : ')
-            target = AF.CryptFile(filename, key)
+            target = Af.CryptFile(filename, key)
             a = target.encrypt()
             if a == 1:
                 print('File successfully encrypted + added .crypt extension')
                 print(f"File is now named : '{filename}.crypt' ")
             if a == 2:
                 print('Cannot encrypt the file  when it is already empty')
             if a == 3:
```

### Comparing `AshCrypt-1.3.6/AshCrypt/Database.py` & `AshCrypt-2.0.0/AshCrypt/Database.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from datetime import datetime
 from typing import Union
 import sqlite3
 import os
 
 
 @dataclass
-class Database():
+class Database:
     dbname: str = field()
     tablename: str = field(default='Classified')
     conn: sqlite3.Connection = field(init=False, repr=False)
     c: sqlite3.Cursor = field(init=False, repr=False)
 
     def __post_init__(self):
         self.conn = sqlite3.connect(self.dbname)
@@ -22,28 +22,28 @@
             with self.conn:
                 self.c.execute(
                     'SELECT page_count * page_size FROM pragma_page_count() , pragma_page_size')
                 size_info = self.c.fetchone()
                 size = size_info[0] / 1024 / 1024
                 return size
         except sqlite3.Error as e:
-            return (0, e)
+            return 0, e
 
     @property
     def last_mod(self) -> Union[datetime, tuple]:
         try:
             time_stat = datetime.fromtimestamp(os.stat(self.dbname).st_mtime)
             return time_stat
 
         except OSError as e:
-            return (0, e)
+            return 0, e
 
     @property
     def default_routing(self):
-        return (f'DEFAULT ROUTING ALL METHODS TO "{self.tablename}"')
+        return f'DEFAULT ROUTING ALL METHODS TO "{self.tablename}"'
 
     def query(self, *querys: str) -> list:
         result = []
         for i, query in enumerate(querys):
             if not isinstance(query, str):
                 result.append({f'query {i}': (0.0, TypeError)})
             try:
@@ -65,209 +65,209 @@
             try:
                 with self.conn:
                     self.c.execute(
                         f"CREATE TABLE IF NOT EXISTS {self.tablename} "
                         "(ID INTEGER PRIMARY KEY, Name Text , Content BLOB ,Key TEXT )")
                 return 11
             except sqlite3.Error as e:
-                return (0.0, e)
+                return 0.0, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
                         f"CREATE TABLE IF NOT EXISTS {optional_tablename} "
                         "(ID INTEGER PRIMARY KEY,"
                         "Name TEXT ,"
                         "Content BLOB ,"
                         "Key TEXT )")
                     self.tablename = optional_tablename
                 return 1
 
             except sqlite3.Error as e:
-                return (0, e)
+                return 0, e
 
     def insert(self, name, content, key, optional_table_name=None):
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
                         f"INSERT INTO {self.tablename} (Name , Content ,Key) VALUES (? , ? , ?) ",
                         (name,
                          content,
                          key))
 
                 return 11
             except sqlite3.Error as e:
-                return (0.0, e)
+                return 0.0, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
                         f"INSERT INTO {optional_table_name} (Name, Content ,Key) VALUES (? , ? , ?) ",
                         (name,
                          content,
                          key))
                 return 1
             except sqlite3.Error as e:
-                return (0, e)
+                return 0, e
 
     def update(
             self,
             column_name: str,
             new_column_val: str,
-            ID: int,
+            idd: int,
             optional_table_name=None):
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
-                        (f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? '),
+                        f'UPDATE {self.tablename} SET {column_name} = ? WHERE ID = ? ',
                         (new_column_val,
-                         ID))
+                         idd))
                     return 11
 
             except sqlite3.Error as e:
-                return (0.0, e)
+                return 0.0, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        (f'UPDATE {optional_table_name} SET ? = ? WHERE ID = ? '),
+                        f'UPDATE {optional_table_name} SET ? = ? WHERE ID = ? ',
                         (column_name,
                          new_column_val,
-                         ID))
+                         idd))
                     return 1
 
             except sqlite3.Error as e:
-                return (0, e)
+                return 0, e
 
     def content(self, optional_tablename=None):
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(f'SELECT * FROM {self.tablename} ')
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
-                return (0.0, e)
+                return 0.0, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(f'SELECT * FROM {optional_tablename} ')
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
-                return (0, e)
+                return 0, e
 
-    def content_by_id(self, id: int, optional_tablename=None):
+    def content_by_id(self, idd: int, optional_tablename=None):
         if optional_tablename is None:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (id,))
+                        f'SELECT * FROM {self.tablename} WHERE ID = ? ', (idd,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
-                return (0.0, e)
+                return 0.0, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'SELECT * FROM {optional_tablename} WHERE ID = ? ', (id,))
+                        f'SELECT * FROM {optional_tablename} WHERE ID = ? ', (idd,))
                     for row in self.c.fetchall():
                         yield row
 
             except sqlite3.Error as e:
-                return (0, e)
+                return 0, e
 
     def show_contents(self, *optional_tablenames):
         if optional_tablenames:
             try:
                 for arg in optional_tablenames:
                     with self.conn:
                         self.c.execute(f'SELECT * FROM {arg} ')
                         for row in self.c.fetchall():
                             yield {arg: row}
 
             except sqlite3.Error as e:
-                return (0.0, e)
+                return 0.0, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(f'SELECT * FROM {self.tablename} ')
                     for row in self.c.fetchall():
                         yield {self.tablename: row}
 
             except sqlite3.Error as e:
-                return (0, e)
+                return 0, e
 
     def show_tables(self) -> tuple:
         try:
             with self.conn:
                 self.c.execute(
                     "SELECT name FROM sqlite_master WHERE type= 'table' ")
                 for row in self.c.fetchall():
                     yield row
 
         except sqlite3.Error as e:
-            return (0, e)
+            return 0, e
 
     def dropall(self):
         try:
             with self.conn:
                 self.c.execute(
                     "SELECT name FROM sqlite_master WHERE type= 'table' ")
                 for table in self.c.fetchall():
                     self.c.execute(f'DROP TABLE {table[0]}')
                 return 1
 
         except sqlite3.Error as e:
-            return (0, e)
+            return 0, e
 
     def drop_table(self, *table_names):
         if table_names:
             try:
                 for arg in table_names:
                     with self.conn:
                         self.c.execute(f"DROP TABLE {arg}")
                 return 1
             except sqlite3.Error as e:
-                return (0.0, e)
+                return 0.0, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(f'DROP TABLE {self.tablename}')
                     return 1
 
             except sqlite3.Error as e:
-                return (0, e)
+                return 0, e
 
-    def drop_content(self, ID, optional_table_name=None):
+    def drop_content(self, idd, optional_table_name=None):
         if optional_table_name is None:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'DELETE FROM {self.tablename} WHERE ID = {ID}')
+                        f'DELETE FROM {self.tablename} WHERE ID = {idd}')
                 return 11
 
             except sqlite3.Error as e:
-                return (0.0, e)
+                return 0.0, e
 
         else:
             try:
                 with self.conn:
                     self.c.execute(
-                        f'DELETE FROM {optional_table_name} WHERE ID = {ID}')
+                        f'DELETE FROM {optional_table_name} WHERE ID = {idd}')
                 return 1
 
             except sqlite3.Error as e:
-                return (0, e)
+                return 0, e
```

### Comparing `AshCrypt-1.3.6/AshCrypt/FileCrypt.py` & `AshCrypt-2.0.0/AshCrypt/FileCrypt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from AshCrypt import Ash
 import os
 
 
-class KeyError(Exception):
+class KeyLengthError(Exception):
     def __init__(self):
         self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
 
 
-class CryptFile():
+class CryptFile:
     def __init__(self, filename, key):
         self.filename = filename
         self.not_256_bit_key = 0
         if self.keyverify(key) == 1:
             self.key = key
         else:
-            self.not_256_bit_key = 1  # Raise KeyError()
+            self.not_256_bit_key = 1  # Raise KeyError() / you can switch error handling
 
     @staticmethod
     def genkey() -> str:
-        return Ash.Enc.genMainkey()
+        return Ash.Enc.genkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
         try:
             if isinstance(key, str):
                 a = bytes.fromhex(key.strip())
                 if len(a) == 32:
@@ -35,29 +35,28 @@
 
     def encrypt(self) -> int:
         if os.path.isdir(self.filename):
             return 7
         if self.not_256_bit_key == 1:
             return 5
         try:
-            go_ahead_rename_crypt = 0
             if not os.path.exists(self.filename):
                 return 3
             else:
                 if os.path.splitext(self.filename)[1] == '.crypt':
                     return 6
                 else:
                     with open(self.filename, 'rb') as f:
                         filecontent = f.read()
                     with open(self.filename, 'wb') as f:
                         if filecontent:
                             try:
                                 ins = Ash.Enc(
                                     message=filecontent, mainkey=self.key)
-                                new_content = ins.encToBytes()
+                                new_content = ins.enc_to_bytes()
                                 f.write(new_content)
                                 go_ahead_rename_crypt = 1
                             except BaseException:
                                 f.write(filecontent)
                                 return 0
                         else:
                             f.write(filecontent)
@@ -70,29 +69,28 @@
 
     def decrypt(self) -> int:
         if os.path.isdir(self.filename):
             return 7
         if self.not_256_bit_key == 1:
             return 5
         try:
-            go_ahead_remove_crypt = 0
             if not os.path.exists(self.filename):
                 return 3
             else:
                 if os.path.splitext(self.filename)[1] != '.crypt':
                     return 6
                 else:
                     with open(self.filename, 'rb') as f:
                         enc_content = f.read()
                     with open(self.filename, 'wb') as f:
                         if enc_content:
                             try:
                                 ins = Ash.Dec(
                                     message=enc_content, mainkey=self.key)
-                                a = ins.decToBytes()
+                                a = ins.dec_to_bytes()
                                 f.write(a)
                                 go_ahead_remove_crypt = 1
                             except Exception:
                                 f.write(enc_content)
                                 return 0
                         else:
                             f.write(enc_content)
@@ -105,8 +103,8 @@
         except Exception:
             return 4
 
     def __str__(self):
         return f'Encrypting/Decrypting File {self.filename} With {self.key} Key '
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({self.filename},{self.key})'
+        return f'{self.__class__.__name__}({self.filename},{self.key})'
```

### Comparing `AshCrypt-1.3.6/AshCrypt/TextCrypt.py` & `AshCrypt-2.0.0/AshCrypt/TextCrypt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from typing import Union
 from AshCrypt import Ash
 
 
-class KeyError(Exception):
+class KeyLengthError(Exception):
     def __init__(self):
         self.display = 'Key must be 256 Bit long !'
         super().__init__(self.display)
 
 
-class Crypt():
+class Crypt:
     def __init__(self, text: Union[str, bytes], key: str):
         self.text = text
         if self.keyverify(key) == 1:
             self.key = key
         else:
             raise KeyError()
 
     @staticmethod
     def genkey() -> str:
-        return Ash.Enc.genMainkey()
+        return Ash.Enc.genkey()
 
     @staticmethod
     def keyverify(key: str) -> int:
         if isinstance(key, str):
             try:
                 a = bytes.fromhex(key.strip())
                 if len(a) == 32:
@@ -33,33 +33,33 @@
         else:
             return 2
 
     def encrypt(self) -> tuple:
         if self.text:
             try:
                 ins = Ash.Enc(self.text, self.key)
-                new_content = ins.encToStr()
+                new_content = ins.enc_to_str()
                 return 1, new_content
             except BaseException:
                 output = 'E'
                 return 0, output
         else:
             return 0.0, 0.0
 
     def decrypt(self) -> tuple:
         if self.text:
             try:
                 dec_instance = Ash.Dec(message=self.text, mainkey=self.key)
-                a = dec_instance.decToStr()
-                output = (a)
+                a = dec_instance.dec_to_str()
+                output = a
                 return 1, output
             except Exception:
-                output = (self.text)
+                output = self.text
                 return 0, output
         else:
             return 0.0, 0.0
 
     def __str__(self):
-        return f'Encrypting/Decrypting Text {(self.text)[:8]}.. With {self.key} Key '
+        return f'Encrypting/Decrypting Text {self.text[:8]}.. With {self.key} Key '
 
     def __repr__(self):
-        return f'{self.__class__.__name__}({(self.text)[:8]},{self.key})'
+        return f'{self.__class__.__name__}({self.text[:8]},{self.key})'
```

### Comparing `AshCrypt-1.3.6/AshCrypt/__pycache__/Ash.cpython-39.pyc` & `AshCrypt-2.0.0/AshCrypt/__pycache__/Ash.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jul 11 22:44:20 2023 UTC, .py size: 5207 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 44db ad64 5714 0000  a.......D..dW...
+00000000: 610d 0d0a 0000 0000 a5e9 b364 6114 0000  a..........da...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
 00000040: 0100 6400 6402 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c04  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000070: 6d0b 5a0b 0100 6400 6406 6c09 5a0c 6400  m.Z...d.d.l.Z.d.
@@ -28,29 +28,29 @@
 000001b0: 0000 0000 0000 0002 0000 0003 0000 0003  ................
 000001c0: 0000 0073 2000 0000 6401 7c01 9b00 6402  ...s ...d.|...d.
 000001d0: 9d03 7c00 5f00 7401 8300 a002 7c00 6a00  ..|._.t.....|.j.
 000001e0: a101 0100 6400 5300 2903 4e7a 3549 7465  ....d.S.).Nz5Ite
 000001f0: 7261 7469 6f6e 7320 6d75 7374 2062 6520  rations must be 
 00000200: 6265 7477 6565 6e20 3530 2061 6e64 2031  between 50 and 1
 00000210: 3030 3030 302e 2052 4543 4549 5645 4420  00000. RECEIVED 
-00000220: 3a20 fa01 20a9 035a 0764 6973 706c 6179  : .. ..Z.display
+00000220: 3a20 fa01 20a9 03da 0764 6973 706c 6179  : .. ....display
 00000230: da05 7375 7065 72da 085f 5f69 6e69 745f  ..super..__init_
 00000240: 5f29 02da 0473 656c 6672 0b00 0000 a901  _)...selfr......
 00000250: da09 5f5f 636c 6173 735f 5fa9 00fa 2a43  ..__class__...*C
 00000260: 3a5c 576f 726b 5c47 6974 4875 6257 6f72  :\Work\GitHubWor
 00000270: 6b5c 4145 532d 3235 365c 4173 6843 7279  k\AES-256\AshCry
-00000280: 7074 5c41 7368 2e70 7972 1000 0000 0e00  pt\Ash.pyr......
+00000280: 7074 5c41 7368 2e70 7972 1100 0000 0e00  pt\Ash.pyr......
 00000290: 0000 7304 0000 0000 010e 017a 2349 7465  ..s........z#Ite
 000002a0: 7261 7469 6f6e 734f 7574 6f66 6152 616e  rationsOutofaRan
 000002b0: 6765 4572 726f 722e 5f5f 696e 6974 5f5f  geError.__init__
 000002c0: 2906 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
 000002d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000002e0: 6e61 6d65 5f5f da03 616e 7972 1000 0000  name__..anyr....
+000002e0: 6e61 6d65 5f5f da03 616e 7972 1100 0000  name__..anyr....
 000002f0: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
-00000300: 1400 0000 7214 0000 0072 1200 0000 7215  ....r....r....r.
+00000300: 1500 0000 7215 0000 0072 1300 0000 7216  ....r....r....r.
 00000310: 0000 0072 0a00 0000 0d00 0000 7302 0000  ...r........s...
 00000320: 0008 0172 0a00 0000 6300 0000 0000 0000  ...r....c.......
 00000330: 0000 0000 0000 0000 0006 0000 0040 0000  .............@..
 00000340: 0073 bc00 0000 6500 5a01 6400 5a02 6503  .s....e.Z.d.Z.e.
 00000350: 6504 6505 6602 1900 6504 6401 6402 9c03  e.e.f...e.d.d...
 00000360: 6403 6404 8404 5a06 6507 6504 6505 6508  d.d...Z.e.e.e.e.
 00000370: 6505 6405 9c04 6406 6407 8404 8301 5a09  e.d...d.d.....Z.
@@ -75,325 +75,326 @@
 000004a0: 6a7c 006a 0b64 036b 0472 7474 0c7c 006a  j|.j.d.k.rtt.|.j
 000004b0: 0b83 0182 017c 00a0 0d7c 006a 057c 006a  .....|...|.j.|.j
 000004c0: 097c 006a 0ba1 037c 005f 0e7c 00a0 0d7c  .|.j...|._.|...|
 000004d0: 006a 057c 006a 0a7c 006a 0ba1 037c 005f  .j.|.j.|.j...|._
 000004e0: 0f64 0053 0029 044e e910 0000 00e9 3200  .d.S.).N......2.
 000004f0: 0000 e9a0 8601 0029 10da 0a69 7369 6e73  .......)...isins
 00000500: 7461 6e63 65da 0373 7472 da06 656e 636f  tance..str..enco
-00000510: 6465 721d 0000 00da 0562 7974 6573 721e  der......bytesr.
+00000510: 6465 721e 0000 00da 0562 7974 6573 721f  der......bytesr.
 00000520: 0000 00da 026f 73da 0775 7261 6e64 6f6d  .....os..urandom
 00000530: da02 6976 da04 7361 6c74 da06 7065 7070  ..iv..salt..pepp
 00000540: 6572 da0a 6974 6572 6174 696f 6e73 720a  er..iterationsr.
 00000550: 0000 00da 0664 6572 6b65 79da 0665 6e63  .....derkey..enc
 00000560: 4b65 79da 0868 6d61 635f 6b65 7929 0372  Key..hmac_key).r
-00000570: 1100 0000 721d 0000 0072 1e00 0000 7214  ....r....r....r.
-00000580: 0000 0072 1400 0000 7215 0000 0072 1000  ...r....r....r..
+00000570: 1200 0000 721e 0000 0072 1f00 0000 7215  ....r....r....r.
+00000580: 0000 0072 1500 0000 7216 0000 0072 1100  ...r....r....r..
 00000590: 0000 1400 0000 731a 0000 0000 010a 010c  ......s.........
 000005a0: 010a 0106 0206 010c 010c 010c 0106 0114  ................
 000005b0: 010a 0116 017a 0c45 6e63 2e5f 5f69 6e69  .....z.Enc.__ini
-000005c0: 745f 5f29 0472 1e00 0000 da0b 7361 6c74  t__).r......salt
-000005d0: 5f70 6570 7065 7272 2b00 0000 720c 0000  _pepperr+...r...
+000005c0: 745f 5f29 0472 1f00 0000 da0b 7361 6c74  t__).r......salt
+000005d0: 5f70 6570 7065 7272 2c00 0000 720c 0000  _pepperr,...r...
 000005e0: 0063 0300 0000 0000 0000 0000 0000 0300  .c..............
 000005f0: 0000 0600 0000 4300 0000 7318 0000 0074  ......C...s....t
 00000600: 006a 017c 00a0 0264 01a1 017c 0164 027c  .j.|...d...|.d.|
 00000610: 0264 038d 0453 0029 044e fa05 5554 462d  .d...S.).N..UTF-
 00000620: 38e9 2000 0000 2904 5a08 7061 7373 776f  8. ...).Z.passwo
-00000630: 7264 7229 0000 005a 1164 6573 6972 6564  rdr)...Z.desired
+00000630: 7264 722a 0000 005a 1164 6573 6972 6564  rdr*...Z.desired
 00000640: 5f6b 6579 5f62 7974 6573 da06 726f 756e  _key_bytes..roun
 00000650: 6473 2903 da06 6263 7279 7074 5a03 6b64  ds)...bcryptZ.kd
-00000660: 6672 2400 0000 2903 721e 0000 0072 2f00  fr$...).r....r/.
-00000670: 0000 722b 0000 0072 1400 0000 7214 0000  ..r+...r....r...
-00000680: 0072 1500 0000 722c 0000 0024 0000 0073  .r....r,...$...s
+00000660: 6672 2500 0000 2903 721f 0000 0072 3000  fr%...).r....r0.
+00000670: 0000 722c 0000 0072 1500 0000 7215 0000  ..r,...r....r...
+00000680: 0072 1600 0000 722d 0000 0024 0000 0073  .r....r-...$...s
 00000690: 0c00 0000 0002 0401 0801 0201 0201 02fc  ................
 000006a0: 7a0a 456e 632e 6465 726b 6579 a901 720c  z.Enc.derkey..r.
 000006b0: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
 000006c0: 0000 0000 0300 0000 4300 0000 730e 0000  ........C...s...
 000006d0: 0074 00a0 0164 01a1 01a0 02a1 0053 0029  .t...d.......S.)
-000006e0: 024e 7231 0000 0029 0372 2600 0000 7227  .Nr1...).r&...r'
-000006f0: 0000 00da 0368 6578 7214 0000 0072 1400  .....hexr....r..
-00000700: 0000 7214 0000 0072 1500 0000 da0a 6765  ..r....r......ge
-00000710: 6e4d 6169 6e6b 6579 2c00 0000 7302 0000  nMainkey,...s...
-00000720: 0000 027a 0e45 6e63 2e67 656e 4d61 696e  ...z.Enc.genMain
-00000730: 6b65 7963 0100 0000 0000 0000 0000 0000  keyc............
-00000740: 0100 0000 0300 0000 4300 0000 730c 0000  ........C...s...
-00000750: 0074 00a0 017c 006a 02a1 0153 00a9 014e  .t...|.j...S...N
-00000760: 2903 7204 0000 00da 0343 4243 7228 0000  ).r......CBCr(..
-00000770: 00a9 0172 1100 0000 7214 0000 0072 1400  ...r....r....r..
-00000780: 0000 7215 0000 00da 046d 6f64 6530 0000  ..r......mode0..
-00000790: 0073 0200 0000 0001 7a08 456e 632e 6d6f  .s......z.Enc.mo
-000007a0: 6465 6301 0000 0000 0000 0000 0000 0001  dec.............
-000007b0: 0000 0005 0000 0043 0000 0073 1e00 0000  .......C...s....
-000007c0: 7400 7401 6a02 7c00 6a03 6401 8d01 7c00  t.t.j.|.j.d...|.
-000007d0: a004 a100 7405 8300 6402 8d03 5300 a903  ....t...d...S...
-000007e0: 4e29 01da 036b 6579 2902 723a 0000 005a  N)...key).r:...Z
-000007f0: 0762 6163 6b65 6e64 2906 7202 0000 0072  .backend).r....r
-00000800: 0300 0000 da03 4145 5372 2d00 0000 723a  ......AESr-...r:
-00000810: 0000 0072 0600 0000 7239 0000 0072 1400  ...r....r9...r..
-00000820: 0000 7214 0000 0072 1500 0000 da06 6369  ..r....r......ci
-00000830: 7068 6572 3300 0000 730e 0000 0000 0102  pher3...s.......
-00000840: 0104 0104 ff04 0206 0104 fc7a 0a45 6e63  ...........z.Enc
-00000850: 2e63 6970 6865 7263 0100 0000 0000 0000  .cipherc........
-00000860: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00000870: 730c 0000 007c 00a0 00a1 00a0 01a1 0053  s....|.........S
-00000880: 0072 3700 0000 2902 723e 0000 005a 0965  .r7...).r>...Z.e
-00000890: 6e63 7279 7074 6f72 7239 0000 0072 1400  ncryptorr9...r..
-000008a0: 0000 7214 0000 0072 1500 0000 da10 6369  ..r....r......ci
-000008b0: 7068 6572 5f65 6e63 7279 7074 6f72 3a00  pher_encryptor:.
-000008c0: 0000 7302 0000 0000 017a 1445 6e63 2e63  ..s......z.Enc.c
-000008d0: 6970 6865 725f 656e 6372 7970 746f 7263  ipher_encryptorc
-000008e0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-000008f0: 0300 0000 4300 0000 7322 0000 0074 00a0  ....C...s"...t..
-00000900: 0164 01a1 01a0 02a1 007d 017c 01a0 037c  .d.......}.|...|
-00000910: 006a 04a1 017c 01a0 05a1 0017 0053 00a9  .j...|.......S..
-00000920: 024e e980 0000 0029 0672 0500 0000 da05  .N.....).r......
-00000930: 504b 4353 37da 0670 6164 6465 72da 0675  PKCS7..padder..u
-00000940: 7064 6174 6572 1d00 0000 da08 6669 6e61  pdater......fina
-00000950: 6c69 7a65 2902 7211 0000 0072 4300 0000  lize).r....rC...
-00000960: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00000970: 0e70 6164 6465 645f 6d65 7373 6167 653d  .padded_message=
-00000980: 0000 0073 0400 0000 0001 0e01 7a12 456e  ...s........z.En
-00000990: 632e 7061 6464 6564 5f6d 6573 7361 6765  c.padded_message
-000009a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000009b0: 0004 0000 0043 0000 0073 1e00 0000 7c00  .....C...s....|.
-000009c0: a000 a100 a001 7c00 a002 a100 a101 7c00  ......|.......|.
-000009d0: a000 a100 a003 a100 1700 5300 7237 0000  ..........S.r7..
-000009e0: 0029 0472 3f00 0000 7244 0000 0072 4600  .).r?...rD...rF.
-000009f0: 0000 7245 0000 0072 3900 0000 7214 0000  ..rE...r9...r...
-00000a00: 0072 1400 0000 7215 0000 00da 0a63 6970  .r....r......cip
-00000a10: 6865 7274 6578 7441 0000 0073 0600 0000  hertextA...s....
-00000a20: 0001 1001 0aff 7a0e 456e 632e 6369 7068  ......z.Enc.ciph
-00000a30: 6572 7465 7874 6301 0000 0000 0000 0000  ertextc.........
-00000a40: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
-00000a50: 2c00 0000 7c00 6a00 7d01 7401 a002 7c01  ,...|.j.}.t...|.
-00000a60: 7403 a004 a100 a102 7d01 7c01 a005 7c00  t.......}.|...|.
-00000a70: a006 a100 a101 0100 7c01 a007 a100 5300  ........|.....S.
-00000a80: 7237 0000 0029 0872 2e00 0000 7208 0000  r7...).r....r...
-00000a90: 00da 0448 4d41 4372 0700 0000 da06 5348  ...HMACr......SH
-00000aa0: 4135 3132 7244 0000 0072 4700 0000 7245  A512rD...rG...rE
-00000ab0: 0000 00a9 0272 1100 0000 da01 6872 1400  .....r......hr..
-00000ac0: 0000 7214 0000 0072 1500 0000 7248 0000  ..r....r....rH..
-00000ad0: 0045 0000 0073 0800 0000 0001 0601 1001  .E...s..........
-00000ae0: 0e01 7a08 456e 632e 484d 4143 6301 0000  ..z.Enc.HMACc...
-00000af0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
-00000b00: 0043 0000 0073 1200 0000 7400 a001 6401  .C...s....t...d.
-00000b10: 7c00 6a02 a102 7d01 7c01 5300 2902 4efa  |.j...}.|.S.).N.
-00000b20: 0221 4929 03da 0673 7472 7563 74da 0470  .!I)...struct..p
-00000b30: 6163 6b72 2b00 0000 2902 7211 0000 005a  ackr+...).r....Z
-00000b40: 0b69 7465 7273 5f62 7974 6573 7214 0000  .iters_bytesr...
-00000b50: 0072 1400 0000 7215 0000 00da 0f73 6574  .r....r......set
-00000b60: 7570 4974 6572 6174 696f 6e73 4b00 0000  upIterationsK...
-00000b70: 7304 0000 0000 010e 017a 1345 6e63 2e73  s........z.Enc.s
-00000b80: 6574 7570 4974 6572 6174 696f 6e73 6301  etupIterationsc.
-00000b90: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000ba0: 0000 0043 0000 0073 2a00 0000 7c00 a000  ...C...s*...|...
-00000bb0: a100 7c00 6a01 1700 7c00 6a02 1700 7c00  ..|.j...|.j...|.
-00000bc0: 6a03 1700 7c00 a004 a100 1700 7c00 a005  j...|.......|...
-00000bd0: a100 1700 5300 7237 0000 0029 0672 4800  ....S.r7...).rH.
-00000be0: 0000 7228 0000 0072 2900 0000 722a 0000  ..r(...r)...r*..
-00000bf0: 0072 4f00 0000 7247 0000 0072 3900 0000  .rO...rG...r9...
-00000c00: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-00000c10: 0a65 6e63 546f 4279 7465 734f 0000 0073  .encToBytesO...s
-00000c20: 0a00 0000 0001 1801 06ff 0201 06ff 7a0e  ..............z.
-00000c30: 456e 632e 656e 6354 6f42 7974 6573 6301  Enc.encToBytesc.
-00000c40: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00000c50: 0000 0043 0000 0073 1400 0000 7400 a001  ...C...s....t...
-00000c60: 7c00 a002 a100 a101 a003 6401 a101 5300  |.........d...S.
-00000c70: a902 4e72 3000 0000 2904 da06 6261 7365  ..Nr0...)...base
-00000c80: 3634 5a11 7572 6c73 6166 655f 6236 3465  64Z.urlsafe_b64e
-00000c90: 6e63 6f64 6572 5000 0000 da06 6465 636f  ncoderP.....deco
-00000ca0: 6465 7239 0000 0072 1400 0000 7214 0000  der9...r....r...
-00000cb0: 0072 1500 0000 da08 656e 6354 6f53 7472  .r......encToStr
-00000cc0: 5300 0000 7302 0000 0000 017a 0c45 6e63  S...s......z.Enc
-00000cd0: 2e65 6e63 546f 5374 7229 1472 1600 0000  .encToStr).r....
-00000ce0: 7217 0000 0072 1800 0000 7209 0000 0072  r....r....r....r
-00000cf0: 2300 0000 7225 0000 0072 1000 0000 da0c  #...r%...r......
-00000d00: 7374 6174 6963 6d65 7468 6f64 da03 696e  staticmethod..in
-00000d10: 7472 2c00 0000 7236 0000 0072 3a00 0000  tr,...r6...r:...
-00000d20: 723e 0000 0072 3f00 0000 7246 0000 0072  r>...r?...rF...r
-00000d30: 4700 0000 7248 0000 0072 4f00 0000 7250  G...rH...rO...rP
-00000d40: 0000 0072 5400 0000 7214 0000 0072 1400  ...rT...r....r..
-00000d50: 0000 7214 0000 0072 1500 0000 721b 0000  ..r....r....r...
-00000d60: 0013 0000 0073 1c00 0000 0801 1a10 0201  .....s..........
-00000d70: 1607 0201 1003 0803 0807 0803 0e04 0e04  ................
-00000d80: 0e06 0e04 0e04 721b 0000 0063 0000 0000  ......r....c....
-00000d90: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000da0: 0000 0000 7322 0000 0065 005a 0164 005a  ....s"...e.Z.d.Z
-00000db0: 0264 0164 029c 0187 0066 0164 0364 0484  .d.d.....f.d.d..
-00000dc0: 0c5a 0387 0004 005a 0453 0029 05da 154d  .Z.....Z.S.)...M
-00000dd0: 6573 7361 6765 5461 6d70 6572 696e 6745  essageTamperingE
-00000de0: 7272 6f72 4e72 3400 0000 6301 0000 0000  rrorNr4...c.....
-00000df0: 0000 0000 0000 0001 0000 0003 0000 0003  ................
-00000e00: 0000 0073 1800 0000 6401 7c00 5f00 7401  ...s....d.|._.t.
-00000e10: 8300 a002 7c00 6a00 a101 0100 6400 5300  ....|.j.....d.S.
-00000e20: 2902 4e7a 4c48 4d41 4320 6d69 736d 6174  ).NzLHMAC mismat
-00000e30: 6368 2021 204d 6573 7361 6765 2068 6173  ch ! Message has
-00000e40: 2062 6565 6e20 5441 4d50 4552 4544 2077   been TAMPERED w
-00000e50: 6974 6820 2c0a 206f 7220 506f 7373 6962  ith ,. or Possib
-00000e60: 6c65 206b 6579 2064 6966 6665 7265 6e63  le key differenc
-00000e70: 6572 0e00 0000 7239 0000 0072 1200 0000  er....r9...r....
-00000e80: 7214 0000 0072 1500 0000 7210 0000 0058  r....r....r....X
-00000e90: 0000 0073 0400 0000 0001 0601 7a1e 4d65  ...s........z.Me
-00000ea0: 7373 6167 6554 616d 7065 7269 6e67 4572  ssageTamperingEr
-00000eb0: 726f 722e 5f5f 696e 6974 5f5f 2905 7216  ror.__init__).r.
-00000ec0: 0000 0072 1700 0000 7218 0000 0072 1000  ...r....r....r..
-00000ed0: 0000 721a 0000 0072 1400 0000 7214 0000  ..r....r....r...
-00000ee0: 0072 1200 0000 7215 0000 0072 5700 0000  .r....r....rW...
-00000ef0: 5700 0000 7302 0000 0008 0172 5700 0000  W...s......rW...
-00000f00: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000f10: 0004 0000 0040 0000 0073 9200 0000 6500  .....@...s....e.
-00000f20: 5a01 6400 5a02 6503 6504 6505 6602 1900  Z.d.Z.e.e.e.f...
-00000f30: 6504 6401 6402 9c03 6403 6404 8404 5a06  e.d.d...d.d...Z.
-00000f40: 6505 6405 9c01 6406 6407 8404 5a07 6508  e.d...d.d...Z.e.
-00000f50: 6405 9c01 6408 6409 8404 5a09 640a 640b  d...d.d...Z.d.d.
-00000f60: 8400 5a0a 640c 640d 8400 5a0b 640e 640f  ..Z.d.d...Z.d.d.
-00000f70: 8400 5a0c 6505 6405 9c01 6410 6411 8404  ..Z.e.d...d.d...
-00000f80: 5a0d 6505 6405 9c01 6412 6413 8404 5a0e  Z.e.d...d.d...Z.
-00000f90: 6505 6405 9c01 6414 6415 8404 5a0f 6504  e.d...d.d...Z.e.
-00000fa0: 6405 9c01 6416 6417 8404 5a10 6401 5300  d...d.d...Z.d.S.
-00000fb0: 2918 da03 4465 634e 721c 0000 0063 0300  )...DecNr....c..
-00000fc0: 0000 0000 0000 0000 0000 0400 0000 0600  ................
-00000fd0: 0000 4300 0000 7306 0100 0074 007c 0174  ..C...s....t.|.t
-00000fe0: 0183 0272 227c 01a0 0264 01a1 017d 0374  ...r"|...d...}.t
-00000ff0: 03a0 047c 03a1 017c 005f 056e 1074 007c  ...|...|._.n.t.|
-00001000: 0174 0683 0272 327c 017c 005f 057c 027c  .t...r2|.|._.|.|
-00001010: 005f 077c 006a 0564 0064 0285 0219 007c  ._.|.j.d.d.....|
-00001020: 005f 087c 006a 0564 0264 0385 0219 007c  ._.|.j.d.d.....|
-00001030: 005f 097c 006a 0564 0364 0485 0219 007c  ._.|.j.d.d.....|
-00001040: 005f 0a7c 006a 0564 0464 0585 0219 007c  ._.|.j.d.d.....|
-00001050: 005f 0b74 0ca0 0d64 067c 006a 0564 0564  ._.t...d.|.j.d.d
-00001060: 0785 0219 00a1 0264 0819 007c 005f 0e7c  .......d...|._.|
-00001070: 006a 0e64 096b 0073 a87c 006a 0e64 0a6b  .j.d.k.s.|.j.d.k
-00001080: 0472 b274 0f7c 006a 0e83 0182 017c 006a  .r.t.|.j.....|.j
-00001090: 0564 0764 0085 0219 007c 005f 1074 11a0  .d.d.....|._.t..
-000010a0: 127c 006a 077c 006a 0a7c 006a 0ea1 037c  .|.j.|.j.|.j...|
-000010b0: 005f 1374 11a0 127c 006a 077c 006a 0b7c  ._.t...|.j.|.j.|
-000010c0: 006a 0ea1 037c 005f 147c 00a0 15a1 0064  .j...|._.|.....d
-000010d0: 0b75 0090 0172 0274 1683 0082 0164 0053  .u...r.t.....d.S
-000010e0: 0029 0c4e 7230 0000 00e9 4000 0000 e950  .).Nr0....@....P
-000010f0: 0000 00e9 6000 0000 e970 0000 0072 4c00  ....`....p...rL.
-00001100: 0000 e974 0000 0072 0100 0000 7220 0000  ...t...r....r ..
-00001110: 0072 2100 0000 4629 1772 2200 0000 7223  .r!...F).r"...r#
-00001120: 0000 0072 2400 0000 7252 0000 005a 1175  ...r$...rR...Z.u
-00001130: 726c 7361 6665 5f62 3634 6465 636f 6465  rlsafe_b64decode
-00001140: 721d 0000 0072 2500 0000 723c 0000 00da  r....r%...r<....
-00001150: 0872 6563 5f68 6d61 63da 0672 6563 5f69  .rec_hmac..rec_i
-00001160: 76da 0872 6563 5f73 616c 74da 0a72 6563  v..rec_salt..rec
-00001170: 5f70 6570 7065 7272 4d00 0000 da06 756e  _pepperrM.....un
-00001180: 7061 636b da0e 7265 635f 6974 6572 6174  pack..rec_iterat
-00001190: 696f 6e73 720a 0000 00da 0e72 6563 5f63  ionsr......rec_c
-000011a0: 6970 6865 7274 6578 7472 1b00 0000 722c  iphertextr....r,
-000011b0: 0000 00da 0664 6563 4b65 79da 0668 6d61  .....decKey..hma
-000011c0: 635f 6bda 0a76 6572 6966 7948 4d41 4372  c_k..verifyHMACr
-000011d0: 5700 0000 2904 7211 0000 0072 1d00 0000  W...).r....r....
-000011e0: 721e 0000 00da 016d 7214 0000 0072 1400  r......mr....r..
-000011f0: 0000 7215 0000 0072 1000 0000 5e00 0000  ..r....r....^...
-00001200: 732c 0000 0000 010a 010a 010e 010a 0106  s,..............
-00001210: 0106 0110 0110 0110 0110 011c 0114 010a  ................
-00001220: 0110 0116 0104 0104 0104 0104 fd06 040e  ................
-00001230: 017a 0c44 6563 2e5f 5f69 6e69 745f 5f72  .z.Dec.__init__r
-00001240: 3400 0000 6301 0000 0000 0000 0000 0000  4...c...........
-00001250: 0002 0000 0005 0000 0043 0000 0073 2a00  .........C...s*.
-00001260: 0000 7c00 6a00 7d01 7401 a002 7c01 7403  ..|.j.}.t...|.t.
-00001270: a004 a100 a102 7d01 7c01 a005 7c00 6a06  ......}.|...|.j.
-00001280: a101 0100 7c01 a007 a100 5300 7237 0000  ....|.....S.r7..
-00001290: 0029 0872 6600 0000 7208 0000 0072 4800  .).rf...r....rH.
-000012a0: 0000 7207 0000 0072 4900 0000 7244 0000  ..r....rI...rD..
-000012b0: 0072 6400 0000 7245 0000 0072 4a00 0000  .rd...rE...rJ...
-000012c0: 7214 0000 0072 1400 0000 7215 0000 00da  r....r....r.....
-000012d0: 0a61 6374 7561 6c48 4d41 4375 0000 0073  .actualHMACu...s
-000012e0: 0800 0000 0001 0601 1001 0c01 7a0e 4465  ............z.De
-000012f0: 632e 6163 7475 616c 484d 4143 6301 0000  c.actualHMACc...
-00001300: 0000 0000 0000 0000 0001 0000 0004 0000  ................
-00001310: 0043 0000 0073 1200 0000 7400 a001 7c00  .C...s....t...|.
-00001320: a002 a100 7c00 6a03 a102 5300 7237 0000  ....|.j...S.r7..
-00001330: 0029 04da 0368 6d63 5a0e 636f 6d70 6172  .)...hmcZ.compar
-00001340: 655f 6469 6765 7374 7269 0000 0072 5e00  e_digestri...r^.
-00001350: 0000 7239 0000 0072 1400 0000 7214 0000  ..r9...r....r...
-00001360: 0072 1500 0000 7267 0000 007b 0000 0073  .r....rg...{...s
-00001370: 0200 0000 0001 7a0e 4465 632e 7665 7269  ......z.Dec.veri
-00001380: 6679 484d 4143 6301 0000 0000 0000 0000  fyHMACc.........
-00001390: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
-000013a0: 0c00 0000 7400 a001 7c00 6a02 a101 5300  ....t...|.j...S.
-000013b0: 7237 0000 0029 0372 0400 0000 7238 0000  r7...).r....r8..
-000013c0: 0072 5f00 0000 7239 0000 0072 1400 0000  .r_...r9...r....
-000013d0: 7214 0000 0072 1500 0000 723a 0000 007e  r....r....r:...~
-000013e0: 0000 0073 0200 0000 0001 7a08 4465 632e  ...s......z.Dec.
-000013f0: 6d6f 6465 6301 0000 0000 0000 0000 0000  modec...........
-00001400: 0001 0000 0005 0000 0043 0000 0073 1e00  .........C...s..
-00001410: 0000 7400 7401 6a02 7c00 6a03 6401 8d01  ..t.t.j.|.j.d...
-00001420: 7c00 a004 a100 7405 8300 6402 8d03 5300  |.....t...d...S.
-00001430: 723b 0000 0029 0672 0200 0000 7203 0000  r;...).r....r...
-00001440: 0072 3d00 0000 7265 0000 0072 3a00 0000  .r=...re...r:...
-00001450: 7206 0000 0072 3900 0000 7214 0000 0072  r....r9...r....r
-00001460: 1400 0000 7215 0000 0072 3e00 0000 8100  ....r....r>.....
-00001470: 0000 730e 0000 0000 0102 0104 0104 ff04  ..s.............
-00001480: 0206 0104 fc7a 0a44 6563 2e63 6970 6865  .....z.Dec.ciphe
-00001490: 7263 0100 0000 0000 0000 0000 0000 0100  rc..............
-000014a0: 0000 0200 0000 4300 0000 730c 0000 007c  ......C...s....|
-000014b0: 00a0 00a1 00a0 01a1 0053 0072 3700 0000  .........S.r7...
-000014c0: 2902 723e 0000 005a 0964 6563 7279 7074  ).r>...Z.decrypt
-000014d0: 6f72 7239 0000 0072 1400 0000 7214 0000  orr9...r....r...
-000014e0: 0072 1500 0000 da10 6369 7068 6572 5f64  .r......cipher_d
-000014f0: 6563 7279 7074 6f72 8800 0000 7302 0000  ecryptor....s...
-00001500: 0000 017a 1444 6563 2e63 6970 6865 725f  ...z.Dec.cipher_
-00001510: 6465 6372 7970 746f 7263 0100 0000 0000  decryptorc......
-00001520: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001530: 0000 731c 0000 007c 00a0 00a1 00a0 017c  ..s....|.......|
-00001540: 006a 02a1 017c 00a0 00a1 00a0 03a1 0017  .j...|..........
-00001550: 0053 0072 3700 0000 2904 726b 0000 0072  .S.r7...).rk...r
-00001560: 4400 0000 7264 0000 0072 4500 0000 7239  D...rd...rE...r9
-00001570: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00001580: 0000 da11 7072 655f 756e 7061 6464 696e  ....pre_unpaddin
-00001590: 675f 6465 638b 0000 0073 0600 0000 0001  g_dec....s......
-000015a0: 0e01 0aff 7a15 4465 632e 7072 655f 756e  ....z.Dec.pre_un
-000015b0: 7061 6464 696e 675f 6465 6363 0100 0000  padding_decc....
-000015c0: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-000015d0: 4300 0000 7324 0000 0074 00a0 0164 01a1  C...s$...t...d..
-000015e0: 01a0 02a1 007d 017c 01a0 037c 00a0 04a1  .....}.|...|....
-000015f0: 00a1 017c 01a0 05a1 0017 0053 0072 4000  ...|.......S.r@.
-00001600: 0000 2906 7205 0000 0072 4200 0000 da08  ..).r....rB.....
-00001610: 756e 7061 6464 6572 7244 0000 0072 6c00  unpadderrD...rl.
-00001620: 0000 7245 0000 0029 0272 1100 0000 726d  ..rE...).r....rm
-00001630: 0000 0072 1400 0000 7214 0000 0072 1500  ...r....r....r..
-00001640: 0000 da0a 756e 7061 6464 6564 5f6d 8f00  ....unpadded_m..
-00001650: 0000 7304 0000 0000 010e 017a 0e44 6563  ..s........z.Dec
-00001660: 2e75 6e70 6164 6465 645f 6d63 0100 0000  .unpadded_mc....
-00001670: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00001680: 4300 0000 7308 0000 007c 00a0 00a1 0053  C...s....|.....S
-00001690: 0072 3700 0000 2901 726e 0000 0072 3900  .r7...).rn...r9.
-000016a0: 0000 7214 0000 0072 1400 0000 7215 0000  ..r....r....r...
-000016b0: 00da 0a64 6563 546f 4279 7465 7393 0000  ...decToBytes...
-000016c0: 0073 0200 0000 0001 7a0e 4465 632e 6465  .s......z.Dec.de
-000016d0: 6354 6f42 7974 6573 6301 0000 0000 0000  cToBytesc.......
-000016e0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-000016f0: 0073 0e00 0000 7c00 a000 a100 a001 6401  .s....|.......d.
-00001700: a101 5300 7251 0000 0029 0272 6e00 0000  ..S.rQ...).rn...
-00001710: 7253 0000 0072 3900 0000 7214 0000 0072  rS...r9...r....r
-00001720: 1400 0000 7215 0000 00da 0864 6563 546f  ....r......decTo
-00001730: 5374 7296 0000 0073 0200 0000 0001 7a0c  Str....s......z.
-00001740: 4465 632e 6465 6354 6f53 7472 2911 7216  Dec.decToStr).r.
-00001750: 0000 0072 1700 0000 7218 0000 0072 0900  ...r....r....r..
-00001760: 0000 7223 0000 0072 2500 0000 7210 0000  ..r#...r%...r...
-00001770: 0072 6900 0000 da04 626f 6f6c 7267 0000  .ri.....boolrg..
-00001780: 0072 3a00 0000 723e 0000 0072 6b00 0000  .r:...r>...rk...
-00001790: 726c 0000 0072 6e00 0000 726f 0000 0072  rl...rn...ro...r
-000017a0: 7000 0000 7214 0000 0072 1400 0000 7214  p...r....r....r.
-000017b0: 0000 0072 1500 0000 7258 0000 005d 0000  ...r....rX...]..
-000017c0: 0073 1400 0000 0801 1a17 0e06 0e03 0803  .s..............
-000017d0: 0807 0803 0e04 0e04 0e03 7258 0000 0029  ..........rX...)
-000017e0: 165a 2663 7279 7074 6f67 7261 7068 792e  .Z&cryptography.
-000017f0: 6861 7a6d 6174 2e70 7269 6d69 7469 7665  hazmat.primitive
-00001800: 732e 6369 7068 6572 7372 0200 0000 7203  s.ciphersr....r.
-00001810: 0000 0072 0400 0000 5a1e 6372 7970 746f  ...r....Z.crypto
-00001820: 6772 6170 6879 2e68 617a 6d61 742e 7072  graphy.hazmat.pr
-00001830: 696d 6974 6976 6573 7205 0000 005a 1c63  imitivesr....Z.c
-00001840: 7279 7074 6f67 7261 7068 792e 6861 7a6d  ryptography.hazm
-00001850: 6174 2e62 6163 6b65 6e64 7372 0600 0000  at.backendsr....
-00001860: 7207 0000 0072 0800 0000 da06 7479 7069  r....r......typi
-00001870: 6e67 7209 0000 0072 6a00 0000 7233 0000  ngr....rj...r3..
-00001880: 0072 5200 0000 724d 0000 0072 2600 0000  .rR...rM...r&...
-00001890: da09 4578 6365 7074 696f 6e72 0a00 0000  ..Exceptionr....
-000018a0: 721b 0000 0072 5700 0000 7258 0000 0072  r....rW...rX...r
-000018b0: 1400 0000 7214 0000 0072 1400 0000 7215  ....r....r....r.
-000018c0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-000018d0: 0073 1a00 0000 1401 0c01 0c01 1001 0c01  .s..............
-000018e0: 0801 0801 0801 0801 0803 1006 0e44 1006  .............D..
+000006e0: 024e 7232 0000 0029 0372 2700 0000 7228  .Nr2...).r'...r(
+000006f0: 0000 00da 0368 6578 7215 0000 0072 1500  .....hexr....r..
+00000700: 0000 7215 0000 0072 1600 0000 da06 6765  ..r....r......ge
+00000710: 6e6b 6579 2c00 0000 7302 0000 0000 027a  nkey,...s......z
+00000720: 0a45 6e63 2e67 656e 6b65 7963 0100 0000  .Enc.genkeyc....
+00000730: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000740: 4300 0000 730c 0000 0074 00a0 017c 006a  C...s....t...|.j
+00000750: 02a1 0153 00a9 014e 2903 7204 0000 00da  ...S...N).r.....
+00000760: 0343 4243 7229 0000 00a9 0172 1200 0000  .CBCr).....r....
+00000770: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00000780: 046d 6f64 6530 0000 0073 0200 0000 0001  .mode0...s......
+00000790: 7a08 456e 632e 6d6f 6465 6301 0000 0000  z.Enc.modec.....
+000007a0: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
+000007b0: 0000 0073 1e00 0000 7400 7401 6a02 7c00  ...s....t.t.j.|.
+000007c0: 6a03 6401 8d01 7c00 a004 a100 7405 8300  j.d...|.....t...
+000007d0: 6402 8d03 5300 a903 4e29 01da 036b 6579  d...S...N)...key
+000007e0: 2902 723b 0000 005a 0762 6163 6b65 6e64  ).r;...Z.backend
+000007f0: 2906 7202 0000 0072 0300 0000 da03 4145  ).r....r......AE
+00000800: 5372 2e00 0000 723b 0000 0072 0600 0000  Sr....r;...r....
+00000810: 723a 0000 0072 1500 0000 7215 0000 0072  r:...r....r....r
+00000820: 1600 0000 da06 6369 7068 6572 3300 0000  ......cipher3...
+00000830: 730e 0000 0000 0102 0104 0104 ff04 0206  s...............
+00000840: 0104 fc7a 0a45 6e63 2e63 6970 6865 7263  ...z.Enc.cipherc
+00000850: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000860: 0200 0000 4300 0000 730c 0000 007c 00a0  ....C...s....|..
+00000870: 00a1 00a0 01a1 0053 0072 3800 0000 2902  .......S.r8...).
+00000880: 723f 0000 005a 0965 6e63 7279 7074 6f72  r?...Z.encryptor
+00000890: 723a 0000 0072 1500 0000 7215 0000 0072  r:...r....r....r
+000008a0: 1600 0000 da10 6369 7068 6572 5f65 6e63  ......cipher_enc
+000008b0: 7279 7074 6f72 3a00 0000 7302 0000 0000  ryptor:...s.....
+000008c0: 017a 1445 6e63 2e63 6970 6865 725f 656e  .z.Enc.cipher_en
+000008d0: 6372 7970 746f 7263 0100 0000 0000 0000  cryptorc........
+000008e0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+000008f0: 7322 0000 0074 00a0 0164 01a1 01a0 02a1  s"...t...d......
+00000900: 007d 017c 01a0 037c 006a 04a1 017c 01a0  .}.|...|.j...|..
+00000910: 05a1 0017 0053 00a9 024e e980 0000 0029  .....S...N.....)
+00000920: 0672 0500 0000 da05 504b 4353 37da 0670  .r......PKCS7..p
+00000930: 6164 6465 72da 0675 7064 6174 6572 1e00  adder..updater..
+00000940: 0000 da08 6669 6e61 6c69 7a65 2902 7212  ....finalize).r.
+00000950: 0000 0072 4400 0000 7215 0000 0072 1500  ...rD...r....r..
+00000960: 0000 7216 0000 00da 0e70 6164 6465 645f  ..r......padded_
+00000970: 6d65 7373 6167 653d 0000 0073 0400 0000  message=...s....
+00000980: 0001 0e01 7a12 456e 632e 7061 6464 6564  ....z.Enc.padded
+00000990: 5f6d 6573 7361 6765 6301 0000 0000 0000  _messagec.......
+000009a0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+000009b0: 0073 1e00 0000 7c00 a000 a100 a001 7c00  .s....|.......|.
+000009c0: a002 a100 a101 7c00 a000 a100 a003 a100  ......|.........
+000009d0: 1700 5300 7238 0000 0029 0472 4000 0000  ..S.r8...).r@...
+000009e0: 7245 0000 0072 4700 0000 7246 0000 0072  rE...rG...rF...r
+000009f0: 3a00 0000 7215 0000 0072 1500 0000 7216  :...r....r....r.
+00000a00: 0000 00da 0a63 6970 6865 7274 6578 7441  .....ciphertextA
+00000a10: 0000 0073 0600 0000 0001 1001 0aff 7a0e  ...s..........z.
+00000a20: 456e 632e 6369 7068 6572 7465 7874 6301  Enc.ciphertextc.
+00000a30: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00000a40: 0000 0043 0000 0073 2c00 0000 7c00 6a00  ...C...s,...|.j.
+00000a50: 7d01 7401 a002 7c01 7403 a004 a100 a102  }.t...|.t.......
+00000a60: 7d01 7c01 a005 7c00 a006 a100 a101 0100  }.|...|.........
+00000a70: 7c01 a007 a100 5300 7238 0000 0029 0872  |.....S.r8...).r
+00000a80: 2f00 0000 7208 0000 00da 0448 4d41 4372  /...r......HMACr
+00000a90: 0700 0000 da06 5348 4135 3132 7245 0000  ......SHA512rE..
+00000aa0: 0072 4800 0000 7246 0000 00a9 0272 1200  .rH...rF.....r..
+00000ab0: 0000 da01 6872 1500 0000 7215 0000 0072  ....hr....r....r
+00000ac0: 1600 0000 7249 0000 0045 0000 0073 0800  ....rI...E...s..
+00000ad0: 0000 0001 0601 1001 0e01 7a08 456e 632e  ..........z.Enc.
+00000ae0: 484d 4143 6301 0000 0000 0000 0000 0000  HMACc...........
+00000af0: 0002 0000 0004 0000 0043 0000 0073 1200  .........C...s..
+00000b00: 0000 7400 a001 6401 7c00 6a02 a102 7d01  ..t...d.|.j...}.
+00000b10: 7c01 5300 2902 4efa 0221 4929 03da 0673  |.S.).N..!I)...s
+00000b20: 7472 7563 745a 0470 6163 6b72 2c00 0000  tructZ.packr,...
+00000b30: 2902 7212 0000 005a 0b69 7465 7273 5f62  ).r....Z.iters_b
+00000b40: 7974 6573 7215 0000 0072 1500 0000 7216  ytesr....r....r.
+00000b50: 0000 00da 1073 6574 7570 5f69 7465 7261  .....setup_itera
+00000b60: 7469 6f6e 734b 0000 0073 0400 0000 0001  tionsK...s......
+00000b70: 0e01 7a14 456e 632e 7365 7475 705f 6974  ..z.Enc.setup_it
+00000b80: 6572 6174 696f 6e73 6301 0000 0000 0000  erationsc.......
+00000b90: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00000ba0: 0073 2a00 0000 7c00 a000 a100 7c00 6a01  .s*...|.....|.j.
+00000bb0: 1700 7c00 6a02 1700 7c00 6a03 1700 7c00  ..|.j...|.j...|.
+00000bc0: a004 a100 1700 7c00 a005 a100 1700 5300  ......|.......S.
+00000bd0: 7238 0000 0029 0672 4900 0000 7229 0000  r8...).rI...r)..
+00000be0: 0072 2a00 0000 722b 0000 0072 4f00 0000  .r*...r+...rO...
+00000bf0: 7248 0000 0072 3a00 0000 7215 0000 0072  rH...r:...r....r
+00000c00: 1500 0000 7216 0000 00da 0c65 6e63 5f74  ....r......enc_t
+00000c10: 6f5f 6279 7465 734f 0000 0073 0a00 0000  o_bytesO...s....
+00000c20: 0001 1801 06ff 0201 06ff 7a10 456e 632e  ..........z.Enc.
+00000c30: 656e 635f 746f 5f62 7974 6573 6301 0000  enc_to_bytesc...
+00000c40: 0000 0000 0000 0000 0001 0000 0004 0000  ................
+00000c50: 0043 0000 0073 1400 0000 7400 a001 7c00  .C...s....t...|.
+00000c60: a002 a100 a101 a003 6401 a101 5300 a902  ........d...S...
+00000c70: 4e72 3100 0000 2904 da06 6261 7365 3634  Nr1...)...base64
+00000c80: 5a11 7572 6c73 6166 655f 6236 3465 6e63  Z.urlsafe_b64enc
+00000c90: 6f64 6572 5000 0000 da06 6465 636f 6465  oderP.....decode
+00000ca0: 723a 0000 0072 1500 0000 7215 0000 0072  r:...r....r....r
+00000cb0: 1600 0000 da0a 656e 635f 746f 5f73 7472  ......enc_to_str
+00000cc0: 5300 0000 7302 0000 0000 017a 0e45 6e63  S...s......z.Enc
+00000cd0: 2e65 6e63 5f74 6f5f 7374 7229 1472 1700  .enc_to_str).r..
+00000ce0: 0000 7218 0000 0072 1900 0000 7209 0000  ..r....r....r...
+00000cf0: 0072 2400 0000 7226 0000 0072 1100 0000  .r$...r&...r....
+00000d00: da0c 7374 6174 6963 6d65 7468 6f64 da03  ..staticmethod..
+00000d10: 696e 7472 2d00 0000 7237 0000 0072 3b00  intr-...r7...r;.
+00000d20: 0000 723f 0000 0072 4000 0000 7247 0000  ..r?...r@...rG..
+00000d30: 0072 4800 0000 7249 0000 0072 4f00 0000  .rH...rI...rO...
+00000d40: 7250 0000 0072 5400 0000 7215 0000 0072  rP...rT...r....r
+00000d50: 1500 0000 7215 0000 0072 1600 0000 721c  ....r....r....r.
+00000d60: 0000 0013 0000 0073 1c00 0000 0801 1a10  .......s........
+00000d70: 0201 1607 0201 1003 0803 0807 0803 0e04  ................
+00000d80: 0e04 0e06 0e04 0e04 721c 0000 0063 0000  ........r....c..
+00000d90: 0000 0000 0000 0000 0000 0000 0000 0400  ................
+00000da0: 0000 0000 0000 7322 0000 0065 005a 0164  ......s"...e.Z.d
+00000db0: 005a 0264 0164 029c 0187 0066 0164 0364  .Z.d.d.....f.d.d
+00000dc0: 0484 0c5a 0387 0004 005a 0453 0029 05da  ...Z.....Z.S.)..
+00000dd0: 154d 6573 7361 6765 5461 6d70 6572 696e  .MessageTamperin
+00000de0: 6745 7272 6f72 4e72 3500 0000 6301 0000  gErrorNr5...c...
+00000df0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000e00: 0003 0000 0073 1800 0000 6401 7c00 5f00  .....s....d.|._.
+00000e10: 7401 8300 a002 7c00 6a00 a101 0100 6400  t.....|.j.....d.
+00000e20: 5300 2902 4e7a 4c48 4d41 4320 6d69 736d  S.).NzLHMAC mism
+00000e30: 6174 6368 2021 204d 6573 7361 6765 2068  atch ! Message h
+00000e40: 6173 2062 6565 6e20 5441 4d50 4552 4544  as been TAMPERED
+00000e50: 2077 6974 6820 2c0a 206f 7220 506f 7373   with ,. or Poss
+00000e60: 6962 6c65 206b 6579 2064 6966 6665 7265  ible key differe
+00000e70: 6e63 6572 0e00 0000 723a 0000 0072 1300  ncer....r:...r..
+00000e80: 0000 7215 0000 0072 1600 0000 7211 0000  ..r....r....r...
+00000e90: 0058 0000 0073 0400 0000 0001 0601 7a1e  .X...s........z.
+00000ea0: 4d65 7373 6167 6554 616d 7065 7269 6e67  MessageTampering
+00000eb0: 4572 726f 722e 5f5f 696e 6974 5f5f 2905  Error.__init__).
+00000ec0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+00000ed0: 1100 0000 721b 0000 0072 1500 0000 7215  ....r....r....r.
+00000ee0: 0000 0072 1300 0000 7216 0000 0072 5700  ...r....r....rW.
+00000ef0: 0000 5700 0000 7302 0000 0008 0172 5700  ..W...s......rW.
+00000f00: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00000f10: 0000 0004 0000 0040 0000 0073 9200 0000  .......@...s....
+00000f20: 6500 5a01 6400 5a02 6503 6504 6505 6602  e.Z.d.Z.e.e.e.f.
+00000f30: 1900 6504 6401 6402 9c03 6403 6404 8404  ..e.d.d...d.d...
+00000f40: 5a06 6505 6405 9c01 6406 6407 8404 5a07  Z.e.d...d.d...Z.
+00000f50: 6508 6405 9c01 6408 6409 8404 5a09 640a  e.d...d.d...Z.d.
+00000f60: 640b 8400 5a0a 640c 640d 8400 5a0b 640e  d...Z.d.d...Z.d.
+00000f70: 640f 8400 5a0c 6505 6405 9c01 6410 6411  d...Z.e.d...d.d.
+00000f80: 8404 5a0d 6505 6405 9c01 6412 6413 8404  ..Z.e.d...d.d...
+00000f90: 5a0e 6505 6405 9c01 6414 6415 8404 5a0f  Z.e.d...d.d...Z.
+00000fa0: 6504 6405 9c01 6416 6417 8404 5a10 6401  e.d...d.d...Z.d.
+00000fb0: 5300 2918 da03 4465 634e 721d 0000 0063  S.)...DecNr....c
+00000fc0: 0300 0000 0000 0000 0000 0000 0400 0000  ................
+00000fd0: 0600 0000 4300 0000 7306 0100 0074 007c  ....C...s....t.|
+00000fe0: 0174 0183 0272 227c 01a0 0264 01a1 017d  .t...r"|...d...}
+00000ff0: 0374 03a0 047c 03a1 017c 005f 056e 1074  .t...|...|._.n.t
+00001000: 007c 0174 0683 0272 327c 017c 005f 057c  .|.t...r2|.|._.|
+00001010: 027c 005f 077c 006a 0564 0064 0285 0219  .|._.|.j.d.d....
+00001020: 007c 005f 087c 006a 0564 0264 0385 0219  .|._.|.j.d.d....
+00001030: 007c 005f 097c 006a 0564 0364 0485 0219  .|._.|.j.d.d....
+00001040: 007c 005f 0a7c 006a 0564 0464 0585 0219  .|._.|.j.d.d....
+00001050: 007c 005f 0b74 0ca0 0d64 067c 006a 0564  .|._.t...d.|.j.d
+00001060: 0564 0785 0219 00a1 0264 0819 007c 005f  .d.......d...|._
+00001070: 0e7c 006a 0e64 096b 0073 a87c 006a 0e64  .|.j.d.k.s.|.j.d
+00001080: 0a6b 0472 b274 0f7c 006a 0e83 0182 017c  .k.r.t.|.j.....|
+00001090: 006a 0564 0764 0085 0219 007c 005f 1074  .j.d.d.....|._.t
+000010a0: 11a0 127c 006a 077c 006a 0a7c 006a 0ea1  ...|.j.|.j.|.j..
+000010b0: 037c 005f 1374 11a0 127c 006a 077c 006a  .|._.t...|.j.|.j
+000010c0: 0b7c 006a 0ea1 037c 005f 147c 00a0 15a1  .|.j...|._.|....
+000010d0: 0064 0b75 0090 0172 0274 1683 0082 0164  .d.u...r.t.....d
+000010e0: 0053 0029 0c4e 7231 0000 00e9 4000 0000  .S.).Nr1....@...
+000010f0: e950 0000 00e9 6000 0000 e970 0000 0072  .P....`....p...r
+00001100: 4d00 0000 e974 0000 0072 0100 0000 7221  M....t...r....r!
+00001110: 0000 0072 2200 0000 4629 1772 2300 0000  ...r"...F).r#...
+00001120: 7224 0000 0072 2500 0000 7252 0000 005a  r$...r%...rR...Z
+00001130: 1175 726c 7361 6665 5f62 3634 6465 636f  .urlsafe_b64deco
+00001140: 6465 721e 0000 0072 2600 0000 723d 0000  der....r&...r=..
+00001150: 00da 0872 6563 5f68 6d61 63da 0672 6563  ...rec_hmac..rec
+00001160: 5f69 765a 0872 6563 5f73 616c 745a 0a72  _ivZ.rec_saltZ.r
+00001170: 6563 5f70 6570 7065 7272 4e00 0000 5a06  ec_pepperrN...Z.
+00001180: 756e 7061 636b 5a0e 7265 635f 6974 6572  unpackZ.rec_iter
+00001190: 6174 696f 6e73 720a 0000 00da 0e72 6563  ationsr......rec
+000011a0: 5f63 6970 6865 7274 6578 7472 1c00 0000  _ciphertextr....
+000011b0: 722d 0000 00da 0664 6563 4b65 79da 0668  r-.....decKey..h
+000011c0: 6d61 635f 6bda 0a76 6572 6966 7948 4d41  mac_k..verifyHMA
+000011d0: 4372 5700 0000 2904 7212 0000 0072 1e00  CrW...).r....r..
+000011e0: 0000 721f 0000 00da 016d 7215 0000 0072  ..r......mr....r
+000011f0: 1500 0000 7216 0000 0072 1100 0000 5e00  ....r....r....^.
+00001200: 0000 732c 0000 0000 010a 010a 010e 010a  ..s,............
+00001210: 0106 0106 0110 0110 0110 0110 011c 0114  ................
+00001220: 010a 0110 0116 0104 0104 0104 0104 fd06  ................
+00001230: 040e 017a 0c44 6563 2e5f 5f69 6e69 745f  ...z.Dec.__init_
+00001240: 5f72 3500 0000 6301 0000 0000 0000 0000  _r5...c.........
+00001250: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+00001260: 2a00 0000 7c00 6a00 7d01 7401 a002 7c01  *...|.j.}.t...|.
+00001270: 7403 a004 a100 a102 7d01 7c01 a005 7c00  t.......}.|...|.
+00001280: 6a06 a101 0100 7c01 a007 a100 5300 7238  j.....|.....S.r8
+00001290: 0000 0029 0872 6200 0000 7208 0000 0072  ...).rb...r....r
+000012a0: 4900 0000 7207 0000 0072 4a00 0000 7245  I...r....rJ...rE
+000012b0: 0000 0072 6000 0000 7246 0000 0072 4b00  ...r`...rF...rK.
+000012c0: 0000 7215 0000 0072 1500 0000 7216 0000  ..r....r....r...
+000012d0: 00da 0a61 6374 7561 6c48 4d41 4375 0000  ...actualHMACu..
+000012e0: 0073 0800 0000 0001 0601 1001 0c01 7a0e  .s............z.
+000012f0: 4465 632e 6163 7475 616c 484d 4143 6301  Dec.actualHMACc.
+00001300: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00001310: 0000 0043 0000 0073 1200 0000 7400 a001  ...C...s....t...
+00001320: 7c00 a002 a100 7c00 6a03 a102 5300 7238  |.....|.j...S.r8
+00001330: 0000 0029 04da 0368 6d63 5a0e 636f 6d70  ...)...hmcZ.comp
+00001340: 6172 655f 6469 6765 7374 7265 0000 0072  are_digestre...r
+00001350: 5e00 0000 723a 0000 0072 1500 0000 7215  ^...r:...r....r.
+00001360: 0000 0072 1600 0000 7263 0000 007b 0000  ...r....rc...{..
+00001370: 0073 0200 0000 0001 7a0e 4465 632e 7665  .s......z.Dec.ve
+00001380: 7269 6679 484d 4143 6301 0000 0000 0000  rifyHMACc.......
+00001390: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+000013a0: 0073 0c00 0000 7400 a001 7c00 6a02 a101  .s....t...|.j...
+000013b0: 5300 7238 0000 0029 0372 0400 0000 7239  S.r8...).r....r9
+000013c0: 0000 0072 5f00 0000 723a 0000 0072 1500  ...r_...r:...r..
+000013d0: 0000 7215 0000 0072 1600 0000 723b 0000  ..r....r....r;..
+000013e0: 007e 0000 0073 0200 0000 0001 7a08 4465  .~...s......z.De
+000013f0: 632e 6d6f 6465 6301 0000 0000 0000 0000  c.modec.........
+00001400: 0000 0001 0000 0005 0000 0043 0000 0073  ...........C...s
+00001410: 1e00 0000 7400 7401 6a02 7c00 6a03 6401  ....t.t.j.|.j.d.
+00001420: 8d01 7c00 a004 a100 7405 8300 6402 8d03  ..|.....t...d...
+00001430: 5300 723c 0000 0029 0672 0200 0000 7203  S.r<...).r....r.
+00001440: 0000 0072 3e00 0000 7261 0000 0072 3b00  ...r>...ra...r;.
+00001450: 0000 7206 0000 0072 3a00 0000 7215 0000  ..r....r:...r...
+00001460: 0072 1500 0000 7216 0000 0072 3f00 0000  .r....r....r?...
+00001470: 8100 0000 730e 0000 0000 0102 0104 0104  ....s...........
+00001480: ff04 0206 0104 fc7a 0a44 6563 2e63 6970  .......z.Dec.cip
+00001490: 6865 7263 0100 0000 0000 0000 0000 0000  herc............
+000014a0: 0100 0000 0200 0000 4300 0000 730c 0000  ........C...s...
+000014b0: 007c 00a0 00a1 00a0 01a1 0053 0072 3800  .|.........S.r8.
+000014c0: 0000 2902 723f 0000 005a 0964 6563 7279  ..).r?...Z.decry
+000014d0: 7074 6f72 723a 0000 0072 1500 0000 7215  ptorr:...r....r.
+000014e0: 0000 0072 1600 0000 da10 6369 7068 6572  ...r......cipher
+000014f0: 5f64 6563 7279 7074 6f72 8800 0000 7302  _decryptor....s.
+00001500: 0000 0000 017a 1444 6563 2e63 6970 6865  .....z.Dec.ciphe
+00001510: 725f 6465 6372 7970 746f 7263 0100 0000  r_decryptorc....
+00001520: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001530: 4300 0000 731c 0000 007c 00a0 00a1 00a0  C...s....|......
+00001540: 017c 006a 02a1 017c 00a0 00a1 00a0 03a1  .|.j...|........
+00001550: 0017 0053 0072 3800 0000 2904 7267 0000  ...S.r8...).rg..
+00001560: 0072 4500 0000 7260 0000 0072 4600 0000  .rE...r`...rF...
+00001570: 723a 0000 0072 1500 0000 7215 0000 0072  r:...r....r....r
+00001580: 1600 0000 da11 7072 655f 756e 7061 6464  ......pre_unpadd
+00001590: 696e 675f 6465 638b 0000 0073 0600 0000  ing_dec....s....
+000015a0: 0001 0e01 0aff 7a15 4465 632e 7072 655f  ......z.Dec.pre_
+000015b0: 756e 7061 6464 696e 675f 6465 6363 0100  unpadding_decc..
+000015c0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+000015d0: 0000 4300 0000 7324 0000 0074 00a0 0164  ..C...s$...t...d
+000015e0: 01a1 01a0 02a1 007d 017c 01a0 037c 00a0  .......}.|...|..
+000015f0: 04a1 00a1 017c 01a0 05a1 0017 0053 0072  .....|.......S.r
+00001600: 4100 0000 2906 7205 0000 0072 4300 0000  A...).r....rC...
+00001610: da08 756e 7061 6464 6572 7245 0000 0072  ..unpadderrE...r
+00001620: 6800 0000 7246 0000 0029 0272 1200 0000  h...rF...).r....
+00001630: 7269 0000 0072 1500 0000 7215 0000 0072  ri...r....r....r
+00001640: 1600 0000 da0a 756e 7061 6464 6564 5f6d  ......unpadded_m
+00001650: 8f00 0000 7304 0000 0000 010e 017a 0e44  ....s........z.D
+00001660: 6563 2e75 6e70 6164 6465 645f 6d63 0100  ec.unpadded_mc..
+00001670: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00001680: 0000 4300 0000 7308 0000 007c 00a0 00a1  ..C...s....|....
+00001690: 0053 0072 3800 0000 2901 726a 0000 0072  .S.r8...).rj...r
+000016a0: 3a00 0000 7215 0000 0072 1500 0000 7216  :...r....r....r.
+000016b0: 0000 00da 0c64 6563 5f74 6f5f 6279 7465  .....dec_to_byte
+000016c0: 7393 0000 0073 0200 0000 0001 7a10 4465  s....s......z.De
+000016d0: 632e 6465 635f 746f 5f62 7974 6573 6301  c.dec_to_bytesc.
+000016e0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+000016f0: 0000 0043 0000 0073 0e00 0000 7c00 a000  ...C...s....|...
+00001700: a100 a001 6401 a101 5300 7251 0000 0029  ....d...S.rQ...)
+00001710: 0272 6a00 0000 7253 0000 0072 3a00 0000  .rj...rS...r:...
+00001720: 7215 0000 0072 1500 0000 7216 0000 00da  r....r....r.....
+00001730: 0a64 6563 5f74 6f5f 7374 7296 0000 0073  .dec_to_str....s
+00001740: 0200 0000 0001 7a0e 4465 632e 6465 635f  ......z.Dec.dec_
+00001750: 746f 5f73 7472 2911 7217 0000 0072 1800  to_str).r....r..
+00001760: 0000 7219 0000 0072 0900 0000 7224 0000  ..r....r....r$..
+00001770: 0072 2600 0000 7211 0000 0072 6500 0000  .r&...r....re...
+00001780: da04 626f 6f6c 7263 0000 0072 3b00 0000  ..boolrc...r;...
+00001790: 723f 0000 0072 6700 0000 7268 0000 0072  r?...rg...rh...r
+000017a0: 6a00 0000 726b 0000 0072 6c00 0000 7215  j...rk...rl...r.
+000017b0: 0000 0072 1500 0000 7215 0000 0072 1600  ...r....r....r..
+000017c0: 0000 7258 0000 005d 0000 0073 1400 0000  ..rX...]...s....
+000017d0: 0801 1a17 0e06 0e03 0803 0807 0803 0e04  ................
+000017e0: 0e04 0e03 7258 0000 0029 165a 2663 7279  ....rX...).Z&cry
+000017f0: 7074 6f67 7261 7068 792e 6861 7a6d 6174  ptography.hazmat
+00001800: 2e70 7269 6d69 7469 7665 732e 6369 7068  .primitives.ciph
+00001810: 6572 7372 0200 0000 7203 0000 0072 0400  ersr....r....r..
+00001820: 0000 5a1e 6372 7970 746f 6772 6170 6879  ..Z.cryptography
+00001830: 2e68 617a 6d61 742e 7072 696d 6974 6976  .hazmat.primitiv
+00001840: 6573 7205 0000 005a 1c63 7279 7074 6f67  esr....Z.cryptog
+00001850: 7261 7068 792e 6861 7a6d 6174 2e62 6163  raphy.hazmat.bac
+00001860: 6b65 6e64 7372 0600 0000 7207 0000 0072  kendsr....r....r
+00001870: 0800 0000 5a06 7479 7069 6e67 7209 0000  ....Z.typingr...
+00001880: 0072 6600 0000 7234 0000 0072 5200 0000  .rf...r4...rR...
+00001890: 724e 0000 0072 2700 0000 da09 4578 6365  rN...r'.....Exce
+000018a0: 7074 696f 6e72 0a00 0000 721c 0000 0072  ptionr....r....r
+000018b0: 5700 0000 7258 0000 0072 1500 0000 7215  W...rX...r....r.
+000018c0: 0000 0072 1500 0000 7216 0000 00da 083c  ...r....r......<
+000018d0: 6d6f 6475 6c65 3e01 0000 0073 1a00 0000  module>....s....
+000018e0: 1401 0c01 0c01 1001 0c01 0801 0801 0801  ................
+000018f0: 0801 0803 1006 0e44 1006                 .......D..
```

### Comparing `AshCrypt-1.3.6/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc` & `AshCrypt-2.0.0/AshCrypt/__pycache__/AshCryptGUI.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.6/AshCrypt/__pycache__/Database.cpython-39.pyc` & `AshCrypt-2.0.0/AshCrypt/__pycache__/Database.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jul  9 22:27:03 2023 UTC, .py size: 8993 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 3734 ab64 2123 0000  a.......74.d!#..
+00000000: 610d 0d0a 0000 0000 39ed b364 fa22 0000  a.......9..d."..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 4e00 0000 6400  .....@...sN...d.
 00000030: 6401 6c00 6d01 5a01 6d02 5a02 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6402 6c03 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 5a06 6400  m.Z...d.d.l.Z.d.
 00000060: 6404 6c07 5a07 6501 4700 6405 6406 8400  d.l.Z.e.G.d.d...
 00000070: 6406 8302 8301 5a08 6404 5300 2907 e900  d.....Z.d.S.)...
@@ -205,257 +205,257 @@
 00000cc0: 0669 6e73 6572 7459 0000 0073 3200 0000  .insertY...s2...
 00000cd0: 0001 0801 0201 0801 0601 0c01 0201 0201  ................
 00000ce0: 02fe 02fe 2206 0601 1001 2003 0201 0801  ...."..... .....
 00000cf0: 0601 0a01 0201 0201 02fe 02fe 2205 0601  ............"...
 00000d00: 1201 7a0f 4461 7461 6261 7365 2e69 6e73  ..z.Database.ins
 00000d10: 6572 7429 03da 0b63 6f6c 756d 6e5f 6e61  ert)...column_na
 00000d20: 6d65 da0e 6e65 775f 636f 6c75 6d6e 5f76  me..new_column_v
-00000d30: 616c da02 4944 6305 0000 0000 0000 0000  al..IDc.........
-00000d40: 0000 0006 0000 000a 0000 0043 0000 0073  ...........C...s
-00000d50: 0a01 0000 7c04 6400 7500 728a 7a50 7c00  ....|.d.u.r.zP|.
-00000d60: 6a00 8f36 0100 7c00 6a01 a002 6401 7c00  j..6..|.j...d.|.
-00000d70: 6a03 9b00 6402 7c01 9b00 6403 9d05 7c02  j...d.|...d...|.
-00000d80: 7c03 6602 a102 0100 5700 6400 0400 0400  |.f.....W.d.....
-00000d90: 8303 0100 5700 6404 5300 3100 734c 3000  ....W.d.S.1.sL0.
-00000da0: 0100 0100 0100 5900 0100 5700 6e2e 0400  ......Y...W.n...
-00000db0: 7404 6a05 7986 0100 7d05 0100 7a14 6405  t.j.y...}...z.d.
-00000dc0: 7c05 6602 5700 0600 5900 6400 7d05 7e05  |.f.W...Y.d.}.~.
-00000dd0: 5300 6400 7d05 7e05 3000 3000 6e7c 7a4a  S.d.}.~.0.0.n|zJ
-00000de0: 7c00 6a00 8f30 0100 7c00 6a01 a002 6401  |.j..0..|.j...d.
-00000df0: 7c04 9b00 6406 9d03 7c01 7c02 7c03 6603  |...d...|.|.|.f.
-00000e00: a102 0100 5700 6400 0400 0400 8303 0100  ....W.d.........
-00000e10: 5700 6407 5300 3100 73c8 3000 0100 0100  W.d.S.1.s.0.....
-00000e20: 0100 5900 0100 5700 6e30 0400 7404 6a05  ..Y...W.n0..t.j.
-00000e30: 9001 7904 0100 7d05 0100 7a14 6408 7c05  ..y...}...z.d.|.
-00000e40: 6602 5700 0600 5900 6400 7d05 7e05 5300  f.W...Y.d.}.~.S.
-00000e50: 6400 7d05 7e05 3000 3000 6400 5300 2909  d.}.~.0.0.d.S.).
-00000e60: 4e7a 0755 5044 4154 4520 7a05 2053 4554  Nz.UPDATE z. SET
-00000e70: 207a 1220 3d20 3f20 5748 4552 4520 4944   z. = ? WHERE ID
-00000e80: 203d 203f 2072 3200 0000 7224 0000 007a   = ? r2...r$...z
-00000e90: 1820 5345 5420 3f20 3d20 3f20 5748 4552  . SET ? = ? WHER
-00000ea0: 4520 4944 203d 203f 2072 2500 0000 7201  E ID = ? r%...r.
-00000eb0: 0000 0072 3300 0000 2906 7211 0000 0072  ...r3...).r....r
-00000ec0: 3b00 0000 723c 0000 0072 3d00 0000 7239  ;...r<...r=...r9
-00000ed0: 0000 0072 1900 0000 7212 0000 0072 1200  ...r....r....r..
-00000ee0: 0000 7213 0000 00da 0675 7064 6174 6573  ..r......updates
-00000ef0: 0000 0073 3000 0000 0006 0801 0201 0801  ...s0...........
-00000f00: 0601 1201 0201 02ff 02fe 0404 2602 1001  ............&...
-00000f10: 2003 0201 0801 0601 0a01 0201 0201 02fe   ...............
-00000f20: 02fe 0405 2602 1201 7a0f 4461 7461 6261  ....&...z.Databa
-00000f30: 7365 2e75 7064 6174 6563 0200 0000 0000  se.updatec......
-00000f40: 0000 0000 0000 0400 0000 0a00 0000 6300  ..............c.
-00000f50: 0000 731a 0100 007c 0164 0075 0072 907a  ..s....|.d.u.r.z
-00000f60: 567c 006a 008f 3c01 007c 006a 01a0 0264  V|.j..<..|.j...d
-00000f70: 017c 006a 039b 0064 029d 03a1 0101 007c  .|.j...d.......|
-00000f80: 006a 01a0 04a1 0044 005d 0a7d 027c 0256  .j.....D.].}.|.V
-00000f90: 0001 0071 3257 0064 0004 0004 0083 0301  ...q2W.d........
-00000fa0: 006e 1031 0073 5230 0001 0001 0001 0059  .n.1.sR0.......Y
-00000fb0: 0001 0057 006e 2e04 0074 056a 0679 8c01  ...W.n...t.j.y..
-00000fc0: 007d 0301 007a 1464 037c 0366 0257 0006  .}...z.d.|.f.W..
-00000fd0: 0059 0064 007d 037e 0353 0064 007d 037e  .Y.d.}.~.S.d.}.~
-00000fe0: 0330 0030 006e 867a 547c 006a 008f 3a01  .0.0.n.zT|.j..:.
-00000ff0: 007c 006a 01a0 0264 017c 019b 0064 029d  .|.j...d.|...d..
-00001000: 03a1 0101 007c 006a 01a0 04a1 0044 005d  .....|.j.....D.]
-00001010: 0a7d 027c 0256 0001 0071 b857 0064 0004  .}.|.V...q.W.d..
-00001020: 0004 0083 0301 006e 1031 0073 d830 0001  .......n.1.s.0..
-00001030: 0001 0001 0059 0001 0057 006e 3004 0074  .....Y...W.n0..t
-00001040: 056a 0690 0179 1401 007d 0301 007a 1464  .j...y...}...z.d
-00001050: 047c 0366 0257 0006 0059 0064 007d 037e  .|.f.W...Y.d.}.~
-00001060: 0353 0064 007d 037e 0330 0030 0064 0053  .S.d.}.~.0.0.d.S
-00001070: 00a9 054e fa0e 5345 4c45 4354 202a 2046  ...N..SELECT * F
-00001080: 524f 4d20 fa01 2072 2400 0000 7201 0000  ROM .. r$...r...
-00001090: 00a9 0772 0c00 0000 720d 0000 0072 1500  ...r....r....r..
-000010a0: 0000 7209 0000 0072 2d00 0000 720e 0000  ..r....r-...r...
-000010b0: 0072 1700 0000 2904 7211 0000 0072 3400  .r....).r....r4.
-000010c0: 0000 da03 726f 7772 1900 0000 7212 0000  ....rowr....r...
-000010d0: 0072 1200 0000 7213 0000 0072 3700 0000  .r....r....r7...
-000010e0: 9200 0000 731e 0000 0000 0108 0102 0108  ....s...........
-000010f0: 0116 010e 012a 0210 0120 0302 0108 0114  .....*... ......
-00001100: 010e 012a 0212 017a 1044 6174 6162 6173  ...*...z.Databas
-00001110: 652e 636f 6e74 656e 7429 01da 0269 6463  e.content)...idc
-00001120: 0300 0000 0000 0000 0000 0000 0500 0000  ................
-00001130: 0a00 0000 6300 0000 7322 0100 007c 0264  ....c...s"...|.d
-00001140: 0075 0072 947a 5a7c 006a 008f 4001 007c  .u.r.zZ|.j..@..|
-00001150: 006a 01a0 0264 017c 006a 039b 0064 029d  .j...d.|.j...d..
-00001160: 037c 0166 01a1 0201 007c 006a 01a0 04a1  .|.f.....|.j....
-00001170: 0044 005d 0a7d 037c 0356 0001 0071 3657  .D.].}.|.V...q6W
-00001180: 0064 0004 0004 0083 0301 006e 1031 0073  .d.........n.1.s
-00001190: 5630 0001 0001 0001 0059 0001 0057 006e  V0.......Y...W.n
-000011a0: 2e04 0074 056a 0679 9001 007d 0401 007a  ...t.j.y...}...z
-000011b0: 1464 037c 0466 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
-000011c0: 047e 0453 0064 007d 047e 0430 0030 006e  .~.S.d.}.~.0.0.n
-000011d0: 8a7a 587c 006a 008f 3e01 007c 006a 01a0  .zX|.j..>..|.j..
-000011e0: 0264 017c 029b 0064 029d 037c 0166 01a1  .d.|...d...|.f..
-000011f0: 0201 007c 006a 01a0 04a1 0044 005d 0a7d  ...|.j.....D.].}
-00001200: 037c 0356 0001 0071 c057 0064 0004 0004  .|.V...q.W.d....
-00001210: 0083 0301 006e 1031 0073 e030 0001 0001  .....n.1.s.0....
-00001220: 0001 0059 0001 0057 006e 3004 0074 056a  ...Y...W.n0..t.j
-00001230: 0690 0179 1c01 007d 0401 007a 1464 047c  ...y...}...z.d.|
-00001240: 0466 0257 0006 0059 0064 007d 047e 0453  .f.W...Y.d.}.~.S
-00001250: 0064 007d 047e 0430 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
-00001260: 054e 7240 0000 007a 0e20 5748 4552 4520  .Nr@...z. WHERE 
-00001270: 4944 203d 203f 2072 2400 0000 7201 0000  ID = ? r$...r...
-00001280: 0072 4200 0000 2905 7211 0000 0072 4400  .rB...).r....rD.
-00001290: 0000 7234 0000 0072 4300 0000 7219 0000  ..r4...rC...r...
-000012a0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
-000012b0: da0d 636f 6e74 656e 745f 6279 5f69 64a7  ..content_by_id.
-000012c0: 0000 0073 2600 0000 0001 0801 0201 0801  ...s&...........
-000012d0: 0601 10ff 0402 0e01 2a02 1001 2003 0201  ........*... ...
-000012e0: 0801 0601 0eff 0402 0e01 2a02 1201 7a16  ..........*...z.
-000012f0: 4461 7461 6261 7365 2e63 6f6e 7465 6e74  Database.content
-00001300: 5f62 795f 6964 6301 0000 0000 0000 0000  _by_idc.........
-00001310: 0000 0005 0000 000a 0000 0067 0000 0073  ...........g...s
-00001320: 2a01 0000 7c01 7298 7a62 7c01 4400 5d58  *...|.r.zb|.D.]X
-00001330: 7d02 7c00 6a00 8f3e 0100 7c00 6a01 a002  }.|.j..>..|.j...
-00001340: 6401 7c02 9b00 6402 9d03 a101 0100 7c00  d.|...d.......|.
-00001350: 6a01 a003 a100 4400 5d0e 7d03 7c02 7c03  j.....D.].}.|.|.
-00001360: 6901 5600 0100 7134 5700 6400 0400 0400  i.V...q4W.d.....
-00001370: 8303 0100 710a 3100 7358 3000 0100 0100  ....q.1.sX0.....
-00001380: 0100 5900 0100 710a 5700 6e2e 0400 7404  ..Y...q.W.n...t.
-00001390: 6a05 7994 0100 7d04 0100 7a14 6403 7c04  j.y...}...z.d.|.
-000013a0: 6602 5700 0600 5900 6400 7d04 7e04 5300  f.W...Y.d.}.~.S.
-000013b0: 6400 7d04 7e04 3000 3000 6e8e 7a5c 7c00  d.}.~.0.0.n.z\|.
-000013c0: 6a00 8f42 0100 7c00 6a01 a002 6401 7c00  j..B..|.j...d.|.
-000013d0: 6a06 9b00 6402 9d03 a101 0100 7c00 6a01  j...d.......|.j.
-000013e0: a003 a100 4400 5d10 7d03 7c00 6a06 7c03  ....D.].}.|.j.|.
-000013f0: 6901 5600 0100 71c2 5700 6400 0400 0400  i.V...q.W.d.....
-00001400: 8303 0100 6e10 3100 73e8 3000 0100 0100  ....n.1.s.0.....
-00001410: 0100 5900 0100 5700 6e30 0400 7404 6a05  ..Y...W.n0..t.j.
-00001420: 9001 7924 0100 7d04 0100 7a14 6404 7c04  ..y$..}...z.d.|.
-00001430: 6602 5700 0600 5900 6400 7d04 7e04 5300  f.W...Y.d.}.~.S.
-00001440: 6400 7d04 7e04 3000 3000 6400 5300 723f  d.}.~.0.0.d.S.r?
-00001450: 0000 0029 0772 0c00 0000 720d 0000 0072  ...).r....r....r
-00001460: 1500 0000 722d 0000 0072 0e00 0000 7217  ....r-...r....r.
-00001470: 0000 0072 0900 0000 2905 7211 0000 005a  ...r....).r....Z
-00001480: 136f 7074 696f 6e61 6c5f 7461 626c 656e  .optional_tablen
-00001490: 616d 6573 da03 6172 6772 4300 0000 7219  ames..argrC...r.
-000014a0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
-000014b0: 0000 da0d 7368 6f77 5f63 6f6e 7465 6e74  ....show_content
-000014c0: 73be 0000 0073 2000 0000 0001 0401 0201  s....s .........
-000014d0: 0801 0801 1401 0e01 3002 1001 2003 0201  ........0... ...
-000014e0: 0801 1601 0e01 3002 1201 7a16 4461 7461  ......0...z.Data
-000014f0: 6261 7365 2e73 686f 775f 636f 6e74 656e  base.show_conten
-00001500: 7473 6301 0000 0000 0000 0000 0000 0003  tsc.............
-00001510: 0000 000a 0000 0063 0000 0073 8000 0000  .......c...s....
-00001520: 7a4c 7c00 6a00 8f32 0100 7c00 6a01 a002  zL|.j..2..|.j...
-00001530: 6401 a101 0100 7c00 6a01 a003 a100 4400  d.....|.j.....D.
-00001540: 5d0a 7d01 7c01 5600 0100 7120 5700 6400  ].}.|.V...q W.d.
-00001550: 0400 0400 8303 0100 6e10 3100 7340 3000  ........n.1.s@0.
-00001560: 0100 0100 0100 5900 0100 5700 6e2e 0400  ......Y...W.n...
-00001570: 7404 6a05 797a 0100 7d02 0100 7a14 6402  t.j.yz..}...z.d.
-00001580: 7c02 6602 5700 0600 5900 6400 7d02 7e02  |.f.W...Y.d.}.~.
-00001590: 5300 6400 7d02 7e02 3000 3000 6400 5300  S.d.}.~.0.0.d.S.
-000015a0: 2903 4efa 3353 454c 4543 5420 6e61 6d65  ).N.3SELECT name
-000015b0: 2046 524f 4d20 7371 6c69 7465 5f6d 6173   FROM sqlite_mas
-000015c0: 7465 7220 5748 4552 4520 7479 7065 3d20  ter WHERE type= 
-000015d0: 2774 6162 6c65 2720 7201 0000 00a9 0672  'table' r......r
-000015e0: 0c00 0000 720d 0000 0072 1500 0000 722d  ....r....r....r-
-000015f0: 0000 0072 0e00 0000 7217 0000 0029 0372  ...r....r....).r
-00001600: 1100 0000 7243 0000 0072 1900 0000 7212  ....rC...r....r.
-00001610: 0000 0072 1200 0000 7213 0000 00da 0b73  ...r....r......s
-00001620: 686f 775f 7461 626c 6573 d400 0000 7312  how_tables....s.
-00001630: 0000 0000 0102 0108 0106 0102 ff04 020e  ................
-00001640: 012a 0210 017a 1444 6174 6162 6173 652e  .*...z.Database.
-00001650: 7368 6f77 5f74 6162 6c65 7363 0100 0000  show_tablesc....
-00001660: 0000 0000 0000 0000 0300 0000 0a00 0000  ................
-00001670: 4300 0000 7394 0000 007a 607c 006a 008f  C...s....z`|.j..
-00001680: 4601 007c 006a 01a0 0264 01a1 0101 007c  F..|.j...d.....|
-00001690: 006a 01a0 03a1 0044 005d 1a7d 017c 006a  .j.....D.].}.|.j
-000016a0: 01a0 0264 027c 0164 0319 009b 009d 02a1  ...d.|.d........
-000016b0: 0101 0071 2057 0064 0004 0004 0083 0301  ...q W.d........
-000016c0: 0057 0064 0453 0031 0073 5430 0001 0001  .W.d.S.1.sT0....
-000016d0: 0001 0059 0001 0057 006e 2e04 0074 046a  ...Y...W.n...t.j
-000016e0: 0579 8e01 007d 0201 007a 1464 037c 0266  .y...}...z.d.|.f
-000016f0: 0257 0006 0059 0064 007d 027e 0253 0064  .W...Y.d.}.~.S.d
-00001700: 007d 027e 0230 0030 0064 0053 0029 054e  .}.~.0.0.d.S.).N
-00001710: 7248 0000 00fa 0b44 524f 5020 5441 424c  rH.....DROP TABL
-00001720: 4520 7201 0000 0072 2500 0000 7249 0000  E r....r%...rI..
-00001730: 0029 0372 1100 0000 da05 7461 626c 6572  .).r......tabler
-00001740: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00001750: 0000 00da 0764 726f 7061 6c6c df00 0000  .....dropall....
-00001760: 7314 0000 0000 0102 0108 0106 0102 ff04  s...............
-00001770: 020e 0118 0126 0210 017a 1044 6174 6162  .....&...z.Datab
-00001780: 6173 652e 6472 6f70 616c 6c63 0100 0000  ase.dropallc....
-00001790: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
-000017a0: 4700 0000 73f6 0000 007c 0172 7e7a 487c  G...s....|.r~zH|
-000017b0: 0144 005d 3c7d 027c 006a 008f 2201 007c  .D.]<}.|.j.."..|
-000017c0: 006a 01a0 0264 017c 029b 009d 02a1 0101  .j...d.|........
-000017d0: 0057 0064 0004 0004 0083 0301 0071 0a31  .W.d.........q.1
-000017e0: 0073 3c30 0001 0001 0001 0059 0001 0071  .s<0.......Y...q
-000017f0: 0a57 0064 0253 0004 0074 036a 0479 7a01  .W.d.S...t.j.yz.
-00001800: 007d 0301 007a 1464 037c 0366 0257 0006  .}...z.d.|.f.W..
-00001810: 0059 0064 007d 037e 0353 0064 007d 037e  .Y.d.}.~.S.d.}.~
-00001820: 0330 0030 006e 747a 427c 006a 008f 2801  .0.0.ntzB|.j..(.
-00001830: 007c 006a 01a0 0264 017c 006a 059b 009d  .|.j...d.|.j....
-00001840: 02a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
-00001850: 0057 0064 0253 0031 0073 b430 0001 0001  .W.d.S.1.s.0....
-00001860: 0001 0059 0001 0057 006e 3004 0074 036a  ...Y...W.n0..t.j
-00001870: 0490 0079 f001 007d 0301 007a 1464 047c  ...y...}...z.d.|
-00001880: 0366 0257 0006 0059 0064 007d 037e 0353  .f.W...Y.d.}.~.S
-00001890: 0064 007d 037e 0330 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
-000018a0: 054e 724b 0000 0072 2500 0000 7224 0000  .NrK...r%...r$..
-000018b0: 0072 0100 0000 2906 720c 0000 0072 0d00  .r....).r....r..
-000018c0: 0000 7215 0000 0072 0e00 0000 7217 0000  ..r....r....r...
-000018d0: 0072 0900 0000 2904 7211 0000 005a 0b74  .r....).r....Z.t
-000018e0: 6162 6c65 5f6e 616d 6573 7246 0000 0072  able_namesrF...r
-000018f0: 1900 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00001900: 0000 00da 0a64 726f 705f 7461 626c 65eb  .....drop_table.
-00001910: 0000 0073 1c00 0000 0001 0401 0201 0801  ...s............
-00001920: 0801 3201 0601 1001 2003 0201 0801 1401  ..2..... .......
-00001930: 2602 1201 7a13 4461 7461 6261 7365 2e64  &...z.Database.d
-00001940: 726f 705f 7461 626c 6563 0300 0000 0000  rop_tablec......
-00001950: 0000 0000 0000 0400 0000 0a00 0000 4300  ..............C.
-00001960: 0000 73fa 0000 007c 0264 0075 0072 807a  ..s....|.d.u.r.z
-00001970: 467c 006a 008f 2a01 007c 006a 01a0 0264  F|.j..*..|.j...d
-00001980: 017c 006a 039b 0064 027c 019b 009d 04a1  .|.j...d.|......
-00001990: 0101 0057 0064 0004 0004 0083 0301 006e  ...W.d.........n
-000019a0: 1031 0073 4030 0001 0001 0001 0059 0001  .1.s@0.......Y..
-000019b0: 0057 0064 0353 0004 0074 046a 0579 7c01  .W.d.S...t.j.y|.
-000019c0: 007d 0301 007a 1464 047c 0366 0257 0006  .}...z.d.|.f.W..
-000019d0: 0059 0064 007d 037e 0353 0064 007d 037e  .Y.d.}.~.S.d.}.~
-000019e0: 0330 0030 006e 767a 447c 006a 008f 2801  .0.0.nvzD|.j..(.
-000019f0: 007c 006a 01a0 0264 017c 029b 0064 027c  .|.j...d.|...d.|
-00001a00: 019b 009d 04a1 0101 0057 0064 0004 0004  .........W.d....
-00001a10: 0083 0301 006e 1031 0073 b630 0001 0001  .....n.1.s.0....
-00001a20: 0001 0059 0001 0057 0064 0553 0004 0074  ...Y...W.d.S...t
-00001a30: 046a 0590 0079 f401 007d 0301 007a 1464  .j...y...}...z.d
-00001a40: 067c 0366 0257 0006 0059 0064 007d 037e  .|.f.W...Y.d.}.~
-00001a50: 0353 0064 007d 037e 0330 0030 0064 0053  .S.d.}.~.0.0.d.S
-00001a60: 0029 074e 7a0c 4445 4c45 5445 2046 524f  .).Nz.DELETE FRO
-00001a70: 4d20 7a0c 2057 4845 5245 2049 4420 3d20  M z. WHERE ID = 
-00001a80: 7232 0000 0072 2400 0000 7225 0000 0072  r2...r$...r%...r
-00001a90: 0100 0000 7233 0000 0029 0472 1100 0000  ....r3...).r....
-00001aa0: 723d 0000 0072 3900 0000 7219 0000 0072  r=...r9...r....r
-00001ab0: 1200 0000 7212 0000 0072 1300 0000 da0c  ....r....r......
-00001ac0: 6472 6f70 5f63 6f6e 7465 6e74 fe00 0000  drop_content....
-00001ad0: 7322 0000 0000 0108 0102 0108 0106 0110  s"..............
-00001ae0: ff22 0206 0210 0120 0302 0108 0106 010e  ."..... ........
-00001af0: ff22 0206 0212 017a 1544 6174 6162 6173  .".....z.Databas
-00001b00: 652e 6472 6f70 5f63 6f6e 7465 6e74 2901  e.drop_content).
-00001b10: 4e29 014e 2901 4e29 014e 2901 4e29 014e  N).N).N).N).N).N
-00001b20: 2922 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )"..__name__..__
-00001b30: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00001b40: 6e61 6d65 5f5f 7203 0000 0072 0700 0000  name__r....r....
-00001b50: 722a 0000 00da 0f5f 5f61 6e6e 6f74 6174  r*.....__annotat
-00001b60: 696f 6e73 5f5f 7209 0000 0072 0c00 0000  ions__r....r....
-00001b70: 720e 0000 005a 0a43 6f6e 6e65 6374 696f  r....Z.Connectio
-00001b80: 6e72 0d00 0000 5a06 4375 7273 6f72 7214  nr....Z.Cursorr.
-00001b90: 0000 00da 0870 726f 7065 7274 7972 1800  .....propertyr..
-00001ba0: 0000 7205 0000 0072 0400 0000 da05 7475  ..r....r......tu
-00001bb0: 706c 6572 2000 0000 7222 0000 00da 046c  pler ...r".....l
-00001bc0: 6973 7472 3100 0000 7235 0000 0072 3a00  istr1...r5...r:.
-00001bd0: 0000 da03 696e 7472 3e00 0000 7237 0000  ....intr>...r7..
-00001be0: 0072 4500 0000 7247 0000 0072 4a00 0000  .rE...rG...rJ...
-00001bf0: 724d 0000 0072 4e00 0000 724f 0000 0072  rM...rN...rO...r
-00001c00: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-00001c10: 0000 0072 0600 0000 0800 0000 7336 0000  ...r........s6..
-00001c20: 000a 020e 0112 0116 0116 0208 0402 010a  ................
-00001c30: 0b02 0118 0802 010a 0310 130a 1a0a 1f00  ................
-00001c40: fb02 0202 0102 0102 fc0c 1f0a 1510 1708  ................
-00001c50: 160e 0b08 0c08 1372 0600 0000 2909 5a0b  .......r....).Z.
-00001c60: 6461 7461 636c 6173 7365 7372 0200 0000  dataclassesr....
-00001c70: 7203 0000 0072 0400 0000 da06 7479 7069  r....r......typi
-00001c80: 6e67 7205 0000 0072 0e00 0000 721c 0000  ngr....r....r...
-00001c90: 0072 0600 0000 7212 0000 0072 1200 0000  .r....r....r....
-00001ca0: 7212 0000 0072 1300 0000 da08 3c6d 6f64  r....r......<mod
-00001cb0: 756c 653e 0100 0000 730c 0000 0010 010c  ule>....s.......
-00001cc0: 010c 0108 0108 0302 01                   .........
+00000d30: 616c da03 6964 6463 0500 0000 0000 0000  al..iddc........
+00000d40: 0000 0000 0600 0000 0a00 0000 4300 0000  ............C...
+00000d50: 730a 0100 007c 0464 0075 0072 8a7a 507c  s....|.d.u.r.zP|
+00000d60: 006a 008f 3601 007c 006a 01a0 0264 017c  .j..6..|.j...d.|
+00000d70: 006a 039b 0064 027c 019b 0064 039d 057c  .j...d.|...d...|
+00000d80: 027c 0366 02a1 0201 0057 0064 0004 0004  .|.f.....W.d....
+00000d90: 0083 0301 0057 0064 0453 0031 0073 4c30  .....W.d.S.1.sL0
+00000da0: 0001 0001 0001 0059 0001 0057 006e 2e04  .......Y...W.n..
+00000db0: 0074 046a 0579 8601 007d 0501 007a 1464  .t.j.y...}...z.d
+00000dc0: 057c 0566 0257 0006 0059 0064 007d 057e  .|.f.W...Y.d.}.~
+00000dd0: 0553 0064 007d 057e 0530 0030 006e 7c7a  .S.d.}.~.0.0.n|z
+00000de0: 4a7c 006a 008f 3001 007c 006a 01a0 0264  J|.j..0..|.j...d
+00000df0: 017c 049b 0064 069d 037c 017c 027c 0366  .|...d...|.|.|.f
+00000e00: 03a1 0201 0057 0064 0004 0004 0083 0301  .....W.d........
+00000e10: 0057 0064 0753 0031 0073 c830 0001 0001  .W.d.S.1.s.0....
+00000e20: 0001 0059 0001 0057 006e 3004 0074 046a  ...Y...W.n0..t.j
+00000e30: 0590 0179 0401 007d 0501 007a 1464 087c  ...y...}...z.d.|
+00000e40: 0566 0257 0006 0059 0064 007d 057e 0553  .f.W...Y.d.}.~.S
+00000e50: 0064 007d 057e 0530 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
+00000e60: 094e 7a07 5550 4441 5445 207a 0520 5345  .Nz.UPDATE z. SE
+00000e70: 5420 7a12 203d 203f 2057 4845 5245 2049  T z. = ? WHERE I
+00000e80: 4420 3d20 3f20 7232 0000 0072 2400 0000  D = ? r2...r$...
+00000e90: 7a18 2053 4554 203f 203d 203f 2057 4845  z. SET ? = ? WHE
+00000ea0: 5245 2049 4420 3d20 3f20 7225 0000 0072  RE ID = ? r%...r
+00000eb0: 0100 0000 7233 0000 0029 0672 1100 0000  ....r3...).r....
+00000ec0: 723b 0000 0072 3c00 0000 723d 0000 0072  r;...r<...r=...r
+00000ed0: 3900 0000 7219 0000 0072 1200 0000 7212  9...r....r....r.
+00000ee0: 0000 0072 1300 0000 da06 7570 6461 7465  ...r......update
+00000ef0: 7300 0000 7330 0000 0000 0608 0102 0108  s...s0..........
+00000f00: 0106 0112 0102 0102 ff02 fe04 0426 0210  .............&..
+00000f10: 0120 0302 0108 0106 010a 0102 0102 0102  . ..............
+00000f20: fe02 fe04 0526 0212 017a 0f44 6174 6162  .....&...z.Datab
+00000f30: 6173 652e 7570 6461 7465 6302 0000 0000  ase.updatec.....
+00000f40: 0000 0000 0000 0004 0000 000a 0000 0063  ...............c
+00000f50: 0000 0073 1a01 0000 7c01 6400 7500 7290  ...s....|.d.u.r.
+00000f60: 7a56 7c00 6a00 8f3c 0100 7c00 6a01 a002  zV|.j..<..|.j...
+00000f70: 6401 7c00 6a03 9b00 6402 9d03 a101 0100  d.|.j...d.......
+00000f80: 7c00 6a01 a004 a100 4400 5d0a 7d02 7c02  |.j.....D.].}.|.
+00000f90: 5600 0100 7132 5700 6400 0400 0400 8303  V...q2W.d.......
+00000fa0: 0100 6e10 3100 7352 3000 0100 0100 0100  ..n.1.sR0.......
+00000fb0: 5900 0100 5700 6e2e 0400 7405 6a06 798c  Y...W.n...t.j.y.
+00000fc0: 0100 7d03 0100 7a14 6403 7c03 6602 5700  ..}...z.d.|.f.W.
+00000fd0: 0600 5900 6400 7d03 7e03 5300 6400 7d03  ..Y.d.}.~.S.d.}.
+00000fe0: 7e03 3000 3000 6e86 7a54 7c00 6a00 8f3a  ~.0.0.n.zT|.j..:
+00000ff0: 0100 7c00 6a01 a002 6401 7c01 9b00 6402  ..|.j...d.|...d.
+00001000: 9d03 a101 0100 7c00 6a01 a004 a100 4400  ......|.j.....D.
+00001010: 5d0a 7d02 7c02 5600 0100 71b8 5700 6400  ].}.|.V...q.W.d.
+00001020: 0400 0400 8303 0100 6e10 3100 73d8 3000  ........n.1.s.0.
+00001030: 0100 0100 0100 5900 0100 5700 6e30 0400  ......Y...W.n0..
+00001040: 7405 6a06 9001 7914 0100 7d03 0100 7a14  t.j...y...}...z.
+00001050: 6404 7c03 6602 5700 0600 5900 6400 7d03  d.|.f.W...Y.d.}.
+00001060: 7e03 5300 6400 7d03 7e03 3000 3000 6400  ~.S.d.}.~.0.0.d.
+00001070: 5300 a905 4efa 0e53 454c 4543 5420 2a20  S...N..SELECT * 
+00001080: 4652 4f4d 20fa 0120 7224 0000 0072 0100  FROM .. r$...r..
+00001090: 0000 a907 720c 0000 0072 0d00 0000 7215  ....r....r....r.
+000010a0: 0000 0072 0900 0000 722d 0000 0072 0e00  ...r....r-...r..
+000010b0: 0000 7217 0000 0029 0472 1100 0000 7234  ..r....).r....r4
+000010c0: 0000 00da 0372 6f77 7219 0000 0072 1200  .....rowr....r..
+000010d0: 0000 7212 0000 0072 1300 0000 7237 0000  ..r....r....r7..
+000010e0: 0092 0000 0073 1e00 0000 0001 0801 0201  .....s..........
+000010f0: 0801 1601 0e01 2a02 1001 2003 0201 0801  ......*... .....
+00001100: 1401 0e01 2a02 1201 7a10 4461 7461 6261  ....*...z.Databa
+00001110: 7365 2e63 6f6e 7465 6e74 2901 723d 0000  se.content).r=..
+00001120: 0063 0300 0000 0000 0000 0000 0000 0500  .c..............
+00001130: 0000 0a00 0000 6300 0000 7322 0100 007c  ......c...s"...|
+00001140: 0264 0075 0072 947a 5a7c 006a 008f 4001  .d.u.r.zZ|.j..@.
+00001150: 007c 006a 01a0 0264 017c 006a 039b 0064  .|.j...d.|.j...d
+00001160: 029d 037c 0166 01a1 0201 007c 006a 01a0  ...|.f.....|.j..
+00001170: 04a1 0044 005d 0a7d 037c 0356 0001 0071  ...D.].}.|.V...q
+00001180: 3657 0064 0004 0004 0083 0301 006e 1031  6W.d.........n.1
+00001190: 0073 5630 0001 0001 0001 0059 0001 0057  .sV0.......Y...W
+000011a0: 006e 2e04 0074 056a 0679 9001 007d 0401  .n...t.j.y...}..
+000011b0: 007a 1464 037c 0466 0257 0006 0059 0064  .z.d.|.f.W...Y.d
+000011c0: 007d 047e 0453 0064 007d 047e 0430 0030  .}.~.S.d.}.~.0.0
+000011d0: 006e 8a7a 587c 006a 008f 3e01 007c 006a  .n.zX|.j..>..|.j
+000011e0: 01a0 0264 017c 029b 0064 029d 037c 0166  ...d.|...d...|.f
+000011f0: 01a1 0201 007c 006a 01a0 04a1 0044 005d  .....|.j.....D.]
+00001200: 0a7d 037c 0356 0001 0071 c057 0064 0004  .}.|.V...q.W.d..
+00001210: 0004 0083 0301 006e 1031 0073 e030 0001  .......n.1.s.0..
+00001220: 0001 0001 0059 0001 0057 006e 3004 0074  .....Y...W.n0..t
+00001230: 056a 0690 0179 1c01 007d 0401 007a 1464  .j...y...}...z.d
+00001240: 047c 0466 0257 0006 0059 0064 007d 047e  .|.f.W...Y.d.}.~
+00001250: 0453 0064 007d 047e 0430 0030 0064 0053  .S.d.}.~.0.0.d.S
+00001260: 0029 054e 7240 0000 007a 0e20 5748 4552  .).Nr@...z. WHER
+00001270: 4520 4944 203d 203f 2072 2400 0000 7201  E ID = ? r$...r.
+00001280: 0000 0072 4200 0000 2905 7211 0000 0072  ...rB...).r....r
+00001290: 3d00 0000 7234 0000 0072 4300 0000 7219  =...r4...rC...r.
+000012a0: 0000 0072 1200 0000 7212 0000 0072 1300  ...r....r....r..
+000012b0: 0000 da0d 636f 6e74 656e 745f 6279 5f69  ....content_by_i
+000012c0: 64a7 0000 0073 2600 0000 0001 0801 0201  d....s&.........
+000012d0: 0801 0601 10ff 0402 0e01 2a02 1001 2003  ..........*... .
+000012e0: 0201 0801 0601 0eff 0402 0e01 2a02 1201  ............*...
+000012f0: 7a16 4461 7461 6261 7365 2e63 6f6e 7465  z.Database.conte
+00001300: 6e74 5f62 795f 6964 6301 0000 0000 0000  nt_by_idc.......
+00001310: 0000 0000 0005 0000 000a 0000 0067 0000  .............g..
+00001320: 0073 2a01 0000 7c01 7298 7a62 7c01 4400  .s*...|.r.zb|.D.
+00001330: 5d58 7d02 7c00 6a00 8f3e 0100 7c00 6a01  ]X}.|.j..>..|.j.
+00001340: a002 6401 7c02 9b00 6402 9d03 a101 0100  ..d.|...d.......
+00001350: 7c00 6a01 a003 a100 4400 5d0e 7d03 7c02  |.j.....D.].}.|.
+00001360: 7c03 6901 5600 0100 7134 5700 6400 0400  |.i.V...q4W.d...
+00001370: 0400 8303 0100 710a 3100 7358 3000 0100  ......q.1.sX0...
+00001380: 0100 0100 5900 0100 710a 5700 6e2e 0400  ....Y...q.W.n...
+00001390: 7404 6a05 7994 0100 7d04 0100 7a14 6403  t.j.y...}...z.d.
+000013a0: 7c04 6602 5700 0600 5900 6400 7d04 7e04  |.f.W...Y.d.}.~.
+000013b0: 5300 6400 7d04 7e04 3000 3000 6e8e 7a5c  S.d.}.~.0.0.n.z\
+000013c0: 7c00 6a00 8f42 0100 7c00 6a01 a002 6401  |.j..B..|.j...d.
+000013d0: 7c00 6a06 9b00 6402 9d03 a101 0100 7c00  |.j...d.......|.
+000013e0: 6a01 a003 a100 4400 5d10 7d03 7c00 6a06  j.....D.].}.|.j.
+000013f0: 7c03 6901 5600 0100 71c2 5700 6400 0400  |.i.V...q.W.d...
+00001400: 0400 8303 0100 6e10 3100 73e8 3000 0100  ......n.1.s.0...
+00001410: 0100 0100 5900 0100 5700 6e30 0400 7404  ....Y...W.n0..t.
+00001420: 6a05 9001 7924 0100 7d04 0100 7a14 6404  j...y$..}...z.d.
+00001430: 7c04 6602 5700 0600 5900 6400 7d04 7e04  |.f.W...Y.d.}.~.
+00001440: 5300 6400 7d04 7e04 3000 3000 6400 5300  S.d.}.~.0.0.d.S.
+00001450: 723f 0000 0029 0772 0c00 0000 720d 0000  r?...).r....r...
+00001460: 0072 1500 0000 722d 0000 0072 0e00 0000  .r....r-...r....
+00001470: 7217 0000 0072 0900 0000 2905 7211 0000  r....r....).r...
+00001480: 005a 136f 7074 696f 6e61 6c5f 7461 626c  .Z.optional_tabl
+00001490: 656e 616d 6573 da03 6172 6772 4300 0000  enames..argrC...
+000014a0: 7219 0000 0072 1200 0000 7212 0000 0072  r....r....r....r
+000014b0: 1300 0000 da0d 7368 6f77 5f63 6f6e 7465  ......show_conte
+000014c0: 6e74 73be 0000 0073 2000 0000 0001 0401  nts....s .......
+000014d0: 0201 0801 0801 1401 0e01 3002 1001 2003  ..........0... .
+000014e0: 0201 0801 1601 0e01 3002 1201 7a16 4461  ........0...z.Da
+000014f0: 7461 6261 7365 2e73 686f 775f 636f 6e74  tabase.show_cont
+00001500: 656e 7473 6301 0000 0000 0000 0000 0000  entsc...........
+00001510: 0003 0000 000a 0000 0063 0000 0073 8000  .........c...s..
+00001520: 0000 7a4c 7c00 6a00 8f32 0100 7c00 6a01  ..zL|.j..2..|.j.
+00001530: a002 6401 a101 0100 7c00 6a01 a003 a100  ..d.....|.j.....
+00001540: 4400 5d0a 7d01 7c01 5600 0100 7120 5700  D.].}.|.V...q W.
+00001550: 6400 0400 0400 8303 0100 6e10 3100 7340  d.........n.1.s@
+00001560: 3000 0100 0100 0100 5900 0100 5700 6e2e  0.......Y...W.n.
+00001570: 0400 7404 6a05 797a 0100 7d02 0100 7a14  ..t.j.yz..}...z.
+00001580: 6402 7c02 6602 5700 0600 5900 6400 7d02  d.|.f.W...Y.d.}.
+00001590: 7e02 5300 6400 7d02 7e02 3000 3000 6400  ~.S.d.}.~.0.0.d.
+000015a0: 5300 2903 4efa 3353 454c 4543 5420 6e61  S.).N.3SELECT na
+000015b0: 6d65 2046 524f 4d20 7371 6c69 7465 5f6d  me FROM sqlite_m
+000015c0: 6173 7465 7220 5748 4552 4520 7479 7065  aster WHERE type
+000015d0: 3d20 2774 6162 6c65 2720 7201 0000 00a9  = 'table' r.....
+000015e0: 0672 0c00 0000 720d 0000 0072 1500 0000  .r....r....r....
+000015f0: 722d 0000 0072 0e00 0000 7217 0000 0029  r-...r....r....)
+00001600: 0372 1100 0000 7243 0000 0072 1900 0000  .r....rC...r....
+00001610: 7212 0000 0072 1200 0000 7213 0000 00da  r....r....r.....
+00001620: 0b73 686f 775f 7461 626c 6573 d400 0000  .show_tables....
+00001630: 7312 0000 0000 0102 0108 0106 0102 ff04  s...............
+00001640: 020e 012a 0210 017a 1444 6174 6162 6173  ...*...z.Databas
+00001650: 652e 7368 6f77 5f74 6162 6c65 7363 0100  e.show_tablesc..
+00001660: 0000 0000 0000 0000 0000 0300 0000 0a00  ................
+00001670: 0000 4300 0000 7394 0000 007a 607c 006a  ..C...s....z`|.j
+00001680: 008f 4601 007c 006a 01a0 0264 01a1 0101  ..F..|.j...d....
+00001690: 007c 006a 01a0 03a1 0044 005d 1a7d 017c  .|.j.....D.].}.|
+000016a0: 006a 01a0 0264 027c 0164 0319 009b 009d  .j...d.|.d......
+000016b0: 02a1 0101 0071 2057 0064 0004 0004 0083  .....q W.d......
+000016c0: 0301 0057 0064 0453 0031 0073 5430 0001  ...W.d.S.1.sT0..
+000016d0: 0001 0001 0059 0001 0057 006e 2e04 0074  .....Y...W.n...t
+000016e0: 046a 0579 8e01 007d 0201 007a 1464 037c  .j.y...}...z.d.|
+000016f0: 0266 0257 0006 0059 0064 007d 027e 0253  .f.W...Y.d.}.~.S
+00001700: 0064 007d 027e 0230 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
+00001710: 054e 7247 0000 00fa 0b44 524f 5020 5441  .NrG.....DROP TA
+00001720: 424c 4520 7201 0000 0072 2500 0000 7248  BLE r....r%...rH
+00001730: 0000 0029 0372 1100 0000 da05 7461 626c  ...).r......tabl
+00001740: 6572 1900 0000 7212 0000 0072 1200 0000  er....r....r....
+00001750: 7213 0000 00da 0764 726f 7061 6c6c df00  r......dropall..
+00001760: 0000 7314 0000 0000 0102 0108 0106 0102  ..s.............
+00001770: ff04 020e 0118 0126 0210 017a 1044 6174  .......&...z.Dat
+00001780: 6162 6173 652e 6472 6f70 616c 6c63 0100  abase.dropallc..
+00001790: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
+000017a0: 0000 4700 0000 73f6 0000 007c 0172 7e7a  ..G...s....|.r~z
+000017b0: 487c 0144 005d 3c7d 027c 006a 008f 2201  H|.D.]<}.|.j..".
+000017c0: 007c 006a 01a0 0264 017c 029b 009d 02a1  .|.j...d.|......
+000017d0: 0101 0057 0064 0004 0004 0083 0301 0071  ...W.d.........q
+000017e0: 0a31 0073 3c30 0001 0001 0001 0059 0001  .1.s<0.......Y..
+000017f0: 0071 0a57 0064 0253 0004 0074 036a 0479  .q.W.d.S...t.j.y
+00001800: 7a01 007d 0301 007a 1464 037c 0366 0257  z..}...z.d.|.f.W
+00001810: 0006 0059 0064 007d 037e 0353 0064 007d  ...Y.d.}.~.S.d.}
+00001820: 037e 0330 0030 006e 747a 427c 006a 008f  .~.0.0.ntzB|.j..
+00001830: 2801 007c 006a 01a0 0264 017c 006a 059b  (..|.j...d.|.j..
+00001840: 009d 02a1 0101 0057 0064 0004 0004 0083  .......W.d......
+00001850: 0301 0057 0064 0253 0031 0073 b430 0001  ...W.d.S.1.s.0..
+00001860: 0001 0001 0059 0001 0057 006e 3004 0074  .....Y...W.n0..t
+00001870: 036a 0490 0079 f001 007d 0301 007a 1464  .j...y...}...z.d
+00001880: 047c 0366 0257 0006 0059 0064 007d 037e  .|.f.W...Y.d.}.~
+00001890: 0353 0064 007d 037e 0330 0030 0064 0053  .S.d.}.~.0.0.d.S
+000018a0: 0029 054e 724a 0000 0072 2500 0000 7224  .).NrJ...r%...r$
+000018b0: 0000 0072 0100 0000 2906 720c 0000 0072  ...r....).r....r
+000018c0: 0d00 0000 7215 0000 0072 0e00 0000 7217  ....r....r....r.
+000018d0: 0000 0072 0900 0000 2904 7211 0000 005a  ...r....).r....Z
+000018e0: 0b74 6162 6c65 5f6e 616d 6573 7245 0000  .table_namesrE..
+000018f0: 0072 1900 0000 7212 0000 0072 1200 0000  .r....r....r....
+00001900: 7213 0000 00da 0a64 726f 705f 7461 626c  r......drop_tabl
+00001910: 65eb 0000 0073 1c00 0000 0001 0401 0201  e....s..........
+00001920: 0801 0801 3201 0601 1001 2003 0201 0801  ....2..... .....
+00001930: 1401 2602 1201 7a13 4461 7461 6261 7365  ..&...z.Database
+00001940: 2e64 726f 705f 7461 626c 6563 0300 0000  .drop_tablec....
+00001950: 0000 0000 0000 0000 0400 0000 0a00 0000  ................
+00001960: 4300 0000 73fa 0000 007c 0264 0075 0072  C...s....|.d.u.r
+00001970: 807a 467c 006a 008f 2a01 007c 006a 01a0  .zF|.j..*..|.j..
+00001980: 0264 017c 006a 039b 0064 027c 019b 009d  .d.|.j...d.|....
+00001990: 04a1 0101 0057 0064 0004 0004 0083 0301  .....W.d........
+000019a0: 006e 1031 0073 4030 0001 0001 0001 0059  .n.1.s@0.......Y
+000019b0: 0001 0057 0064 0353 0004 0074 046a 0579  ...W.d.S...t.j.y
+000019c0: 7c01 007d 0301 007a 1464 047c 0366 0257  |..}...z.d.|.f.W
+000019d0: 0006 0059 0064 007d 037e 0353 0064 007d  ...Y.d.}.~.S.d.}
+000019e0: 037e 0330 0030 006e 767a 447c 006a 008f  .~.0.0.nvzD|.j..
+000019f0: 2801 007c 006a 01a0 0264 017c 029b 0064  (..|.j...d.|...d
+00001a00: 027c 019b 009d 04a1 0101 0057 0064 0004  .|.........W.d..
+00001a10: 0004 0083 0301 006e 1031 0073 b630 0001  .......n.1.s.0..
+00001a20: 0001 0001 0059 0001 0057 0064 0553 0004  .....Y...W.d.S..
+00001a30: 0074 046a 0590 0079 f401 007d 0301 007a  .t.j...y...}...z
+00001a40: 1464 067c 0366 0257 0006 0059 0064 007d  .d.|.f.W...Y.d.}
+00001a50: 037e 0353 0064 007d 037e 0330 0030 0064  .~.S.d.}.~.0.0.d
+00001a60: 0053 0029 074e 7a0c 4445 4c45 5445 2046  .S.).Nz.DELETE F
+00001a70: 524f 4d20 7a0c 2057 4845 5245 2049 4420  ROM z. WHERE ID 
+00001a80: 3d20 7232 0000 0072 2400 0000 7225 0000  = r2...r$...r%..
+00001a90: 0072 0100 0000 7233 0000 0029 0472 1100  .r....r3...).r..
+00001aa0: 0000 723d 0000 0072 3900 0000 7219 0000  ..r=...r9...r...
+00001ab0: 0072 1200 0000 7212 0000 0072 1300 0000  .r....r....r....
+00001ac0: da0c 6472 6f70 5f63 6f6e 7465 6e74 fe00  ..drop_content..
+00001ad0: 0000 7322 0000 0000 0108 0102 0108 0106  ..s"............
+00001ae0: 0110 ff22 0206 0210 0120 0302 0108 0106  ..."..... ......
+00001af0: 010e ff22 0206 0212 017a 1544 6174 6162  ...".....z.Datab
+00001b00: 6173 652e 6472 6f70 5f63 6f6e 7465 6e74  ase.drop_content
+00001b10: 2901 4e29 014e 2901 4e29 014e 2901 4e29  ).N).N).N).N).N)
+00001b20: 014e 2922 da08 5f5f 6e61 6d65 5f5f da0a  .N)"..__name__..
+00001b30: 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f 7175  __module__..__qu
+00001b40: 616c 6e61 6d65 5f5f 7203 0000 0072 0700  alname__r....r..
+00001b50: 0000 722a 0000 00da 0f5f 5f61 6e6e 6f74  ..r*.....__annot
+00001b60: 6174 696f 6e73 5f5f 7209 0000 0072 0c00  ations__r....r..
+00001b70: 0000 720e 0000 005a 0a43 6f6e 6e65 6374  ..r....Z.Connect
+00001b80: 696f 6e72 0d00 0000 5a06 4375 7273 6f72  ionr....Z.Cursor
+00001b90: 7214 0000 00da 0870 726f 7065 7274 7972  r......propertyr
+00001ba0: 1800 0000 7205 0000 0072 0400 0000 da05  ....r....r......
+00001bb0: 7475 706c 6572 2000 0000 7222 0000 00da  tupler ...r"....
+00001bc0: 046c 6973 7472 3100 0000 7235 0000 0072  .listr1...r5...r
+00001bd0: 3a00 0000 da03 696e 7472 3e00 0000 7237  :.....intr>...r7
+00001be0: 0000 0072 4400 0000 7246 0000 0072 4900  ...rD...rF...rI.
+00001bf0: 0000 724c 0000 0072 4d00 0000 724e 0000  ..rL...rM...rN..
+00001c00: 0072 1200 0000 7212 0000 0072 1200 0000  .r....r....r....
+00001c10: 7213 0000 0072 0600 0000 0800 0000 7336  r....r........s6
+00001c20: 0000 000a 020e 0112 0116 0116 0208 0402  ................
+00001c30: 010a 0b02 0118 0802 010a 0310 130a 1a0a  ................
+00001c40: 1f00 fb02 0202 0102 0102 fc0c 1f0a 1510  ................
+00001c50: 1708 160e 0b08 0c08 1372 0600 0000 2909  .........r....).
+00001c60: 5a0b 6461 7461 636c 6173 7365 7372 0200  Z.dataclassesr..
+00001c70: 0000 7203 0000 0072 0400 0000 da06 7479  ..r....r......ty
+00001c80: 7069 6e67 7205 0000 0072 0e00 0000 721c  pingr....r....r.
+00001c90: 0000 0072 0600 0000 7212 0000 0072 1200  ...r....r....r..
+00001ca0: 0000 7212 0000 0072 1300 0000 da08 3c6d  ..r....r......<m
+00001cb0: 6f64 756c 653e 0100 0000 730c 0000 0010  odule>....s.....
+00001cc0: 010c 010c 0108 0108 0302 01              ...........
```

### Comparing `AshCrypt-1.3.6/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc` & `AshCrypt-2.0.0/AshCrypt/__pycache__/FileCrypt.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jul 11 22:47:20 2023 UTC, .py size: 4017 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 25% similar despite different names*

```diff
@@ -1,206 +1,206 @@
-00000000: 610d 0d0a 0000 0000 f8db ad64 b10f 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 19e9 b364 890f 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3600 0000 6400  .....@...s6...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 4700 6403 6404 8400 6404 6503 8303  Z.G.d.d...d.e...
 00000050: 5a04 4700 6405 6406 8400 6406 8302 5a05  Z.G.d.d...d...Z.
 00000060: 6402 5300 2907 e900 0000 0029 01da 0341  d.S.)......)...A
 00000070: 7368 4e63 0000 0000 0000 0000 0000 0000  shNc............
 00000080: 0000 0000 0300 0000 0000 0000 731c 0000  ............s...
 00000090: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
 000000a0: 0284 085a 0387 0004 005a 0453 0029 03da  ...Z.....Z.S.)..
-000000b0: 084b 6579 4572 726f 7263 0100 0000 0000  .KeyErrorc......
-000000c0: 0000 0000 0000 0100 0000 0300 0000 0300  ................
-000000d0: 0000 7318 0000 0064 017c 005f 0074 0183  ..s....d.|._.t..
-000000e0: 00a0 027c 006a 00a1 0101 0064 0053 0029  ...|.j.....d.S.)
-000000f0: 024e 7a1a 4b65 7920 6d75 7374 2062 6520  .Nz.Key must be 
-00000100: 3235 3620 4269 7420 6c6f 6e67 2021 2903  256 Bit long !).
-00000110: 5a07 6469 7370 6c61 79da 0573 7570 6572  Z.display..super
-00000120: da08 5f5f 696e 6974 5f5f a901 da04 7365  ..__init__....se
-00000130: 6c66 a901 da09 5f5f 636c 6173 735f 5fa9  lf....__class__.
-00000140: 00fa 3043 3a5c 576f 726b 5c47 6974 4875  ..0C:\Work\GitHu
-00000150: 6257 6f72 6b5c 4145 532d 3235 365c 4173  bWork\AES-256\As
-00000160: 6843 7279 7074 5c46 696c 6543 7279 7074  hCrypt\FileCrypt
-00000170: 2e70 7972 0500 0000 0600 0000 7304 0000  .pyr........s...
-00000180: 0000 0106 017a 114b 6579 4572 726f 722e  .....z.KeyError.
-00000190: 5f5f 696e 6974 5f5f 2905 da08 5f5f 6e61  __init__)...__na
-000001a0: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-000001b0: da0c 5f5f 7175 616c 6e61 6d65 5f5f 7205  ..__qualname__r.
-000001c0: 0000 00da 0d5f 5f63 6c61 7373 6365 6c6c  .....__classcell
-000001d0: 5f5f 720a 0000 0072 0a00 0000 7208 0000  __r....r....r...
-000001e0: 0072 0b00 0000 7203 0000 0005 0000 0073  .r....r........s
-000001f0: 0200 0000 0801 7203 0000 0063 0000 0000  ......r....c....
-00000200: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000210: 4000 0000 7366 0000 0065 005a 0164 005a  @...sf...e.Z.d.Z
-00000220: 0264 0164 0284 005a 0365 0465 0564 039c  .d.d...Z.e.e.d..
-00000230: 0164 0464 0584 0483 015a 0665 0465 0565  .d.d.....Z.e.e.e
-00000240: 0764 069c 0264 0764 0884 0483 015a 0865  .d...d.d.....Z.e
-00000250: 0764 039c 0164 0964 0a84 045a 0965 0764  .d...d.d...Z.e.d
-00000260: 039c 0164 0b64 0c84 045a 0a64 0d64 0e84  ...d.d...Z.d.d..
-00000270: 005a 0b64 0f64 1084 005a 0c64 1153 0029  .Z.d.d...Z.d.S.)
-00000280: 12da 0943 7279 7074 4669 6c65 6303 0000  ...CryptFilec...
-00000290: 0000 0000 0000 0000 0003 0000 0003 0000  ................
-000002a0: 0043 0000 0073 2c00 0000 7c01 7c00 5f00  .C...s,...|.|._.
-000002b0: 6401 7c00 5f01 7c00 a002 7c02 a101 6402  d.|._.|...|...d.
-000002c0: 6b02 7222 7c02 7c00 5f03 6e06 6402 7c00  k.r"|.|._.n.d.|.
-000002d0: 5f01 6400 5300 2903 4e72 0100 0000 e901  _.d.S.).Nr......
-000002e0: 0000 0029 04da 0866 696c 656e 616d 65da  ...)...filename.
-000002f0: 0f6e 6f74 5f32 3536 5f62 6974 5f6b 6579  .not_256_bit_key
-00000300: da09 6b65 7976 6572 6966 79da 036b 6579  ..keyverify..key
-00000310: 2903 7207 0000 0072 1200 0000 7215 0000  ).r....r....r...
-00000320: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000330: 7205 0000 000c 0000 0073 0a00 0000 0001  r........s......
-00000340: 0601 0601 0e01 0802 7a12 4372 7970 7446  ........z.CryptF
-00000350: 696c 652e 5f5f 696e 6974 5f5f 2901 da06  ile.__init__)...
-00000360: 7265 7475 726e 6300 0000 0000 0000 0000  returnc.........
-00000370: 0000 0000 0000 0002 0000 0043 0000 0073  ...........C...s
-00000380: 0a00 0000 7400 6a01 a002 a100 5300 2901  ....t.j.....S.).
-00000390: 4e29 0372 0200 0000 da03 456e 635a 0a67  N).r......EncZ.g
-000003a0: 656e 4d61 696e 6b65 7972 0a00 0000 720a  enMainkeyr....r.
-000003b0: 0000 0072 0a00 0000 720b 0000 00da 0667  ...r....r......g
-000003c0: 656e 6b65 7914 0000 0073 0200 0000 0002  enkey....s......
-000003d0: 7a10 4372 7970 7446 696c 652e 6765 6e6b  z.CryptFile.genk
-000003e0: 6579 2902 7215 0000 0072 1600 0000 6301  ey).r....r....c.
-000003f0: 0000 0000 0000 0000 0000 0002 0000 0008  ................
-00000400: 0000 0043 0000 0073 4e00 0000 7a34 7400  ...C...sN...z4t.
-00000410: 7c00 7401 8302 7232 7402 a003 7c00 a004  |.t...r2t...|...
-00000420: a100 a101 7d01 7405 7c01 8301 6401 6b02  ....}.t.|...d.k.
-00000430: 722c 5700 6402 5300 5700 6403 5300 5700  r,W.d.S.W.d.S.W.
-00000440: 6e14 0400 7406 7948 0100 0100 0100 5900  n...t.yH......Y.
-00000450: 6404 5300 3000 6400 5300 2905 4ee9 2000  d.S.0.d.S.).N. .
-00000460: 0000 7211 0000 0072 0100 0000 e902 0000  ..r....r........
-00000470: 0029 07da 0a69 7369 6e73 7461 6e63 65da  .)...isinstance.
-00000480: 0373 7472 da05 6279 7465 73da 0766 726f  .str..bytes..fro
-00000490: 6d68 6578 da05 7374 7269 70da 036c 656e  mhex..strip..len
-000004a0: da0d 4261 7365 4578 6365 7074 696f 6e29  ..BaseException)
-000004b0: 0272 1500 0000 da01 6172 0a00 0000 720a  .r......ar....r.
-000004c0: 0000 0072 0b00 0000 7214 0000 0018 0000  ...r....r.......
-000004d0: 0073 1000 0000 0002 0201 0a01 0e01 0c01  .s..............
-000004e0: 0602 0a01 0c01 7a13 4372 7970 7446 696c  ......z.CryptFil
-000004f0: 652e 6b65 7976 6572 6966 7963 0100 0000  e.keyverifyc....
-00000500: 0000 0000 0000 0000 0600 0000 0900 0000  ................
-00000510: 4300 0000 737a 0100 0074 006a 01a0 027c  C...sz...t.j...|
-00000520: 006a 03a1 0172 1264 0153 007c 006a 0464  .j...r.d.S.|.j.d
-00000530: 026b 0272 2064 0353 0090 017a 3c64 047d  .k.r d.S...z<d.}
-00000540: 0174 006a 01a0 057c 006a 03a1 0173 3c57  .t.j...|.j...s<W
-00000550: 0064 0553 0074 006a 01a0 067c 006a 03a1  .d.S.t.j...|.j..
-00000560: 0164 0219 0064 066b 0272 5857 0064 0753  .d...d.k.rXW.d.S
-00000570: 0074 077c 006a 0364 0883 028f 187d 027c  .t.|.j.d.....}.|
-00000580: 02a0 08a1 007d 0357 0064 0004 0004 0083  .....}.W.d......
-00000590: 0301 006e 1031 0073 8230 0001 0001 0001  ...n.1.s.0......
-000005a0: 0059 0001 0074 077c 006a 0364 0983 028f  .Y...t.|.j.d....
-000005b0: 8e7d 027c 0390 0072 fc7a 2a74 096a 0a7c  .}.|...r.z*t.j.|
-000005c0: 037c 006a 0b64 0a8d 027d 047c 04a0 0ca1  .|.j.d...}.|....
-000005d0: 007d 057c 02a0 0d7c 05a1 0101 0064 027d  .}.|...|.....d.}
-000005e0: 0157 006e 2e04 0074 0e90 0079 f801 0001  .W.n...t...y....
-000005f0: 0001 007c 02a0 0d7c 03a1 0101 0059 0057  ...|...|.....Y.W
-00000600: 0064 0004 0004 0083 0301 0057 0064 0453  .d.........W.d.S
-00000610: 0030 006e 1c7c 02a0 0d7c 03a1 0101 0057  .0.n.|...|.....W
-00000620: 0064 0004 0004 0083 0301 0057 0064 0b53  .d.........W.d.S
-00000630: 0057 0064 0004 0004 0083 0301 006e 1231  .W.d.........n.1
-00000640: 0090 0173 2e30 0001 0001 0001 0059 0001  ...s.0.......Y..
-00000650: 007c 0164 026b 0290 0172 5c74 00a0 0f7c  .|.d.k...r\t...|
-00000660: 006a 037c 006a 0364 0617 00a1 0201 0057  .j.|.j.d.......W
-00000670: 0064 0253 0057 006e 1604 0074 1090 0179  .d.S.W.n...t...y
-00000680: 7401 0001 0001 0059 0064 0c53 0030 0064  t......Y.d.S.0.d
-00000690: 0053 00a9 0d4e e907 0000 0072 1100 0000  .S...N.....r....
-000006a0: e905 0000 0072 0100 0000 e903 0000 007a  .....r.........z
-000006b0: 062e 6372 7970 74e9 0600 0000 5a02 7262  ..crypt.....Z.rb
-000006c0: da02 7762 2902 da07 6d65 7373 6167 655a  ..wb)...messageZ
-000006d0: 076d 6169 6e6b 6579 721a 0000 00e9 0400  .mainkeyr.......
-000006e0: 0000 2911 da02 6f73 da04 7061 7468 da05  ..)...os..path..
-000006f0: 6973 6469 7272 1200 0000 7213 0000 00da  isdirr....r.....
-00000700: 0665 7869 7374 73da 0873 706c 6974 6578  .exists..splitex
-00000710: 74da 046f 7065 6eda 0472 6561 6472 0200  t..open..readr..
-00000720: 0000 7217 0000 0072 1500 0000 5a0a 656e  ..r....r....Z.en
-00000730: 6354 6f42 7974 6573 da05 7772 6974 6572  cToBytes..writer
-00000740: 2100 0000 da06 7265 6e61 6d65 da09 4578  !.....rename..Ex
-00000750: 6365 7074 696f 6e29 0672 0700 0000 5a15  ception).r....Z.
-00000760: 676f 5f61 6865 6164 5f72 656e 616d 655f  go_ahead_rename_
-00000770: 6372 7970 74da 0166 5a0b 6669 6c65 636f  crypt..fZ.fileco
-00000780: 6e74 656e 74da 0369 6e73 5a0b 6e65 775f  ntent..insZ.new_
-00000790: 636f 6e74 656e 7472 0a00 0000 720a 0000  contentr....r...
-000007a0: 0072 0b00 0000 da07 656e 6372 7970 7424  .r......encrypt$
-000007b0: 0000 0073 3e00 0000 0001 0e01 0401 0a01  ...s>...........
-000007c0: 0401 0401 0401 0e01 0602 1601 0602 0e01  ................
-000007d0: 2601 0e01 0601 0201 0401 06ff 0602 0801  &...............
-000007e0: 0a01 0801 0e01 0a01 1802 0a01 3201 0a01  ............2...
-000007f0: 1401 0a01 0e01 7a11 4372 7970 7446 696c  ......z.CryptFil
-00000800: 652e 656e 6372 7970 7463 0100 0000 0000  e.encryptc......
-00000810: 0000 0000 0000 0600 0000 0900 0000 4300  ..............C.
-00000820: 0000 7382 0100 0074 006a 01a0 027c 006a  ..s....t.j...|.j
-00000830: 03a1 0172 1264 0153 007c 006a 0464 026b  ...r.d.S.|.j.d.k
-00000840: 0272 2064 0353 0090 017a 4464 047d 0174  .r d.S...zDd.}.t
-00000850: 006a 01a0 057c 006a 03a1 0173 3c57 0064  .j...|.j...s<W.d
-00000860: 0553 0074 006a 01a0 067c 006a 03a1 0164  .S.t.j...|.j...d
-00000870: 0219 0064 066b 0372 5857 0064 0753 0074  ...d.k.rXW.d.S.t
-00000880: 077c 006a 0364 0883 028f 187d 027c 02a0  .|.j.d.....}.|..
-00000890: 08a1 007d 0357 0064 0004 0004 0083 0301  ...}.W.d........
-000008a0: 006e 1031 0073 8230 0001 0001 0001 0059  .n.1.s.0.......Y
-000008b0: 0001 0074 077c 006a 0364 0983 028f 8e7d  ...t.|.j.d.....}
-000008c0: 027c 0390 0072 fc7a 2a74 096a 0a7c 037c  .|...r.z*t.j.|.|
-000008d0: 006a 0b64 0a8d 027d 047c 04a0 0ca1 007d  .j.d...}.|.....}
-000008e0: 057c 02a0 0d7c 05a1 0101 0064 027d 0157  .|...|.....d.}.W
-000008f0: 006e 2e04 0074 0e90 0079 f801 0001 0001  .n...t...y......
-00000900: 007c 02a0 0d7c 03a1 0101 0059 0057 0064  .|...|.....Y.W.d
-00000910: 0004 0004 0083 0301 0057 0064 0453 0030  .........W.d.S.0
-00000920: 006e 1c7c 02a0 0d7c 03a1 0101 0057 0064  .n.|...|.....W.d
-00000930: 0004 0004 0083 0301 0057 0064 0b53 0057  .........W.d.S.W
-00000940: 0064 0004 0004 0083 0301 006e 1231 0090  .d.........n.1..
-00000950: 0173 2e30 0001 0001 0001 0059 0001 007c  .s.0.......Y...|
-00000960: 0164 026b 0290 0172 6474 00a0 0f7c 006a  .d.k...rdt...|.j
-00000970: 0374 006a 01a0 067c 006a 03a1 0164 0419  .t.j...|.j...d..
-00000980: 00a1 0201 0057 0064 0253 0057 006e 1604  .....W.d.S.W.n..
-00000990: 0074 0e90 0179 7c01 0001 0001 0059 0064  .t...y|......Y.d
-000009a0: 0c53 0030 0064 0053 0072 2300 0000 2910  .S.0.d.S.r#...).
-000009b0: 722b 0000 0072 2c00 0000 722d 0000 0072  r+...r,...r-...r
-000009c0: 1200 0000 7213 0000 0072 2e00 0000 722f  ....r....r....r/
-000009d0: 0000 0072 3000 0000 7231 0000 0072 0200  ...r0...r1...r..
-000009e0: 0000 5a03 4465 6372 1500 0000 5a0a 6465  ..Z.Decr....Z.de
-000009f0: 6354 6f42 7974 6573 7232 0000 0072 3400  cToBytesr2...r4.
-00000a00: 0000 7233 0000 0029 0672 0700 0000 5a15  ..r3...).r....Z.
-00000a10: 676f 5f61 6865 6164 5f72 656d 6f76 655f  go_ahead_remove_
-00000a20: 6372 7970 7472 3500 0000 5a0b 656e 635f  cryptr5...Z.enc_
-00000a30: 636f 6e74 656e 7472 3600 0000 7222 0000  contentr6...r"..
-00000a40: 0072 0a00 0000 720a 0000 0072 0b00 0000  .r....r....r....
-00000a50: da07 6465 6372 7970 7447 0000 0073 4a00  ..decryptG...sJ.
-00000a60: 0000 0001 0e01 0401 0a01 0401 0401 0401  ................
-00000a70: 0e01 0602 1601 0602 0e01 2601 0e01 0601  ..........&.....
-00000a80: 0201 0401 06ff 0602 0801 0a01 0801 0e01  ................
-00000a90: 0a01 1802 0a01 3201 0a01 0401 0a01 04ff  ......2.........
-00000aa0: 0201 02ff 02ff 0403 0a01 0e01 7a11 4372  ............z.Cr
-00000ab0: 7970 7446 696c 652e 6465 6372 7970 7463  yptFile.decryptc
-00000ac0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00000ad0: 0500 0000 4300 0000 7316 0000 0064 017c  ....C...s....d.|
-00000ae0: 006a 009b 0064 027c 006a 019b 0064 039d  .j...d.|.j...d..
-00000af0: 0553 0029 044e 7a1b 456e 6372 7970 7469  .S.).Nz.Encrypti
-00000b00: 6e67 2f44 6563 7279 7074 696e 6720 4669  ng/Decrypting Fi
-00000b10: 6c65 207a 0620 5769 7468 207a 0520 4b65  le z. With z. Ke
-00000b20: 7920 2902 7212 0000 0072 1500 0000 7206  y ).r....r....r.
-00000b30: 0000 0072 0a00 0000 720a 0000 0072 0b00  ...r....r....r..
-00000b40: 0000 da07 5f5f 7374 725f 5f6c 0000 0073  ....__str__l...s
-00000b50: 0200 0000 0001 7a11 4372 7970 7446 696c  ......z.CryptFil
-00000b60: 652e 5f5f 7374 725f 5f63 0100 0000 0000  e.__str__c......
-00000b70: 0000 0000 0000 0100 0000 0600 0000 4300  ..............C.
-00000b80: 0000 731e 0000 007c 006a 006a 019b 0064  ..s....|.j.j...d
-00000b90: 017c 006a 029b 0064 027c 006a 039b 0064  .|.j...d.|.j...d
-00000ba0: 039d 0653 0029 044e fa01 28fa 012c fa01  ...S.).N..(..,..
-00000bb0: 2929 0472 0900 0000 720c 0000 0072 1200  )).r....r....r..
-00000bc0: 0000 7215 0000 0072 0600 0000 720a 0000  ..r....r....r...
-00000bd0: 0072 0a00 0000 720b 0000 00da 085f 5f72  .r....r......__r
-00000be0: 6570 725f 5f6f 0000 0073 0200 0000 0001  epr__o...s......
-00000bf0: 7a12 4372 7970 7446 696c 652e 5f5f 7265  z.CryptFile.__re
-00000c00: 7072 5f5f 4e29 0d72 0c00 0000 720d 0000  pr__N).r....r...
-00000c10: 0072 0e00 0000 7205 0000 00da 0c73 7461  .r....r......sta
-00000c20: 7469 636d 6574 686f 6472 1c00 0000 7218  ticmethodr....r.
-00000c30: 0000 00da 0369 6e74 7214 0000 0072 3700  .....intr....r7.
-00000c40: 0000 7238 0000 0072 3900 0000 723d 0000  ..r8...r9...r=..
-00000c50: 0072 0a00 0000 720a 0000 0072 0a00 0000  .r....r....r....
-00000c60: 720b 0000 0072 1000 0000 0b00 0000 7312  r....r........s.
-00000c70: 0000 0008 0108 0802 0110 0302 0112 0b0e  ................
-00000c80: 230e 2508 0372 1000 0000 2906 da08 4173  #.%..r....)...As
-00000c90: 6843 7279 7074 7202 0000 0072 2b00 0000  hCryptr....r+...
-00000ca0: 7234 0000 0072 0300 0000 7210 0000 0072  r4...r....r....r
-00000cb0: 0a00 0000 720a 0000 0072 0a00 0000 720b  ....r....r....r.
-00000cc0: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000cd0: 0073 0600 0000 0c01 0803 1006            .s..........
+000000b0: 0e4b 6579 4c65 6e67 7468 4572 726f 7263  .KeyLengthErrorc
+000000c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000000d0: 0300 0000 0300 0000 7318 0000 0064 017c  ........s....d.|
+000000e0: 005f 0074 0183 00a0 027c 006a 00a1 0101  ._.t.....|.j....
+000000f0: 0064 0053 0029 024e 7a1a 4b65 7920 6d75  .d.S.).Nz.Key mu
+00000100: 7374 2062 6520 3235 3620 4269 7420 6c6f  st be 256 Bit lo
+00000110: 6e67 2021 2903 5a07 6469 7370 6c61 79da  ng !).Z.display.
+00000120: 0573 7570 6572 da08 5f5f 696e 6974 5f5f  .super..__init__
+00000130: a901 da04 7365 6c66 a901 da09 5f5f 636c  ....self....__cl
+00000140: 6173 735f 5fa9 00fa 3043 3a5c 576f 726b  ass__...0C:\Work
+00000150: 5c47 6974 4875 6257 6f72 6b5c 4145 532d  \GitHubWork\AES-
+00000160: 3235 365c 4173 6843 7279 7074 5c46 696c  256\AshCrypt\Fil
+00000170: 6543 7279 7074 2e70 7972 0500 0000 0600  eCrypt.pyr......
+00000180: 0000 7304 0000 0000 0106 017a 174b 6579  ..s........z.Key
+00000190: 4c65 6e67 7468 4572 726f 722e 5f5f 696e  LengthError.__in
+000001a0: 6974 5f5f 2905 da08 5f5f 6e61 6d65 5f5f  it__)...__name__
+000001b0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+000001c0: 7175 616c 6e61 6d65 5f5f 7205 0000 00da  qualname__r.....
+000001d0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 720a  .__classcell__r.
+000001e0: 0000 0072 0a00 0000 7208 0000 0072 0b00  ...r....r....r..
+000001f0: 0000 7203 0000 0005 0000 0073 0200 0000  ..r........s....
+00000200: 0801 7203 0000 0063 0000 0000 0000 0000  ..r....c........
+00000210: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
+00000220: 7366 0000 0065 005a 0164 005a 0264 0164  sf...e.Z.d.Z.d.d
+00000230: 0284 005a 0365 0465 0564 039c 0164 0464  ...Z.e.e.d...d.d
+00000240: 0584 0483 015a 0665 0465 0565 0764 069c  .....Z.e.e.e.d..
+00000250: 0264 0764 0884 0483 015a 0865 0764 039c  .d.d.....Z.e.d..
+00000260: 0164 0964 0a84 045a 0965 0764 039c 0164  .d.d...Z.e.d...d
+00000270: 0b64 0c84 045a 0a64 0d64 0e84 005a 0b64  .d...Z.d.d...Z.d
+00000280: 0f64 1084 005a 0c64 1153 0029 12da 0943  .d...Z.d.S.)...C
+00000290: 7279 7074 4669 6c65 6303 0000 0000 0000  ryptFilec.......
+000002a0: 0000 0000 0003 0000 0003 0000 0043 0000  .............C..
+000002b0: 0073 2c00 0000 7c01 7c00 5f00 6401 7c00  .s,...|.|._.d.|.
+000002c0: 5f01 7c00 a002 7c02 a101 6402 6b02 7222  _.|...|...d.k.r"
+000002d0: 7c02 7c00 5f03 6e06 6402 7c00 5f01 6400  |.|._.n.d.|._.d.
+000002e0: 5300 2903 4e72 0100 0000 e901 0000 0029  S.).Nr.........)
+000002f0: 04da 0866 696c 656e 616d 65da 0f6e 6f74  ...filename..not
+00000300: 5f32 3536 5f62 6974 5f6b 6579 da09 6b65  _256_bit_key..ke
+00000310: 7976 6572 6966 79da 036b 6579 2903 7207  yverify..key).r.
+00000320: 0000 0072 1200 0000 7215 0000 0072 0a00  ...r....r....r..
+00000330: 0000 720a 0000 0072 0b00 0000 7205 0000  ..r....r....r...
+00000340: 000c 0000 0073 0a00 0000 0001 0601 0601  .....s..........
+00000350: 0e01 0802 7a12 4372 7970 7446 696c 652e  ....z.CryptFile.
+00000360: 5f5f 696e 6974 5f5f 2901 da06 7265 7475  __init__)...retu
+00000370: 726e 6300 0000 0000 0000 0000 0000 0000  rnc.............
+00000380: 0000 0002 0000 0043 0000 0073 0a00 0000  .......C...s....
+00000390: 7400 6a01 a002 a100 5300 2901 4e29 0372  t.j.....S.).N).r
+000003a0: 0200 0000 da03 456e 63da 0667 656e 6b65  ......Enc..genke
+000003b0: 7972 0a00 0000 720a 0000 0072 0a00 0000  yr....r....r....
+000003c0: 720b 0000 0072 1800 0000 1400 0000 7302  r....r........s.
+000003d0: 0000 0000 027a 1043 7279 7074 4669 6c65  .....z.CryptFile
+000003e0: 2e67 656e 6b65 7929 0272 1500 0000 7216  .genkey).r....r.
+000003f0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+00000400: 0200 0000 0800 0000 4300 0000 734e 0000  ........C...sN..
+00000410: 007a 3474 007c 0074 0183 0272 3274 02a0  .z4t.|.t...r2t..
+00000420: 037c 00a0 04a1 00a1 017d 0174 057c 0183  .|.......}.t.|..
+00000430: 0164 016b 0272 2c57 0064 0253 0057 0064  .d.k.r,W.d.S.W.d
+00000440: 0353 0057 006e 1404 0074 0679 4801 0001  .S.W.n...t.yH...
+00000450: 0001 0059 0064 0453 0030 0064 0053 0029  ...Y.d.S.0.d.S.)
+00000460: 054e e920 0000 0072 1100 0000 7201 0000  .N. ...r....r...
+00000470: 00e9 0200 0000 2907 da0a 6973 696e 7374  ......)...isinst
+00000480: 616e 6365 da03 7374 72da 0562 7974 6573  ance..str..bytes
+00000490: da07 6672 6f6d 6865 78da 0573 7472 6970  ..fromhex..strip
+000004a0: da03 6c65 6eda 0d42 6173 6545 7863 6570  ..len..BaseExcep
+000004b0: 7469 6f6e 2902 7215 0000 00da 0161 720a  tion).r......ar.
+000004c0: 0000 0072 0a00 0000 720b 0000 0072 1400  ...r....r....r..
+000004d0: 0000 1800 0000 7310 0000 0000 0202 010a  ......s.........
+000004e0: 010e 010c 0106 020a 010c 017a 1343 7279  ...........z.Cry
+000004f0: 7074 4669 6c65 2e6b 6579 7665 7269 6679  ptFile.keyverify
+00000500: 6301 0000 0000 0000 0000 0000 0006 0000  c...............
+00000510: 0009 0000 0043 0000 0073 7401 0000 7400  .....C...st...t.
+00000520: 6a01 a002 7c00 6a03 a101 7212 6401 5300  j...|.j...r.d.S.
+00000530: 7c00 6a04 6402 6b02 7220 6403 5300 9001  |.j.d.k.r d.S...
+00000540: 7a36 7400 6a01 a005 7c00 6a03 a101 7338  z6t.j...|.j...s8
+00000550: 5700 6404 5300 7400 6a01 a006 7c00 6a03  W.d.S.t.j...|.j.
+00000560: a101 6402 1900 6405 6b02 7254 5700 6406  ..d...d.k.rTW.d.
+00000570: 5300 7407 7c00 6a03 6407 8302 8f18 7d01  S.t.|.j.d.....}.
+00000580: 7c01 a008 a100 7d02 5700 6400 0400 0400  |.....}.W.d.....
+00000590: 8303 0100 6e10 3100 737e 3000 0100 0100  ....n.1.s~0.....
+000005a0: 0100 5900 0100 7407 7c00 6a03 6408 8302  ..Y...t.|.j.d...
+000005b0: 8f8c 7d01 7c02 9000 72f6 7a2a 7409 6a0a  ..}.|...r.z*t.j.
+000005c0: 7c02 7c00 6a0b 6409 8d02 7d03 7c03 a00c  |.|.j.d...}.|...
+000005d0: a100 7d04 7c01 a00d 7c04 a101 0100 6402  ..}.|...|.....d.
+000005e0: 7d05 5700 6e2c 0400 740e 79f2 0100 0100  }.W.n,..t.y.....
+000005f0: 0100 7c01 a00d 7c02 a101 0100 5900 5700  ..|...|.....Y.W.
+00000600: 6400 0400 0400 8303 0100 5700 640a 5300  d.........W.d.S.
+00000610: 3000 6e1c 7c01 a00d 7c02 a101 0100 5700  0.n.|...|.....W.
+00000620: 6400 0400 0400 8303 0100 5700 640b 5300  d.........W.d.S.
+00000630: 5700 6400 0400 0400 8303 0100 6e12 3100  W.d.........n.1.
+00000640: 9001 7328 3000 0100 0100 0100 5900 0100  ..s(0.......Y...
+00000650: 7c05 6402 6b02 9001 7256 7400 a00f 7c00  |.d.k...rVt...|.
+00000660: 6a03 7c00 6a03 6405 1700 a102 0100 5700  j.|.j.d.......W.
+00000670: 6402 5300 5700 6e16 0400 7410 9001 796e  d.S.W.n...t...yn
+00000680: 0100 0100 0100 5900 640c 5300 3000 6400  ......Y.d.S.0.d.
+00000690: 5300 a90d 4ee9 0700 0000 7211 0000 00e9  S...N.....r.....
+000006a0: 0500 0000 e903 0000 007a 062e 6372 7970  .........z..cryp
+000006b0: 74e9 0600 0000 5a02 7262 da02 7762 2902  t.....Z.rb..wb).
+000006c0: da07 6d65 7373 6167 655a 076d 6169 6e6b  ..messageZ.maink
+000006d0: 6579 7201 0000 0072 1a00 0000 e904 0000  eyr....r........
+000006e0: 0029 11da 026f 73da 0470 6174 68da 0569  .)...os..path..i
+000006f0: 7364 6972 7212 0000 0072 1300 0000 da06  sdirr....r......
+00000700: 6578 6973 7473 da08 7370 6c69 7465 7874  exists..splitext
+00000710: da04 6f70 656e da04 7265 6164 7202 0000  ..open..readr...
+00000720: 0072 1700 0000 7215 0000 005a 0c65 6e63  .r....r....Z.enc
+00000730: 5f74 6f5f 6279 7465 73da 0577 7269 7465  _to_bytes..write
+00000740: 7221 0000 00da 0672 656e 616d 65da 0945  r!.....rename..E
+00000750: 7863 6570 7469 6f6e 2906 7207 0000 00da  xception).r.....
+00000760: 0166 5a0b 6669 6c65 636f 6e74 656e 74da  .fZ.filecontent.
+00000770: 0369 6e73 5a0b 6e65 775f 636f 6e74 656e  .insZ.new_conten
+00000780: 745a 1567 6f5f 6168 6561 645f 7265 6e61  tZ.go_ahead_rena
+00000790: 6d65 5f63 7279 7074 720a 0000 0072 0a00  me_cryptr....r..
+000007a0: 0000 720b 0000 00da 0765 6e63 7279 7074  ..r......encrypt
+000007b0: 2400 0000 733c 0000 0000 010e 0104 010a  $...s<..........
+000007c0: 0104 0104 010e 0106 0216 0106 020e 0126  ...............&
+000007d0: 010e 0106 0102 0104 0106 ff06 0208 010a  ................
+000007e0: 0108 010c 010a 0118 020a 0132 010a 0114  ...........2....
+000007f0: 010a 010e 017a 1143 7279 7074 4669 6c65  .....z.CryptFile
+00000800: 2e65 6e63 7279 7074 6301 0000 0000 0000  .encryptc.......
+00000810: 0000 0000 0006 0000 0009 0000 0043 0000  .............C..
+00000820: 0073 7c01 0000 7400 6a01 a002 7c00 6a03  .s|...t.j...|.j.
+00000830: a101 7212 6401 5300 7c00 6a04 6402 6b02  ..r.d.S.|.j.d.k.
+00000840: 7220 6403 5300 9001 7a3e 7400 6a01 a005  r d.S...z>t.j...
+00000850: 7c00 6a03 a101 7338 5700 6404 5300 7400  |.j...s8W.d.S.t.
+00000860: 6a01 a006 7c00 6a03 a101 6402 1900 6405  j...|.j...d...d.
+00000870: 6b03 7254 5700 6406 5300 7407 7c00 6a03  k.rTW.d.S.t.|.j.
+00000880: 6407 8302 8f18 7d01 7c01 a008 a100 7d02  d.....}.|.....}.
+00000890: 5700 6400 0400 0400 8303 0100 6e10 3100  W.d.........n.1.
+000008a0: 737e 3000 0100 0100 0100 5900 0100 7407  s~0.......Y...t.
+000008b0: 7c00 6a03 6408 8302 8f8c 7d01 7c02 9000  |.j.d.....}.|...
+000008c0: 72f6 7a2a 7409 6a0a 7c02 7c00 6a0b 6409  r.z*t.j.|.|.j.d.
+000008d0: 8d02 7d03 7c03 a00c a100 7d04 7c01 a00d  ..}.|.....}.|...
+000008e0: 7c04 a101 0100 6402 7d05 5700 6e2c 0400  |.....d.}.W.n,..
+000008f0: 740e 79f2 0100 0100 0100 7c01 a00d 7c02  t.y.......|...|.
+00000900: a101 0100 5900 5700 6400 0400 0400 8303  ....Y.W.d.......
+00000910: 0100 5700 640a 5300 3000 6e1c 7c01 a00d  ..W.d.S.0.n.|...
+00000920: 7c02 a101 0100 5700 6400 0400 0400 8303  |.....W.d.......
+00000930: 0100 5700 640b 5300 5700 6400 0400 0400  ..W.d.S.W.d.....
+00000940: 8303 0100 6e12 3100 9001 7328 3000 0100  ....n.1...s(0...
+00000950: 0100 0100 5900 0100 7c05 6402 6b02 9001  ....Y...|.d.k...
+00000960: 725e 7400 a00f 7c00 6a03 7400 6a01 a006  r^t...|.j.t.j...
+00000970: 7c00 6a03 a101 640a 1900 a102 0100 5700  |.j...d.......W.
+00000980: 6402 5300 5700 6e16 0400 740e 9001 7976  d.S.W.n...t...yv
+00000990: 0100 0100 0100 5900 640c 5300 3000 6400  ......Y.d.S.0.d.
+000009a0: 5300 7223 0000 0029 1072 2b00 0000 722c  S.r#...).r+...r,
+000009b0: 0000 0072 2d00 0000 7212 0000 0072 1300  ...r-...r....r..
+000009c0: 0000 722e 0000 0072 2f00 0000 7230 0000  ..r....r/...r0..
+000009d0: 0072 3100 0000 7202 0000 005a 0344 6563  .r1...r....Z.Dec
+000009e0: 7215 0000 005a 0c64 6563 5f74 6f5f 6279  r....Z.dec_to_by
+000009f0: 7465 7372 3200 0000 7234 0000 0072 3300  tesr2...r4...r3.
+00000a00: 0000 2906 7207 0000 0072 3500 0000 5a0b  ..).r....r5...Z.
+00000a10: 656e 635f 636f 6e74 656e 7472 3600 0000  enc_contentr6...
+00000a20: 7222 0000 005a 1567 6f5f 6168 6561 645f  r"...Z.go_ahead_
+00000a30: 7265 6d6f 7665 5f63 7279 7074 720a 0000  remove_cryptr...
+00000a40: 0072 0a00 0000 720b 0000 00da 0764 6563  .r....r......dec
+00000a50: 7279 7074 4600 0000 7348 0000 0000 010e  ryptF...sH......
+00000a60: 0104 010a 0104 0104 010e 0106 0216 0106  ................
+00000a70: 020e 0126 010e 0106 0102 0104 0106 ff06  ...&............
+00000a80: 0208 010a 0108 010c 010a 0118 020a 0132  ...............2
+00000a90: 010a 0104 010a 0104 ff02 0102 ff02 ff04  ................
+00000aa0: 030a 010e 017a 1143 7279 7074 4669 6c65  .....z.CryptFile
+00000ab0: 2e64 6563 7279 7074 6301 0000 0000 0000  .decryptc.......
+00000ac0: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00000ad0: 0073 1600 0000 6401 7c00 6a00 9b00 6402  .s....d.|.j...d.
+00000ae0: 7c00 6a01 9b00 6403 9d05 5300 2904 4e7a  |.j...d...S.).Nz
+00000af0: 1b45 6e63 7279 7074 696e 672f 4465 6372  .Encrypting/Decr
+00000b00: 7970 7469 6e67 2046 696c 6520 7a06 2057  ypting File z. W
+00000b10: 6974 6820 7a05 204b 6579 2029 0272 1200  ith z. Key ).r..
+00000b20: 0000 7215 0000 0072 0600 0000 720a 0000  ..r....r....r...
+00000b30: 0072 0a00 0000 720b 0000 00da 075f 5f73  .r....r......__s
+00000b40: 7472 5f5f 6a00 0000 7302 0000 0000 017a  tr__j...s......z
+00000b50: 1143 7279 7074 4669 6c65 2e5f 5f73 7472  .CryptFile.__str
+00000b60: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
+00000b70: 0000 0006 0000 0043 0000 0073 1e00 0000  .......C...s....
+00000b80: 7c00 6a00 6a01 9b00 6401 7c00 6a02 9b00  |.j.j...d.|.j...
+00000b90: 6402 7c00 6a03 9b00 6403 9d06 5300 2904  d.|.j...d...S.).
+00000ba0: 4efa 0128 fa01 2cfa 0129 2904 7209 0000  N..(..,..)).r...
+00000bb0: 0072 0c00 0000 7212 0000 0072 1500 0000  .r....r....r....
+00000bc0: 7206 0000 0072 0a00 0000 720a 0000 0072  r....r....r....r
+00000bd0: 0b00 0000 da08 5f5f 7265 7072 5f5f 6d00  ......__repr__m.
+00000be0: 0000 7302 0000 0000 017a 1243 7279 7074  ..s......z.Crypt
+00000bf0: 4669 6c65 2e5f 5f72 6570 725f 5f4e 290d  File.__repr__N).
+00000c00: 720c 0000 0072 0d00 0000 720e 0000 0072  r....r....r....r
+00000c10: 0500 0000 da0c 7374 6174 6963 6d65 7468  ......staticmeth
+00000c20: 6f64 721c 0000 0072 1800 0000 da03 696e  odr....r......in
+00000c30: 7472 1400 0000 7237 0000 0072 3800 0000  tr....r7...r8...
+00000c40: 7239 0000 0072 3d00 0000 720a 0000 0072  r9...r=...r....r
+00000c50: 0a00 0000 720a 0000 0072 0b00 0000 7210  ....r....r....r.
+00000c60: 0000 000b 0000 0073 1200 0000 0801 0808  .......s........
+00000c70: 0201 1003 0201 120b 0e22 0e24 0803 7210  .........".$..r.
+00000c80: 0000 0029 06da 0841 7368 4372 7970 7472  ...)...AshCryptr
+00000c90: 0200 0000 722b 0000 0072 3400 0000 7203  ....r+...r4...r.
+00000ca0: 0000 0072 1000 0000 720a 0000 0072 0a00  ...r....r....r..
+00000cb0: 0000 720a 0000 0072 0b00 0000 da08 3c6d  ..r....r......<m
+00000cc0: 6f64 756c 653e 0100 0000 7306 0000 000c  odule>....s.....
+00000cd0: 0108 0310 06                             .....
```

### Comparing `AshCrypt-1.3.6/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc` & `AshCrypt-2.0.0/AshCrypt/__pycache__/TextCrypt.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Tue Jul 11 22:47:20 2023 UTC, .py size: 1799 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,152 +1,153 @@
-00000000: 610d 0d0a 0000 0000 f8db ad64 0707 0000  a..........d....
+00000000: 610d 0d0a 0000 0000 dbe9 b364 0507 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3a00 0000 6400  .....@...s:...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 4700 6403 6404 8400 6404  m.Z...G.d.d...d.
 00000050: 6504 8303 5a05 4700 6405 6406 8400 6406  e...Z.G.d.d...d.
 00000060: 8302 5a06 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
 00000070: 01da 0555 6e69 6f6e 2901 da03 4173 6863  ...Union)...Ashc
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0300 0000 0000 0000 731c 0000 0065 005a  ........s....e.Z
 000000a0: 0164 005a 0287 0066 0164 0164 0284 085a  .d.Z...f.d.d...Z
-000000b0: 0387 0004 005a 0453 0029 03da 084b 6579  .....Z.S.)...Key
-000000c0: 4572 726f 7263 0100 0000 0000 0000 0000  Errorc..........
-000000d0: 0000 0100 0000 0300 0000 0300 0000 7318  ..............s.
-000000e0: 0000 0064 017c 005f 0074 0183 00a0 027c  ...d.|._.t.....|
-000000f0: 006a 00a1 0101 0064 0053 0029 024e 7a1a  .j.....d.S.).Nz.
-00000100: 4b65 7920 6d75 7374 2062 6520 3235 3620  Key must be 256 
-00000110: 4269 7420 6c6f 6e67 2021 2903 da07 6469  Bit long !)...di
-00000120: 7370 6c61 79da 0573 7570 6572 da08 5f5f  splay..super..__
-00000130: 696e 6974 5f5f a901 da04 7365 6c66 a901  init__....self..
-00000140: da09 5f5f 636c 6173 735f 5fa9 00fa 3043  ..__class__...0C
-00000150: 3a5c 576f 726b 5c47 6974 4875 6257 6f72  :\Work\GitHubWor
-00000160: 6b5c 4145 532d 3235 365c 4173 6843 7279  k\AES-256\AshCry
-00000170: 7074 5c54 6578 7443 7279 7074 2e70 7972  pt\TextCrypt.pyr
-00000180: 0700 0000 0600 0000 7304 0000 0000 0106  ........s.......
-00000190: 017a 114b 6579 4572 726f 722e 5f5f 696e  .z.KeyError.__in
-000001a0: 6974 5f5f 2905 da08 5f5f 6e61 6d65 5f5f  it__)...__name__
-000001b0: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-000001c0: 7175 616c 6e61 6d65 5f5f 7207 0000 00da  qualname__r.....
-000001d0: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 720c  .__classcell__r.
-000001e0: 0000 0072 0c00 0000 720a 0000 0072 0d00  ...r....r....r..
-000001f0: 0000 7204 0000 0005 0000 0073 0200 0000  ..r........s....
-00000200: 0801 7204 0000 0063 0000 0000 0000 0000  ..r....c........
-00000210: 0000 0000 0000 0000 0400 0000 4000 0000  ............@...
-00000220: 7376 0000 0065 005a 0164 005a 0265 0365  sv...e.Z.d.Z.e.e
-00000230: 0465 0566 0219 0065 0464 019c 0264 0264  .e.f...e.d...d.d
-00000240: 0384 045a 0665 0765 0464 049c 0164 0564  ...Z.e.e.d...d.d
-00000250: 0684 0483 015a 0865 0765 0465 0964 079c  .....Z.e.e.e.d..
-00000260: 0264 0864 0984 0483 015a 0a65 0b64 049c  .d.d.....Z.e.d..
-00000270: 0164 0a64 0b84 045a 0c65 0b64 049c 0164  .d.d...Z.e.d...d
-00000280: 0c64 0d84 045a 0d64 0e64 0f84 005a 0e64  .d...Z.d.d...Z.d
-00000290: 1064 1184 005a 0f64 1253 0029 13da 0543  .d...Z.d.S.)...C
-000002a0: 7279 7074 a902 da04 7465 7874 da03 6b65  rypt....text..ke
-000002b0: 7963 0300 0000 0000 0000 0000 0000 0300  yc..............
-000002c0: 0000 0300 0000 4300 0000 7326 0000 007c  ......C...s&...|
-000002d0: 017c 005f 007c 00a0 017c 02a1 0164 016b  .|._.|...|...d.k
-000002e0: 0272 1c7c 027c 005f 026e 0674 0383 0082  .r.|.|._.n.t....
-000002f0: 0164 0053 0029 024e e901 0000 0029 0472  .d.S.).N.....).r
-00000300: 1400 0000 da09 6b65 7976 6572 6966 7972  ......keyverifyr
-00000310: 1500 0000 7204 0000 0029 0372 0900 0000  ....r....).r....
-00000320: 7214 0000 0072 1500 0000 720c 0000 0072  r....r....r....r
-00000330: 0c00 0000 720d 0000 0072 0700 0000 0c00  ....r....r......
-00000340: 0000 7308 0000 0000 0106 010e 0108 027a  ..s............z
-00000350: 0e43 7279 7074 2e5f 5f69 6e69 745f 5f29  .Crypt.__init__)
-00000360: 01da 0672 6574 7572 6e63 0000 0000 0000  ...returnc......
-00000370: 0000 0000 0000 0000 0000 0200 0000 4300  ..............C.
-00000380: 0000 730a 0000 0074 006a 01a0 02a1 0053  ..s....t.j.....S
-00000390: 0029 014e 2903 7203 0000 00da 0345 6e63  .).N).r......Enc
-000003a0: da0a 6765 6e4d 6169 6e6b 6579 720c 0000  ..genMainkeyr...
-000003b0: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-000003c0: da06 6765 6e6b 6579 1300 0000 7302 0000  ..genkey....s...
-000003d0: 0000 027a 0c43 7279 7074 2e67 656e 6b65  ...z.Crypt.genke
-000003e0: 7929 0272 1500 0000 7218 0000 0063 0100  y).r....r....c..
-000003f0: 0000 0000 0000 0000 0000 0200 0000 0800  ................
-00000400: 0000 4300 0000 734e 0000 0074 007c 0074  ..C...sN...t.|.t
-00000410: 0183 0272 467a 2474 02a0 037c 00a0 04a1  ...rFz$t...|....
-00000420: 00a1 017d 0174 057c 0183 0164 016b 0272  ...}.t.|...d.k.r
-00000430: 2c57 0064 0253 0057 0071 4a04 0074 0679  ,W.d.S.W.qJ..t.y
-00000440: 4201 0001 0001 0059 0064 0353 0030 006e  B......Y.d.S.0.n
-00000450: 0464 0453 0064 0053 0029 054e e920 0000  .d.S.d.S.).N. ..
-00000460: 0072 1600 0000 7201 0000 00e9 0200 0000  .r....r.........
-00000470: 2907 da0a 6973 696e 7374 616e 6365 da03  )...isinstance..
-00000480: 7374 72da 0562 7974 6573 da07 6672 6f6d  str..bytes..from
-00000490: 6865 78da 0573 7472 6970 da03 6c65 6eda  hex..strip..len.
-000004a0: 0945 7863 6570 7469 6f6e 2902 7215 0000  .Exception).r...
-000004b0: 00da 0161 720c 0000 0072 0c00 0000 720d  ...ar....r....r.
-000004c0: 0000 0072 1700 0000 1700 0000 7310 0000  ...r........s...
-000004d0: 0000 020a 0102 010e 010c 010a 010c 010a  ................
-000004e0: 037a 0f43 7279 7074 2e6b 6579 7665 7269  .z.Crypt.keyveri
-000004f0: 6679 6301 0000 0000 0000 0000 0000 0004  fyc.............
-00000500: 0000 0008 0000 0043 0000 0073 5200 0000  .......C...sR...
-00000510: 7c00 6a00 724a 7a22 7401 a002 7c00 6a00  |.j.rJz"t...|.j.
-00000520: 7c00 6a03 a102 7d01 7c01 a004 a100 7d02  |.j...}.|.....}.
-00000530: 6401 7c02 6602 5700 5300 0400 7405 7946  d.|.f.W.S...t.yF
-00000540: 0100 0100 0100 6402 7d03 6403 7c03 6602  ......d.}.d.|.f.
-00000550: 0600 5900 5300 3000 6e04 6404 5300 6400  ..Y.S.0.n.d.S.d.
-00000560: 5300 2905 4e72 1600 0000 da01 4572 0100  S.).Nr......Er..
-00000570: 0000 a902 e700 0000 0000 0000 0072 2800  .............r(.
-00000580: 0000 2906 7214 0000 0072 0300 0000 7219  ..).r....r....r.
-00000590: 0000 0072 1500 0000 da08 656e 6354 6f53  ...r......encToS
-000005a0: 7472 da0d 4261 7365 4578 6365 7074 696f  tr..BaseExceptio
-000005b0: 6e29 0472 0900 0000 da03 696e 73da 0b6e  n).r......ins..n
-000005c0: 6577 5f63 6f6e 7465 6e74 da06 6f75 7470  ew_content..outp
-000005d0: 7574 720c 0000 0072 0c00 0000 720d 0000  utr....r....r...
-000005e0: 00da 0765 6e63 7279 7074 2400 0000 7312  ...encrypt$...s.
-000005f0: 0000 0000 0106 0102 0110 0108 010a 010c  ................
-00000600: 0104 0110 027a 0d43 7279 7074 2e65 6e63  .....z.Crypt.enc
-00000610: 7279 7074 6301 0000 0000 0000 0000 0000  ryptc...........
-00000620: 0004 0000 0008 0000 0043 0000 0073 5a00  .........C...sZ.
-00000630: 0000 7c00 6a00 7252 7a28 7401 6a02 7c00  ..|.j.rRz(t.j.|.
-00000640: 6a00 7c00 6a03 6401 8d02 7d01 7c01 a004  j.|.j.d...}.|...
-00000650: a100 7d02 7c02 7d03 6402 7c03 6602 5700  ..}.|.}.d.|.f.W.
-00000660: 5300 0400 7405 794e 0100 0100 0100 7c00  S...t.yN......|.
-00000670: 6a00 7d03 6403 7c03 6602 0600 5900 5300  j.}.d.|.f...Y.S.
-00000680: 3000 6e04 6404 5300 6400 5300 2905 4e29  0.n.d.S.d.S.).N)
-00000690: 02da 076d 6573 7361 6765 da07 6d61 696e  ...message..main
-000006a0: 6b65 7972 1600 0000 7201 0000 0072 2700  keyr....r....r'.
-000006b0: 0000 2906 7214 0000 0072 0300 0000 da03  ..).r....r......
-000006c0: 4465 6372 1500 0000 da08 6465 6354 6f53  Decr......decToS
-000006d0: 7472 7224 0000 0029 0472 0900 0000 5a0c  trr$...).r....Z.
-000006e0: 6465 635f 696e 7374 616e 6365 7225 0000  dec_instancer%..
-000006f0: 0072 2d00 0000 720c 0000 0072 0c00 0000  .r-...r....r....
-00000700: 720d 0000 00da 0764 6563 7279 7074 3000  r......decrypt0.
-00000710: 0000 7314 0000 0000 0106 0102 0112 0108  ..s.............
-00000720: 0104 010a 010c 0106 0110 027a 0d43 7279  ...........z.Cry
-00000730: 7074 2e64 6563 7279 7074 6301 0000 0000  pt.decryptc.....
-00000740: 0000 0000 0000 0001 0000 0005 0000 0043  ...............C
-00000750: 0000 0073 1e00 0000 6401 7c00 6a00 6400  ...s....d.|.j.d.
-00000760: 6402 8502 1900 9b00 6403 7c00 6a01 9b00  d.......d.|.j...
-00000770: 6404 9d05 5300 2905 4e7a 1b45 6e63 7279  d...S.).Nz.Encry
-00000780: 7074 696e 672f 4465 6372 7970 7469 6e67  pting/Decrypting
-00000790: 2054 6578 7420 e908 0000 007a 082e 2e20   Text .....z... 
-000007a0: 5769 7468 207a 0520 4b65 7920 7213 0000  With z. Key r...
-000007b0: 0072 0800 0000 720c 0000 0072 0c00 0000  .r....r....r....
-000007c0: 720d 0000 00da 075f 5f73 7472 5f5f 3d00  r......__str__=.
-000007d0: 0000 7302 0000 0000 017a 0d43 7279 7074  ..s......z.Crypt
-000007e0: 2e5f 5f73 7472 5f5f 6301 0000 0000 0000  .__str__c.......
-000007f0: 0000 0000 0001 0000 0006 0000 0043 0000  .............C..
-00000800: 0073 2600 0000 7c00 6a00 6a01 9b00 6401  .s&...|.j.j...d.
-00000810: 7c00 6a02 6400 6402 8502 1900 9b00 6403  |.j.d.d.......d.
-00000820: 7c00 6a03 9b00 6404 9d06 5300 2905 4efa  |.j...d...S.).N.
-00000830: 0128 7234 0000 00fa 012c fa01 2929 0472  .(r4.....,..)).r
-00000840: 0b00 0000 720e 0000 0072 1400 0000 7215  ....r....r....r.
-00000850: 0000 0072 0800 0000 720c 0000 0072 0c00  ...r....r....r..
-00000860: 0000 720d 0000 00da 085f 5f72 6570 725f  ..r......__repr_
-00000870: 5f40 0000 0073 0200 0000 0001 7a0e 4372  _@...s......z.Cr
-00000880: 7970 742e 5f5f 7265 7072 5f5f 4e29 1072  ypt.__repr__N).r
-00000890: 0e00 0000 720f 0000 0072 1000 0000 7202  ....r....r....r.
-000008a0: 0000 0072 1f00 0000 7220 0000 0072 0700  ...r....r ...r..
-000008b0: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
-000008c0: 721b 0000 00da 0369 6e74 7217 0000 00da  r......intr.....
-000008d0: 0574 7570 6c65 722e 0000 0072 3300 0000  .tupler....r3...
-000008e0: 7235 0000 0072 3900 0000 720c 0000 0072  r5...r9...r....r
-000008f0: 0c00 0000 720c 0000 0072 0d00 0000 7212  ....r....r....r.
-00000900: 0000 000b 0000 0073 1200 0000 0801 1807  .......s........
-00000910: 0201 1003 0201 120c 0e0c 0e0d 0803 7212  ..............r.
-00000920: 0000 004e 2907 da06 7479 7069 6e67 7202  ...N)...typingr.
-00000930: 0000 00da 0841 7368 4372 7970 7472 0300  .....AshCryptr..
-00000940: 0000 7224 0000 0072 0400 0000 7212 0000  ..r$...r....r...
-00000950: 0072 0c00 0000 720c 0000 0072 0c00 0000  .r....r....r....
-00000960: 720d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-00000970: 0000 0073 0600 0000 0c01 0c03 1006       ...s..........
+000000b0: 0387 0004 005a 0453 0029 03da 0e4b 6579  .....Z.S.)...Key
+000000c0: 4c65 6e67 7468 4572 726f 7263 0100 0000  LengthErrorc....
+000000d0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000000e0: 0300 0000 7318 0000 0064 017c 005f 0074  ....s....d.|._.t
+000000f0: 0183 00a0 027c 006a 00a1 0101 0064 0053  .....|.j.....d.S
+00000100: 0029 024e 7a1a 4b65 7920 6d75 7374 2062  .).Nz.Key must b
+00000110: 6520 3235 3620 4269 7420 6c6f 6e67 2021  e 256 Bit long !
+00000120: 2903 da07 6469 7370 6c61 79da 0573 7570  )...display..sup
+00000130: 6572 da08 5f5f 696e 6974 5f5f a901 da04  er..__init__....
+00000140: 7365 6c66 a901 da09 5f5f 636c 6173 735f  self....__class_
+00000150: 5fa9 00fa 3043 3a5c 576f 726b 5c47 6974  _...0C:\Work\Git
+00000160: 4875 6257 6f72 6b5c 4145 532d 3235 365c  HubWork\AES-256\
+00000170: 4173 6843 7279 7074 5c54 6578 7443 7279  AshCrypt\TextCry
+00000180: 7074 2e70 7972 0700 0000 0600 0000 7304  pt.pyr........s.
+00000190: 0000 0000 0106 017a 174b 6579 4c65 6e67  .......z.KeyLeng
+000001a0: 7468 4572 726f 722e 5f5f 696e 6974 5f5f  thError.__init__
+000001b0: 2905 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
+000001c0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
+000001d0: 6e61 6d65 5f5f 7207 0000 00da 0d5f 5f63  name__r......__c
+000001e0: 6c61 7373 6365 6c6c 5f5f 720c 0000 0072  lasscell__r....r
+000001f0: 0c00 0000 720a 0000 0072 0d00 0000 7204  ....r....r....r.
+00000200: 0000 0005 0000 0073 0200 0000 0801 7204  .......s......r.
+00000210: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000220: 0000 0000 0400 0000 4000 0000 7376 0000  ........@...sv..
+00000230: 0065 005a 0164 005a 0265 0365 0465 0566  .e.Z.d.Z.e.e.e.f
+00000240: 0219 0065 0464 019c 0264 0264 0384 045a  ...e.d...d.d...Z
+00000250: 0665 0765 0464 049c 0164 0564 0684 0483  .e.e.d...d.d....
+00000260: 015a 0865 0765 0465 0964 079c 0264 0864  .Z.e.e.e.d...d.d
+00000270: 0984 0483 015a 0a65 0b64 049c 0164 0a64  .....Z.e.d...d.d
+00000280: 0b84 045a 0c65 0b64 049c 0164 0c64 0d84  ...Z.e.d...d.d..
+00000290: 045a 0d64 0e64 0f84 005a 0e64 1064 1184  .Z.d.d...Z.d.d..
+000002a0: 005a 0f64 1253 0029 13da 0543 7279 7074  .Z.d.S.)...Crypt
+000002b0: a902 da04 7465 7874 da03 6b65 7963 0300  ....text..keyc..
+000002c0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+000002d0: 0000 4300 0000 7326 0000 007c 017c 005f  ..C...s&...|.|._
+000002e0: 007c 00a0 017c 02a1 0164 016b 0272 1c7c  .|...|...d.k.r.|
+000002f0: 027c 005f 026e 0674 0383 0082 0164 0053  .|._.n.t.....d.S
+00000300: 0029 024e e901 0000 0029 0472 1400 0000  .).N.....).r....
+00000310: da09 6b65 7976 6572 6966 7972 1500 0000  ..keyverifyr....
+00000320: da08 4b65 7945 7272 6f72 2903 7209 0000  ..KeyError).r...
+00000330: 0072 1400 0000 7215 0000 0072 0c00 0000  .r....r....r....
+00000340: 720c 0000 0072 0d00 0000 7207 0000 000c  r....r....r.....
+00000350: 0000 0073 0800 0000 0001 0601 0e01 0802  ...s............
+00000360: 7a0e 4372 7970 742e 5f5f 696e 6974 5f5f  z.Crypt.__init__
+00000370: 2901 da06 7265 7475 726e 6300 0000 0000  )...returnc.....
+00000380: 0000 0000 0000 0000 0000 0002 0000 0043  ...............C
+00000390: 0000 0073 0a00 0000 7400 6a01 a002 a100  ...s....t.j.....
+000003a0: 5300 2901 4e29 0372 0300 0000 da03 456e  S.).N).r......En
+000003b0: 63da 0667 656e 6b65 7972 0c00 0000 720c  c..genkeyr....r.
+000003c0: 0000 0072 0c00 0000 720d 0000 0072 1b00  ...r....r....r..
+000003d0: 0000 1300 0000 7302 0000 0000 027a 0c43  ......s......z.C
+000003e0: 7279 7074 2e67 656e 6b65 7929 0272 1500  rypt.genkey).r..
+000003f0: 0000 7219 0000 0063 0100 0000 0000 0000  ..r....c........
+00000400: 0000 0000 0200 0000 0800 0000 4300 0000  ............C...
+00000410: 734e 0000 0074 007c 0074 0183 0272 467a  sN...t.|.t...rFz
+00000420: 2474 02a0 037c 00a0 04a1 00a1 017d 0174  $t...|.......}.t
+00000430: 057c 0183 0164 016b 0272 2c57 0064 0253  .|...d.k.r,W.d.S
+00000440: 0057 0071 4a04 0074 0679 4201 0001 0001  .W.qJ..t.yB.....
+00000450: 0059 0064 0353 0030 006e 0464 0453 0064  .Y.d.S.0.n.d.S.d
+00000460: 0053 0029 054e e920 0000 0072 1600 0000  .S.).N. ...r....
+00000470: 7201 0000 00e9 0200 0000 2907 da0a 6973  r.........)...is
+00000480: 696e 7374 616e 6365 da03 7374 72da 0562  instance..str..b
+00000490: 7974 6573 da07 6672 6f6d 6865 78da 0573  ytes..fromhex..s
+000004a0: 7472 6970 da03 6c65 6eda 0945 7863 6570  trip..len..Excep
+000004b0: 7469 6f6e 2902 7215 0000 00da 0161 720c  tion).r......ar.
+000004c0: 0000 0072 0c00 0000 720d 0000 0072 1700  ...r....r....r..
+000004d0: 0000 1700 0000 7310 0000 0000 020a 0102  ......s.........
+000004e0: 010e 010c 010a 010c 010a 037a 0f43 7279  ...........z.Cry
+000004f0: 7074 2e6b 6579 7665 7269 6679 6301 0000  pt.keyverifyc...
+00000500: 0000 0000 0000 0000 0004 0000 0008 0000  ................
+00000510: 0043 0000 0073 5200 0000 7c00 6a00 724a  .C...sR...|.j.rJ
+00000520: 7a22 7401 a002 7c00 6a00 7c00 6a03 a102  z"t...|.j.|.j...
+00000530: 7d01 7c01 a004 a100 7d02 6401 7c02 6602  }.|.....}.d.|.f.
+00000540: 5700 5300 0400 7405 7946 0100 0100 0100  W.S...t.yF......
+00000550: 6402 7d03 6403 7c03 6602 0600 5900 5300  d.}.d.|.f...Y.S.
+00000560: 3000 6e04 6404 5300 6400 5300 2905 4e72  0.n.d.S.d.S.).Nr
+00000570: 1600 0000 da01 4572 0100 0000 a902 e700  ......Er........
+00000580: 0000 0000 0000 0072 2800 0000 2906 7214  .......r(...).r.
+00000590: 0000 0072 0300 0000 721a 0000 0072 1500  ...r....r....r..
+000005a0: 0000 da0a 656e 635f 746f 5f73 7472 da0d  ....enc_to_str..
+000005b0: 4261 7365 4578 6365 7074 696f 6e29 0472  BaseException).r
+000005c0: 0900 0000 da03 696e 73da 0b6e 6577 5f63  ......ins..new_c
+000005d0: 6f6e 7465 6e74 da06 6f75 7470 7574 720c  ontent..outputr.
+000005e0: 0000 0072 0c00 0000 720d 0000 00da 0765  ...r....r......e
+000005f0: 6e63 7279 7074 2400 0000 7312 0000 0000  ncrypt$...s.....
+00000600: 0106 0102 0110 0108 010a 010c 0104 0110  ................
+00000610: 027a 0d43 7279 7074 2e65 6e63 7279 7074  .z.Crypt.encrypt
+00000620: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00000630: 0008 0000 0043 0000 0073 5a00 0000 7c00  .....C...sZ...|.
+00000640: 6a00 7252 7a28 7401 6a02 7c00 6a00 7c00  j.rRz(t.j.|.j.|.
+00000650: 6a03 6401 8d02 7d01 7c01 a004 a100 7d02  j.d...}.|.....}.
+00000660: 7c02 7d03 6402 7c03 6602 5700 5300 0400  |.}.d.|.f.W.S...
+00000670: 7405 794e 0100 0100 0100 7c00 6a00 7d03  t.yN......|.j.}.
+00000680: 6403 7c03 6602 0600 5900 5300 3000 6e04  d.|.f...Y.S.0.n.
+00000690: 6404 5300 6400 5300 2905 4e29 02da 076d  d.S.d.S.).N)...m
+000006a0: 6573 7361 6765 da07 6d61 696e 6b65 7972  essage..mainkeyr
+000006b0: 1600 0000 7201 0000 0072 2700 0000 2906  ....r....r'...).
+000006c0: 7214 0000 0072 0300 0000 da03 4465 6372  r....r......Decr
+000006d0: 1500 0000 da0a 6465 635f 746f 5f73 7472  ......dec_to_str
+000006e0: 7224 0000 0029 0472 0900 0000 5a0c 6465  r$...).r....Z.de
+000006f0: 635f 696e 7374 616e 6365 7225 0000 0072  c_instancer%...r
+00000700: 2d00 0000 720c 0000 0072 0c00 0000 720d  -...r....r....r.
+00000710: 0000 00da 0764 6563 7279 7074 3000 0000  .....decrypt0...
+00000720: 7314 0000 0000 0106 0102 0112 0108 0104  s...............
+00000730: 010a 010c 0106 0110 027a 0d43 7279 7074  .........z.Crypt
+00000740: 2e64 6563 7279 7074 6301 0000 0000 0000  .decryptc.......
+00000750: 0000 0000 0001 0000 0005 0000 0043 0000  .............C..
+00000760: 0073 1e00 0000 6401 7c00 6a00 6400 6402  .s....d.|.j.d.d.
+00000770: 8502 1900 9b00 6403 7c00 6a01 9b00 6404  ......d.|.j...d.
+00000780: 9d05 5300 2905 4e7a 1b45 6e63 7279 7074  ..S.).Nz.Encrypt
+00000790: 696e 672f 4465 6372 7970 7469 6e67 2054  ing/Decrypting T
+000007a0: 6578 7420 e908 0000 007a 082e 2e20 5769  ext .....z... Wi
+000007b0: 7468 207a 0520 4b65 7920 7213 0000 0072  th z. Key r....r
+000007c0: 0800 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+000007d0: 0000 00da 075f 5f73 7472 5f5f 3d00 0000  .....__str__=...
+000007e0: 7302 0000 0000 017a 0d43 7279 7074 2e5f  s......z.Crypt._
+000007f0: 5f73 7472 5f5f 6301 0000 0000 0000 0000  _str__c.........
+00000800: 0000 0001 0000 0006 0000 0043 0000 0073  ...........C...s
+00000810: 2600 0000 7c00 6a00 6a01 9b00 6401 7c00  &...|.j.j...d.|.
+00000820: 6a02 6400 6402 8502 1900 9b00 6403 7c00  j.d.d.......d.|.
+00000830: 6a03 9b00 6404 9d06 5300 2905 4efa 0128  j...d...S.).N..(
+00000840: 7234 0000 00fa 012c fa01 2929 0472 0b00  r4.....,..)).r..
+00000850: 0000 720e 0000 0072 1400 0000 7215 0000  ..r....r....r...
+00000860: 0072 0800 0000 720c 0000 0072 0c00 0000  .r....r....r....
+00000870: 720d 0000 00da 085f 5f72 6570 725f 5f40  r......__repr__@
+00000880: 0000 0073 0200 0000 0001 7a0e 4372 7970  ...s......z.Cryp
+00000890: 742e 5f5f 7265 7072 5f5f 4e29 1072 0e00  t.__repr__N).r..
+000008a0: 0000 720f 0000 0072 1000 0000 7202 0000  ..r....r....r...
+000008b0: 0072 1f00 0000 7220 0000 0072 0700 0000  .r....r ...r....
+000008c0: da0c 7374 6174 6963 6d65 7468 6f64 721b  ..staticmethodr.
+000008d0: 0000 00da 0369 6e74 7217 0000 00da 0574  .....intr......t
+000008e0: 7570 6c65 722e 0000 0072 3300 0000 7235  upler....r3...r5
+000008f0: 0000 0072 3900 0000 720c 0000 0072 0c00  ...r9...r....r..
+00000900: 0000 720c 0000 0072 0d00 0000 7212 0000  ..r....r....r...
+00000910: 000b 0000 0073 1200 0000 0801 1807 0201  .....s..........
+00000920: 1003 0201 120c 0e0c 0e0d 0803 7212 0000  ............r...
+00000930: 004e 2907 da06 7479 7069 6e67 7202 0000  .N)...typingr...
+00000940: 00da 0841 7368 4372 7970 7472 0300 0000  ...AshCryptr....
+00000950: 7224 0000 0072 0400 0000 7212 0000 0072  r$...r....r....r
+00000960: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
+00000970: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00000980: 0073 0600 0000 0c01 0c03 1006            .s..........
```

### Comparing `AshCrypt-1.3.6/AshCrypt/__pycache__/qr.cpython-39.pyc` & `AshCrypt-2.0.0/AshCrypt/__pycache__/qr.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Jul  9 22:29:03 2023 UTC, .py size: 536 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,45 @@
-00000000: 610d 0d0a 0000 0000 af34 ab64 1802 0000  a........4.d....
+00000000: 610d 0d0a 0000 0000 ffeb b364 f301 0000  a..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6503 6502 6504 6505 6602 1900 6403  ..e.e.e.e.f...d.
 00000050: 9c02 6404 6405 8404 5a06 6401 5300 2906  ..d.d...Z.d.S.).
 00000060: e900 0000 004e 2901 da05 556e 696f 6e29  .....N)...Union)
 00000070: 02da 0474 6578 74da 0672 6574 7572 6e63  ...text..returnc
 00000080: 0100 0000 0000 0000 0000 0000 0500 0000  ................
-00000090: 0a00 0000 4300 0000 738c 0000 007a 5a7c  ....C...s....zZ|
+00000090: 0a00 0000 4300 0000 7382 0000 007a 507c  ....C...s....zP|
 000000a0: 00a0 00a1 007d 0174 016a 0264 0174 016a  .....}.t.j.d.t.j
 000000b0: 036a 0464 0264 0364 048d 047d 027c 02a0  .j.d.d.d...}.|..
 000000c0: 057c 01a1 0101 007c 026a 0664 0564 068d  .|.....|.j.d.d..
 000000d0: 0101 007c 026a 0764 0764 0864 098d 027d  ...|.j.d.d.d...}
-000000e0: 037c 03a0 0864 0aa1 0101 007c 03a0 09a1  .|...d.....|....
-000000f0: 0001 0057 0064 0353 0004 0074 0a79 8601  ...W.d.S...t.y..
-00000100: 007d 0401 007a 1464 0b7c 0466 0257 0006  .}...z.d.|.f.W..
-00000110: 0059 0064 007d 047e 0453 0064 007d 047e  .Y.d.}.~.S.d.}.~
-00000120: 0430 0030 0064 0053 0029 0c4e e90a 0000  .0.0.d.S.).N....
-00000130: 00e9 1400 0000 e901 0000 0029 04da 0776  ...........)...v
-00000140: 6572 7369 6f6e 5a10 6572 726f 725f 636f  ersionZ.error_co
-00000150: 7272 6563 7469 6f6e 5a08 626f 785f 7369  rrectionZ.box_si
-00000160: 7a65 da06 626f 7264 6572 5429 015a 0366  ze..borderT).Z.f
-00000170: 6974 da05 626c 6163 6bda 0577 6869 7465  it..black..white
-00000180: 2902 5a0a 6669 6c6c 5f63 6f6c 6f72 5a0a  ).Z.fill_colorZ.
-00000190: 6261 636b 5f63 6f6c 6f72 7a09 7172 7631  back_colorz.qrv1
-000001a0: 302e 706e 6772 0100 0000 290b da05 7374  0.pngr....)...st
-000001b0: 7269 70da 0671 7263 6f64 655a 0651 5243  rip..qrcodeZ.QRC
-000001c0: 6f64 65da 0963 6f6e 7374 616e 7473 5a0f  ode..constantsZ.
-000001d0: 4552 524f 525f 434f 5252 4543 545f 4c5a  ERROR_CORRECT_LZ
-000001e0: 0861 6464 5f64 6174 615a 046d 616b 655a  .add_dataZ.makeZ
-000001f0: 0a6d 616b 655f 696d 6167 65da 0473 6176  .make_image..sav
-00000200: 65da 0473 686f 77da 0945 7863 6570 7469  e..show..Excepti
-00000210: 6f6e 2905 7203 0000 00da 0178 da02 7172  on).r......x..qr
-00000220: da03 696d 67da 0165 a900 7216 0000 00fa  ..img..e..r.....
-00000230: 2943 3a5c 576f 726b 5c47 6974 4875 6257  )C:\Work\GitHubW
-00000240: 6f72 6b5c 4145 532d 3235 365c 4173 6843  ork\AES-256\AshC
-00000250: 7279 7074 5c71 722e 7079 da03 7471 7205  rypt\qr.py..tqr.
-00000260: 0000 0073 2000 0000 0001 0201 0801 0401  ...s ...........
-00000270: 0201 0601 0201 02fc 0605 0a01 0c01 0e01  ................
-00000280: 0a01 0801 0602 0e01 7218 0000 0029 0772  ........r....).r
-00000290: 0d00 0000 da06 7479 7069 6e67 7202 0000  ......typingr...
-000002a0: 00da 0373 7472 da03 696e 74da 0574 7570  ...str..int..tup
-000002b0: 6c65 7218 0000 0072 1600 0000 7216 0000  ler....r....r...
-000002c0: 0072 1600 0000 7217 0000 00da 083c 6d6f  .r....r......<mo
-000002d0: 6475 6c65 3e01 0000 0073 0400 0000 0801  dule>....s......
-000002e0: 0c03                                     ..
+000000e0: 037c 03a0 08a1 0001 0057 0064 0353 0004  .|.......W.d.S..
+000000f0: 0074 0979 7c01 007d 0401 007a 1464 0a7c  .t.y|..}...z.d.|
+00000100: 0466 0257 0006 0059 0064 007d 047e 0453  .f.W...Y.d.}.~.S
+00000110: 0064 007d 047e 0430 0030 0064 0053 0029  .d.}.~.0.0.d.S.)
+00000120: 0b4e e90a 0000 00e9 1400 0000 e901 0000  .N..............
+00000130: 0029 04da 0776 6572 7369 6f6e 5a10 6572  .)...versionZ.er
+00000140: 726f 725f 636f 7272 6563 7469 6f6e 5a08  ror_correctionZ.
+00000150: 626f 785f 7369 7a65 da06 626f 7264 6572  box_size..border
+00000160: 5429 015a 0366 6974 da05 626c 6163 6bda  T).Z.fit..black.
+00000170: 0577 6869 7465 2902 5a0a 6669 6c6c 5f63  .white).Z.fill_c
+00000180: 6f6c 6f72 5a0a 6261 636b 5f63 6f6c 6f72  olorZ.back_color
+00000190: 7201 0000 0029 0ada 0573 7472 6970 da06  r....)...strip..
+000001a0: 7172 636f 6465 5a06 5152 436f 6465 da09  qrcodeZ.QRCode..
+000001b0: 636f 6e73 7461 6e74 735a 0f45 5252 4f52  constantsZ.ERROR
+000001c0: 5f43 4f52 5245 4354 5f4c 5a08 6164 645f  _CORRECT_LZ.add_
+000001d0: 6461 7461 5a04 6d61 6b65 5a0a 6d61 6b65  dataZ.makeZ.make
+000001e0: 5f69 6d61 6765 da04 7368 6f77 da09 4578  _image..show..Ex
+000001f0: 6365 7074 696f 6e29 0572 0300 0000 da01  ception).r......
+00000200: 78da 0271 72da 0369 6d67 da01 65a9 0072  x..qr..img..e..r
+00000210: 1500 0000 fa29 433a 5c57 6f72 6b5c 4769  .....)C:\Work\Gi
+00000220: 7448 7562 576f 726b 5c41 4553 2d32 3536  tHubWork\AES-256
+00000230: 5c41 7368 4372 7970 745c 7172 2e70 79da  \AshCrypt\qr.py.
+00000240: 0374 7172 0500 0000 731e 0000 0000 0102  .tqr....s.......
+00000250: 0108 0104 0102 0106 0102 0102 fc06 050a  ................
+00000260: 010c 010e 0108 0106 020e 0172 1700 0000  ...........r....
+00000270: 2907 720d 0000 00da 0674 7970 696e 6772  ).r......typingr
+00000280: 0200 0000 da03 7374 72da 0369 6e74 da05  ......str..int..
+00000290: 7475 706c 6572 1700 0000 7215 0000 0072  tupler....r....r
+000002a0: 1500 0000 7215 0000 0072 1600 0000 da08  ....r....r......
+000002b0: 3c6d 6f64 756c 653e 0100 0000 7304 0000  <module>....s...
+000002c0: 0008 010c 03                             .....
```

### Comparing `AshCrypt-1.3.6/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc` & `AshCrypt-2.0.0/AshCrypt/unittests/__pycache__/unittestAsh.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.6/AshCrypt/unittests/unittestAsh.py` & `AshCrypt-2.0.0/AshCrypt/unittests/unittestAsh.py`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.6/AshCrypt.egg-info/PKG-INFO` & `AshCrypt-2.0.0/AshCrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.3.6
+Version: 2.0.0
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.3.6/AshCrypt.egg-info/SOURCES.txt` & `AshCrypt-2.0.0/AshCrypt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.6/LICENSE` & `AshCrypt-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AshCrypt-1.3.6/PKG-INFO` & `AshCrypt-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AshCrypt
-Version: 1.3.6
+Version: 2.0.0
 Summary: Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with a database module to store encrypted content.
 Home-page: https://github.com/AshGw/AES-256.git
 Author: Ashref Gwader
 Author-email: AshrefGw@proton.me
 Keywords: Cryptography application,cryptography libraryAES-256
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `AshCrypt-1.3.6/README.md` & `AshCrypt-2.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 <br>check [GUI](https://github.com/AshGw/AES-256#AshCryptGUI) header for more info.
 
 **Library :** 
 <br>A simple, secure, and developer-oriented library for
 encryption and decryption with AES-256 (CBC) . 
 <br>The core of the library is the module `Ash`
 It offers an intuitive interface, seamless integration with precompiled 
-functions, and robust security measures to safeguard
+functions, and top security measures to safeguard
 sensitive data,  providing a hassle-free experience when dealing with cryptographic libraries.
 <br>View [Features](https://github.com/AshGw/AES-256#features) Header for more details.
 
 
 
 
 
@@ -118,15 +118,15 @@
 
 <br>You can check [Features](https://github.com/AshGw/AES-256#features) tag below to learn more about the security features.
 <br>You can check the [unittesting file](AshCrypt/unittests/unittestAsh.py) to verify how it works.
 
 ### Usage ##
 1) Generate a key if you don't have one already
 ```python
-mainkey = Enc.genMainkey()
+mainkey = Enc.genkey()
 ```
 2) Before encrypting or decrypting anything, first set the arguments you want to pass, you can have an encrypted message or a  decrypted message , and a mainkey to use.
 <br>Set the correct mainkey ( 64 byte long key ) 
 ```python
 mainkey = '6ce113be19e898c2b98df82b7fa8efb166928925fc05574a54eb1114c3410900'
 ```
 The message can be of type string or bytes.
@@ -152,19 +152,19 @@
 ```python
 instanceE = Enc(message=message, mainkey=mainkey)
 ```
 
 4) Now you'd have to specify the output, you can encrypt to bytes or encrypt to URL-safe strings.
 <br> Here I chose to encrypt to bytes
 ```python
-output = instanceE.encToBytes()
+output = instanceE.enc_to_bytes()
 ```
 you can also encrypt to a URL safe string
 ```python
-output = instanceE.encToStr()
+output = instanceE.enc_to_str()
 ```
 That simple, that's it.
 
 
 
 
 ## Features ## 
@@ -187,15 +187,15 @@
 Note that bcrypt is intentionally slow and computationally expensive, enhancing protection against brute-force attacks. The number of iterations, including salt and pepper, increases derivation time to strike a balance between security and performance. Use a suitable value based on your machine's capabilities and desired security level.
 <br>Im using 50 just to demonstrate the process and make it quick.
 <br>The bare minimum is 50, the max is 100 000, choose somewhere in between.
 <br>In my use case 50 takes around 0.5 secs while using the maximum number of iterations takes around 11 minutes to derive the keys and finish the cryptographic operations at hand.
 <br>You can check how it works by checking this [Jupyter Notebook](demo/demo.ipynb) demo file
 <br>Note that im using a 512 bit long key to demonstrate the process although as I mentioned earlier you can use any key length with `Ash`.
 ## AshCryptGUI ##
-The GUI as mentioned above is a fully fledged application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
+The GUI as mentioned above is a full, application , you can use it to encrypt files , texts , keep track of files by storing them on demand to a main database , also on demand it can keep track of the keys used for cryptographic operations.
 ### Usage ###
 1) Set the main key up. If you don't have one , press on the button `generate` to generate a secure safe key ready for use. 
 2) Now you're able to encrypt files or text (text is limited to 200 characters max)
 ####  Text : 
 - You can insert some text in the entry right below the `TEXT ENCRYPTION` label.<br>The given text will be encrypted and you can choose if you want to have that text displayed as a qr code, a qr image will pop on the screen and you'll be able to scan it using your phone.
 - Insert some encrypted text below the `TEXT DECRYPTION` label.<br>The Given text will be decrypted and you'd have the option to display the "plaintext" as a qr code to be scanned by other devices.
 <br>If the text cannot be decrypted it will display itself , so you might as well use this to display the key you're using as a qr code
```

### Comparing `AshCrypt-1.3.6/setup.py` & `AshCrypt-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup , find_packages
 
 with open('AshCrypt/README.md','r') as f:
     readme = f.read()
 
 setup(
     name='AshCrypt',
-    version='1.3.6',
+    version='2.0.0',
     author='Ashref Gwader',
     author_email='AshrefGw@proton.me',
     python_requires='>=3.7',
     description="Comprehensive AES-256 Cryptography App & library equipped with files & text handling modules along with"
                 " a database module to store encrypted content.",
     long_description_content_type='text/markdown',
     long_description=readme,
```

