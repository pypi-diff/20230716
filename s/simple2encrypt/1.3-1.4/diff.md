# Comparing `tmp/simple2encrypt-1.3.tar.gz` & `tmp/simple2encrypt-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple2encrypt-1.3.tar", last modified: Sun Jul 16 21:13:07 2023, max compression
+gzip compressed data, was "simple2encrypt-1.4.tar", last modified: Sun Jul 16 21:34:37 2023, max compression
```

## Comparing `simple2encrypt-1.3.tar` & `simple2encrypt-1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:13:07.628150 simple2encrypt-1.3/
--rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.3/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     3386 2023-07-16 21:13:07.628150 simple2encrypt-1.3/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.3/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)     5298 2023-07-16 21:12:49.000000 simple2encrypt-1.3/encryption_utils.py
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:13:07.628150 simple2encrypt-1.3/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     3733 2023-07-16 21:12:37.000000 simple2encrypt-1.3/setup.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:13:07.628150 simple2encrypt-1.3/simple2encrypt.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     3386 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      276 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       55 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/requires.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 21:13:07.000000 simple2encrypt-1.3/simple2encrypt.egg-info/top_level.txt
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:34:37.084186 simple2encrypt-1.4/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1068 2023-07-16 09:23:14.000000 simple2encrypt-1.4/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     3526 2023-07-16 21:34:37.084186 simple2encrypt-1.4/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      348 2023-07-16 09:23:14.000000 simple2encrypt-1.4/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)     5297 2023-07-16 21:34:22.000000 simple2encrypt-1.4/encryption_utils.py
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-07-16 21:34:37.084186 simple2encrypt-1.4/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     3918 2023-07-16 21:34:15.000000 simple2encrypt-1.4/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-07-16 21:34:37.084186 simple2encrypt-1.4/simple2encrypt.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     3526 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      276 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       85 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       17 2023-07-16 21:34:37.000000 simple2encrypt-1.4/simple2encrypt.egg-info/top_level.txt
```

### Comparing `simple2encrypt-1.3/LICENSE` & `simple2encrypt-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simple2encrypt-1.3/PKG-INFO` & `simple2encrypt-1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.3
+Version: 1.4
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Encryption Utils
 
-`encryption_utils` is a Python library that provides utility functions for encryption and file operations. It includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, reading and writing binary data from/to files, and handling user input.
+`encryption_utils` is a Python library that provides utility functions for encryption and file operations. It 
+includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, 
+reading and writing binary data from/to files, and handling user input.
 
 ## Installation
 
 You can install `encryption_utils` using `pip`:
 
 ```
 pip install simple2encrypt
 ```
 
 ## Usage
 simple2encrypt
 ### Encryption
 
-To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the library. Here's an example:
+
+To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the 
+library. Here's an example:
 
 ```
 from encryption_utils import Encryption
 
 # Initialize the Encryption object with the key and data
 key = b'mysecretpassword'  # Encryption key
 data = b'mydata'  # Data to be encrypted or decrypted
@@ -71,15 +75,16 @@
 print("Generated key:", key)
 write_binary(path_key, key)
 
 ```
 
 ### Reading and Writing Binary Data
 
-The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. Here's an example:
+The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. 
+Here's an example:
 
 ```
 from encryption_utils import read_binary, write_binary
 
 file_path = 'file.bin'
 
 # Read binary data from a file
@@ -104,21 +109,25 @@
 print("User name:", user_name)
 ```
 
 ### Creating Encryption Key (Command Line)
 
 The library also provides a command-line interface for creating a new encryption key. Here's an example usage:
 
+aes-key  # Executes the main function from encryption_utils module
 ```
-encrypt_data my-key.bin mysecretpassword
+aes-key [file name] [secret-password]
 ```
+aes-message  # Executes the main function from example_message module
+
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.3.
+The current version of `encryption_utils` is 1.4
 
 ## License
 
-This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
+This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
+See the `LICENSE` file for more information.
```

### Comparing `simple2encrypt-1.3/encryption_utils.py` & `simple2encrypt-1.4/encryption_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import sys
 
 from Crypto.Cipher import AES
 from Crypto.Protocol.KDF import PBKDF2
 from Crypto.Util.Padding import pad, unpad
 
-__version__ = '1.3'
+__version__ = '1.4'
 
 
 class Encryption:
     """
     A class for performing encryption and decryption using the AES algorithm.
     """
 
@@ -158,12 +158,12 @@
     try:
         key = generate_key(args.password, length=32)
         key_path = args.filename
         write_binary(key_path, key)
         print(f"A new file was created based on your password. The file name is: {key_path}")
     except (ValueError, FileExistsError) as write_error:
         print(write_error)
-        sys.exit(1)
+        sys.exit()
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `simple2encrypt-1.3/setup.py` & `simple2encrypt-1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from setuptools import setup
 
 description = """
 # Encryption Utils
 
-`encryption_utils` is a Python library that provides utility functions for encryption and file operations. It includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, reading and writing binary data from/to files, and handling user input.
+`encryption_utils` is a Python library that provides utility functions for encryption and file operations. It 
+includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, 
+reading and writing binary data from/to files, and handling user input.
 
 ## Installation
 
 You can install `encryption_utils` using `pip`:
 
 ```
 pip install simple2encrypt
 ```
 
 ## Usage
 simple2encrypt
 ### Encryption
 
-To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the library. Here's an example:
+
+To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the 
+library. Here's an example:
 
 ```
 from encryption_utils import Encryption
 
 # Initialize the Encryption object with the key and data
 key = b'mysecretpassword'  # Encryption key
 data = b'mydata'  # Data to be encrypted or decrypted
@@ -62,15 +66,16 @@
 print("Generated key:", key)
 write_binary(path_key, key)
 
 ```
 
 ### Reading and Writing Binary Data
 
-The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. Here's an example:
+The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. 
+Here's an example:
 
 ```
 from encryption_utils import read_binary, write_binary
 
 file_path = 'file.bin'
 
 # Read binary data from a file
@@ -95,43 +100,48 @@
 print("User name:", user_name)
 ```
 
 ### Creating Encryption Key (Command Line)
 
 The library also provides a command-line interface for creating a new encryption key. Here's an example usage:
 
+aes-key  # Executes the main function from encryption_utils module
 ```
-encrypt_data my-key.bin mysecretpassword
+aes-key [file name] [secret-password]
 ```
+aes-message  # Executes the main function from example_message module
+
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.3.
+The current version of `encryption_utils` is 1.4
 
 ## License
 
-This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
+This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
+See the `LICENSE` file for more information.
 
 """
 
 setup(
     name='simple2encrypt',
-    version='1.3',
+    version='1.4',
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
-            'encrypt_data = encryption_utils:main',
+            'aes-key = encryption_utils:main',
+            'aes-message = example_message:main',
         ],
     }
 )
```

### Comparing `simple2encrypt-1.3/simple2encrypt.egg-info/PKG-INFO` & `simple2encrypt-1.4/simple2encrypt.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 Metadata-Version: 2.1
 Name: simple2encrypt
-Version: 1.3
+Version: 1.4
 Summary: Utility functions for encryption and file operations
 Home-page: https://github.com/nhman-python/crypto-utils
 Author: nhman-python
 Author-email: wbgblfix@duck.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Encryption Utils
 
-`encryption_utils` is a Python library that provides utility functions for encryption and file operations. It includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, reading and writing binary data from/to files, and handling user input.
+`encryption_utils` is a Python library that provides utility functions for encryption and file operations. It 
+includes functionalities for encrypting and decrypting data using the AES algorithm, generating encryption keys, 
+reading and writing binary data from/to files, and handling user input.
 
 ## Installation
 
 You can install `encryption_utils` using `pip`:
 
 ```
 pip install simple2encrypt
 ```
 
 ## Usage
 simple2encrypt
 ### Encryption
 
-To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the library. Here's an example:
+
+To perform encryption and decryption using the AES algorithm, you can use the `Encryption` class provided by the 
+library. Here's an example:
 
 ```
 from encryption_utils import Encryption
 
 # Initialize the Encryption object with the key and data
 key = b'mysecretpassword'  # Encryption key
 data = b'mydata'  # Data to be encrypted or decrypted
@@ -71,15 +75,16 @@
 print("Generated key:", key)
 write_binary(path_key, key)
 
 ```
 
 ### Reading and Writing Binary Data
 
-The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. Here's an example:
+The `read_binary` and `write_binary` functions can be used to read and write binary data from/to files, respectively. 
+Here's an example:
 
 ```
 from encryption_utils import read_binary, write_binary
 
 file_path = 'file.bin'
 
 # Read binary data from a file
@@ -104,21 +109,25 @@
 print("User name:", user_name)
 ```
 
 ### Creating Encryption Key (Command Line)
 
 The library also provides a command-line interface for creating a new encryption key. Here's an example usage:
 
+aes-key  # Executes the main function from encryption_utils module
 ```
-encrypt_data my-key.bin mysecretpassword
+aes-key [file name] [secret-password]
 ```
+aes-message  # Executes the main function from example_message module
+
 
 This will create a new encryption key file named `my-key.bin` based on the provided password.
 
 ## Version
 
-The current version of `encryption_utils` is 1.3.
+The current version of `encryption_utils` is 1.4
 
 ## License
 
-This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). See the `LICENSE` file for more information.
+This library is distributed under the [MIT License](https://github.com/nhman-python/crypto-utils/blob/main/LICENSE). 
+See the `LICENSE` file for more information.
```

