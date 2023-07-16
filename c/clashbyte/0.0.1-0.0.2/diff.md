# Comparing `tmp/clashbyte-0.0.1.tar.gz` & `tmp/clashbyte-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clashbyte-0.0.1.tar", last modified: Sun Jul 16 01:10:01 2023, max compression
+gzip compressed data, was "clashbyte-0.0.2.tar", last modified: Sun Jul 16 01:46:41 2023, max compression
```

## Comparing `clashbyte-0.0.1.tar` & `clashbyte-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 01:10:01.515553 clashbyte-0.0.1/
--rw-rw-rw-   0        0        0     1085 2023-07-15 15:59:16.000000 clashbyte-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      830 2023-07-16 01:10:01.514552 clashbyte-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       67 2023-07-16 00:39:18.000000 clashbyte-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-16 01:10:01.503558 clashbyte-0.0.1/clashbyte/
--rw-rw-rw-   0        0        0      287 2023-07-15 19:56:50.000000 clashbyte-0.0.1/clashbyte/__init__.py
--rw-rw-rw-   0        0        0     4938 2023-07-16 00:58:49.000000 clashbyte-0.0.1/clashbyte/apis.py
--rw-rw-rw-   0        0        0     2137 2023-07-15 20:34:49.000000 clashbyte-0.0.1/clashbyte/toolbox.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:10:01.510551 clashbyte-0.0.1/clashbyte.egg-info/
--rw-rw-rw-   0        0        0      830 2023-07-16 01:10:01.000000 clashbyte-0.0.1/clashbyte.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2023-07-16 01:10:01.000000 clashbyte-0.0.1/clashbyte.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 01:10:01.000000 clashbyte-0.0.1/clashbyte.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-16 01:10:01.000000 clashbyte-0.0.1/clashbyte.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-16 01:10:01.000000 clashbyte-0.0.1/clashbyte.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 01:10:01.516550 clashbyte-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1300 2023-07-15 20:04:35.000000 clashbyte-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 01:10:01.512551 clashbyte-0.0.1/tests/
--rw-rw-rw-   0        0        0     2176 2023-07-16 01:09:01.000000 clashbyte-0.0.1/tests/test_clash_meta_apis.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:46:41.649707 clashbyte-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2023-07-15 15:59:16.000000 clashbyte-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1223 2023-07-16 01:46:41.648714 clashbyte-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      470 2023-07-16 01:28:22.000000 clashbyte-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 01:46:41.632723 clashbyte-0.0.2/clashbyte/
+-rw-rw-rw-   0        0        0      287 2023-07-16 01:44:45.000000 clashbyte-0.0.2/clashbyte/__init__.py
+-rw-rw-rw-   0        0        0     4972 2023-07-16 01:46:14.000000 clashbyte-0.0.2/clashbyte/apis.py
+-rw-rw-rw-   0        0        0     2137 2023-07-15 20:34:49.000000 clashbyte-0.0.2/clashbyte/toolbox.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:46:41.642716 clashbyte-0.0.2/clashbyte.egg-info/
+-rw-rw-rw-   0        0        0     1223 2023-07-16 01:46:41.000000 clashbyte-0.0.2/clashbyte.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-07-16 01:46:41.000000 clashbyte-0.0.2/clashbyte.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 01:46:41.000000 clashbyte-0.0.2/clashbyte.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-07-16 01:46:41.000000 clashbyte-0.0.2/clashbyte.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-16 01:46:41.000000 clashbyte-0.0.2/clashbyte.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 01:46:41.649707 clashbyte-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1264 2023-07-16 01:24:53.000000 clashbyte-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 01:46:41.645716 clashbyte-0.0.2/tests/
+-rw-rw-rw-   0        0        0     2158 2023-07-16 01:44:22.000000 clashbyte-0.0.2/tests/test_clash_meta_apis.py
```

### Comparing `clashbyte-0.0.1/LICENSE` & `clashbyte-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clashbyte-0.0.1/PKG-INFO` & `clashbyte-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: clashbyte
-Version: 0.0.1
-Home-page: https://github.com/QIN2DIM/hcaptcha-challenger
+Version: 0.0.2
+Home-page: https://github.com/QIN2DIM/ClashByte
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 License: MIT
 Keywords: clashbyte,clash,clash-meta,clashapi
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
@@ -17,7 +17,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # ClashByte
 Clash &amp; Clash.Meta 外部控制的 Python 实现
+
+## Get started
+
+1. Install package
+
+   ```bash
+   pip install -U clashbyte
+   ```
+
+2. hello world
+
+   ```python
+   from clashbyte import ClashMetaAPI
+   
+   CONTROLLER_URL = "http://127.0.0.1:9090"
+   
+   if __name__ == '__main__':
+       clash = ClashMetaAPI.from_secret(controller_url=CONTROLLER_URL)
+       if clash.is_alive:
+           print(f"{clash.version=}")
+   ```
+
+
```

### Comparing `clashbyte-0.0.1/clashbyte/apis.py` & `clashbyte-0.0.2/clashbyte/apis.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # Time       : 2023/7/7 3:10
 # Author     : QIN2DIM
 # Github     : https://github.com/QIN2DIM
 # Description:
 from __future__ import annotations
 
+import os
 import socket
 from dataclasses import dataclass
 from typing import Literal
 from urllib.parse import urlparse
 
 import httpx
 from loguru import logger
@@ -22,36 +23,36 @@
 @dataclass
 class ClashMeta:
     """https://wiki.metacubex.one/api/"""
 
 
 @dataclass
 class ClashMetaAPI:
+    secret: str = ""
     controller_url: str = ""
 
-    _client: httpx.Client = None
+    _client = None
+    _core = None
 
-    _core: ClashMeta = None
+    def __post_init__(self):
+        if not self.controller_url:
+            self.controller_url = os.environ.get("CLASH_URL", "http://127.0.0.1:9090")
+        if not self.secret:
+            self.secret = os.environ.get("CLASH_SECRET", "")
 
-    @classmethod
-    def from_secret(
-            cls, secret: str | None = "", controller_url: str | None = "http://127.0.0.1:9090"
-    ) -> ClashMetaAPI | None:
-        headers = {"Authorization": f"Bearer {secret}"}
-        if not secret:
+        headers = {"Authorization": f"Bearer {self.secret}"}
+        if not self.secret:
             logger.warning(
                 "Please set your external secret key. \n"
-                'python -c "import secrets;print(secrets.token_hex()[:16])"',
+                'python -c "import secrets;print(secrets.token_hex())"',
                 documentation="https://wiki.metacubex.one/api/#_1",
             )
             del headers["Authorization"]
-        instance = cls(controller_url=controller_url)
-        instance._client = httpx.Client(base_url=controller_url, headers=headers)
-        instance._core = ClashMeta()
-        return instance
+        self._client: httpx.Client = httpx.Client(base_url=self.controller_url, headers=headers)
+        self._core: ClashMeta = ClashMeta()
 
     @property
     def is_alive(self):
         u = urlparse(self.controller_url)
         try:
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 host, port = u.netloc.split(":")
```

### Comparing `clashbyte-0.0.1/clashbyte/toolbox.py` & `clashbyte-0.0.2/clashbyte/toolbox.py`

 * *Files identical despite different names*

### Comparing `clashbyte-0.0.1/clashbyte.egg-info/PKG-INFO` & `clashbyte-0.0.2/clashbyte.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: clashbyte
-Version: 0.0.1
-Home-page: https://github.com/QIN2DIM/hcaptcha-challenger
+Version: 0.0.2
+Home-page: https://github.com/QIN2DIM/ClashByte
 Author: QIN2DIM
 Author-email: yaoqinse@gmail.com
 License: MIT
 Keywords: clashbyte,clash,clash-meta,clashapi
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
@@ -17,7 +17,30 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # ClashByte
 Clash &amp; Clash.Meta 外部控制的 Python 实现
+
+## Get started
+
+1. Install package
+
+   ```bash
+   pip install -U clashbyte
+   ```
+
+2. hello world
+
+   ```python
+   from clashbyte import ClashMetaAPI
+   
+   CONTROLLER_URL = "http://127.0.0.1:9090"
+   
+   if __name__ == '__main__':
+       clash = ClashMetaAPI.from_secret(controller_url=CONTROLLER_URL)
+       if clash.is_alive:
+           print(f"{clash.version=}")
+   ```
+
+
```

### Comparing `clashbyte-0.0.1/setup.py` & `clashbyte-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,17 @@
     version=clashbyte.__version__,
     keywords=["clashbyte", "clash", "clash-meta", "clashapi"],
     author="QIN2DIM",
     author_email="yaoqinse@gmail.com",
     long_description=Path(__file__).parent.joinpath("README.md").read_text(encoding="utf8"),
     long_description_content_type="text/markdown",
     license="MIT",
-    url="https://github.com/QIN2DIM/hcaptcha-challenger",
+    url="https://github.com/QIN2DIM/ClashByte",
     packages=find_packages(include=["clashbyte", "clashbyte.*", "LICENSE"]),
-    install_requires=[
-        "loguru>=0.7.0",
-        "httpx>=0.24.1",
-    ],
+    install_requires=["loguru>=0.7.0", "httpx>=0.24.1"],
     extras_require={"dev": ["nox", "pytest"], "test": ["pytest", "black"]},
     python_requires=">=3.8",
     classifiers=[
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
```

### Comparing `clashbyte-0.0.1/tests/test_clash_meta_apis.py` & `clashbyte-0.0.2/tests/test_clash_meta_apis.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,37 +12,36 @@
 import httpx
 from loguru import logger
 
 from clashbyte import ClashMetaAPI
 from clashbyte import project, init_log
 
 # 快速生成密钥，添加到 Clash-Verge 外部控制组件
-# python -c "import secrets;print(secrets.token_hex()[:16])"
+# python -c "import secrets;print(secrets.token_hex())"
 CONTROLLER_SECRET = os.environ.get("CLASH_SECRET")
 CONTROLLER_URL = "http://127.0.0.1:9090"
 
 cache_dir = Path("cache")
 cache_dir.mkdir(exist_ok=True)
 
 init_log(
     stdout_level="DEBUG",
     error=project.logs.joinpath("error.log"),
     runtime=project.logs.joinpath("runtime.log"),
     serialize=project.logs.joinpath("serialize.log"),
 )
 
-clash = ClashMetaAPI.from_secret(CONTROLLER_SECRET, CONTROLLER_URL)
-
+clash = ClashMetaAPI(CONTROLLER_SECRET, CONTROLLER_URL)
 
 def write_result(result, fp: Path):
     cache = json.dumps(result, indent=4)
     fp.write_text(cache)
 
 
-def test_is_live():
+def test_is_alive():
     logger.debug(clash.is_alive)
 
 
 @logger.catch()
 def test_get_dns_query():
     clash.flush_fakeip_cache()
     names = ["www.bilibili.com", "www.baidu.com", "www.google.com", "www.youtube.com"]
```

