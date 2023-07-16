# Comparing `tmp/simple2encrypt-1.1.tar.gz` & `tmp/simple2encrypt-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.1.tar", last modified: Sun Jul 16 20:24:47 2023, max compression
+gzip compressed data, was "simple2encrypt-1.2.tar", last modified: Sun Jul 16 21:05:19 2023, max compression
```

## Comparing `simple2encrypt-1.1.tar` & `simple2encrypt-1.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 20:24:47.872068 simple2encrypt-1.1/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.1/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3395 2023-07-16 20:24:47.872068 simple2encrypt-1.1/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.1/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     4891 2023-07-16 20:18:57.000000 simple2encrypt-1.1/encryption_utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 20:24:47.872068 simple2encrypt-1.1/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     3625 2023-07-16 20:23:52.000000 simple2encrypt-1.1/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 20:24:47.872068 simple2encrypt-1.1/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3395 2023-07-16 20:24:47.000000 simple2encrypt-1.1/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      235 2023-07-16 20:24:47.000000 simple2encrypt-1.1/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 20:24:47.000000 simple2encrypt-1.1/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 20:24:47.000000 simple2encrypt-1.1/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 20:24:47.000000 simple2encrypt-1.1/simple2encrypt.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:05:19.444137 simple2encrypt-1.2/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.2/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3386 2023-07-16 21:05:19.444137 simple2encrypt-1.2/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.2/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     5298 2023-07-16 20:54:29.000000 simple2encrypt-1.2/encryption_utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:05:19.444137 simple2encrypt-1.2/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     3722 2023-07-16 21:03:35.000000 simple2encrypt-1.2/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:05:19.444137 simple2encrypt-1.2/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3386 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      276 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       55 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 21:05:19.000000 simple2encrypt-1.2/simple2encrypt.egg-info/top_level.txt
```

### Comparing `simple2encrypt-1.1/LICENSE` & `simple2encrypt-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.1/PKG-INFO` & `simple2encrypt-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.1
+Version: 1.2
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,15 +19,15 @@
 You can install `encryption_utils` using `pip`:
 
 ```
 pip install simple2encrypt
 ```
 
 ## Usage
-simple-encrypt
+simple2encrypt
 ### Encryption
 
 To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the library. Here's an example:
 
 ```
 from encryption_utils import Encryption
 
@@ -76,15 +76,15 @@
 ### Reading and Writing Binary Data
 
 The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. Here's an example:
 
 ```
 from encryption_utils import read_binary, write_binary
 
-file_path = '/path/to/file.bin'
+file_path = 'file.bin'
 
 # Read binary data from a file
 data = read_binary(file_path)
 print("Read data:", data)
 
 # Write binary data to a file
 data_to_write = b'mydata'
@@ -112,13 +112,13 @@
 encrypt_data my-key.bin mysecretpassword
 ```
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.0.
+The current version of `encryption_utils` is 1.2.
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.1/encryption_utils.py` & `simple2encrypt-1.2/encryption_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.1'
+__version__ = '1.2'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
 
@@ -44,39 +44,49 @@
         """
         initialization_vector = self.data[:AES.block_size]  # Extract the IV from the data
         cipher = AES.new(self.key, AES.MODE_CBC, iv=initialization_vector)
         decrypted_data = cipher.decrypt(self.data[AES.block_size:])
         return unpad(decrypted_data, cipher.block_size)
 
 
-def folder_encrypt(folder_path: str, key: bytes) -> None:
+def folder_encrypt(folder_path: str, key: bytes, add_extension='.enc') -> None:
     """
     Encrypts all files within a given folder.
 
-    :param key: The key for the encryption
+    :param add_extension: Add the extension to the end of the file
     :param folder_path: Path to the folder containing the files to be encrypted.
+    :param key: The key for encryption.
     :raises ValueError: If the provided folder path is not a directory.
     """
     if not os.path.isdir(folder_path):
         raise ValueError("Expected a folder path, but received a different type of path.")
+
     for file in os.listdir(folder_path):
-        data = read_binary(file)
-        encrypt = Encryption(key, data)
-        encrypted_data = encrypt.encrypt()
-        full_path = os.path.join(folder_path, file, '.enc')
-        write_binary(full_path, encrypted_data)
+        file_path = os.path.join(folder_path, file)
+        if os.path.isfile(file_path):
+            data = read_binary(file_path)
+            encryption = Encryption(key, data)
+            encrypted_data = encryption.encrypt()
+            new_file_path = file_path + add_extension
+            write_binary(new_file_path, encrypted_data)
 
 
 def delete_extension(path: str) -> str:
     """
-    Remove the file extension from a path.
+    Remove the last file extension from a path.
+
     :param path: The file path
-    :return:  without the extension
+    :return: The path without the last extension
     """
-    return path[:-4]
+    dir_name, basename = os.path.split(path)
+    while '.' in basename:
+        basename, extension = os.path.splitext(basename)
+        if extension:
+            return os.path.join(dir_name, basename)
+    return path
 
 
 def generate_key(password: str, length: int) -> bytes:
     """
     Create a new key based on the password and save it to a file.
     :param password: Password for a key generation
     :param length: Length key
@@ -96,31 +106,31 @@
     :param file_path: Path of the file
     :return: Binary data from the file
     """
     if not os.path.exists(file_path):
         raise FileNotFoundError(f"File '{file_path}' not found.")
     if os.path.isdir(file_path):
         raise ValueError("Path is a directory. File path is expected.")
-    with open(file_path, 'rb') as file:
-        return file.read()
+    with open(file_path, 'rb') as f:
+        return f.read()
 
 
 def write_binary(file_path, data):
     """
     Write binary data to a file.
     :param file_path: Path of the file to write the data to
     :param data:  write
     :return: True if the file was saved successfully
     """
     if os.path.exists(file_path):
         raise FileNotFoundError(f"File '{file_path}' already exists.")
     if os.path.isdir(file_path):
         raise ValueError("Path is a directory. File path is expected.")
-    with open(file_path, 'wb') as file:
-        file.write(data)
+    with open(file_path, 'wb') as f:
+        f.write(data)
         return True
 
 
 def custom_input(question: str) -> str:
     """
     Take a question as input from the user and return their response.
     :param question: Question to ask the user
```

### Comparing `simple2encrypt-1.1/setup.py` & `simple2encrypt-1.2/simple2encrypt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,33 @@
-from setuptools import setup
-description = """
+Metadata-Version: 2.1
+Name: simple2encrypt
+Version: 1.2
+Summary: Utility functions for encryption and file operations
+Home-page: https://github.com/nhman-python/crypto-utils
+Author: nhman-python
+Author-email: wbgblfix@duck.com
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
 # Encryption Utils
 
 `encryption_utils` is a Python library that provides utility functions for encryption and file operations. It includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, reading and writing binary data from/to files, and handling user input.
 
 ## Installation
 
 You can install `encryption_utils` using `pip`:
 
 ```
 pip install simple2encrypt
 ```
 
 ## Usage
-simple-encrypt
+simple2encrypt
 ### Encryption
 
 To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the library. Here's an example:
 
 ```
 from encryption_utils import Encryption
 
@@ -66,15 +76,15 @@
 ### Reading and Writing Binary Data
 
 The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. Here's an example:
 
 ```
 from encryption_utils import read_binary, write_binary
 
-file_path = '/path/to/file.bin'
+file_path = 'file.bin'
 
 # Read binary data from a file
 data = read_binary(file_path)
 print("Read data:", data)
 
 # Write binary data to a file
 data_to_write = b'mydata'
@@ -102,31 +112,13 @@
 encrypt_data my-key.bin mysecretpassword
 ```
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.0.
+The current version of `encryption_utils` is 1.2.
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
 
-"""
-
-
-setup(
-    name='simple2encrypt',
-    version='1.1',
-    description='Utility functions for encryption and file operations',
-    author='nhman-python',
-    author_email='wbgblfix@duck.com',
-    url='https://github.com/nhman-python/crypto-utils',
-    license='MIT',
-    long_description=description,
-    long_description_content_type='text/markdown',
-    py_modules=['encryption_utils'],
-    install_requires=[
-        'pycryptodome',  # Dependency on pycryptodome package
-    ],
-)
```

### Comparing `simple2encrypt-1.1/simple2encrypt.egg-info/PKG-INFO` & `simple2encrypt-1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,24 @@
-Metadata-Version: 2.1
-Name: simple2encrypt
-Version: 1.1
-Summary: Utility functions for encryption and file operations
-Home-page: https://github.com/nhman-python/crypto-utils
-Author: nhman-python
-Author-email: wbgblfix@duck.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
+from setuptools import setup
 
+description = """
 # Encryption Utils
 
 `encryption_utils` is a Python library that provides utility functions for encryption and file operations. It includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, reading and writing binary data from/to files, and handling user input.
 
 ## Installation
 
 You can install `encryption_utils` using `pip`:
 
 ```
 pip install simple2encrypt
 ```
 
 ## Usage
-simple-encrypt
+simple2encrypt
 ### Encryption
 
 To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the library. Here's an example:
 
 ```
 from encryption_utils import Encryption
 
@@ -76,15 +67,15 @@
 ### Reading and Writing Binary Data
 
 The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. Here's an example:
 
 ```
 from encryption_utils import read_binary, write_binary
 
-file_path = '/path/to/file.bin'
+file_path = 'file.bin'
 
 # Read binary data from a file
 data = read_binary(file_path)
 print("Read data:", data)
 
 # Write binary data to a file
 data_to_write = b'mydata'
@@ -112,13 +103,34 @@
 encrypt_data my-key.bin mysecretpassword
 ```
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.0.
+The current version of `encryption_utils` is 1.2.
 
 ## License
 
 This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
 
+"""
+
+setup(
+    name='simple2encrypt',
+    version='1.2',
+    description='Utility functions for encryption and file operations',
+    author='nhman-python',
+    author_email='wbgblfix@duck.com',
+    url='https://github.com/nhman-python/crypto-utils',
+    license='MIT',
+    long_description=description,
+    long_description_content_type='text/markdown',
+    py_modules=['encryption_utils'],
+    install_requires=[
+        'pycryptodome',  # Dependency on pycryptodome package
+    ],
+    entry_points={
+        'console_scripts': [
+            'encrypt_data = encryption_utils:main']
+    }
+)
```

