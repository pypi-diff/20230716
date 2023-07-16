# Comparing `tmp/simple2encrypt-1.4.tar.gz` & `tmp/simple2encrypt-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.4.tar", last modified: Sun Jul 16 21:34:37 2023, max compression
+gzip compressed data, was "simple2encrypt-1.5.tar", last modified: Sun Jul 16 21:44:12 2023, max compression
```

## Comparing `simple2encrypt-1.4.tar` & `simple2encrypt-1.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:34:37.084186 simple2encrypt-1.4/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.4/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3526 2023-07-16 21:34:37.084186 simple2encrypt-1.4/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.4/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     5297 2023-07-16 21:34:22.000000 simple2encrypt-1.4/encryption_utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:34:37.084186 simple2encrypt-1.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     3918 2023-07-16 21:34:15.000000 simple2encrypt-1.4/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:34:37.084186 simple2encrypt-1.4/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3526 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      276 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:44:12.208202 simple2encrypt-1.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3526 2023-07-16 21:44:12.208202 simple2encrypt-1.5/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.5/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     5297 2023-07-16 21:42:50.000000 simple2encrypt-1.5/encryption_utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)      980 2023-07-16 21:26:59.000000 simple2encrypt-1.5/example_message.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:44:12.208202 simple2encrypt-1.5/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     3905 2023-07-16 21:43:53.000000 simple2encrypt-1.5/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:44:12.208202 simple2encrypt-1.5/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3526 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      295 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       33 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/top_level.txt
```

### Comparing `simple2encrypt-1.4/LICENSE` & `simple2encrypt-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.4/PKG-INFO` & `simple2encrypt-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.4
+Version: 1.5
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -120,14 +120,14 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.4
+The current version of `encryption_utils` is 1.5
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.4/encryption_utils.py` & `simple2encrypt-1.5/encryption_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.4'
+__version__ = '1.5'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
```

### Comparing `simple2encrypt-1.4/setup.py` & `simple2encrypt-1.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,37 +111,34 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.4
+The current version of `encryption_utils` is 1.5
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
 
 """
 
 setup(
     name='simple2encrypt',
-    version='1.4',
+    version='1.5',
     description='Utility functions for encryption and file operations',
     author='nhman-python',
     author_email='wbgblfix@duck.com',
     url='https://github.com/nhman-python/crypto-utils',
     license='MIT',
     long_description=description,
     long_description_content_type='text/markdown',
-    py_modules=['encryption_utils'],
+    py_modules=['encryption_utils', 'example_message'],
     install_requires=[
         'pycryptodome',  # Dependency on pycryptodome package
     ],
     entry_points={
-        'console_scripts': [
-            'aes-key = encryption_utils:main',
-            'aes-message = example_message:main',
-        ],
-    }
+        'console_scripts': ['aes-key = encryption_utils:main', 'aes-message = example_message:main', ],
+    },
 )
```

### Comparing `simple2encrypt-1.4/simple2encrypt.egg-info/PKG-INFO` & `simple2encrypt-1.5/simple2encrypt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.4
+Version: 1.5
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -120,14 +120,14 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.4
+The current version of `encryption_utils` is 1.5
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

