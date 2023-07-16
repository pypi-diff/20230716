# Comparing `tmp/aifactory-1.7.1.tar.gz` & `tmp/aifactory-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.7.1.tar", last modified: Sun Jul 16 03:23:32 2023, max compression
+gzip compressed data, was "aifactory-1.7.2.tar", last modified: Sun Jul 16 03:49:57 2023, max compression
```

## Comparing `aifactory-1.7.1.tar` & `aifactory-1.7.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:23:32.642670 aifactory-1.7.1/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 03:23:32.642504 aifactory-1.7.1/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:23:32.641552 aifactory-1.7.1/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)     7464 2023-07-16 03:22:58.000000 aifactory-1.7.1/aifactory/score.py
--rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/train.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:23:32.642280 aifactory-1.7.1/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      308 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-07-16 03:23:32.642733 aifactory-1.7.1/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-16 03:23:12.000000 aifactory-1.7.1/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:49:57.018251 aifactory-1.7.2/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 03:49:57.018100 aifactory-1.7.2/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:49:57.017124 aifactory-1.7.2/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)     7466 2023-07-16 03:49:36.000000 aifactory-1.7.2/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.7.2/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:49:57.017895 aifactory-1.7.2/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-07-16 03:49:56.000000 aifactory-1.7.2/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-07-16 03:49:57.018303 aifactory-1.7.2/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-16 03:48:59.000000 aifactory-1.7.2/setup.py
```

### Comparing `aifactory-1.7.1/aifactory/api.py` & `aifactory-1.7.2/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.1/aifactory/demo.py` & `aifactory-1.7.2/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.1/aifactory/grade.py` & `aifactory-1.7.2/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.1/aifactory/make_zip.py` & `aifactory-1.7.2/aifactory/make_zip.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.1/aifactory/score.py` & `aifactory-1.7.2/aifactory/score.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 bridge_url = "https://grade-bridge.aifactory.space/grade"
 bridge_test_url = "https://grade-bridge-test.aifactory.space/grade"
 
 api_url = "https://api.aifactory.space/competition-submission/getResultByRequestID/"
 api_test_url = "https://api-test.aifactory.space/competition-submission/getResultByRequestID/"
 
 # test
-getUrl = 'https://apc1.aifactory.site/getUrl'
+getUrl = 'https://signed.aifactory.site/getUrl'
 bridgeUrl = 'https://apc1.aifactory.site'
 apiUrl ="https://api-renewal.aifactory.space"
 getResultUrl = "https://api-renewal.aifactory.space/submission/getResultByRequestID/"
 
 def make_zip(main_name):
   run_type = 0
   main_filename = ''
@@ -157,15 +157,15 @@
       data=data
     ) 
 
     if res.status_code != 200 :
       print("파일 전송 오류")       
       return 
     
-    submitData = {"key" : key, "modelname" : model_name, "RequestID": requestID, "FileName": fileName}
+    submitData = {"key" : key, "modelname" : model_name, "requestID": requestID, "fileName": fileName}
     res = requests.post(bridgeUrl + "/uploadCompleted", json=submitData)
     if res.status_code != 200:
       print("중계 서버 오류 : uploadCompleted")
       return 
     
     print("파일 전송 완료")
```

