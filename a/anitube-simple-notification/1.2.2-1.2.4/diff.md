# Comparing `tmp/anitube-simple-notification-1.2.2.tar.gz` & `tmp/anitube-simple-notification-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anitube-simple-notification-1.2.2.tar", last modified: Sun Jul 16 11:52:25 2023, max compression
+gzip compressed data, was "anitube-simple-notification-1.2.4.tar", last modified: Sun Jul 16 12:46:19 2023, max compression
```

## Comparing `anitube-simple-notification-1.2.2.tar` & `anitube-simple-notification-1.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 11:52:25.494387 anitube-simple-notification-1.2.2/
--rw-r--r--   0 root         (0) root         (0)    35149 2023-07-16 11:51:55.000000 anitube-simple-notification-1.2.2/COPYING
--rw-r--r--   0 root         (0) root         (0)    42296 2023-07-16 11:52:25.494387 anitube-simple-notification-1.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1131 2023-07-16 11:51:55.000000 anitube-simple-notification-1.2.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 11:52:25.490387 anitube-simple-notification-1.2.2/anitube_simple_notification.egg-info/
--rw-r--r--   0 root         (0) root         (0)    42296 2023-07-16 11:52:25.000000 anitube-simple-notification-1.2.2/anitube_simple_notification.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      406 2023-07-16 11:52:25.000000 anitube-simple-notification-1.2.2/anitube_simple_notification.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 11:52:25.000000 anitube-simple-notification-1.2.2/anitube_simple_notification.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-16 11:52:25.000000 anitube-simple-notification-1.2.2/anitube_simple_notification.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-16 11:52:25.000000 anitube-simple-notification-1.2.2/anitube_simple_notification.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-07-16 11:52:25.000000 anitube-simple-notification-1.2.2/anitube_simple_notification.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1032 2023-07-16 11:51:55.000000 anitube-simple-notification-1.2.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 11:52:25.494387 anitube-simple-notification-1.2.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 11:52:25.494387 anitube-simple-notification-1.2.2/src/
--rw-r--r--   0 root         (0) root         (0)     4420 2023-07-16 11:51:55.000000 anitube-simple-notification-1.2.2/src/config.py
--rw-r--r--   0 root         (0) root         (0)     3933 2023-07-16 11:51:55.000000 anitube-simple-notification-1.2.2/src/db.py
--rw-r--r--   0 root         (0) root         (0)     4127 2023-07-16 11:51:55.000000 anitube-simple-notification-1.2.2/src/main.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-07-16 11:51:55.000000 anitube-simple-notification-1.2.2/src/notify.py
--rw-r--r--   0 root         (0) root         (0)     3455 2023-07-16 11:51:55.000000 anitube-simple-notification-1.2.2/src/scraper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 12:46:19.097165 anitube-simple-notification-1.2.4/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-07-16 12:45:53.000000 anitube-simple-notification-1.2.4/COPYING
+-rw-r--r--   0 root         (0) root         (0)    42600 2023-07-16 12:46:19.093165 anitube-simple-notification-1.2.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-07-16 12:45:53.000000 anitube-simple-notification-1.2.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 12:46:19.093165 anitube-simple-notification-1.2.4/anitube_simple_notification.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    42600 2023-07-16 12:46:19.000000 anitube-simple-notification-1.2.4/anitube_simple_notification.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      406 2023-07-16 12:46:19.000000 anitube-simple-notification-1.2.4/anitube_simple_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-16 12:46:19.000000 anitube-simple-notification-1.2.4/anitube_simple_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-16 12:46:19.000000 anitube-simple-notification-1.2.4/anitube_simple_notification.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-16 12:46:19.000000 anitube-simple-notification-1.2.4/anitube_simple_notification.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-16 12:46:19.000000 anitube-simple-notification-1.2.4/anitube_simple_notification.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-07-16 12:45:53.000000 anitube-simple-notification-1.2.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-16 12:46:19.097165 anitube-simple-notification-1.2.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-16 12:46:19.093165 anitube-simple-notification-1.2.4/src/
+-rw-r--r--   0 root         (0) root         (0)     4420 2023-07-16 12:45:53.000000 anitube-simple-notification-1.2.4/src/config.py
+-rw-r--r--   0 root         (0) root         (0)     3933 2023-07-16 12:45:53.000000 anitube-simple-notification-1.2.4/src/db.py
+-rw-r--r--   0 root         (0) root         (0)     4127 2023-07-16 12:45:53.000000 anitube-simple-notification-1.2.4/src/main.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-07-16 12:45:53.000000 anitube-simple-notification-1.2.4/src/notify.py
+-rw-r--r--   0 root         (0) root         (0)     3455 2023-07-16 12:45:53.000000 anitube-simple-notification-1.2.4/src/scraper.py
```

### Comparing `anitube-simple-notification-1.2.2/COPYING` & `anitube-simple-notification-1.2.4/COPYING`

 * *Files identical despite different names*

### Comparing `anitube-simple-notification-1.2.2/PKG-INFO` & `anitube-simple-notification-1.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anitube-simple-notification
-Version: 1.2.2
+Version: 1.2.4
 Summary: Getting notification from anitube.in.ua.
 Author-email: Kostiantyn Klochko <kklochko@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,14 +689,35 @@
 
 Anitube Simple Notification
 ===========================
 
 Anitube Simple Notification is a application made for getting
 notification when a content is updated on the web-site (anitube.in.ua).
 
+Install
+=======
+
+Ensure that python and pip are installed:
+
+.. code:: shell
+
+   python --version
+   python -m pip -V
+   # or
+   python3 --version
+   python3 -m pip -V
+
+Install the package:
+
+.. code:: shell
+
+   pip install anitube-simple-notification
+   # or
+   pip3 install anitube-simple-notification
+
 Usage
 =====
 
 In application folder create file with name ``config.toml``. If a value
 is wrong, then a error will be shown. If there no value or a wrong value
 then it will be default.
 
@@ -715,16 +736,16 @@
 
 The last comma of the urls list can be ommited.
 
 Run the program by one of the commands:
 
 .. code:: shell
 
-   python3 main.py
-   python main.py
+   anitube-simple-notification
+   asn
 
 Author
 ======
 
 Kostiantyn Klochko (c) 2022-2023
 
 Donation
```

### Comparing `anitube-simple-notification-1.2.2/README.rst` & `anitube-simple-notification-1.2.4/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,34 @@
 Anitube Simple Notification
 ===========================
 
 Anitube Simple Notification is a application made for getting
 notification when a content is updated on the web-site (anitube.in.ua).
 
+Install
+=======
+
+Ensure that python and pip are installed:
+
+.. code:: shell
+
+   python --version
+   python -m pip -V
+   # or
+   python3 --version
+   python3 -m pip -V
+
+Install the package:
+
+.. code:: shell
+
+   pip install anitube-simple-notification
+   # or
+   pip3 install anitube-simple-notification
+
 Usage
 =====
 
 In application folder create file with name ``config.toml``. If a value
 is wrong, then a error will be shown. If there no value or a wrong value
 then it will be default.
 
@@ -26,16 +47,16 @@
 
 The last comma of the urls list can be ommited.
 
 Run the program by one of the commands:
 
 .. code:: shell
 
-   python3 main.py
-   python main.py
+   anitube-simple-notification
+   asn
 
 Author
 ======
 
 Kostiantyn Klochko (c) 2022-2023
 
 Donation
```

### Comparing `anitube-simple-notification-1.2.2/anitube_simple_notification.egg-info/PKG-INFO` & `anitube-simple-notification-1.2.4/anitube_simple_notification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anitube-simple-notification
-Version: 1.2.2
+Version: 1.2.4
 Summary: Getting notification from anitube.in.ua.
 Author-email: Kostiantyn Klochko <kklochko@protonmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -689,14 +689,35 @@
 
 Anitube Simple Notification
 ===========================
 
 Anitube Simple Notification is a application made for getting
 notification when a content is updated on the web-site (anitube.in.ua).
 
+Install
+=======
+
+Ensure that python and pip are installed:
+
+.. code:: shell
+
+   python --version
+   python -m pip -V
+   # or
+   python3 --version
+   python3 -m pip -V
+
+Install the package:
+
+.. code:: shell
+
+   pip install anitube-simple-notification
+   # or
+   pip3 install anitube-simple-notification
+
 Usage
 =====
 
 In application folder create file with name ``config.toml``. If a value
 is wrong, then a error will be shown. If there no value or a wrong value
 then it will be default.
 
@@ -715,16 +736,16 @@
 
 The last comma of the urls list can be ommited.
 
 Run the program by one of the commands:
 
 .. code:: shell
 
-   python3 main.py
-   python main.py
+   anitube-simple-notification
+   asn
 
 Author
 ======
 
 Kostiantyn Klochko (c) 2022-2023
 
 Donation
```

### Comparing `anitube-simple-notification-1.2.2/pyproject.toml` & `anitube-simple-notification-1.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anitube-simple-notification"
-version = "1.2.2"
+version = "1.2.4"
 authors = [
   { name="Kostiantyn Klochko", email="kklochko@protonmail.com" },
 ]
 description = "Getting notification from anitube.in.ua."
 readme = "README.rst"
 license = { file="COPYING" }
 requires-python = ">=3.10"
@@ -24,15 +24,15 @@
     "rich~=13.1.0",
     "tomli~=2.0.1",
     "loguru~=0.5.3",
     "platformdirs~=3.0.0"
 ]
 
 [project.scripts]
-ans = "src.main:main"
+asn = "src.main:main"
 anitube-simple-notification = "src.main:main"
 
 [project.urls]
 "Homepage" = "https://gitlab.com/KKlochko/anitube-simple-notification"
 "Bug Tracker" = "https://gitlab.com/KKlochko/anitube-simple-notification/issues"
 
 [tool.setuptools]
```

### Comparing `anitube-simple-notification-1.2.2/src/config.py` & `anitube-simple-notification-1.2.4/src/config.py`

 * *Files identical despite different names*

### Comparing `anitube-simple-notification-1.2.2/src/db.py` & `anitube-simple-notification-1.2.4/src/db.py`

 * *Files identical despite different names*

### Comparing `anitube-simple-notification-1.2.2/src/main.py` & `anitube-simple-notification-1.2.4/src/main.py`

 * *Files identical despite different names*

### Comparing `anitube-simple-notification-1.2.2/src/notify.py` & `anitube-simple-notification-1.2.4/src/notify.py`

 * *Files identical despite different names*

### Comparing `anitube-simple-notification-1.2.2/src/scraper.py` & `anitube-simple-notification-1.2.4/src/scraper.py`

 * *Files identical despite different names*

