# Comparing `tmp/storage-local-0.0.5.tar.gz` & `tmp/storage-local-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "storage-local-0.0.5.tar", last modified: Wed May 24 02:16:46 2023, max compression
+gzip compressed data, was "storage-local-0.0.6.tar", last modified: Sun Jul 16 04:29:06 2023, max compression
```

## Comparing `storage-local-0.0.5.tar` & `storage-local-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:16:46.753436 storage-local-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-24 02:16:46.753436 storage-local-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-24 02:16:12.000000 storage-local-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:16:46.753436 storage-local-0.0.5/circles_local_aws_s3_storage_python/
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-24 02:16:12.000000 storage-local-0.0.5/circles_local_aws_s3_storage_python/AWSStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-24 02:16:12.000000 storage-local-0.0.5/circles_local_aws_s3_storage_python/CirclesStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-24 02:16:12.000000 storage-local-0.0.5/circles_local_aws_s3_storage_python/FileTypeDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-24 02:16:12.000000 storage-local-0.0.5/circles_local_aws_s3_storage_python/StorageDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-24 02:16:12.000000 storage-local-0.0.5/circles_local_aws_s3_storage_python/StorageInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:16:12.000000 storage-local-0.0.5/circles_local_aws_s3_storage_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 02:16:12.000000 storage-local-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 02:16:46.753436 storage-local-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-24 02:16:12.000000 storage-local-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:16:46.753436 storage-local-0.0.5/storage_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-24 02:16:46.000000 storage-local-0.0.5/storage_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-24 02:16:46.000000 storage-local-0.0.5/storage_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:16:46.000000 storage-local-0.0.5/storage_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-24 02:16:46.000000 storage-local-0.0.5/storage_local.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:16:46.753436 storage-local-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 02:16:12.000000 storage-local-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-24 02:16:12.000000 storage-local-0.0.5/tests/test_S3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-24 02:16:12.000000 storage-local-0.0.5/tests/test_circles_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:29:06.866941 storage-local-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-16 04:29:06.862941 storage-local-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-16 04:28:35.000000 storage-local-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:29:06.862941 storage-local-0.0.6/circles_local_aws_s3_storage_python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-16 04:28:35.000000 storage-local-0.0.6/circles_local_aws_s3_storage_python/AWSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-07-16 04:28:35.000000 storage-local-0.0.6/circles_local_aws_s3_storage_python/CirclesStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-16 04:28:35.000000 storage-local-0.0.6/circles_local_aws_s3_storage_python/FileTypeDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-16 04:28:35.000000 storage-local-0.0.6/circles_local_aws_s3_storage_python/StorageDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-07-16 04:28:35.000000 storage-local-0.0.6/circles_local_aws_s3_storage_python/StorageInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:28:35.000000 storage-local-0.0.6/circles_local_aws_s3_storage_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-16 04:28:35.000000 storage-local-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 04:29:06.866941 storage-local-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-07-16 04:28:35.000000 storage-local-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:29:06.862941 storage-local-0.0.6/storage_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-16 04:29:06.000000 storage-local-0.0.6/storage_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-16 04:29:06.000000 storage-local-0.0.6/storage_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:29:06.000000 storage-local-0.0.6/storage_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-16 04:29:06.000000 storage-local-0.0.6/storage_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:29:06.862941 storage-local-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:28:35.000000 storage-local-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-16 04:28:35.000000 storage-local-0.0.6/tests/test_S3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-07-16 04:28:35.000000 storage-local-0.0.6/tests/test_circles_storage.py
```

### Comparing `storage-local-0.0.5/circles_local_aws_s3_storage_python/AWSStorage.py` & `storage-local-0.0.6/circles_local_aws_s3_storage_python/AWSStorage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 
 import os
 import boto3
 
 from circles_local_aws_s3_storage_python.StorageInterface import StorageInterface
 from circles_local_aws_s3_storage_python.StorageDB import StorageDB
 
-
+debug = False
 class AwsS3Storage(StorageInterface):
+    
 
     def __init__(self, bucket_name, region):
+        if (debug): print("Initializing AwsS3Storage bucket_name="+str(bucket_name)+' region='+str(region))
         self.region = region
         self.bucket_name = bucket_name
         self.database = StorageDB()
+        if (debug): print("AWS_ACCESS_KEY_ID: " +os.getenv("AWS_ACCESS_KEY_ID"))
+        if (debug): print("AWS_SECRET_ACCESS_KEY: " +os.getenv("AWS_SECRET_ACCESS_KEY"))
         self.client = boto3.client('s3',
                                    aws_access_key_id=os.getenv(
                                        "AWS_ACCESS_KEY_ID"),
                                    aws_secret_access_key=os.getenv("AWS_SECRET_ACCESS_KEY"))
 
     # uploads file to S3
```

### Comparing `storage-local-0.0.5/circles_local_aws_s3_storage_python/CirclesStorage.py` & `storage-local-0.0.6/circles_local_aws_s3_storage_python/CirclesStorage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from circles_local_aws_s3_storage_python.FileTypeDB import file_type_db
 import os
 from circles_local_aws_s3_storage_python.AWSStorage import AwsS3Storage
 from dotenv.main import load_dotenv
 load_dotenv()
 
+debug=False
 
 class circles_storage:
 
     def __init__(self):
-        print("REGION:"+str(os.getenv("REGION")))
+        if (debug): print("REGION:"+str(os.getenv("REGION")))
         self.s3 = AwsS3Storage(os.getenv("BUCKET_NAME"), os.getenv("REGION"))
         self.db = file_type_db()
 
     # returns the folder name from DB according to entity_type_id
     def get_folder(self, entity_type_id):
         select_stmt = "SELECT file_type FROM storage.file_type_table WHERE id = %s"
         select_data = (entity_type_id)
```

### Comparing `storage-local-0.0.5/circles_local_aws_s3_storage_python/FileTypeDB.py` & `storage-local-0.0.6/circles_local_aws_s3_storage_python/FileTypeDB.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.5/circles_local_aws_s3_storage_python/StorageDB.py` & `storage-local-0.0.6/circles_local_aws_s3_storage_python/StorageDB.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,20 +10,20 @@
             host=os.getenv("RDS_HOSTNAME"),
             user=os.getenv("RDS_USERNAME"),
             passwd=os.getenv("RDS_PASSWORD"),
             database=os.getenv("RDS_DB_NAME")
         )
         self.cursor = self.mydb.cursor()
 
-    def uploadToDataBase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, extension_id) -> int:
+    def uploadToDataBase(self, file_path, filename,  region, created_user_id, storage_type_id, file_type_id, file_extension_id) -> int:
         add_storage = ("INSERT INTO storage.storage_table "
-                       "(path, filename, region, created_user_id, updated_user_id, storage_type_id, file_type_id, extension_id) "
+                       "(path, filename, region, created_user_id, updated_user_id, storage_type_id, file_type_id, file_extension_id) "
                        "VALUES (%s, %s, %s, %s, %s, %s, %s, %s)")
         storage_data = (file_path, filename, region, created_user_id,
-                        created_user_id, storage_type_id, file_type_id, extension_id)
+                        created_user_id, storage_type_id, file_type_id, file_extension_id)
         self.cursor.execute(add_storage, storage_data)
         self.mydb.commit()
         select_stmt = "SELECT LAST_INSERT_ID()"
         self.cursor.execute(select_stmt)
         last_insert_id = self.cursor.fetchone()[0]
         return int(last_insert_id)
```

### Comparing `storage-local-0.0.5/circles_local_aws_s3_storage_python/StorageInterface.py` & `storage-local-0.0.6/circles_local_aws_s3_storage_python/StorageInterface.py`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.5/setup.py` & `storage-local-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='storage-local',
-    version='0.0.5',
+    version='0.0.6',
     author="Circles",
     author_email="info@circle.zone",
     description="PyPI Package for Circles S3 functions",
     long_description="This is a package for sharing common S3 function used in different repositories",
     long_description_content_type="text/markdown",
     url="https://github.com/javatechy/dokr",
     packages=setuptools.find_packages(),
```

### Comparing `storage-local-0.0.5/storage_local.egg-info/SOURCES.txt` & `storage-local-0.0.6/storage_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `storage-local-0.0.5/tests/test_S3.py` & `storage-local-0.0.6/tests/test_S3.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,36 +4,50 @@
 import unittest
 from dotenv.main import load_dotenv
 
 from circles_local_aws_s3_storage_python.AWSStorage import AwsS3Storage
 from circles_local_aws_s3_storage_python.StorageDB import StorageDB
 load_dotenv()
 
+# TODO: Get the debug from Environment using our method in Python util/SDK
+debug=False
 
 class s3_test(unittest.TestCase):
     def setUp(self) -> None:
+        # TODO: Write to Logger with Storge_Testing Component Id
+        if (debug): print('Bucket=', end='')
+        if (debug): print(os.getenv("BUCKET_NAME"))
+        if (debug): print('Region=',  end='')
+        if (debug): print(os.getenv("REGION"))
+        if (debug): print(os.getenv("BUCKET_NAME"))
         self.s3_resource = boto3.resource('s3')
         self.awsS3 = AwsS3Storage(
             os.getenv("BUCKET_NAME"), os.getenv("REGION"))
         self.test_file_contents = b'this it a file test!'
         self.database = StorageDB()
 
     def test_upload(self):
         cwd = os.getcwd()
+        # TODO: Use consts
         filepath = os.path.join(cwd, 'tests/test.txt')
+        # TODO: Use consts
         functionId = self.awsS3.upload_file(
             filepath, 'test.txt', 'python/', 1)
         s3_object = self.s3_resource.Object(
             os.getenv("BUCKET_NAME"), 'python/test.txt')
         s3_file_contents = s3_object.get()['Body'].read()
         self.assertEqual(s3_file_contents, self.test_file_contents)
         actualId = self.database.getLastId()
         self.assertEqual(functionId, actualId)
 
     def test_download(self):
+        # As I'm not sure setUp was running and we need to run test_upload() before running test_download()
+        self.setUp()
+        self.test_upload()
+        
         cwd = os.getcwd()
         self.awsS3.download_file(
             'python/test.txt', cwd+'/test.txt')
         assert os.path.isfile(
             cwd+'/test.txt')
 
     def test_logical_delete(self):
```

### Comparing `storage-local-0.0.5/tests/test_circles_storage.py` & `storage-local-0.0.6/tests/test_circles_storage.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from circles_local_aws_s3_storage_python.CirclesStorage import circles_storage
 import os
 import unittest
 from dotenv.main import load_dotenv
 load_dotenv()
 
+debug = False;
 
 class circles_storage_test(unittest.TestCase):
     def setUp(self) -> None:
         self.circles_storage = circles_storage()
-        print("REGION:"+str(os.getenv("REGION")))
+        if (debug): print("REGION:"+str(os.getenv("REGION")))
 
     def test_get_folder(self):
         actual_folder = self.circles_storage.get_folder(1)
         expected_folder = 'Profile Image'
         self.assertEqual(actual_folder, expected_folder)
 
     def test_get_region_and_folder(self):
```

