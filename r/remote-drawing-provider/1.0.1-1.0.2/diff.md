# Comparing `tmp/remote-drawing-provider-1.0.1.tar.gz` & `tmp/remote-drawing-provider-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remote-drawing-provider-1.0.1.tar", last modified: Sat Apr 29 08:42:31 2023, max compression
+gzip compressed data, was "dist\remote-drawing-provider-1.0.2.tar", last modified: Sun Jul 16 02:28:48 2023, max compression
```

## Comparing `remote-drawing-provider-1.0.1.tar` & `remote-drawing-provider-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 xyqian    (1004) xyqian    (1004)        0 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)     1061 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/LICENSE
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      777 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/PKG-INFO
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      207 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/README.md
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      543 2023-04-29 08:38:15.000000 remote-drawing-provider-1.0.1/pyproject.toml
-drwxrwxr-x   0 xyqian    (1004) xyqian    (1004)        0 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/remote_drawing_provider/
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      152 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/remote_drawing_provider/__init__.py
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)     1146 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/remote_drawing_provider/logger.py
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      972 2023-04-29 08:32:54.000000 remote-drawing-provider-1.0.1/remote_drawing_provider/provider.py
-drwxrwxr-x   0 xyqian    (1004) xyqian    (1004)        0 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      777 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/PKG-INFO
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      381 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/SOURCES.txt
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)        1 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/dependency_links.txt
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)       31 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/requires.txt
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)       24 2023-04-29 08:42:31.000000 remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/top_level.txt
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)       38 2023-04-29 08:42:31.578202 remote-drawing-provider-1.0.1/setup.cfg
--rw-rw-r--   0 xyqian    (1004) xyqian    (1004)      355 2023-04-29 08:38:23.000000 remote-drawing-provider-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/
+-rw-rw-rw-   0        0        0     1061 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      808 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-16 02:23:06.000000 remote-drawing-provider-1.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/remote_drawing_provider/
+-rw-rw-rw-   0        0        0      152 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/remote_drawing_provider/__init__.py
+-rw-rw-rw-   0        0        0     1144 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/remote_drawing_provider/logger.py
+-rw-rw-rw-   0        0        0      974 2023-07-16 02:23:16.000000 remote-drawing-provider-1.0.2/remote_drawing_provider/provider.py
+drwxrwxrwx   0        0        0        0 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/
+-rw-rw-rw-   0        0        0      808 2023-07-16 02:28:47.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 02:28:47.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-16 02:28:47.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 02:28:47.000000 remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 02:28:48.000000 remote-drawing-provider-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      355 2023-07-14 13:02:26.000000 remote-drawing-provider-1.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `remote-drawing-provider-1.0.1/LICENSE` & `remote-drawing-provider-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `remote-drawing-provider-1.0.1/PKG-INFO` & `remote-drawing-provider-1.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: remote-drawing-provider
-Version: 1.0.1
-Summary: Remote Drawing Provider
-Home-page: https://github.com/XiaoyanQian/remote-drawing
-Author: XY-qian
-Author-email: XY-qian <xiaoyanqian1010@gmail.com>
-Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
-Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# remote-drawing-provider
-
-## install
-
-```bash
-pip install remote-drawing-provider
-```
-
-## using
-
-```python
-from remote-drawing-provider.provider import send
-
-send(method='visualize_point_cloud',[args])
-```
+Metadata-Version: 2.1
+Name: remote-drawing-provider
+Version: 1.0.2
+Summary: Remote Drawing Provider
+Home-page: https://github.com/XiaoyanQian/remote-drawing
+Author: XY-qian
+Author-email: XY-qian <xiaoyanqian1010@gmail.com>
+Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
+Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# remote-drawing-provider
+
+## install
+
+```bash
+pip install remote-drawing-provider
+```
+
+## using
+
+```python
+from remote-drawing-provider.provider import send
+
+send(method='visualize_point_cloud',[args])
+```
```

### Comparing `remote-drawing-provider-1.0.1/pyproject.toml` & `remote-drawing-provider-1.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [project]
 name = "remote-drawing-provider"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="XY-qian", email="xiaoyanqian1010@gmail.com" },
 ]
 description = "Remote Drawing Provider"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
 ]
 dependencies = [
     "numpy",
     "torch",
+    "colorama>=0.4.6",
     "websockets>=11.0.2"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/XiaoyanQian/remote-drawing"
 "Bug Tracker" = "https://github.com/XiaoyanQian/remote-drawing/issues"
```

### Comparing `remote-drawing-provider-1.0.1/remote_drawing_provider/logger.py` & `remote-drawing-provider-1.0.2/remote_drawing_provider/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import os
-
-from datetime import datetime
-
 from colorama import init
 from colorama import Fore, Back, Style
+from datetime import datetime
 
 __all__ = ['log_info', 'log_warn', 'log_error', 'log_end', 'format_capacity']
 init()
 
 
 def get_time():
     return datetime.utcnow().isoformat(sep=' ', timespec='milliseconds')
```

### Comparing `remote-drawing-provider-1.0.1/remote_drawing_provider/provider.py` & `remote-drawing-provider-1.0.2/remote_drawing_provider/provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import zlib
 import torch
 from io import BytesIO
-from logger import *
 from websockets.sync.client import connect
 
+from .logger import *
+
 Port = 65532
 RenderType = 'Provider'
 TypeHeader = 'X-Client-Type'
 Headers = {TypeHeader: RenderType}
 
 __all__ = ['send']
```

### Comparing `remote-drawing-provider-1.0.1/remote_drawing_provider.egg-info/PKG-INFO` & `remote-drawing-provider-1.0.2/remote_drawing_provider.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-Metadata-Version: 2.1
-Name: remote-drawing-provider
-Version: 1.0.1
-Summary: Remote Drawing Provider
-Home-page: https://github.com/XiaoyanQian/remote-drawing
-Author: XY-qian
-Author-email: XY-qian <xiaoyanqian1010@gmail.com>
-Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
-Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# remote-drawing-provider
-
-## install
-
-```bash
-pip install remote-drawing-provider
-```
-
-## using
-
-```python
-from remote-drawing-provider.provider import send
-
-send(method='visualize_point_cloud',[args])
-```
+Metadata-Version: 2.1
+Name: remote-drawing-provider
+Version: 1.0.2
+Summary: Remote Drawing Provider
+Home-page: https://github.com/XiaoyanQian/remote-drawing
+Author: XY-qian
+Author-email: XY-qian <xiaoyanqian1010@gmail.com>
+Project-URL: Homepage, https://github.com/XiaoyanQian/remote-drawing
+Project-URL: Bug Tracker, https://github.com/XiaoyanQian/remote-drawing/issues
+Platform: any
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# remote-drawing-provider
+
+## install
+
+```bash
+pip install remote-drawing-provider
+```
+
+## using
+
+```python
+from remote-drawing-provider.provider import send
+
+send(method='visualize_point_cloud',[args])
+```
```

