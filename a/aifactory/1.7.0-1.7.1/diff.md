# Comparing `tmp/aifactory-1.7.0.tar.gz` & `tmp/aifactory-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifactory-1.7.0.tar", last modified: Sun Jul 16 02:36:32 2023, max compression
+gzip compressed data, was "aifactory-1.7.1.tar", last modified: Sun Jul 16 03:23:32 2023, max compression
```

## Comparing `aifactory-1.7.0.tar` & `aifactory-1.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 02:36:32.786422 aifactory-1.7.0/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 02:36:32.786210 aifactory-1.7.0/PKG-INFO
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 02:36:32.784138 aifactory-1.7.0/aifactory/
--rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/__init__.py
--rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/api.py
--rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/demo.py
--rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/grade.py
--rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/make_zip.py
--rw-r--r--   0 kyj        (501) staff       (20)     7471 2023-07-16 02:30:23.000000 aifactory-1.7.0/aifactory/score.py
--rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.7.0/aifactory/train.py
-drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 02:36:32.785639 aifactory-1.7.0/aifactory.egg-info/
--rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/PKG-INFO
--rw-r--r--   0 kyj        (501) staff       (20)      308 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/SOURCES.txt
--rw-r--r--   0 kyj        (501) staff       (20)        1 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/dependency_links.txt
--rw-r--r--   0 kyj        (501) staff       (20)       41 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/requires.txt
--rw-r--r--   0 kyj        (501) staff       (20)       17 2023-07-16 02:36:32.000000 aifactory-1.7.0/aifactory.egg-info/top_level.txt
--rw-r--r--   0 kyj        (501) staff       (20)       38 2023-07-16 02:36:32.786502 aifactory-1.7.0/setup.cfg
--rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-16 01:38:33.000000 aifactory-1.7.0/setup.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:23:32.642670 aifactory-1.7.1/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 03:23:32.642504 aifactory-1.7.1/PKG-INFO
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:23:32.641552 aifactory-1.7.1/aifactory/
+-rw-r--r--   0 kyj        (501) staff       (20)        0 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/__init__.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3743 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/api.py
+-rw-r--r--   0 kyj        (501) staff       (20)     3710 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/demo.py
+-rw-r--r--   0 kyj        (501) staff       (20)    14314 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/grade.py
+-rw-r--r--   0 kyj        (501) staff       (20)     5966 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/make_zip.py
+-rw-r--r--   0 kyj        (501) staff       (20)     7464 2023-07-16 03:22:58.000000 aifactory-1.7.1/aifactory/score.py
+-rw-r--r--   0 kyj        (501) staff       (20)       50 2023-05-10 03:11:14.000000 aifactory-1.7.1/aifactory/train.py
+drwxr-xr-x   0 kyj        (501) staff       (20)        0 2023-07-16 03:23:32.642280 aifactory-1.7.1/aifactory.egg-info/
+-rw-r--r--   0 kyj        (501) staff       (20)      228 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/PKG-INFO
+-rw-r--r--   0 kyj        (501) staff       (20)      308 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/SOURCES.txt
+-rw-r--r--   0 kyj        (501) staff       (20)        1 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/dependency_links.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       41 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/requires.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       17 2023-07-16 03:23:32.000000 aifactory-1.7.1/aifactory.egg-info/top_level.txt
+-rw-r--r--   0 kyj        (501) staff       (20)       38 2023-07-16 03:23:32.642733 aifactory-1.7.1/setup.cfg
+-rw-r--r--   0 kyj        (501) staff       (20)      430 2023-07-16 03:23:12.000000 aifactory-1.7.1/setup.py
```

### Comparing `aifactory-1.7.0/aifactory/api.py` & `aifactory-1.7.1/aifactory/api.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.0/aifactory/demo.py` & `aifactory-1.7.1/aifactory/demo.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.0/aifactory/grade.py` & `aifactory-1.7.1/aifactory/grade.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.0/aifactory/make_zip.py` & `aifactory-1.7.1/aifactory/make_zip.py`

 * *Files identical despite different names*

### Comparing `aifactory-1.7.0/aifactory/score.py` & `aifactory-1.7.1/aifactory/score.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 bridge_url = "https://grade-bridge.aifactory.space/grade"
 bridge_test_url = "https://grade-bridge-test.aifactory.space/grade"
 
 api_url = "https://api.aifactory.space/competition-submission/getResultByRequestID/"
 api_test_url = "https://api-test.aifactory.space/competition-submission/getResultByRequestID/"
 
 # test
-getUrl = 'https://signed.aifactory.site/getUrl'
+getUrl = 'https://apc1.aifactory.site/getUrl'
 bridgeUrl = 'https://apc1.aifactory.site'
 apiUrl ="https://api-renewal.aifactory.space"
 getResultUrl = "https://api-renewal.aifactory.space/submission/getResultByRequestID/"
 
 def make_zip(main_name):
   run_type = 0
   main_filename = ''
@@ -104,29 +104,29 @@
     main_name = "task.py"
 
   print("file : {0}".format(main_name))
   make_zip(main_name)
   
   with open('./aif.zip', 'rb') as f:
     data = f.read()
-    
+
   try:        
-    submitData = {"key" : key, "modelname" : model_name, "RequestID": "0", "FileName": "0"}    
+    submitData = {"key" : key, "modelname" : model_name, "requestID": "0", "fileName": "0"}    
     res = requests.post(bridgeUrl + "/submit", json=submitData)
     if res.status_code != 200:
       print("중계서버 오류")
       return 
     
     dataJson = json.loads(res.text)  
     requestID = dataJson['requestID']
       
     while True:
       res = requests.get(apiUrl + "/score-request/" + requestID)  
       if res.status_code != 200:
-        print("중계서버 오류")
+        print("API 서버 오류")
         return
       dataJson = json.loads(res.text)  
       status = dataJson["status"]
       if status == -1 :
         print(dataJson["error"])
         return
       elif status == 1 :
@@ -157,15 +157,15 @@
       data=data
     ) 
 
     if res.status_code != 200 :
       print("파일 전송 오류")       
       return 
     
-    submitData = {"key" : key, "modelname" : "test111", "RequestID": requestID, "FileName": fileName}
+    submitData = {"key" : key, "modelname" : model_name, "RequestID": requestID, "FileName": fileName}
     res = requests.post(bridgeUrl + "/uploadCompleted", json=submitData)
     if res.status_code != 200:
       print("중계 서버 오류 : uploadCompleted")
       return 
     
     print("파일 전송 완료")
```

