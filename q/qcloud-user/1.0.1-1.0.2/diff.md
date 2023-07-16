# Comparing `tmp/qcloud_user-1.0.1.tar.gz` & `tmp/qcloud_user-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_user-1.0.1.tar", last modified: Fri Jun 30 01:16:38 2023, max compression
+gzip compressed data, was "qcloud_user-1.0.2.tar", last modified: Sun Jul 16 09:17:12 2023, max compression
```

## Comparing `qcloud_user-1.0.1.tar` & `qcloud_user-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:16:38.796097 qcloud_user-1.0.1/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.1/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)     4398 2023-06-30 01:16:38.795974 qcloud_user-1.0.1/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)     3399 2023-06-30 01:14:34.000000 qcloud_user-1.0.1/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      721 2023-06-30 01:16:24.000000 qcloud_user-1.0.1/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:16:38.795577 qcloud_user-1.0.1/qcloud_user.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)     4398 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      316 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       44 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      153 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       12 2023-06-30 01:16:38.000000 qcloud_user-1.0.1/qcloud_user.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-06-30 01:16:38.796135 qcloud_user-1.0.1/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      793 2023-06-30 01:16:33.000000 qcloud_user-1.0.1/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:16:38.794350 qcloud_user-1.0.1/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-06-30 01:16:38.795794 qcloud_user-1.0.1/src/qcloud_user/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.1/src/qcloud_user/__init__.py
--rwxr-x---   0 agilbert   (501) staff       (20)    21719 2023-06-29 05:57:07.000000 qcloud_user-1.0.1/src/qcloud_user/qcloud_user.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-16 09:17:12.135599 qcloud_user-1.0.2/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:49:28.000000 qcloud_user-1.0.2/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-07-16 09:17:12.135482 qcloud_user-1.0.2/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)     3473 2023-07-12 22:23:41.000000 qcloud_user-1.0.2/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      721 2023-07-12 22:21:59.000000 qcloud_user-1.0.2/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-16 09:17:12.135093 qcloud_user-1.0.2/qcloud_user.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)     4472 2023-07-16 09:17:12.000000 qcloud_user-1.0.2/qcloud_user.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      316 2023-07-16 09:17:12.000000 qcloud_user-1.0.2/qcloud_user.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-16 09:17:12.000000 qcloud_user-1.0.2/qcloud_user.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       44 2023-07-16 09:17:12.000000 qcloud_user-1.0.2/qcloud_user.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      153 2023-07-16 09:17:12.000000 qcloud_user-1.0.2/qcloud_user.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       12 2023-07-16 09:17:12.000000 qcloud_user-1.0.2/qcloud_user.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-16 09:17:12.135635 qcloud_user-1.0.2/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      793 2023-07-12 22:21:51.000000 qcloud_user-1.0.2/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-16 09:17:12.133914 qcloud_user-1.0.2/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-16 09:17:12.135309 qcloud_user-1.0.2/src/qcloud_user/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-27 02:16:27.000000 qcloud_user-1.0.2/src/qcloud_user/__init__.py
+-rwxr-x---   0 agilbert   (501) staff       (20)    22024 2023-07-16 09:16:55.000000 qcloud_user-1.0.2/src/qcloud_user/qcloud_user.py
```

### Comparing `qcloud_user-1.0.1/LICENSE.txt` & `qcloud_user-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_user-1.0.1/PKG-INFO` & `qcloud_user-1.0.2/qcloud_user.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qcloud_user
-Version: 1.0.1
+Name: qcloud-user
+Version: 1.0.2
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -72,15 +72,16 @@
 ...
 ```
 The number of threads can be specified by using the `--ncpu` flag, for example:
 ```
 qcloud --submit --ncpu 4 job1.inp 
 ```
 Note that if the number of threads specified exceeds the number of cores on 
-an individual compute node, the job will not run.
+an individual compute node, the job will not run.  Your QCloud administrator
+will be able to inform you what this limit is.
 
 If the job submission is successful, a unique job identifier will be returned:
 ```
 [✓] Submitted job id gv6uqutvNmU0:             helium
 ```
 A local registry of these IDs is kept, so it is not essential to use them in the
 commands below. However, they may be required to disambiguate multiple jobs
```

### Comparing `qcloud_user-1.0.1/README.md` & `qcloud_user-1.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -47,15 +47,16 @@
 ...
 ```
 The number of threads can be specified by using the `--ncpu` flag, for example:
 ```
 qcloud --submit --ncpu 4 job1.inp 
 ```
 Note that if the number of threads specified exceeds the number of cores on 
-an individual compute node, the job will not run.
+an individual compute node, the job will not run.  Your QCloud administrator
+will be able to inform you what this limit is.
 
 If the job submission is successful, a unique job identifier will be returned:
 ```
 [✓] Submitted job id gv6uqutvNmU0:             helium
 ```
 A local registry of these IDs is kept, so it is not essential to use them in the
 commands below. However, they may be required to disambiguate multiple jobs
```

### Comparing `qcloud_user-1.0.1/pyproject.toml` & `qcloud_user-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_user"
-version = "1.0.1"
+version = "1.0.2"
 description = "Q-Cloud CLI for users" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_user-1.0.1/qcloud_user.egg-info/PKG-INFO` & `qcloud_user-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: qcloud-user
-Version: 1.0.1
+Name: qcloud_user
+Version: 1.0.2
 Summary: Q-Cloud CLI for users
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -72,15 +72,16 @@
 ...
 ```
 The number of threads can be specified by using the `--ncpu` flag, for example:
 ```
 qcloud --submit --ncpu 4 job1.inp 
 ```
 Note that if the number of threads specified exceeds the number of cores on 
-an individual compute node, the job will not run.
+an individual compute node, the job will not run.  Your QCloud administrator
+will be able to inform you what this limit is.
 
 If the job submission is successful, a unique job identifier will be returned:
 ```
 [✓] Submitted job id gv6uqutvNmU0:             helium
 ```
 A local registry of these IDs is kept, so it is not essential to use them in the
 commands below. However, they may be required to disambiguate multiple jobs
```

### Comparing `qcloud_user-1.0.1/setup.py` & `qcloud_user-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 setuptools.setup(
     name="qcloud_user",
     python_requires='>=3.7',
-    version="1.0.1",
+    version="1.0.2",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="suppor@q-chem.com",
     description="CLI for interacting with Q-Cloud clusters",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=['qcloud_user'],
```

### Comparing `qcloud_user-1.0.1/src/qcloud_user/qcloud_user.py` & `qcloud_user-1.0.2/src/qcloud_user/qcloud_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -631,14 +631,16 @@
             help="password reset using a code")
 
         parser.add_argument("--submit", dest="submit", action='store_true',
             help="submit job(s)")
 
         parser.add_argument("--ncpu", dest="ncpu", default = 1,
             help="specify the number of openmp threads to use.")
+        parser.add_argument("--ncpus", dest="ncpu", default = 1,
+            help="specify the number of openmp threads to use.")
 
         parser.add_argument("--cancel", dest="cancel", action='store_true',
             help="cancel queued or running job(s)")
 
         parser.add_argument("--info", dest="info", action='store_true',
             help="print the timestamps for each state for each job")
 
@@ -656,14 +658,17 @@
 
         parser.add_argument("--clear", dest="clear", action='store_true',
             help="clear downloaded jobs from registry")
 
         parser.add_argument("--remove", dest="remove", action='store_true',
             help="remove jobs from registry regardless of status")
 
+        parser.add_argument("--dump", dest="dump", action='store_true',
+            help="dump contents of local job database")
+
         parser.add_argument("--debug", dest="debug", action='store_true',
             help="add debug printing")
 
         args, extra_args = parser.parse_known_args()
 
         if args.debug:
            DEBUG = True
@@ -724,14 +729,17 @@
         elif args.remove:
            if len(extra_args) > 0:
               remove(token, extra_args, config, db)
 
         elif args.submit:
            ret = submit(token, extra_args, args.ncpu, config, db)
 
+        elif args.dump:
+           db.dump()
+
         else:
            print("Invalid option")
 
 
     except KeyboardInterrupt:
         print("\n")
         pass
```

