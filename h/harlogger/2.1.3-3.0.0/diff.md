# Comparing `tmp/harlogger-2.1.3.tar.gz` & `tmp/harlogger-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlogger-2.1.3.tar", last modified: Tue May 16 09:39:59 2023, max compression
+gzip compressed data, was "harlogger-3.0.0.tar", last modified: Sun Jul 16 15:30:35 2023, max compression
```

## Comparing `harlogger-2.1.3.tar` & `harlogger-3.0.0.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:39:59.263680 harlogger-2.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-16 09:39:43.000000 harlogger-2.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46960 2023-05-16 09:39:59.263680 harlogger-2.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-16 09:39:43.000000 harlogger-2.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:39:59.263680 harlogger-2.1.3/harlogger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 09:39:43.000000 harlogger-2.1.3/harlogger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-05-16 09:39:43.000000 harlogger-2.1.3/harlogger/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:39:59.263680 harlogger-2.1.3/harlogger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46960 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 09:39:59.000000 harlogger-2.1.3/harlogger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-16 09:39:43.000000 harlogger-2.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 09:39:43.000000 harlogger-2.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:39:59.263680 harlogger-2.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:30:35.663331 harlogger-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-07-16 15:30:18.000000 harlogger-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    46994 2023-07-16 15:30:35.663331 harlogger-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-07-16 15:30:18.000000 harlogger-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:30:35.663331 harlogger-3.0.0/harlogger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/haralyzer_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/http_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6713 2023-07-16 15:30:18.000000 harlogger-3.0.0/harlogger/sniffers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 15:30:35.663331 harlogger-3.0.0/harlogger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    46994 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 15:30:35.000000 harlogger-3.0.0/harlogger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-16 15:30:18.000000 harlogger-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-16 15:30:18.000000 harlogger-3.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 15:30:35.663331 harlogger-3.0.0/setup.cfg
```

### Comparing `harlogger-2.1.3/LICENSE` & `harlogger-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `harlogger-2.1.3/PKG-INFO` & `harlogger-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: harlogger
-Version: 2.1.3
+Version: 3.0.0
 Summary: Simple utlity for sniffing decrypted HTTP/HTTPS traffic on an iOS device (either jailbroken or not)
-Author-email: doronz88 <doron88@gmail.com>
-Maintainer-email: doronz88 <doron88@gmail.com>
+Author-email: doronz88 <doron88@gmail.com>, netanelc305 <netanelc305@protonmail.com>
+Maintainer-email: doronz88 <doron88@gmail.com>, netanelc305 <netanelc305@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -681,21 +681,20 @@
         
 Project-URL: Homepage, https://github.com/doronz88/harlogger
 Project-URL: Bug Reports, https://github.com/doronz88/harlogger/issues
 Keywords: ios,http,https,har,sniffer,jailbroken
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Description
 
 Simple pure python utility for sniffing HTTP/HTTPS decrypted traffic recorded by one of Apple's not-so-well documented
```

### Comparing `harlogger-2.1.3/README.md` & `harlogger-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `harlogger-2.1.3/harlogger.egg-info/PKG-INFO` & `harlogger-3.0.0/harlogger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: harlogger
-Version: 2.1.3
+Version: 3.0.0
 Summary: Simple utlity for sniffing decrypted HTTP/HTTPS traffic on an iOS device (either jailbroken or not)
-Author-email: doronz88 <doron88@gmail.com>
-Maintainer-email: doronz88 <doron88@gmail.com>
+Author-email: doronz88 <doron88@gmail.com>, netanelc305 <netanelc305@protonmail.com>
+Maintainer-email: doronz88 <doron88@gmail.com>, netanelc305 <netanelc305@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
         
@@ -681,21 +681,20 @@
         
 Project-URL: Homepage, https://github.com/doronz88/harlogger
 Project-URL: Bug Reports, https://github.com/doronz88/harlogger/issues
 Keywords: ios,http,https,har,sniffer,jailbroken
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # Description
 
 Simple pure python utility for sniffing HTTP/HTTPS decrypted traffic recorded by one of Apple's not-so-well documented
```

### Comparing `harlogger-2.1.3/pyproject.toml` & `harlogger-3.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 [project]
 name = "harlogger"
-version = "2.1.3"
+version = "3.0.0"
 description = "Simple utlity for sniffing decrypted HTTP/HTTPS traffic on an iOS device (either jailbroken or not)"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "http", "https", "har", "sniffer", "jailbroken"]
 authors = [
-    { name = "doronz88", email = "doron88@gmail.com" }
+    { name = "doronz88", email = "doron88@gmail.com" },
+    { name = "netanelc305", email = "netanelc305@protonmail.com" }
+
 ]
 maintainers = [
-    { name = "doronz88", email = "doron88@gmail.com" }
+    { name = "doronz88", email = "doron88@gmail.com" },
+    { name = "netanelc305", email = "netanelc305@protonmail.com" }
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dynamic = ["dependencies"]
```

