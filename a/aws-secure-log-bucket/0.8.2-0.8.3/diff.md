# Comparing `tmp/aws-secure-log-bucket-0.8.2.tar.gz` & `tmp/aws-secure-log-bucket-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-secure-log-bucket-0.8.2.tar", last modified: Sat Jul 15 18:16:05 2023, max compression
+gzip compressed data, was "aws-secure-log-bucket-0.8.3.tar", last modified: Sun Jul 16 18:16:00 2023, max compression
```

## Comparing `aws-secure-log-bucket-0.8.2.tar` & `aws-secure-log-bucket-0.8.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:16:05.734124 aws-secure-log-bucket-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-15 18:16:05.734124 aws-secure-log-bucket-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 18:16:05.734124 aws-secure-log-bucket-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:16:05.730124 aws-secure-log-bucket-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:16:05.734124 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket/
--rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:16:05.734124 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23403 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@0.8.2.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:15:51.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:16:05.734124 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-15 18:16:05.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-15 18:16:05.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:16:05.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-15 18:16:05.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 18:16:05.000000 aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.087033 aws-secure-log-bucket-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/
+-rw-r--r--   0 runner    (1001) docker     (123)     9159 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23402 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@0.8.3.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:15:48.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 18:16:00.091034 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-16 18:16:00.000000 aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/top_level.txt
```

### Comparing `aws-secure-log-bucket-0.8.2/LICENSE` & `aws-secure-log-bucket-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.2/PKG-INFO` & `aws-secure-log-bucket-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-secure-log-bucket
-Version: 0.8.2
+Version: 0.8.3
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/yicr/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `aws-secure-log-bucket-0.8.2/README.md` & `aws-secure-log-bucket-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.2/setup.py` & `aws-secure-log-bucket-0.8.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-secure-log-bucket",
-    "version": "0.8.2",
+    "version": "0.8.3",
     "description": "secure multiple transition phases in a single lifecycle policy bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/yicr/aws-secure-log-bucket.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_secure_log_bucket",
         "aws_secure_log_bucket._jsii"
     ],
     "package_data": {
         "aws_secure_log_bucket._jsii": [
-            "aws-secure-log-bucket@0.8.2.jsii.tgz"
+            "aws-secure-log-bucket@0.8.3.jsii.tgz"
         ],
         "aws_secure_log_bucket": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket/__init__.py` & `aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@0.8.2.jsii.tgz` & `aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket/_jsii/aws-secure-log-bucket@0.8.3.jsii.tgz`

 * *Files 24% similar despite different names*

#### Comparing `aws-secure-log-bucket@0.8.2.jsii.tgz-content` & `aws-secure-log-bucket@0.8.3.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'8jnWsrgAi9GJ5G32xcFAc1CQYMeWr5bcjzaIo2IQPYg='", "'version'": "'0.8.3'"}*

```diff
@@ -3303,15 +3303,15 @@
             }
         }
     },
     "description": "secure multiple transition phases in a single lifecycle policy bucket.",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "8xwNfHkg/GNsWcGIHhhN4Ww1cNA2t3Ekl6mh3xET9jU=",
+    "fingerprint": "8jnWsrgAi9GJ5G32xcFAc1CQYMeWr5bcjzaIo2IQPYg=",
     "homepage": "https://github.com/yicr/aws-secure-log-bucket.git",
     "jsiiVersion": "1.84.0 (build 5404dcf)",
     "keywords": [
         "aws",
         "aws-cdk",
         "bucket",
         "cdk",
@@ -3515,9 +3515,9 @@
                         "primitive": "number"
                     }
                 }
             ],
             "symbolId": "src/index:StorageClassTransitionProperty"
         }
     },
-    "version": "0.8.2"
+    "version": "0.8.3"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -33,10 +33,10 @@
         });
     }
 }
 exports.SecureLogBucket = SecureLogBucket;
 _a = JSII_RTTI_SYMBOL_1;
 SecureLogBucket[_a] = {
     fqn: "aws-secure-log-bucket.SecureLogBucket",
-    version: "0.8.2"
+    version: "0.8.3"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSxtQ0FBbUM7QUFDbkMseUNBQXlDO0FBQ3pDLHlEQUF5RTtBQWV6RSxNQUFhLGVBQWdCLFNBQVEsZ0NBQVk7SUFFL0MsWUFBWSxLQUFnQixFQUFFLEVBQVUsRUFBRSxLQUE0QjtRQUNwRSxLQUFLLENBQUMsS0FBSyxFQUFFLEVBQUUsRUFBRTtZQUNmLFVBQVUsRUFBRSxLQUFLLEVBQUUsVUFBVTtZQUM3QixVQUFVLEVBQUUsMENBQXNCLENBQUMsV0FBVztZQUM5QyxjQUFjLEVBQUUsQ0FBQztvQkFDZixFQUFFLEVBQUUsNkJBQTZCO29CQUNqQyxPQUFPLEVBQUUsSUFBSTtvQkFDYixXQUFXLEVBQUU7d0JBQ1g7NEJBQ0UsWUFBWSxFQUFFLEVBQUUsQ0FBQyxZQUFZLENBQUMsaUJBQWlCOzRCQUMvQyxlQUFlLEVBQUUsR0FBRyxDQUFDLFFBQVEsQ0FBQyxJQUFJLENBQUMsS0FBSyxFQUFFLHFCQUFxQixFQUFFLG9CQUFvQixJQUFJLEVBQUUsQ0FBQzt5QkFDN0Y7d0JBQ0Q7NEJBQ0UsWUFBWSxFQUFFLEVBQUUsQ0FBQyxZQUFZLENBQUMsbUJBQW1COzRCQUNqRCxlQUFlLEVBQUUsR0FBRyxDQUFDLFFBQVEsQ0FBQyxJQUFJLENBQUMsS0FBSyxFQUFFLHFCQUFxQixFQUFFLHNCQUFzQixJQUFJLEdBQUcsQ0FBQzt5QkFDaEc7d0JBQ0Q7NEJBQ0UsWUFBWSxFQUFFLEVBQUUsQ0FBQyxZQUFZLENBQUMsT0FBTzs0QkFDckMsZUFBZSxFQUFFLEdBQUcsQ0FBQyxRQUFRLENBQUMsSUFBSSxDQUFDLEtBQUssRUFBRSxxQkFBcUIsRUFBRSxXQUFXLElBQUksR0FBRyxDQUFDO3lCQUNyRjt3QkFDRDs0QkFDRSxZQUFZLEVBQUUsRUFBRSxDQUFDLFlBQVksQ0FBQyxZQUFZOzRCQUMxQyxlQUFlLEVBQUUsR0FBRyxDQUFDLFFBQVEsQ0FBQyxJQUFJLENBQUMsS0FBSyxFQUFFLHFCQUFxQixFQUFFLGVBQWUsSUFBSSxHQUFHLENBQUM7eUJBQ3pGO3FCQUNGO2lCQUNGLENBQUM7U0FDSCxDQUFDLENBQUM7SUFDTCxDQUFDOztBQTdCSCwwQ0E4QkMiLCJzb3VyY2VzQ29udGVudCI6WyJpbXBvcnQgKiBhcyBjZGsgZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0ICogYXMgczMgZnJvbSAnYXdzLWNkay1saWIvYXdzLXMzJztcbmltcG9ydCB7IFNlY3VyZUJ1Y2tldCwgU2VjdXJlQnVja2V0RW5jcnlwdGlvbiB9IGZyb20gJ2F3cy1zZWN1cmUtYnVja2V0JztcbmltcG9ydCB7IENvbnN0cnVjdCB9IGZyb20gJ2NvbnN0cnVjdHMnO1xuXG5leHBvcnQgaW50ZXJmYWNlIFNlY3VyZUxvZ0J1Y2tldFByb3BzIHtcbiAgcmVhZG9ubHkgYnVja2V0TmFtZT86IHN0cmluZztcbiAgcmVhZG9ubHkgY2hhbmdlQ2xhc3NUcmFuc2l0aW9uPzogU3RvcmFnZUNsYXNzVHJhbnNpdGlvblByb3BlcnR5O1xufVxuXG5leHBvcnQgaW50ZXJmYWNlIFN0b3JhZ2VDbGFzc1RyYW5zaXRpb25Qcm9wZXJ0eSB7XG4gIHJlYWRvbmx5IGluZnJlcXVlbnRBY2Nlc3NEYXlzOiBudW1iZXI7XG4gIHJlYWRvbmx5IGludGVsbGlnZW50VGllcmluZ0RheXM6IG51bWJlcjtcbiAgcmVhZG9ubHkgZ2xhY2llckRheXM6IG51bWJlcjtcbiAgcmVhZG9ubHkgZGVlcEFyY2hpdmVEYXlzOiBudW1iZXI7XG59XG5cbmV4cG9ydCBjbGFzcyBTZWN1cmVMb2dCdWNrZXQgZXh0ZW5kcyBTZWN1cmVCdWNrZXQge1xuXG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzPzogU2VjdXJlTG9nQnVja2V0UHJvcHMpIHtcbiAgICBzdXBlcihzY29wZSwgaWQsIHtcbiAgICAgIGJ1Y2tldE5hbWU6IHByb3BzPy5idWNrZXROYW1lLFxuICAgICAgZW5jcnlwdGlvbjogU2VjdXJlQnVja2V0RW5jcnlwdGlvbi5LTVNfTUFOQUdFRCxcbiAgICAgIGxpZmVjeWNsZVJ1bGVzOiBbe1xuICAgICAgICBpZDogJ2FyY2hpdmUtc3RlcC1saWZlY3ljbGUtcnVsZScsXG4gICAgICAgIGVuYWJsZWQ6IHRydWUsXG4gICAgICAgIHRyYW5zaXRpb25zOiBbXG4gICAgICAgICAge1xuICAgICAgICAgICAgc3RvcmFnZUNsYXNzOiBzMy5TdG9yYWdlQ2xhc3MuSU5GUkVRVUVOVF9BQ0NFU1MsXG4gICAgICAgICAgICB0cmFuc2l0aW9uQWZ0ZXI6IGNkay5EdXJhdGlvbi5kYXlzKHByb3BzPy5jaGFuZ2VDbGFzc1RyYW5zaXRpb24/LmluZnJlcXVlbnRBY2Nlc3NEYXlzID8/IDYwKSxcbiAgICAgICAgICB9LFxuICAgICAgICAgIHtcbiAgICAgICAgICAgIHN0b3JhZ2VDbGFzczogczMuU3RvcmFnZUNsYXNzLklOVEVMTElHRU5UX1RJRVJJTkcsXG4gICAgICAgICAgICB0cmFuc2l0aW9uQWZ0ZXI6IGNkay5EdXJhdGlvbi5kYXlzKHByb3BzPy5jaGFuZ2VDbGFzc1RyYW5zaXRpb24/LmludGVsbGlnZW50VGllcmluZ0RheXMgPz8gMTIwKSxcbiAgICAgICAgICB9LFxuICAgICAgICAgIHtcbiAgICAgICAgICAgIHN0b3JhZ2VDbGFzczogczMuU3RvcmFnZUNsYXNzLkdMQUNJRVIsXG4gICAgICAgICAgICB0cmFuc2l0aW9uQWZ0ZXI6IGNkay5EdXJhdGlvbi5kYXlzKHByb3BzPy5jaGFuZ2VDbGFzc1RyYW5zaXRpb24/LmdsYWNpZXJEYXlzID8/IDE4MCksXG4gICAgICAgICAgfSxcbiAgICAgICAgICB7XG4gICAgICAgICAgICBzdG9yYWdlQ2xhc3M6IHMzLlN0b3JhZ2VDbGFzcy5ERUVQX0FSQ0hJVkUsXG4gICAgICAgICAgICB0cmFuc2l0aW9uQWZ0ZXI6IGNkay5EdXJhdGlvbi5kYXlzKHByb3BzPy5jaGFuZ2VDbGFzc1RyYW5zaXRpb24/LmRlZXBBcmNoaXZlRGF5cyA/PyAzNjApLFxuICAgICAgICAgIH0sXG4gICAgICAgIF0sXG4gICAgICB9XSxcbiAgICB9KTtcbiAgfVxufSJdfQ==
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9716435185185185%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.71.138'}", "'version'": "'0.8.3'"}*

```diff
@@ -22,15 +22,15 @@
         "jest-junit": "^15",
         "jsii": "1.x",
         "jsii-diff": "^1.84.0",
         "jsii-docgen": "^7.2.9",
         "jsii-pacmak": "^1.84.0",
         "jsii-rosetta": "1.x",
         "npm-check-updates": "^16",
-        "projen": "^0.71.137",
+        "projen": "^0.71.138",
         "standard-version": "^9",
         "ts-jest": "^27",
         "ts-node": "^10.9.1",
         "typescript": "^4.9.5"
     },
     "engines": {
         "node": ">= 16.0.0"
@@ -136,9 +136,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.8.2"
+    "version": "0.8.3"
 }
```

### Comparing `aws-secure-log-bucket-0.8.2/src/aws_secure_log_bucket.egg-info/PKG-INFO` & `aws-secure-log-bucket-0.8.3/src/aws_secure_log_bucket.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-secure-log-bucket
-Version: 0.8.2
+Version: 0.8.3
 Summary: secure multiple transition phases in a single lifecycle policy bucket.
 Home-page: https://github.com/yicr/aws-secure-log-bucket.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/yicr/aws-secure-log-bucket.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

