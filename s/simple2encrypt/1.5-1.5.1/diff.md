# Comparing `tmp/simple2encrypt-1.5.tar.gz` & `tmp/simple2encrypt-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.5.tar", last modified: Sun Jul 16 21:44:12 2023, max compression
+gzip compressed data, was "simple2encrypt-1.5.1.tar", last modified: Sun Jul 16 21:52:43 2023, max compression
```

## Comparing `simple2encrypt-1.5.tar` & `simple2encrypt-1.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:44:12.208202 simple2encrypt-1.5/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3526 2023-07-16 21:44:12.208202 simple2encrypt-1.5/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.5/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     5297 2023-07-16 21:42:50.000000 simple2encrypt-1.5/encryption_utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)      980 2023-07-16 21:26:59.000000 simple2encrypt-1.5/example_message.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:44:12.208202 simple2encrypt-1.5/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     3905 2023-07-16 21:43:53.000000 simple2encrypt-1.5/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:44:12.208202 simple2encrypt-1.5/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3526 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      295 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       33 2023-07-16 21:44:12.000000 simple2encrypt-1.5/simple2encrypt.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:52:43.920217 simple2encrypt-1.5.1/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.5.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3530 2023-07-16 21:52:43.920217 simple2encrypt-1.5.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.5.1/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     5318 2023-07-16 21:52:21.000000 simple2encrypt-1.5.1/encryption_utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1305 2023-07-16 21:48:50.000000 simple2encrypt-1.5.1/example_message.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:52:43.920217 simple2encrypt-1.5.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     3909 2023-07-16 21:50:43.000000 simple2encrypt-1.5.1/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:52:43.920217 simple2encrypt-1.5.1/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3530 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      295 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       33 2023-07-16 21:52:43.000000 simple2encrypt-1.5.1/simple2encrypt.egg-info/top_level.txt
```

### Comparing `simple2encrypt-1.5/LICENSE` & `simple2encrypt-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.5/PKG-INFO` & `simple2encrypt-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.5
+Version: 1.5.1
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
 
-The current version of `encryption_utils` is 1.5
+The current version of `encryption_utils` is 1.5.1
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.5/encryption_utils.py` & `simple2encrypt-1.5.1/encryption_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.5'
+__version__ = '1.5.1'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
 
@@ -156,14 +156,14 @@
 
     file_name = args.filename
     try:
         key = generate_key(args.password, length=32)
         key_path = args.filename
         write_binary(key_path, key)
         print(f"A new file was created based on your password. The file name is: {key_path}")
-    except (ValueError, FileExistsError) as write_error:
+    except (ValueError, FileExistsError, FileNotFoundError) as write_error:
         print(write_error)
         sys.exit()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `simple2encrypt-1.5/example_message.py` & `simple2encrypt-1.5.1/example_message.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,27 @@
+import argparse
+
 from encryption_utils import custom_input, Encryption, read_binary
 
+parser = argparse.ArgumentParser(prog='message encryption', description='encrypt message with AES encryption from the '
+                                                                        'key file')
+parser.add_argument('file_key', help='the key to encrypt the message')
+args = parser.parse_args()
+
 
 def main():
     """
     The Main function for encrypting and decrypting a message.
     """
     # Get user input
     message = custom_input('Enter your message: ')
     convert = bytes(message.encode())
     try:
         # Read the encryption key from the file
-        key = read_binary('my.key')
+        key = read_binary(args.file_key)
 
         # Encrypt the message
         encryptor = Encryption(key, convert)
         encrypted_message = encryptor.encrypt()
         print(f'The encrypted message: {encrypted_message}')
 
         # Decrypt the message
```

### Comparing `simple2encrypt-1.5/setup.py` & `simple2encrypt-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,26 +111,26 @@
 aes-message  # Executes the main function from example_message module
 
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.5
+The current version of `encryption_utils` is 1.5.1
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
 
 """
 
 setup(
     name='simple2encrypt',
-    version='1.5',
+    version='1.5.1',
     description='Utility functions for encryption and file operations',
     author='nhman-python',
     author_email='wbgblfix@duck.com',
     url='https://github.com/nhman-python/crypto-utils',
     license='MIT',
     long_description=description,
     long_description_content_type='text/markdown',
```

### Comparing `simple2encrypt-1.5/simple2encrypt.egg-info/PKG-INFO` & `simple2encrypt-1.5.1/simple2encrypt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.5
+Version: 1.5.1
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
 
-The current version of `encryption_utils` is 1.5
+The current version of `encryption_utils` is 1.5.1
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
 See the `LICENSE` file for more information.
```

