# Comparing `tmp/masterpass-0.2.1.tar.gz` & `tmp/masterpass-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masterpass-0.2.1.tar", last modified: Mon Mar  6 22:50:56 2023, max compression
+gzip compressed data, was "masterpass-0.2.2.tar", last modified: Sun Jul 16 16:47:25 2023, max compression
```

## Comparing `masterpass-0.2.1.tar` & `masterpass-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-03-06 22:50:56.028857 masterpass-0.2.1/
--rw-r--r--   0 pedro      (503) staff       (20)     2404 2023-03-06 22:50:56.028545 masterpass-0.2.1/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)     1792 2023-03-06 22:50:03.000000 masterpass-0.2.1/README.md
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-03-06 22:50:56.025964 masterpass-0.2.1/master/
--rw-r--r--   0 pedro      (503) staff       (20)       18 2023-03-06 22:50:44.000000 masterpass-0.2.1/master/__init__.py
--rwxr-xr-x   0 pedro      (503) staff       (20)     2147 2023-03-06 22:50:05.000000 masterpass-0.2.1/master/cli.py
--rw-r--r--   0 pedro      (503) staff       (20)      702 2023-02-21 19:31:05.000000 masterpass-0.2.1/master/logger.py
--rw-r--r--   0 pedro      (503) staff       (20)     2500 2023-03-06 22:31:55.000000 masterpass-0.2.1/master/master.py
-drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-03-06 22:50:56.027998 masterpass-0.2.1/masterpass.egg-info/
--rw-r--r--   0 pedro      (503) staff       (20)     2404 2023-03-06 22:50:55.000000 masterpass-0.2.1/masterpass.egg-info/PKG-INFO
--rw-r--r--   0 pedro      (503) staff       (20)      258 2023-03-06 22:50:55.000000 masterpass-0.2.1/masterpass.egg-info/SOURCES.txt
--rw-r--r--   0 pedro      (503) staff       (20)        1 2023-03-06 22:50:55.000000 masterpass-0.2.1/masterpass.egg-info/dependency_links.txt
--rw-r--r--   0 pedro      (503) staff       (20)       43 2023-03-06 22:50:55.000000 masterpass-0.2.1/masterpass.egg-info/entry_points.txt
--rw-r--r--   0 pedro      (503) staff       (20)        7 2023-03-06 22:50:55.000000 masterpass-0.2.1/masterpass.egg-info/top_level.txt
--rw-r--r--   0 pedro      (503) staff       (20)       38 2023-03-06 22:50:56.028953 masterpass-0.2.1/setup.cfg
--rw-r--r--   0 pedro      (503) staff       (20)      993 2023-03-06 22:50:09.000000 masterpass-0.2.1/setup.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-16 16:47:25.103395 masterpass-0.2.2/
+-rw-r--r--   0 pedro      (503) staff       (20)     1076 2023-07-16 16:43:11.000000 masterpass-0.2.2/LICENSE
+-rw-r--r--   0 pedro      (503) staff       (20)     2749 2023-07-16 16:47:25.097844 masterpass-0.2.2/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)     2109 2023-07-16 16:31:39.000000 masterpass-0.2.2/README.md
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-16 16:47:25.096711 masterpass-0.2.2/master/
+-rw-r--r--   0 pedro      (503) staff       (20)       18 2023-07-16 16:28:05.000000 masterpass-0.2.2/master/__init__.py
+-rwxr-xr-x   0 pedro      (503) staff       (20)     3604 2023-07-16 16:28:35.000000 masterpass-0.2.2/master/cli.py
+-rw-r--r--   0 pedro      (503) staff       (20)      953 2023-07-16 16:09:16.000000 masterpass-0.2.2/master/logger.py
+-rw-r--r--   0 pedro      (503) staff       (20)     2179 2023-07-16 16:09:38.000000 masterpass-0.2.2/master/master.py
+drwxr-xr-x   0 pedro      (503) staff       (20)        0 2023-07-16 16:47:25.097628 masterpass-0.2.2/masterpass.egg-info/
+-rw-r--r--   0 pedro      (503) staff       (20)     2749 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/PKG-INFO
+-rw-r--r--   0 pedro      (503) staff       (20)      266 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/SOURCES.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        1 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/dependency_links.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       43 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/entry_points.txt
+-rw-r--r--   0 pedro      (503) staff       (20)        7 2023-07-16 16:47:25.000000 masterpass-0.2.2/masterpass.egg-info/top_level.txt
+-rw-r--r--   0 pedro      (503) staff       (20)       38 2023-07-16 16:47:25.103451 masterpass-0.2.2/setup.cfg
+-rw-r--r--   0 pedro      (503) staff       (20)      946 2023-07-16 16:19:44.000000 masterpass-0.2.2/setup.py
```

### Comparing `masterpass-0.2.1/PKG-INFO` & `masterpass-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: masterpass
-Version: 0.2.1
-Summary: Deterministic passwords for everyone
+Version: 0.2.2
+Summary: Deterministic password generator
 Home-page: https://github.com/jpedro/master
 Download-URL: https://github.com/jpedro/master/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
-Keywords: deterministic password
+Keywords: deterministic password generator
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Master
 
-![Strong password](https://raw.githubusercontent.com/jpedro/master/master/.github/assets/password.jpeg)
+[![Deploy pages](https://github.com/jpedro/master/actions/workflows/pages.yaml/badge.svg)](https://github.com/jpedro/master/actions/workflows/pages.yaml)
 
-Deterministic passwords for everyone.
+Generates deterministic passwords
+
+Inspired by [spectre.app](https://spectre.app/) but simpler.
 
-This uses a sha256 hashed combination of `username + password + service`
-to generate the same password, over and over again, thus eliminating
-the need to store, maintain and back up other generated passwords.
 
-The username and password **are not stored anywhere**.
+![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg)
+<!-- ![Strong password](https://raw.githubusercontent.com/jpedro/master/master/docs/blink.gif) -->
+
+This uses a sha256 hashed combination of `username + password + service`
+to generate the same password, thus eliminating the need to store,
+maintain and back up other generated passwords.
 
-The used service name list is kept under the file `~/.config/master/list.txt`
-(or whatever `MASTER_LIST` points to) *purely for autocompletion*,
-which will be added later.
+The used service name list is kept under the file
+`~/.config/master/list.txt` (or whatever `MASTER_LIST` points to)
+*purely for autocompletion*, which will be added later.
 
 
 ## Install
 
     pip install masterpass
 
 Yes, yes. The package is called `masterpass` but the binary is called
@@ -69,7 +74,13 @@
 | `MASTER_PASSWORD`   | (None) [1]                    |
 | `MASTER_SEPARATOR`  | `-`                           |
 | `MASTER_LENGTH`     | `6`                           |
 | `MASTER_CHUNKS`     | `6`                           |
 
 **Note [1]:** If you don't set the `MASTER_USERNAME` or the
 `MASTER_PASSWORD` you will be prompted for them.
+
+
+## Online
+
+[jpedro.github.io/master](https://jpedro.github.io/master/) has the
+browser experience.
```

### Comparing `masterpass-0.2.1/README.md` & `masterpass-0.2.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Master
 
-![Strong password](https://raw.githubusercontent.com/jpedro/master/master/.github/assets/password.jpeg)
+[![Deploy pages](https://github.com/jpedro/master/actions/workflows/pages.yaml/badge.svg)](https://github.com/jpedro/master/actions/workflows/pages.yaml)
 
-Deterministic passwords for everyone.
+Generates deterministic passwords
+
+Inspired by [spectre.app](https://spectre.app/) but simpler.
 
-This uses a sha256 hashed combination of `username + password + service`
-to generate the same password, over and over again, thus eliminating
-the need to store, maintain and back up other generated passwords.
 
-The username and password **are not stored anywhere**.
+![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg)
+<!-- ![Strong password](https://raw.githubusercontent.com/jpedro/master/master/docs/blink.gif) -->
+
+This uses a sha256 hashed combination of `username + password + service`
+to generate the same password, thus eliminating the need to store,
+maintain and back up other generated passwords.
 
-The used service name list is kept under the file `~/.config/master/list.txt`
-(or whatever `MASTER_LIST` points to) *purely for autocompletion*,
-which will be added later.
+The used service name list is kept under the file
+`~/.config/master/list.txt` (or whatever `MASTER_LIST` points to)
+*purely for autocompletion*, which will be added later.
 
 
 ## Install
 
     pip install masterpass
 
 Yes, yes. The package is called `masterpass` but the binary is called
@@ -51,7 +55,13 @@
 | `MASTER_PASSWORD`   | (None) [1]                    |
 | `MASTER_SEPARATOR`  | `-`                           |
 | `MASTER_LENGTH`     | `6`                           |
 | `MASTER_CHUNKS`     | `6`                           |
 
 **Note [1]:** If you don't set the `MASTER_USERNAME` or the
 `MASTER_PASSWORD` you will be prompted for them.
+
+
+## Online
+
+[jpedro.github.io/master](https://jpedro.github.io/master/) has the
+browser experience.
```

### Comparing `masterpass-0.2.1/masterpass.egg-info/PKG-INFO` & `masterpass-0.2.2/masterpass.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,45 @@
 Metadata-Version: 2.1
 Name: masterpass
-Version: 0.2.1
-Summary: Deterministic passwords for everyone
+Version: 0.2.2
+Summary: Deterministic password generator
 Home-page: https://github.com/jpedro/master
 Download-URL: https://github.com/jpedro/master/tarball/master
 Author: jpedro
 Author-email: jpedro.barbosa@gmail.com
 License: MIT
-Keywords: deterministic password
+Keywords: deterministic password generator
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Master
 
-![Strong password](https://raw.githubusercontent.com/jpedro/master/master/.github/assets/password.jpeg)
+[![Deploy pages](https://github.com/jpedro/master/actions/workflows/pages.yaml/badge.svg)](https://github.com/jpedro/master/actions/workflows/pages.yaml)
 
-Deterministic passwords for everyone.
+Generates deterministic passwords
+
+Inspired by [spectre.app](https://spectre.app/) but simpler.
 
-This uses a sha256 hashed combination of `username + password + service`
-to generate the same password, over and over again, thus eliminating
-the need to store, maintain and back up other generated passwords.
 
-The username and password **are not stored anywhere**.
+![Pictutre](https://raw.githubusercontent.com/jpedro/master/master/docs/strong.jpg)
+<!-- ![Strong password](https://raw.githubusercontent.com/jpedro/master/master/docs/blink.gif) -->
+
+This uses a sha256 hashed combination of `username + password + service`
+to generate the same password, thus eliminating the need to store,
+maintain and back up other generated passwords.
 
-The used service name list is kept under the file `~/.config/master/list.txt`
-(or whatever `MASTER_LIST` points to) *purely for autocompletion*,
-which will be added later.
+The used service name list is kept under the file
+`~/.config/master/list.txt` (or whatever `MASTER_LIST` points to)
+*purely for autocompletion*, which will be added later.
 
 
 ## Install
 
     pip install masterpass
 
 Yes, yes. The package is called `masterpass` but the binary is called
@@ -69,7 +74,13 @@
 | `MASTER_PASSWORD`   | (None) [1]                    |
 | `MASTER_SEPARATOR`  | `-`                           |
 | `MASTER_LENGTH`     | `6`                           |
 | `MASTER_CHUNKS`     | `6`                           |
 
 **Note [1]:** If you don't set the `MASTER_USERNAME` or the
 `MASTER_PASSWORD` you will be prompted for them.
+
+
+## Online
+
+[jpedro.github.io/master](https://jpedro.github.io/master/) has the
+browser experience.
```

### Comparing `masterpass-0.2.1/setup.py` & `masterpass-0.2.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 from setuptools import setup
 from master import VERSION
 
 setup(
     name="masterpass",
     version=VERSION,
-    description="Deterministic passwords for everyone",
+    description="Deterministic password generator",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     author="jpedro",
     author_email="jpedro.barbosa@gmail.com",
     url="https://github.com/jpedro/master",
     download_url="https://github.com/jpedro/master/tarball/master",
-    keywords="deterministic password",
+    keywords="deterministic password generator",
     license="MIT",
     python_requires='>=3',
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
     ],
     packages=[
         "master",
     ],
-    # install_requires=[
-    #     "click",
-    # ],
     entry_points={
         "console_scripts": [
             "master=master.cli:main",
         ],
     },
 )
```

