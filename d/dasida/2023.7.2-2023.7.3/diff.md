# Comparing `tmp/dasida-2023.7.2.tar.gz` & `tmp/dasida-2023.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dasida-2023.7.2.tar", last modified: Sun Jul 16 10:53:53 2023, max compression
+gzip compressed data, was "dasida-2023.7.3.tar", last modified: Sun Jul 16 11:09:05 2023, max compression
```

## Comparing `dasida-2023.7.2.tar` & `dasida-2023.7.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 10:53:53.975634 dasida-2023.7.2/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1063 2023-07-02 01:00:04.000000 dasida-2023.7.2/LICENSE
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-16 10:53:53.975634 dasida-2023.7.2/PKG-INFO
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       34 2023-07-02 01:00:04.000000 dasida-2023.7.2/README.md
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 10:53:53.971634 dasida-2023.7.2/dasida/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       58 2023-07-02 01:54:32.000000 dasida-2023.7.2/dasida/__init__.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 10:53:53.975634 dasida-2023.7.2/dasida/aws/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       99 2023-07-02 01:54:15.000000 dasida-2023.7.2/dasida/aws/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1680 2023-07-02 01:00:04.000000 dasida-2023.7.2/dasida/aws/common.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     8466 2023-07-02 01:00:04.000000 dasida-2023.7.2/dasida/aws/s3.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     9428 2023-07-02 01:52:41.000000 dasida-2023.7.2/dasida/aws/secretsmanager.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)    12353 2023-07-02 01:00:04.000000 dasida-2023.7.2/dasida/aws/sqs.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     4008 2023-07-02 01:00:04.000000 dasida-2023.7.2/dasida/aws/ssm.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 10:53:53.975634 dasida-2023.7.2/dasida/docker/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       33 2023-07-02 01:00:04.000000 dasida-2023.7.2/dasida/docker/__init__.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     1240 2023-07-02 01:00:04.000000 dasida-2023.7.2/dasida/docker/docker.py
--rw-rw-r--   0 eugene    (1001) eugene    (1001)     8652 2023-07-16 10:44:10.000000 dasida-2023.7.2/dasida/scripts.py
-drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 10:53:53.971634 dasida-2023.7.2/dasida.egg-info/
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-16 10:53:53.000000 dasida-2023.7.2/dasida.egg-info/PKG-INFO
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-16 10:53:53.000000 dasida-2023.7.2/dasida.egg-info/SOURCES.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)        1 2023-07-16 10:53:53.000000 dasida-2023.7.2/dasida.egg-info/dependency_links.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       49 2023-07-16 10:53:53.000000 dasida-2023.7.2/dasida.egg-info/entry_points.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)       79 2023-07-16 10:53:53.000000 dasida-2023.7.2/dasida.egg-info/requires.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)        7 2023-07-16 10:53:53.000000 dasida-2023.7.2/dasida.egg-info/top_level.txt
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      262 2023-07-02 01:00:04.000000 dasida-2023.7.2/pyproject.toml
--rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-16 10:53:53.975634 dasida-2023.7.2/setup.cfg
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.213165 dasida-2023.7.3/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1063 2023-07-16 11:07:17.000000 dasida-2023.7.3/LICENSE
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-16 11:09:05.213165 dasida-2023.7.3/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       34 2023-07-16 11:07:17.000000 dasida-2023.7.3/README.md
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.209165 dasida-2023.7.3/dasida/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       58 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/__init__.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.213165 dasida-2023.7.3/dasida/aws/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       99 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1680 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/common.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     8466 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/s3.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     9428 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/secretsmanager.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)    12353 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/sqs.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     4008 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/aws/ssm.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.213165 dasida-2023.7.3/dasida/docker/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       33 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/docker/__init__.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     1240 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/docker/docker.py
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)     8713 2023-07-16 11:07:17.000000 dasida-2023.7.3/dasida/scripts.py
+drwxrwxr-x   0 eugene    (1001) eugene    (1001)        0 2023-07-16 11:09:05.209165 dasida-2023.7.3/dasida.egg-info/
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      160 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/PKG-INFO
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/SOURCES.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        1 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/dependency_links.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       49 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/entry_points.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)       79 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/requires.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)        7 2023-07-16 11:09:05.000000 dasida-2023.7.3/dasida.egg-info/top_level.txt
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      262 2023-07-16 11:07:17.000000 dasida-2023.7.3/pyproject.toml
+-rw-rw-r--   0 eugene    (1001) eugene    (1001)      437 2023-07-16 11:09:05.217165 dasida-2023.7.3/setup.cfg
```

### Comparing `dasida-2023.7.2/LICENSE` & `dasida-2023.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.2/dasida/aws/common.py` & `dasida-2023.7.3/dasida/aws/common.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.2/dasida/aws/s3.py` & `dasida-2023.7.3/dasida/aws/s3.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.2/dasida/aws/secretsmanager.py` & `dasida-2023.7.3/dasida/aws/secretsmanager.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.2/dasida/aws/sqs.py` & `dasida-2023.7.3/dasida/aws/sqs.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.2/dasida/aws/ssm.py` & `dasida-2023.7.3/dasida/aws/ssm.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.2/dasida/docker/docker.py` & `dasida-2023.7.3/dasida/docker/docker.py`

 * *Files identical despite different names*

### Comparing `dasida-2023.7.2/dasida/scripts.py` & `dasida-2023.7.3/dasida/scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,18 @@
             break
 
     print(f"\nAdd new secret '{secret_name}' as follows?:")
     for k, v in secrets.items():
         print(f" - {k}: {v}")
 
     proceed = inquirer.confirm(message="Confirm?", default=False).execute()
-    _ = aws.secretsmanager.create_secrets(secret_name=secret_name, secrets=secrets, profile_name=profile)
+    if proceed:
+        _ = aws.secretsmanager.create_secrets(secret_name=secret_name, secrets=secrets, profile_name=profile)
+    else:
+        logger.error("Abort!")
 
 
 ################################################################
 # AWS S3
 ################################################################
 @dasida.group()
 def s3():
```

