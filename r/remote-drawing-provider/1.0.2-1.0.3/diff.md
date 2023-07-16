# Comparing `tmp/remote-drawing-provider-1.0.2.tar.gz` & `tmp/remote-drawing-provider-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\remote-drawing-provider-1.0.2.tar", last modified: Sun Jul 16 02:28:48 2023, max compression
+gzip compressed data, was "dist\remote-drawing-provider-1.0.3.tar", last modified: Sun Jul 16 02:35:36 2023, max compression
```

## Comparing `remote-drawing-provider-1.0.2.tar` & `remote-drawing-provider-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/
--rw-rw-rw-   0        0        0     1061 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      808 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/README.md
--rw-rw-rw-   0        0        0      566 2023-07-16 02:23:06.000000 remote-drawing-provider-1.0.2/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/remote_drawing_provider/
--rw-rw-rw-   0        0        0      152 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/remote_drawing_provider/__init__.py
--rw-rw-rw-   0        0        0     1144 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/remote_drawing_provider/logger.py
--rw-rw-rw-   0        0        0      974 2023-07-16 02:23:16.000000 remote-drawing-provider-1.0.2/remote_drawing_provider/provider.py
-drwxrwxrwx   0        0        0        0 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/
--rw-rw-rw-   0        0        0      808 2023-07-16 02:28:47.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 02:28:47.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-16 02:28:47.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-16 02:28:47.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      355 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/
+-rw-rw-rw-   0        0        0     1061 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      880 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-07-16 02:33:08.000000 remote-drawing-provider-1.0.3/README.md
+-rw-rw-rw-   0        0        0      570 2023-07-16 02:34:41.000000 remote-drawing-provider-1.0.3/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/remote_drawing_provider/
+-rw-rw-rw-   0        0        0      152 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.3/remote_drawing_provider/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.3/remote_drawing_provider/logger.py
+-rw-rw-rw-   0        0        0      974 2023-07-16 02:23:16.000000 remote-drawing-provider-1.0.3/remote_drawing_provider/provider.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/remote_drawing_provider.egg-info/
+-rw-rw-rw-   0        0        0      880 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/remote_drawing_provider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/remote_drawing_provider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/remote_drawing_provider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/remote_drawing_provider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/remote_drawing_provider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 02:35:36.000000 remote-drawing-provider-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      355 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.3/setup.py
```

### Comparing `remote-drawing-provider-1.0.2/LICENSE` & `remote-drawing-provider-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `remote-drawing-provider-1.0.2/PKG-INFO` & `remote-drawing-provider-1.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: remote-drawing-provider
-Version: 1.0.2
+Version: 1.0.3
 Summary: Remote Drawing Provider
 Home-page: https://github.com/XiaoyanQian/remote-drawing
 Author: XY-qian
-Author-email: XY-qian <xiaoyanqian1010@gmail.com>
+Author-email: XiaoyanQian <xiaoyanqian1010@gmail.com>
 Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
 Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -21,11 +21,15 @@
 ```bash
 pip install remote-drawing-provider
 ```
 
 ## using
 
 ```python
-from remote-drawing-provider.provider import send
+import torch
+from remote_drawing_provider.provider import send
 
-send(method='visualize_point_cloud',[args])
+args = {
+    'point_cloud': torch.randn(1000,3)
+}
+send(method='visualize_point_cloud', **args)
 ```
```

### Comparing `remote-drawing-provider-1.0.2/pyproject.toml` & `remote-drawing-provider-1.0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "remote-drawing-provider"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
-  { name="XY-qian", email="xiaoyanqian1010@gmail.com" },
+  { name="XiaoyanQian", email="xiaoyanqian1010@gmail.com" },
 ]
 description = "Remote Drawing Provider"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
```

### Comparing `remote-drawing-provider-1.0.2/remote_drawing_provider/logger.py` & `remote-drawing-provider-1.0.3/remote_drawing_provider/logger.py`

 * *Files identical despite different names*

### Comparing `remote-drawing-provider-1.0.2/remote_drawing_provider/provider.py` & `remote-drawing-provider-1.0.3/remote_drawing_provider/provider.py`

 * *Files identical despite different names*

### Comparing `remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/PKG-INFO` & `remote-drawing-provider-1.0.3/remote_drawing_provider.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: remote-drawing-provider
-Version: 1.0.2
+Version: 1.0.3
 Summary: Remote Drawing Provider
 Home-page: https://github.com/XiaoyanQian/remote-drawing
 Author: XY-qian
-Author-email: XY-qian <xiaoyanqian1010@gmail.com>
+Author-email: XiaoyanQian <xiaoyanqian1010@gmail.com>
 Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
 Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -21,11 +21,15 @@
 ```bash
 pip install remote-drawing-provider
 ```
 
 ## using
 
 ```python
-from remote-drawing-provider.provider import send
+import torch
+from remote_drawing_provider.provider import send
 
-send(method='visualize_point_cloud',[args])
+args = {
+    'point_cloud': torch.randn(1000,3)
+}
+send(method='visualize_point_cloud', **args)
 ```
```

