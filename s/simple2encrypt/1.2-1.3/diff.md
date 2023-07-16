# Comparing `tmp/simple2encrypt-1.2.tar.gz` & `tmp/simple2encrypt-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.2.tar", last modified: Sun Jul 16 21:05:19 2023, max compression
+gzip compressed data, was "simple2encrypt-1.3.tar", last modified: Sun Jul 16 21:13:07 2023, max compression
```

## Comparing `simple2encrypt-1.2.tar` & `simple2encrypt-1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:05:19.444137 simple2encrypt-1.2/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.2/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3386 2023-07-16 21:05:19.444137 simple2encrypt-1.2/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.2/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     5298 2023-07-16 20:54:29.000000 simple2encrypt-1.2/encryption_utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:05:19.444137 simple2encrypt-1.2/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     3722 2023-07-16 21:03:35.000000 simple2encrypt-1.2/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:05:19.444137 simple2encrypt-1.2/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3386 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      276 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       55 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:13:07.628150 simple2encrypt-1.3/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.3/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3386 2023-07-16 21:13:07.628150 simple2encrypt-1.3/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.3/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     5298 2023-07-16 21:12:49.000000 simple2encrypt-1.3/encryption_utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:13:07.628150 simple2encrypt-1.3/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     3733 2023-07-16 21:12:37.000000 simple2encrypt-1.3/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:13:07.628150 simple2encrypt-1.3/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3386 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      276 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       55 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/top_level.txt
```

### Comparing `simple2encrypt-1.2/LICENSE` & `simple2encrypt-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.2/PKG-INFO` & `simple2encrypt-1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.2
+Version: 1.3
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -112,13 +112,13 @@
 encrypt_data my-key.bin mysecretpassword
 ```
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.2.
+The current version of `encryption_utils` is 1.3.
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.2/encryption_utils.py` & `simple2encrypt-1.3/encryption_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.2'
+__version__ = '1.3'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
```

### Comparing `simple2encrypt-1.2/setup.py` & `simple2encrypt-1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,34 +103,35 @@
 encrypt_data my-key.bin mysecretpassword
 ```
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.2.
+The current version of `encryption_utils` is 1.3.
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
 
 """
 
 setup(
     name='simple2encrypt',
-    version='1.2',
+    version='1.3',
     description='Utility functions for encryption and file operations',
     author='nhman-python',
     author_email='wbgblfix@duck.com',
     url='https://github.com/nhman-python/crypto-utils',
     license='MIT',
     long_description=description,
     long_description_content_type='text/markdown',
     py_modules=['encryption_utils'],
     install_requires=[
         'pycryptodome',  # Dependency on pycryptodome package
     ],
     entry_points={
         'console_scripts': [
-            'encrypt_data = encryption_utils:main']
+            'encrypt_data = encryption_utils:main',
+        ],
     }
 )
```

### Comparing `simple2encrypt-1.2/simple2encrypt.egg-info/PKG-INFO` & `simple2encrypt-1.3/simple2encrypt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.2
+Version: 1.3
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -112,13 +112,13 @@
 encrypt_data my-key.bin mysecretpassword
 ```
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.2.
+The current version of `encryption_utils` is 1.3.
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
```

