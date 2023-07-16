# Comparing `tmp/tmailor-0.0.10.tar.gz` & `tmp/tmailor-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmailor-0.0.10.tar", last modified: Sun Jul 16 12:55:04 2023, max compression
+gzip compressed data, was "tmailor-0.0.11.tar", last modified: Sun Jul 16 13:42:58 2023, max compression
```

## Comparing `tmailor-0.0.10.tar` & `tmailor-0.0.11.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 12:55:04.434247 tmailor-0.0.10/
--rw-r--r--   0 runner    (1000) runner    (1000)     1082 2023-07-16 12:53:15.000000 tmailor-0.0.10/LICENSE
--rw-r--r--   0 runner    (1000) runner    (1000)     2913 2023-07-16 12:55:04.434247 tmailor-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     2306 2023-07-16 12:53:15.000000 tmailor-0.0.10/README.md
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-16 12:55:04.434247 tmailor-0.0.10/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)     1000 2023-07-16 12:53:15.000000 tmailor-0.0.10/setup.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 12:55:04.434247 tmailor-0.0.10/tmailor/
--rw-r--r--   0 runner    (1000) runner    (1000)       35 2023-07-16 12:53:15.000000 tmailor-0.0.10/tmailor/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     2050 2023-07-16 12:53:15.000000 tmailor-0.0.10/tmailor/client.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 12:55:04.434247 tmailor-0.0.10/tmailor/ext/
--rw-r--r--   0 runner    (1000) runner    (1000)       68 2023-07-16 12:53:15.000000 tmailor-0.0.10/tmailor/ext/__init__.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 12:55:04.434247 tmailor-0.0.10/tmailor/ext/utilities/
--rw-r--r--   0 runner    (1000) runner    (1000)       72 2023-07-16 12:53:15.000000 tmailor-0.0.10/tmailor/ext/utilities/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      807 2023-07-16 12:53:15.000000 tmailor-0.0.10/tmailor/ext/utilities/exceptions.py
--rw-r--r--   0 runner    (1000) runner    (1000)      331 2023-07-16 12:53:15.000000 tmailor-0.0.10/tmailor/ext/utilities/headers.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1570 2023-07-16 12:53:15.000000 tmailor-0.0.10/tmailor/ext/utilities/objects.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 12:55:04.434247 tmailor-0.0.10/tmailor.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     2913 2023-07-16 12:55:04.000000 tmailor-0.0.10/tmailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-07-16 12:55:04.000000 tmailor-0.0.10/tmailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-16 12:55:04.000000 tmailor-0.0.10/tmailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-07-16 12:55:04.000000 tmailor-0.0.10/tmailor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1082 2023-07-16 13:37:58.000000 tmailor-0.0.11/LICENSE
+-rw-r--r--   0 runner    (1000) runner    (1000)     2913 2023-07-16 13:42:58.296985 tmailor-0.0.11/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     2306 2023-07-16 13:37:58.000000 tmailor-0.0.11/README.md
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-07-16 13:42:58.296985 tmailor-0.0.11/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)     1016 2023-07-16 13:42:06.000000 tmailor-0.0.11/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/tmailor/
+-rw-r--r--   0 runner    (1000) runner    (1000)       35 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     3917 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/client.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/tmailor/ext/
+-rw-r--r--   0 runner    (1000) runner    (1000)       68 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/__init__.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/tmailor/ext/utilities/
+-rw-r--r--   0 runner    (1000) runner    (1000)       72 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/utilities/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      807 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/utilities/exceptions.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      331 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/utilities/headers.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     2036 2023-07-16 13:37:58.000000 tmailor-0.0.11/tmailor/ext/utilities/objects.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-07-16 13:42:58.296985 tmailor-0.0.11/tmailor.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     2913 2023-07-16 13:42:58.000000 tmailor-0.0.11/tmailor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      348 2023-07-16 13:42:58.000000 tmailor-0.0.11/tmailor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-07-16 13:42:58.000000 tmailor-0.0.11/tmailor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2023-07-16 13:42:58.000000 tmailor-0.0.11/tmailor.egg-info/top_level.txt
```

### Comparing `tmailor-0.0.10/LICENSE` & `tmailor-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `tmailor-0.0.10/PKG-INFO` & `tmailor-0.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmailor
-Version: 0.0.10
+Version: 0.0.11
 Summary: A temporary email address is: a library that provides email addresses without registration, used to receive incoming emails without disclosing your actual email.
 Home-page: https://github.com/heromr/tmailor
 Author: HeroMR
 Author-email: mrhero4006@gmail.com
 License: MIT
 Keywords: python,tmailor,temp mail,disposable email,temp mailbox,fake email
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tmailor Version: 0.0.10 Summary: A temporary email
+Metadata-Version: 2.1 Name: tmailor Version: 0.0.11 Summary: A temporary email
 address is: a library that provides email addresses without registration, used
 to receive incoming emails without disclosing your actual email. Home-page:
 https://github.com/heromr/tmailor Author: HeroMR Author-email:
 mrhero4006@gmail.com License: MIT Keywords: python,tmailor,temp mail,disposable
 email,temp mailbox,fake email Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
```

### Comparing `tmailor-0.0.10/README.md` & `tmailor-0.0.11/README.md`

 * *Files identical despite different names*

### Comparing `tmailor-0.0.10/tmailor/ext/utilities/exceptions.py` & `tmailor-0.0.11/tmailor/ext/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `tmailor-0.0.10/tmailor.egg-info/PKG-INFO` & `tmailor-0.0.11/tmailor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmailor
-Version: 0.0.10
+Version: 0.0.11
 Summary: A temporary email address is: a library that provides email addresses without registration, used to receive incoming emails without disclosing your actual email.
 Home-page: https://github.com/heromr/tmailor
 Author: HeroMR
 Author-email: mrhero4006@gmail.com
 License: MIT
 Keywords: python,tmailor,temp mail,disposable email,temp mailbox,fake email
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tmailor Version: 0.0.10 Summary: A temporary email
+Metadata-Version: 2.1 Name: tmailor Version: 0.0.11 Summary: A temporary email
 address is: a library that provides email addresses without registration, used
 to receive incoming emails without disclosing your actual email. Home-page:
 https://github.com/heromr/tmailor Author: HeroMR Author-email:
 mrhero4006@gmail.com License: MIT Keywords: python,tmailor,temp mail,disposable
 email,temp mailbox,fake email Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: Operating System :: OS Independent
```

