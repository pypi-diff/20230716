# Comparing `tmp/my-encryption-utils-1.0.tar.gz` & `tmp/my-encryption-utils-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my-encryption-utils-1.0.tar", last modified: Sun Jul 16 12:18:34 2023, max compression
+gzip compressed data, was "my-encryption-utils-1.1.tar", last modified: Sun Jul 16 19:47:15 2023, max compression
```

## Comparing `my-encryption-utils-1.0.tar` & `my-encryption-utils-1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 12:18:34.012059 my-encryption-utils-1.0/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 my-encryption-utils-1.0/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)      198 2023-07-16 12:18:34.012059 my-encryption-utils-1.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 my-encryption-utils-1.0/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     4175 2023-07-16 12:14:08.000000 my-encryption-utils-1.0/encryption_utils.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 12:18:34.012059 my-encryption-utils-1.0/my_encryption_utils.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      198 2023-07-16 12:18:33.000000 my-encryption-utils-1.0/my_encryption_utils.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      260 2023-07-16 12:18:33.000000 my-encryption-utils-1.0/my_encryption_utils.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 12:18:33.000000 my-encryption-utils-1.0/my_encryption_utils.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 12:18:33.000000 my-encryption-utils-1.0/my_encryption_utils.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 12:18:33.000000 my-encryption-utils-1.0/my_encryption_utils.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 12:18:34.012059 my-encryption-utils-1.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     2169 2023-07-16 12:18:09.000000 my-encryption-utils-1.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 19:47:15.176005 my-encryption-utils-1.1/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 my-encryption-utils-1.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     1990 2023-07-16 19:47:15.176005 my-encryption-utils-1.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 my-encryption-utils-1.1/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     4177 2023-07-16 13:02:12.000000 my-encryption-utils-1.1/encryption_utils.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 19:47:15.176005 my-encryption-utils-1.1/my_encryption_utils.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1990 2023-07-16 19:47:15.000000 my-encryption-utils-1.1/my_encryption_utils.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      260 2023-07-16 19:47:15.000000 my-encryption-utils-1.1/my_encryption_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 19:47:15.000000 my-encryption-utils-1.1/my_encryption_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 19:47:15.000000 my-encryption-utils-1.1/my_encryption_utils.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 19:47:15.000000 my-encryption-utils-1.1/my_encryption_utils.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 19:47:15.176005 my-encryption-utils-1.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     2203 2023-07-16 12:19:46.000000 my-encryption-utils-1.1/setup.py
```

### Comparing `my-encryption-utils-1.0/LICENSE` & `my-encryption-utils-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `my-encryption-utils-1.0/encryption_utils.py` & `my-encryption-utils-1.1/encryption_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,21 @@
 encryption_utils.py
 Utility functions for encryption and file operations.
 """
 
 import argparse
 import os
 import sys
+
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.0'
+__version__ = '1.1'
+
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
 
     def __init__(self, key, data):
```

### Comparing `my-encryption-utils-1.0/setup.py` & `my-encryption-utils-1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,16 +49,17 @@
 -------
 This project is licensed under the MIT License. See the LICENSE file for more information.
 """
 
 
 setup(
     name='my-encryption-utils',
-    version='1.0',
+    version='1.1',
     description='Utility functions for encryption and file operations',
     author='nhman python',
     author_email='wbgblfix@duck.com',
+    long_description=description,
     py_modules=['encryption_utils'],
     install_requires=[
         'pycryptodome',  # Dependency on pycryptodome package
     ],
 )
```

