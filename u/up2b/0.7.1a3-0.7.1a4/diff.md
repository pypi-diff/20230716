# Comparing `tmp/up2b-0.7.1a3.tar.gz` & `tmp/up2b-0.7.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up2b-0.7.1a3.tar", last modified: Sat Jun 17 03:07:32 2023, max compression
+gzip compressed data, was "up2b-0.7.1a4.tar", last modified: Sun Jul 16 02:05:46 2023, max compression
```

## Comparing `up2b-0.7.1a3.tar` & `up2b-0.7.1a4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.003206 up2b-0.7.1a3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.003206 up2b-0.7.1a3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-17 03:07:21.000000 up2b-0.7.1a3/.github/workflows/check.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-17 03:07:21.000000 up2b-0.7.1a3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-06-17 03:07:21.000000 up2b-0.7.1a3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-17 03:07:21.000000 up2b-0.7.1a3/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-17 03:07:21.000000 up2b-0.7.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-17 03:07:32.007206 up2b-0.7.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-17 03:07:21.000000 up2b-0.7.1a3/README.en_US.md
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-17 03:07:21.000000 up2b-0.7.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-17 03:07:21.000000 up2b-0.7.1a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 03:07:21.000000 up2b-0.7.1a3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-17 03:07:32.007206 up2b-0.7.1a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.003206 up2b-0.7.1a3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/tests/images/
--rw-r--r--   0 runner    (1001) docker     (123)    28768 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/images/1.png
--rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/images/2.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/images/3.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/test_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-17 03:07:21.000000 up2b-0.7.1a3/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/up2b/
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/up2b/up2b_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/
--rw-r--r--   0 runner    (1001) docker     (123)    16307 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10523 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/imgtg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12689 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/imgtu.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8390 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/up2b_api/sm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-06-17 03:07:21.000000 up2b-0.7.1a3/up2b/up2b_lib/watermark.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 03:07:32.007206 up2b-0.7.1a3/up2b.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8399 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-17 03:07:31.000000 up2b-0.7.1a3/up2b.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.941675 up2b-0.7.1a4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.925675 up2b-0.7.1a4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.933675 up2b-0.7.1a4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-16 02:05:34.000000 up2b-0.7.1a4/.github/workflows/check.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-07-16 02:05:34.000000 up2b-0.7.1a4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-16 02:05:34.000000 up2b-0.7.1a4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-16 02:05:34.000000 up2b-0.7.1a4/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-16 02:05:34.000000 up2b-0.7.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-16 02:05:46.941675 up2b-0.7.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-07-16 02:05:34.000000 up2b-0.7.1a4/README.en_US.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-16 02:05:34.000000 up2b-0.7.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-16 02:05:34.000000 up2b-0.7.1a4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-16 02:05:34.000000 up2b-0.7.1a4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 02:05:46.941675 up2b-0.7.1a4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.933675 up2b-0.7.1a4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.933675 up2b-0.7.1a4/tests/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    28768 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/images/1.png
+-rw-r--r--   0 runner    (1001) docker     (123)   142746 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/images/2.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/images/3.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/test_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-16 02:05:34.000000 up2b-0.7.1a4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.933675 up2b-0.7.1a4/up2b/
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.941675 up2b-0.7.1a4/up2b/up2b_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.941675 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10373 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/imgtg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12680 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/imgtu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/up2b_api/sm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4908 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-07-16 02:05:34.000000 up2b-0.7.1a4/up2b/up2b_lib/watermark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:05:46.937675 up2b-0.7.1a4/up2b.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8410 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-16 02:05:46.000000 up2b-0.7.1a4/up2b.egg-info/top_level.txt
```

### Comparing `up2b-0.7.1a3/.github/workflows/check.yaml` & `up2b-0.7.1a4/.github/workflows/check.yaml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/.github/workflows/publish.yaml` & `up2b-0.7.1a4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/LICENSE` & `up2b-0.7.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/PKG-INFO` & `up2b-0.7.1a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up2b
-Version: 0.7.1a3
+Version: 0.7.1a4
 Summary: 上传图片到图床
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,21 +49,21 @@
 支持 Linux、macOS 和 Windows。
 
 ## 特点
 
 支持以下图床自动上传:
 
 - sm.ms
-- imgse.com(原imgtu.com)
+- imgse.com(原 imgtu.com)
 - github.com
 - imgtg.com
 
-成功上传到`github`后会返回`jsdelivr`的CDN链接，加快在中国境内对图片的访问速度。
+成功上传到`github`后会返回`jsdelivr`的 CDN 链接，加快在中国境内对图片的访问速度。
 
-支持jpeg/jpg和png图片的自动压缩，但仅在测试阶段，可能有些小问题，如果你不想在使用此功能时出现错误或达不到预期则不建议使用。
+支持 jpeg/jpg 和 png 图片的自动压缩，但仅在测试阶段，可能有些小问题，如果你不想在使用此功能时出现错误或达不到预期则不建议使用。
 
 ## 怎么用
 
 安装`up2b`包:
 
 ```shell
 pip install up2b
@@ -102,36 +102,36 @@
 - 4
   - imgtg.com
 
 ```bash
 # 如果你想选择sm.ms
 up2b choose 0
 ```
+
 > 你可能也注意到了，图床的 code 不连续，这是因为最初写这个项目的时候没有考虑到一些图床挂掉的可能性，删掉一些挂掉的图床后，为了使配置文件不冲突，所以图床 code 无法连续。
 >
-> 
->
 > 在 1.0 版本中，将不会再使用数字作为图床的 code，这个问题将会解决，同时会启用全新的配置文件，与 0.X.X 版本的配置文件将不通用。
 
 ### 2 保存认证信息
 
 #### **普通图床：**
 
-git仓库本身并不算是图床，所以git仓库之外的图床都是普通图床。
+git 仓库本身并不算是图床，所以 git 仓库之外的图床都是普通图床。
 
 使用普通图床时，用`login`命令进行认证信息的配置，如：
 
 ```shell
 up2b login username password
 ```
-#### **git仓库：**
 
-此包所指的git仓库包括`github`。
+#### **git 仓库：**
+
+此包所指的 git 仓库包括`github`。
 
-使用git仓库作为图床，需要用或`login-git`命令进行认证信息的配置。
+使用 git 仓库作为图床，需要用或`login-git`命令进行认证信息的配置。
 
 认证信息需要四个参数：
 
 - `ACCESS_TOKEN` 私密令牌
 - `USERNAME` 用户名
 - `REPO` 仓库名
 - `FOLDER` 想要保存在仓库里的哪个文件夹中，会自动创建不存在的文件夹
@@ -154,16 +154,14 @@
 Options:
 	-aw, --add-watermark  对要上传的图片添加文字水印
 	-ac, --auto-compress  允许自动压缩图片
 	-ic, --ignore-cache   忽略数据库缓存，强制上传图片
 	-h, --help            Show this message and exit.
 ```
 
-
-
 将`up2b upload`命令填到`Typora`里，命令里有个参数`-ac`为可选参数，其作用为开启自动压缩功能，如果不加此参数，上传图片时不会自动压缩，超出图床限制大小就会报错。而添加此参数，则会自动将超限图片压缩到限制图片大小或以下，保证顺利上传。
 
 但自动压缩功能当前没有经过严谨地测试，所以不能保证不出问题，有问题请将异常的截图发在电报群里。
 
 开启自动压缩功能：
 
 ```shell
@@ -197,15 +195,15 @@
 ### 创建虚拟环境
 
 如果你不担心对环境中的其他包产生影响，也不介意自己的 Python 库中多一些可能永远用不到的包，则可以忽略此步。
 
 > 如果你使用的环境管理工具为 pthon 内置的 venv，请自行创建环境，这里不多介绍。
 
 ```bash
-conda create -n up2b-temp python=3.10
+conda create -n up2b-temp python=3.11
 conda activate up2b-temp
 ```
 
 ### 安装依赖
 
 ```bash
 pip install build
@@ -230,15 +228,15 @@
 以下是 v1 版本的初步功能设计。
 
 - [ ] 设计通用配置文件规则
 
   - [ ] 图床类型
     - [ ] git
     - [ ] api
-    - [ ] 非api
+    - [ ] 非 api
 
 - [ ] 图床可用性检测及无效标记
 
   - [ ] 对配置文件中的图床进行可达（超时）检测
   - [ ] 对不可达（超时）的图床添加一个无效标记，并记录检测时间
   - [ ] 用户可设置检测周期，在检测周期内不会检测无效图床以节约时间
   - [ ] 用户可设置删除（软删除）无效图床配置的周期次数，当达到或超过此次数的检测周期后，将在配置文件中将此图床标记为永久失效（软删除）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up2b Version: 0.7.1a3 Summary:
+Metadata-Version: 2.1 Name: up2b Version: 0.7.1a4 Summary:
 ä¸ä¼ å¾çå°å¾åº Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2021 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -20,41 +20,42 @@
 Description-Content-Type: text/markdown Provides-Extra: mark License-File:
 LICENSE [English](https://github.com/thep0y/up2b) >
 å½ä»¤è¡ç®¡çå¤ªéº»ç¦ï¼è¯è¯[up2b-gui](https://github.com/thep0y/up2b-
 gui)å§ï¼
                               ****** UP2B ******
                                   [Downloads]
 ä¸ä¸ªè½å¨ç»ç«¯ä¸­å°å¾çä¸ä¼ å°å¾åºçåã æ¯æ LinuxãmacOS å
-Windowsã ## ç¹ç¹ æ¯æä»¥ä¸å¾åºèªå¨ä¸ä¼ : - sm.ms - imgse.com
-(åimgtu.com) - github.com - imgtg.com
-æåä¸ä¼ å°`github`åä¼è¿å`jsdelivr`çCDNé¾æ¥ï¼å å¿«å¨ä¸­å½å¢åå¯¹å¾ççè®¿é®éåº¦ã
-æ¯æjpeg/
-jpgåpngå¾ççèªå¨åç¼©ï¼ä½ä»å¨æµè¯é¶æ®µï¼å¯è½æäºå°é®é¢ï¼å¦æä½ ä¸æ³å¨ä½¿ç¨æ­¤åè½æ¶åºç°éè¯¯æè¾¾ä¸å°é¢æåä¸å»ºè®®ä½¿ç¨ã
+Windowsã ## ç¹ç¹ æ¯æä»¥ä¸å¾åºèªå¨ä¸ä¼ : - sm.ms - imgse.com(å
+imgtu.com) - github.com - imgtg.com
+æåä¸ä¼ å°`github`åä¼è¿å`jsdelivr`ç CDN
+é¾æ¥ï¼å å¿«å¨ä¸­å½å¢åå¯¹å¾ççè®¿é®éåº¦ã æ¯æ jpeg/jpg å
+png
+å¾ççèªå¨åç¼©ï¼ä½ä»å¨æµè¯é¶æ®µï¼å¯è½æäºå°é®é¢ï¼å¦æä½ ä¸æ³å¨ä½¿ç¨æ­¤åè½æ¶åºç°éè¯¯æè¾¾ä¸å°é¢æåä¸å»ºè®®ä½¿ç¨ã
 ## æä¹ç¨ å®è£`up2b`å: ```shell pip install up2b ```
 å®è£åï¼ä¼å¤åºä¸æ¡`up2b`å½ä»¤ï¼ ``` Usage: python -m up2b [OPTIONS]
 COMMAND [ARGS]... Options: -h, --help æ¾ç¤ºæ¬å¸®å©ä¿¡æ¯ -v, --version
 æ¾ç¤ºçæ¬ä¿¡æ¯ Commands: choose éæ©å¾åº config-watermark
 éç½®æå­æ°´å° current æ¾ç¤ºæ­£å¨ä½¿ç¨çå¾åº list
 ååºæ¯æçææå¾åº login ä¿å­å¾åºç»å½ä¿¡æ¯ login-git ä¿å­ git
 ç»å½ä¿¡æ¯ upload ä¸ä¼ å¾ç ``` ### 1 éæ©å¾åº
 ç¬¬ä¸æ¬¡ä½¿ç¨æ¶ï¼å¿é¡»åéæ©å¾åºã
 `up2b`ç`choose`å½ä»¤çå¯éå¼ä¸ºï¼ - 0 - sm.ms - 1 - imgse.com - 2 -
 github.com - 4 - imgtg.com ```bash # å¦æä½ æ³éæ©sm.ms up2b choose 0 ```
 > ä½ å¯è½ä¹æ³¨æå°äºï¼å¾åºç code
 ä¸è¿ç»­ï¼è¿æ¯å ä¸ºæååè¿ä¸ªé¡¹ç®çæ¶åæ²¡æèèå°ä¸äºå¾åºææçå¯è½æ§ï¼å æä¸äºææçå¾åºåï¼ä¸ºäºä½¿éç½®æä»¶ä¸å²çªï¼æä»¥å¾åº
-code æ æ³è¿ç»­ã > > > > å¨ 1.0
+code æ æ³è¿ç»­ã > > å¨ 1.0
 çæ¬ä¸­ï¼å°ä¸ä¼åä½¿ç¨æ°å­ä½ä¸ºå¾åºç
 codeï¼è¿ä¸ªé®é¢å°ä¼è§£å³ï¼åæ¶ä¼å¯ç¨å¨æ°çéç½®æä»¶ï¼ä¸
 0.X.X çæ¬çéç½®æä»¶å°ä¸éç¨ã ### 2 ä¿å­è®¤è¯ä¿¡æ¯ ####
-**æ®éå¾åºï¼**
-gitä»åºæ¬èº«å¹¶ä¸ç®æ¯å¾åºï¼æä»¥gitä»åºä¹å¤çå¾åºé½æ¯æ®éå¾åºã
+**æ®éå¾åºï¼** git ä»åºæ¬èº«å¹¶ä¸ç®æ¯å¾åºï¼æä»¥ git
+ä»åºä¹å¤çå¾åºé½æ¯æ®éå¾åºã
 ä½¿ç¨æ®éå¾åºæ¶ï¼ç¨`login`å½ä»¤è¿è¡è®¤è¯ä¿¡æ¯çéç½®ï¼å¦ï¼
-```shell up2b login username password ``` #### **gitä»åºï¼**
-æ­¤åææçgitä»åºåæ¬`github`ã
-ä½¿ç¨gitä»åºä½ä¸ºå¾åºï¼éè¦ç¨æ`login-
+```shell up2b login username password ``` #### **git ä»åºï¼**
+æ­¤åææç git ä»åºåæ¬`github`ã ä½¿ç¨ git
+ä»åºä½ä¸ºå¾åºï¼éè¦ç¨æ`login-
 git`å½ä»¤è¿è¡è®¤è¯ä¿¡æ¯çéç½®ã è®¤è¯ä¿¡æ¯éè¦åä¸ªåæ°ï¼ -
 `ACCESS_TOKEN` ç§å¯ä»¤ç - `USERNAME` ç¨æ·å - `REPO` ä»åºå -
 `FOLDER`
 æ³è¦ä¿å­å¨ä»åºéçåªä¸ªæä»¶å¤¹ä¸­ï¼ä¼èªå¨åå»ºä¸å­å¨çæä»¶å¤¹
 æ¯å¦ï¼ææ³å°å¾çä¿å­å¨`image-
 bed`ä»åºéç`md`æä»¶å¤¹åï¼è¾å¥æ­¤å½ä»¤ï¼ ```shell up2b login-git
 access_token username image-bed md ``` ### 3 (å¯é) å¨ typora
@@ -74,22 +75,22 @@
 /s2.loli.net/2023/03/04/wNqgOpn4Tz5ZUHQ.png) ## èªè¡æå
 å¦ææ­¤é¡¹ç®ä¸­æ´æ°äºæäºç¹æ§å¯¹ä½ æ¥è¯´å¾æç¨ï¼ä½å°æªåå¸æ°ç
 releaseï¼é£ä¹ä½ å¯ä»¥èªè¡æåå®è£ã ### åå»ºèæç¯å¢
 å¦æä½ ä¸æå¿å¯¹ç¯å¢ä¸­çå¶ä»åäº§çå½±åï¼ä¹ä¸ä»æèªå·±ç
 Python åºä¸­å¤ä¸äºå¯è½æ°¸è¿ç¨ä¸å°çåï¼åå¯ä»¥å¿½ç¥æ­¤æ­¥ã >
 å¦æä½ ä½¿ç¨çç¯å¢ç®¡çå·¥å·ä¸º pthon åç½®ç
 venvï¼è¯·èªè¡åå»ºç¯å¢ï¼è¿éä¸å¤ä»ç»ã ```bash conda create -
-n up2b-temp python=3.10 conda activate up2b-temp ``` ### å®è£ä¾èµ ```bash
+n up2b-temp python=3.11 conda activate up2b-temp ``` ### å®è£ä¾èµ ```bash
 pip install build ``` ### æå ```bash python -m build ```
 ä¼å¨é¡¹ç®çæ ¹ç®å½åå»º`dist`ç®å½ï¼éé¢å°±ææåå¥½ç`whl`æä»¶ï¼å®è£å³å¯ï¼
 ``` pip install -U dist/up2b-*-py3-none-any.whl ``` ## TODO
 é´äºå¾åºç½ç«åçéåº¦è¶ä¹æ³è±¡ï¼æä»¥å¨ä¸ä¸ªå¤§çæ¬ä¸­æä¸æç®åå¯¹ä»»ä½å¾åºè¿è¡æ¯æï¼èæ¯ä½¿ç¨éç½®æä»¶çæ¹å¼ç±ç¨æ·èªè¡æ·»å å¾åºï¼å¹¶æ·»å æ£æµå¾åºå¯ç¨æ§çåè½ã
 ä»¥ä¸æ¯ v1 çæ¬çåæ­¥åè½è®¾è®¡ã - [ ]
-è®¾è®¡éç¨éç½®æä»¶è§å - [ ] å¾åºç±»å - [ ] git - [ ] api - [ ]
-éapi - [ ] å¾åºå¯ç¨æ§æ£æµåæ ææ è®° - [ ]
+è®¾è®¡éç¨éç½®æä»¶è§å - [ ] å¾åºç±»å - [ ] git - [ ] api - [ ] é
+api - [ ] å¾åºå¯ç¨æ§æ£æµåæ ææ è®° - [ ]
 å¯¹éç½®æä»¶ä¸­çå¾åºè¿è¡å¯è¾¾ï¼è¶æ¶ï¼æ£æµ - [ ]
 å¯¹ä¸å¯è¾¾ï¼è¶æ¶ï¼çå¾åºæ·»å ä¸ä¸ªæ ææ è®°ï¼å¹¶è®°å½æ£æµæ¶é´
 - [ ]
 ç¨æ·å¯è®¾ç½®æ£æµå¨æï¼å¨æ£æµå¨æåä¸ä¼æ£æµæ æå¾åºä»¥èçº¦æ¶é´
 - [ ]
 ç¨æ·å¯è®¾ç½®å é¤ï¼è½¯å é¤ï¼æ æå¾åºéç½®çå¨ææ¬¡æ°ï¼å½è¾¾å°æè¶è¿æ­¤æ¬¡æ°çæ£æµå¨æåï¼å°å¨éç½®æä»¶ä¸­å°æ­¤å¾åºæ è®°ä¸ºæ°¸ä¹å¤±æï¼è½¯å é¤ï¼
 - [ ] ç¨æ·å¯å¨éç½®æä»¶ä¸­å é¤æ ææ è®° - [ ] æ¬å°ç½é¡µéç½®
```

### Comparing `up2b-0.7.1a3/README.en_US.md` & `up2b-0.7.1a4/README.en_US.md`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/README.md` & `up2b-0.7.1a4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,21 +13,21 @@
 支持 Linux、macOS 和 Windows。
 
 ## 特点
 
 支持以下图床自动上传:
 
 - sm.ms
-- imgse.com(原imgtu.com)
+- imgse.com(原 imgtu.com)
 - github.com
 - imgtg.com
 
-成功上传到`github`后会返回`jsdelivr`的CDN链接，加快在中国境内对图片的访问速度。
+成功上传到`github`后会返回`jsdelivr`的 CDN 链接，加快在中国境内对图片的访问速度。
 
-支持jpeg/jpg和png图片的自动压缩，但仅在测试阶段，可能有些小问题，如果你不想在使用此功能时出现错误或达不到预期则不建议使用。
+支持 jpeg/jpg 和 png 图片的自动压缩，但仅在测试阶段，可能有些小问题，如果你不想在使用此功能时出现错误或达不到预期则不建议使用。
 
 ## 怎么用
 
 安装`up2b`包:
 
 ```shell
 pip install up2b
@@ -66,36 +66,36 @@
 - 4
   - imgtg.com
 
 ```bash
 # 如果你想选择sm.ms
 up2b choose 0
 ```
+
 > 你可能也注意到了，图床的 code 不连续，这是因为最初写这个项目的时候没有考虑到一些图床挂掉的可能性，删掉一些挂掉的图床后，为了使配置文件不冲突，所以图床 code 无法连续。
 >
-> 
->
 > 在 1.0 版本中，将不会再使用数字作为图床的 code，这个问题将会解决，同时会启用全新的配置文件，与 0.X.X 版本的配置文件将不通用。
 
 ### 2 保存认证信息
 
 #### **普通图床：**
 
-git仓库本身并不算是图床，所以git仓库之外的图床都是普通图床。
+git 仓库本身并不算是图床，所以 git 仓库之外的图床都是普通图床。
 
 使用普通图床时，用`login`命令进行认证信息的配置，如：
 
 ```shell
 up2b login username password
 ```
-#### **git仓库：**
 
-此包所指的git仓库包括`github`。
+#### **git 仓库：**
+
+此包所指的 git 仓库包括`github`。
 
-使用git仓库作为图床，需要用或`login-git`命令进行认证信息的配置。
+使用 git 仓库作为图床，需要用或`login-git`命令进行认证信息的配置。
 
 认证信息需要四个参数：
 
 - `ACCESS_TOKEN` 私密令牌
 - `USERNAME` 用户名
 - `REPO` 仓库名
 - `FOLDER` 想要保存在仓库里的哪个文件夹中，会自动创建不存在的文件夹
@@ -118,16 +118,14 @@
 Options:
 	-aw, --add-watermark  对要上传的图片添加文字水印
 	-ac, --auto-compress  允许自动压缩图片
 	-ic, --ignore-cache   忽略数据库缓存，强制上传图片
 	-h, --help            Show this message and exit.
 ```
 
-
-
 将`up2b upload`命令填到`Typora`里，命令里有个参数`-ac`为可选参数，其作用为开启自动压缩功能，如果不加此参数，上传图片时不会自动压缩，超出图床限制大小就会报错。而添加此参数，则会自动将超限图片压缩到限制图片大小或以下，保证顺利上传。
 
 但自动压缩功能当前没有经过严谨地测试，所以不能保证不出问题，有问题请将异常的截图发在电报群里。
 
 开启自动压缩功能：
 
 ```shell
@@ -161,15 +159,15 @@
 ### 创建虚拟环境
 
 如果你不担心对环境中的其他包产生影响，也不介意自己的 Python 库中多一些可能永远用不到的包，则可以忽略此步。
 
 > 如果你使用的环境管理工具为 pthon 内置的 venv，请自行创建环境，这里不多介绍。
 
 ```bash
-conda create -n up2b-temp python=3.10
+conda create -n up2b-temp python=3.11
 conda activate up2b-temp
 ```
 
 ### 安装依赖
 
 ```bash
 pip install build
@@ -194,15 +192,15 @@
 以下是 v1 版本的初步功能设计。
 
 - [ ] 设计通用配置文件规则
 
   - [ ] 图床类型
     - [ ] git
     - [ ] api
-    - [ ] 非api
+    - [ ] 非 api
 
 - [ ] 图床可用性检测及无效标记
 
   - [ ] 对配置文件中的图床进行可达（超时）检测
   - [ ] 对不可达（超时）的图床添加一个无效标记，并记录检测时间
   - [ ] 用户可设置检测周期，在检测周期内不会检测无效图床以节约时间
   - [ ] 用户可设置删除（软删除）无效图床配置的周期次数，当达到或超过此次数的检测周期后，将在配置文件中将此图床标记为永久失效（软删除）
```

#### html2text {}

```diff
@@ -1,39 +1,40 @@
 [English](https://github.com/thep0y/up2b) > å½ä»¤è¡ç®¡çå¤ªéº»ç¦ï¼è¯è¯
 [up2b-gui](https://github.com/thep0y/up2b-gui)å§ï¼
                               ****** UP2B ******
                                   [Downloads]
 ä¸ä¸ªè½å¨ç»ç«¯ä¸­å°å¾çä¸ä¼ å°å¾åºçåã æ¯æ LinuxãmacOS å
-Windowsã ## ç¹ç¹ æ¯æä»¥ä¸å¾åºèªå¨ä¸ä¼ : - sm.ms - imgse.com
-(åimgtu.com) - github.com - imgtg.com
-æåä¸ä¼ å°`github`åä¼è¿å`jsdelivr`çCDNé¾æ¥ï¼å å¿«å¨ä¸­å½å¢åå¯¹å¾ççè®¿é®éåº¦ã
-æ¯æjpeg/
-jpgåpngå¾ççèªå¨åç¼©ï¼ä½ä»å¨æµè¯é¶æ®µï¼å¯è½æäºå°é®é¢ï¼å¦æä½ ä¸æ³å¨ä½¿ç¨æ­¤åè½æ¶åºç°éè¯¯æè¾¾ä¸å°é¢æåä¸å»ºè®®ä½¿ç¨ã
+Windowsã ## ç¹ç¹ æ¯æä»¥ä¸å¾åºèªå¨ä¸ä¼ : - sm.ms - imgse.com(å
+imgtu.com) - github.com - imgtg.com
+æåä¸ä¼ å°`github`åä¼è¿å`jsdelivr`ç CDN
+é¾æ¥ï¼å å¿«å¨ä¸­å½å¢åå¯¹å¾ççè®¿é®éåº¦ã æ¯æ jpeg/jpg å
+png
+å¾ççèªå¨åç¼©ï¼ä½ä»å¨æµè¯é¶æ®µï¼å¯è½æäºå°é®é¢ï¼å¦æä½ ä¸æ³å¨ä½¿ç¨æ­¤åè½æ¶åºç°éè¯¯æè¾¾ä¸å°é¢æåä¸å»ºè®®ä½¿ç¨ã
 ## æä¹ç¨ å®è£`up2b`å: ```shell pip install up2b ```
 å®è£åï¼ä¼å¤åºä¸æ¡`up2b`å½ä»¤ï¼ ``` Usage: python -m up2b [OPTIONS]
 COMMAND [ARGS]... Options: -h, --help æ¾ç¤ºæ¬å¸®å©ä¿¡æ¯ -v, --version
 æ¾ç¤ºçæ¬ä¿¡æ¯ Commands: choose éæ©å¾åº config-watermark
 éç½®æå­æ°´å° current æ¾ç¤ºæ­£å¨ä½¿ç¨çå¾åº list
 ååºæ¯æçææå¾åº login ä¿å­å¾åºç»å½ä¿¡æ¯ login-git ä¿å­ git
 ç»å½ä¿¡æ¯ upload ä¸ä¼ å¾ç ``` ### 1 éæ©å¾åº
 ç¬¬ä¸æ¬¡ä½¿ç¨æ¶ï¼å¿é¡»åéæ©å¾åºã
 `up2b`ç`choose`å½ä»¤çå¯éå¼ä¸ºï¼ - 0 - sm.ms - 1 - imgse.com - 2 -
 github.com - 4 - imgtg.com ```bash # å¦æä½ æ³éæ©sm.ms up2b choose 0 ```
 > ä½ å¯è½ä¹æ³¨æå°äºï¼å¾åºç code
 ä¸è¿ç»­ï¼è¿æ¯å ä¸ºæååè¿ä¸ªé¡¹ç®çæ¶åæ²¡æèèå°ä¸äºå¾åºææçå¯è½æ§ï¼å æä¸äºææçå¾åºåï¼ä¸ºäºä½¿éç½®æä»¶ä¸å²çªï¼æä»¥å¾åº
-code æ æ³è¿ç»­ã > > > > å¨ 1.0
+code æ æ³è¿ç»­ã > > å¨ 1.0
 çæ¬ä¸­ï¼å°ä¸ä¼åä½¿ç¨æ°å­ä½ä¸ºå¾åºç
 codeï¼è¿ä¸ªé®é¢å°ä¼è§£å³ï¼åæ¶ä¼å¯ç¨å¨æ°çéç½®æä»¶ï¼ä¸
 0.X.X çæ¬çéç½®æä»¶å°ä¸éç¨ã ### 2 ä¿å­è®¤è¯ä¿¡æ¯ ####
-**æ®éå¾åºï¼**
-gitä»åºæ¬èº«å¹¶ä¸ç®æ¯å¾åºï¼æä»¥gitä»åºä¹å¤çå¾åºé½æ¯æ®éå¾åºã
+**æ®éå¾åºï¼** git ä»åºæ¬èº«å¹¶ä¸ç®æ¯å¾åºï¼æä»¥ git
+ä»åºä¹å¤çå¾åºé½æ¯æ®éå¾åºã
 ä½¿ç¨æ®éå¾åºæ¶ï¼ç¨`login`å½ä»¤è¿è¡è®¤è¯ä¿¡æ¯çéç½®ï¼å¦ï¼
-```shell up2b login username password ``` #### **gitä»åºï¼**
-æ­¤åææçgitä»åºåæ¬`github`ã
-ä½¿ç¨gitä»åºä½ä¸ºå¾åºï¼éè¦ç¨æ`login-
+```shell up2b login username password ``` #### **git ä»åºï¼**
+æ­¤åææç git ä»åºåæ¬`github`ã ä½¿ç¨ git
+ä»åºä½ä¸ºå¾åºï¼éè¦ç¨æ`login-
 git`å½ä»¤è¿è¡è®¤è¯ä¿¡æ¯çéç½®ã è®¤è¯ä¿¡æ¯éè¦åä¸ªåæ°ï¼ -
 `ACCESS_TOKEN` ç§å¯ä»¤ç - `USERNAME` ç¨æ·å - `REPO` ä»åºå -
 `FOLDER`
 æ³è¦ä¿å­å¨ä»åºéçåªä¸ªæä»¶å¤¹ä¸­ï¼ä¼èªå¨åå»ºä¸å­å¨çæä»¶å¤¹
 æ¯å¦ï¼ææ³å°å¾çä¿å­å¨`image-
 bed`ä»åºéç`md`æä»¶å¤¹åï¼è¾å¥æ­¤å½ä»¤ï¼ ```shell up2b login-git
 access_token username image-bed md ``` ### 3 (å¯é) å¨ typora
@@ -53,22 +54,22 @@
 /s2.loli.net/2023/03/04/wNqgOpn4Tz5ZUHQ.png) ## èªè¡æå
 å¦ææ­¤é¡¹ç®ä¸­æ´æ°äºæäºç¹æ§å¯¹ä½ æ¥è¯´å¾æç¨ï¼ä½å°æªåå¸æ°ç
 releaseï¼é£ä¹ä½ å¯ä»¥èªè¡æåå®è£ã ### åå»ºèæç¯å¢
 å¦æä½ ä¸æå¿å¯¹ç¯å¢ä¸­çå¶ä»åäº§çå½±åï¼ä¹ä¸ä»æèªå·±ç
 Python åºä¸­å¤ä¸äºå¯è½æ°¸è¿ç¨ä¸å°çåï¼åå¯ä»¥å¿½ç¥æ­¤æ­¥ã >
 å¦æä½ ä½¿ç¨çç¯å¢ç®¡çå·¥å·ä¸º pthon åç½®ç
 venvï¼è¯·èªè¡åå»ºç¯å¢ï¼è¿éä¸å¤ä»ç»ã ```bash conda create -
-n up2b-temp python=3.10 conda activate up2b-temp ``` ### å®è£ä¾èµ ```bash
+n up2b-temp python=3.11 conda activate up2b-temp ``` ### å®è£ä¾èµ ```bash
 pip install build ``` ### æå ```bash python -m build ```
 ä¼å¨é¡¹ç®çæ ¹ç®å½åå»º`dist`ç®å½ï¼éé¢å°±ææåå¥½ç`whl`æä»¶ï¼å®è£å³å¯ï¼
 ``` pip install -U dist/up2b-*-py3-none-any.whl ``` ## TODO
 é´äºå¾åºç½ç«åçéåº¦è¶ä¹æ³è±¡ï¼æä»¥å¨ä¸ä¸ªå¤§çæ¬ä¸­æä¸æç®åå¯¹ä»»ä½å¾åºè¿è¡æ¯æï¼èæ¯ä½¿ç¨éç½®æä»¶çæ¹å¼ç±ç¨æ·èªè¡æ·»å å¾åºï¼å¹¶æ·»å æ£æµå¾åºå¯ç¨æ§çåè½ã
 ä»¥ä¸æ¯ v1 çæ¬çåæ­¥åè½è®¾è®¡ã - [ ]
-è®¾è®¡éç¨éç½®æä»¶è§å - [ ] å¾åºç±»å - [ ] git - [ ] api - [ ]
-éapi - [ ] å¾åºå¯ç¨æ§æ£æµåæ ææ è®° - [ ]
+è®¾è®¡éç¨éç½®æä»¶è§å - [ ] å¾åºç±»å - [ ] git - [ ] api - [ ] é
+api - [ ] å¾åºå¯ç¨æ§æ£æµåæ ææ è®° - [ ]
 å¯¹éç½®æä»¶ä¸­çå¾åºè¿è¡å¯è¾¾ï¼è¶æ¶ï¼æ£æµ - [ ]
 å¯¹ä¸å¯è¾¾ï¼è¶æ¶ï¼çå¾åºæ·»å ä¸ä¸ªæ ææ è®°ï¼å¹¶è®°å½æ£æµæ¶é´
 - [ ]
 ç¨æ·å¯è®¾ç½®æ£æµå¨æï¼å¨æ£æµå¨æåä¸ä¼æ£æµæ æå¾åºä»¥èçº¦æ¶é´
 - [ ]
 ç¨æ·å¯è®¾ç½®å é¤ï¼è½¯å é¤ï¼æ æå¾åºéç½®çå¨ææ¬¡æ°ï¼å½è¾¾å°æè¶è¿æ­¤æ¬¡æ°çæ£æµå¨æåï¼å°å¨éç½®æä»¶ä¸­å°æ­¤å¾åºæ è®°ä¸ºæ°¸ä¹å¤±æï¼è½¯å é¤ï¼
 - [ ] ç¨æ·å¯å¨éç½®æä»¶ä¸­å é¤æ ææ è®° - [ ] æ¬å°ç½é¡µéç½®
```

### Comparing `up2b-0.7.1a3/pyproject.toml` & `up2b-0.7.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/tests/images/1.png` & `up2b-0.7.1a4/tests/images/1.png`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/tests/images/2.jpeg` & `up2b-0.7.1a4/tests/images/2.jpeg`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/tests/images/3.jpeg` & `up2b-0.7.1a4/tests/images/3.jpeg`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/tests/server.py` & `up2b-0.7.1a4/tests/server.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/tests/test_upload.py` & `up2b-0.7.1a4/tests/test_upload.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/tests/test_utils.py` & `up2b-0.7.1a4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/up2b/__init__.py` & `up2b-0.7.1a4/up2b/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,16 @@
 # @Modified At: 2023-04-19 14:45:15
 # @Modified By: thepoy
 
 import sys
 import json
 import click
 
-from typing import Any, Dict, Optional, Tuple, Type, Union
+from typing import Any, Dict, Tuple, Type, Union
 from colort import display_style as ds
-from up2b.up2b_lib.custom_types import AuthData
 from up2b.up2b_lib.up2b_api import choose_image_bed
 from up2b.up2b_lib.up2b_api.sm import SM
 from up2b.up2b_lib.up2b_api.imgtu import Imgtu
 from up2b.up2b_lib.up2b_api.github import Github
 from up2b.up2b_lib.up2b_api.imgtg import Imgtg
 from up2b.up2b_lib.constants import (
     CACHE_PATH,
@@ -256,15 +255,15 @@
 def _read_image_bed(
     auto_compress: bool = False,
     add_watermark: bool = False,
     ignore_cache: bool = False,
 ) -> Union[SM, Imgtu, Imgtg, Github]:
     conf = read_conf()
 
-    selected_code = conf.get("image_bed")
+    selected_code = conf.image_bed
     if not selected_code:
         logger.fatal("当前图床为空，请先选择要使用的图床")
 
     assert isinstance(selected_code, int)
 
     try:
         code = ImageBedCode(selected_code)
@@ -316,45 +315,44 @@
                     }
                 )
             )
 
 
 def print_list() -> int:
     conf = read_conf()
-    auth_data: AuthData = conf.get("auth_data", {})  # type: ignore
+    auth_data = conf.auth_data
+
+    assert isinstance(auth_data, dict)
 
     if not auth_data:
-        selected_code = conf.get("image_bed")
-        if selected_code is None:
+        if conf.image_bed is None:
             logger.warning(
                 "no image bed selected, "
                 + "you need to use `--choose-site` or `-c` to select the image bed first."
             )
 
-        if selected_code:
-            code = ImageBedCode(selected_code)
-
+        if conf.image_bed:
             logger.warning(
                 "no authentication information has been configured",
                 image_bed=ds.format_with_multiple_styles(
-                    IMAGE_BEDS[code]().__str__(),
-                    ds.backgorud_color.dark_gray,
-                    ds.foreground_color.white,
+                    IMAGE_BEDS[conf.image_bed](conf=conf).__str__(),
+                    ds.bc.dark_gray,
+                    ds.fc.white,
                 ),
-                code=selected_code,
+                code=conf.image_bed,
             )
 
     def print_item(symbol, color, idx):
-        ib = IMAGE_BEDS[ImageBedCode(idx)]()
+        ib = IMAGE_BEDS[ImageBedCode(idx)](conf=conf)
         click.echo(
             f"""{ds.format_with_one_style(" " + symbol, color)} {idx} {ib}: {ib.description}"""
         )
 
     for i in ImageBedCode:
-        if auth_data.get(str(i)):
+        if auth_data.get(i):
             print_item(chr(10003), ds.fc.green, i)
         else:
             print_item(chr(10007), ds.fc.red, i)
 
     return 0
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/cache.py` & `up2b-0.7.1a4/up2b/up2b_lib/cache.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/constants.py` & `up2b-0.7.1a4/up2b/up2b_lib/constants.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/custom_types.py` & `up2b-0.7.1a4/up2b/up2b_lib/custom_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 # @Email:       thepoy@163.com
 # @File Name:   custom_types.py
 # @Created At:  2021-02-09 11:27:21
 # @Modified At: 2023-02-21 12:41:21
 # @Modified By: thepoy
 
 from enum import IntEnum
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, List, Optional, Union
 from dataclasses import dataclass, asdict
 from pathlib import Path
 
+from up2b.up2b_lib.constants import ImageBedCode
+
 
 class ImageBedType(IntEnum):
     common = 1
     git = 2
 
 
 @dataclass
@@ -35,14 +37,21 @@
 ConfigFile = Dict[str, Union[int, AuthData, WaterMarkConfig]]
 DeletedResponse = Dict[str, Union[bool, str]]
 ImageType = Union[ImagePath, ImageStream]
 Images = List[ImageType]
 
 
 @dataclass
+class Config:
+    image_bed: Optional[ImageBedCode]
+    auth_data: Dict[ImageBedCode, Dict[str, str]]
+    watermark: WaterMarkConfig
+
+
+@dataclass
 class BaseResponse:
     def to_dict(self) -> Dict[str, Any]:
         return asdict(self)
 
 
 @dataclass
 class ErrorResponse(BaseResponse):
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/i18n.py` & `up2b-0.7.1a4/up2b/up2b_lib/i18n.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/log.py` & `up2b-0.7.1a4/up2b/up2b_lib/log.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/__init__.py` & `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,9 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Author:      thepoy
-# @Email:       thepoy@163.com
-# @File Name:   __init__.py
-# @Created At:  2021-02-13 09:02:21
-# @Modified At: 2023-04-19 14:41:12
-# @Modified By: thepoy
 
 import os
 import time
 import json
 import shutil
 import requests
 
@@ -28,15 +22,15 @@
 
 if PYTHON_VERSION >= (3, 8):
     from functools import cached_property
 else:
     cached_property = property
 
 from up2b.up2b_lib.custom_types import (
-    ConfigFile,
+    Config,
     DownloadErrorResponse,
     ErrorResponse,
     GitGetAllImagesResponse,
     ImageBedType,
     ImagePath,
     ImageStream,
     ImageType,
@@ -96,31 +90,32 @@
     def description(self) -> str:
         pass
 
 
 class Base(ImageBedAbstract):
     image_bed_code: ImageBedCode
     max_size: int
-    conf: ConfigFile
+    conf: Config
     image_bed_type: ImageBedType
     timeout = timeout()
     cache = Cache()
 
     def __init__(
         self,
         auto_compress: bool = False,
         add_watermark: bool = False,
         ignore_cache: bool = False,
+        conf: Optional[Config] = None,
     ):
-        self.conf = read_conf()
+        self.conf = conf if conf != None else read_conf()
 
         self.auth_info: Optional[AuthInfo] = self._read_auth_info()
         self.add_watermark: bool = add_watermark
         if self.add_watermark:
-            if not self.conf.get("watermark"):
+            if not self.conf.watermark:
                 logger.fatal(
                     "you have enabled the function of adding watermark, but the watermark is not configured, please configure the text watermark through `--config-text-watermark`"
                 )
         self.auto_compress: bool = auto_compress
         self.ignore_cache: bool = ignore_cache
 
     def check_login(self):
@@ -128,21 +123,21 @@
             logger.fatal(
                 "you have not logged in yet, please log in first.",
                 code=self.image_bed_code,
                 name=self,
             )
 
     def _read_auth_info(self) -> Optional[AuthInfo]:
-        auth_data = self.conf.get("auth_data")
+        auth_data = self.conf.auth_data
         if not auth_data:
             return
 
         assert isinstance(auth_data, dict)
 
-        auth_info = auth_data.get(str(self.image_bed_code))
+        auth_info = auth_data.get(self.image_bed_code)
 
         assert auth_info is None or isinstance(auth_info, dict)
 
         return auth_info
 
     def _save_auth_info(self, auth_info: Dict[str, str]):
         logger.debug("current image bed code", code=self.image_bed_code)
@@ -352,16 +347,17 @@
     folder: str
 
     def __init__(
         self,
         auto_compress: bool = False,
         add_watermark: bool = False,
         ignore_cache: bool = False,
+        conf: Optional[Config] = None,
     ):
-        super().__init__(auto_compress, add_watermark, ignore_cache)
+        super().__init__(auto_compress, add_watermark, ignore_cache, conf)
 
         if self.auth_info:
             self.token = self.auth_info["token"]
             self.username = self.auth_info["username"]
             self.repo = self.auth_info["repo"]
             self.folder = self.auth_info["folder"]
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/__init__.pyi` & `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/__init__.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -3,149 +3,109 @@
 import requests
 
 from abc import ABC, abstractmethod
 from typing import overload, Optional, List, Tuple, Dict, Union
 from up2b.up2b_lib.cache import Cache
 from up2b.up2b_lib.constants import ImageBedCode
 from up2b.up2b_lib.custom_types import (
-    ConfigFile,
+    Config,
     DownloadErrorResponse,
     ErrorResponse,
     GitGetAllImagesResponse,
     ImageBedType,
     ImagePath,
     ImageStream,
     ImageType,
     AuthInfo,
     ImgtuResponse,
     SMMSResponse,
     UploadErrorResponse,
 )
 
-
-def choose_image_bed(image_bed_code: int) -> None:
-    ...
-
+def choose_image_bed(image_bed_code: int) -> None: ...
 
 AllImagesResponse = (
     List[GitGetAllImagesResponse] | List[SMMSResponse] | List[ImgtuResponse]
 )
 
-
 class ImageBedAbstract(ABC):
     @abstractmethod
-    def get_all_images(self) -> Union[AllImagesResponse, ErrorResponse]:
-        ...
-
+    def get_all_images(self) -> Union[AllImagesResponse, ErrorResponse]: ...
     @abstractmethod
     def upload_image(self, image_path: ImagePath) -> Union[str, UploadErrorResponse]:
         pass
-
     @abstractmethod
     def upload_image_stream(
         self, image: ImageStream
-    ) -> Union[str, UploadErrorResponse]:
-        ...
-
+    ) -> Union[str, UploadErrorResponse]: ...
     @overload
     @abstractmethod
     def delete_image(
         self, unique_id: str, retries: int = ...
-    ) -> Optional[ErrorResponse]:
-        ...
-
+    ) -> Optional[ErrorResponse]: ...
     @overload
     @abstractmethod
     def delete_image(
         self,
         sha: str,
         url: str,
         message: str = ...,
-    ) -> Optional[ErrorResponse]:
-        ...
-
+    ) -> Optional[ErrorResponse]: ...
     @overload
     @abstractmethod
     def delete_images(
         self, unique_ids: List[str], retries: int = ...
-    ) -> Dict[str, ErrorResponse]:
-        ...
-
+    ) -> Dict[str, ErrorResponse]: ...
     @overload
     @abstractmethod
     def delete_images(
         self,
         info: List[Tuple[str, str]],
         message: str = ...,
-    ) -> Dict[str, ErrorResponse]:
-        ...
-
+    ) -> Dict[str, ErrorResponse]: ...
     @property
     @abstractmethod
-    def description(self) -> str:
-        ...
-
+    def description(self) -> str: ...
 
 class Base:
     image_bed_code: ImageBedCode
     max_size: int
-    conf: ConfigFile
+    conf: Config
     image_bed_type: ImageBedType
     conf_file: str
     auth_info: Optional[AuthInfo]
     add_watermark: bool
     auto_compress: bool
     ignore_cache: bool
     timeout: float
     cache: Cache
 
     def __init__(
         self,
         auto_compress: bool = ...,
         add_watermark: bool = ...,
         ignore_cache: bool = ...,
-    ) -> None:
-        ...
-
-    def check_login(self) -> None:
-        ...
-
-    def _read_auth_info(self) -> Optional[AuthInfo]:
-        ...
-
-    def _save_auth_info(self, auth_info: Dict[str, str]) -> None:
-        ...
-
+        conf: Optional[Config] = ...,
+    ) -> None: ...
+    def check_login(self) -> None: ...
+    def _read_auth_info(self) -> Optional[AuthInfo]: ...
+    def _save_auth_info(self, auth_info: Dict[str, str]) -> None: ...
     def _exceed_max_size(
         self, images: Tuple[Union[ImageType, DownloadErrorResponse]]
-    ) -> Tuple[bool, Optional[str]]:
-        ...
-
+    ) -> Tuple[bool, Optional[str]]: ...
     def _check_images_valid(
         self, images: Tuple[Union[ImageType, DownloadErrorResponse]]
-    ):
-        ...
-
-    def _compress_image(self, image: ImageType) -> ImageType:
-        ...
-
-    def _add_watermark(self, image_path: ImagePath) -> ImagePath:
-        ...
-
-    def _clear_cache(self) -> None:
-        ...
-
-    def _check_cache(self, image: Path) -> Tuple[str, str, bool]:
-        ...
-
+    ): ...
+    def _compress_image(self, image: ImageType) -> ImageType: ...
+    def _add_watermark(self, image_path: ImagePath) -> ImagePath: ...
+    def _clear_cache(self) -> None: ...
+    def _check_cache(self, image: Path) -> Tuple[str, str, bool]: ...
     def upload_images(
         self, *images: Union[ImageType, DownloadErrorResponse], to_console: bool = ...
-    ) -> List[Union[str, UploadErrorResponse]]:
-        ...
-
+    ) -> List[Union[str, UploadErrorResponse]]: ...
 
 class GitBase(Base, ImageBedAbstract):
     headers: Dict[str, str]
     api_url: str
 
     token: str
     username: str
@@ -153,46 +113,34 @@
     folder: str
 
     def __init__(
         self,
         auto_compress: bool = ...,
         add_watermark: bool = ...,
         ignore_cache: bool = ...,
-    ) -> None:
-        ...
-
-    def login(self, token: str, username: str, repo: str, folder: str = ...) -> None:
-        ...
-
+        conf: Optional[Config] = ...,
+    ) -> None: ...
+    def login(
+        self, token: str, username: str, repo: str, folder: str = ...
+    ) -> None: ...
     def _upload(
         self, image: ImageType, data: Dict[str, str], request_method: str = ...
-    ) -> Union[str, UploadErrorResponse]:
-        ...
-
+    ) -> Union[str, UploadErrorResponse]: ...
     @abstractmethod
     def _get_all_images_in_image_bed(
         self,
-    ) -> requests.Response:
-        ...
-
-    def get_all_images(self) -> Union[List[GitGetAllImagesResponse], ErrorResponse]:
-        ...
-
+    ) -> requests.Response: ...
+    def get_all_images(self) -> Union[List[GitGetAllImagesResponse], ErrorResponse]: ...
     def _delete_image(
         self,
         sha: str,
         url: str,
         message: str = ...,
         extra: Optional[Dict[str, str]] = ...,
-    ) -> Optional[ErrorResponse]:
-        ...
-
+    ) -> Optional[ErrorResponse]: ...
     def delete_images(
         self,
         info: List[Tuple[str, str]],
         message: str = ...,
-    ) -> Dict[str, ErrorResponse]:
-        ...
-
+    ) -> Dict[str, ErrorResponse]: ...
     @property
-    def base_url(self) -> str:
-        ...
+    def base_url(self) -> str: ...
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/github.py` & `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import os
 import requests
 
 from base64 import b64encode
 from typing import Optional
 from up2b.up2b_lib.custom_types import (
+    Config,
     ImageBedType,
     ImagePath,
     ImageStream,
     ErrorResponse,
 )
 from up2b.up2b_lib.up2b_api import GitBase
 from up2b.up2b_lib.constants import ImageBedCode
@@ -32,35 +33,36 @@
     image_bed_type = ImageBedType.git
 
     def __init__(
         self,
         auto_compress: bool = False,
         add_watermark: bool = False,
         ignore_cache: bool = False,
+        conf: Optional[Config] = None,
     ):
-        super().__init__(auto_compress, add_watermark, ignore_cache)
+        super().__init__(auto_compress, add_watermark, ignore_cache, conf)
 
         if hasattr(self, "token"):
             self.headers = {
                 "Accept": "application/vnd.github.v3+json",
                 "Authorization": "token " + self.token,
             }
 
     def upload_image(self, image_path: ImagePath):
         basename = os.path.basename(image_path)
-        logger.debug("uploading: %s", basename)
+        logger.debug("uploading", name=basename)
         with open(image_path, "rb") as fb:
             data = {
                 "content": b64encode(fb.read()).decode("utf-8"),
                 "message": "up2b - " + basename,
             }
         return self._upload(image_path, data)
 
     def upload_image_stream(self, image: ImageStream):
-        logger.debug("uploading: %s", image.filename)
+        logger.debug("uploading", name=image.filename)
         data = {
             "content": b64encode(image.stream).decode("utf-8"),
             "message": "up2b - " + image.filename,
         }
         return self._upload(image, data)
 
     def _get_all_images_in_image_bed(self):
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/imgtg.py` & `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/imgtg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Author:      thepoy
-# @Email:       thepoy@163.com
-# @File Name:   imgtg.py
-# @Created At:  2023-01-10 13:39:51
-# @Modified At: 2023-04-19 14:38:19
-# @Modified By: thepoy
 
 import os
-from pathlib import Path
 import re
 import time
 import json
 import mimetypes
 import requests
 
 from urllib import parse
 from typing import List, Optional, Set, Tuple, Union
+from pathlib import Path
 from up2b.up2b_lib.custom_types import (
+    Config,
     ErrorResponse,
     ImageBedType,
     ImageType,
     ImageStream,
     ImagePath,
     ImgtuResponse,
     UploadErrorResponse,
@@ -45,16 +40,17 @@
     }
 
     def __init__(
         self,
         auto_compress: bool = False,
         add_watermark: bool = False,
         ignore_cache: bool = False,
+        conf: Optional[Config] = None,
     ):
-        super().__init__(auto_compress, add_watermark, ignore_cache)
+        super().__init__(auto_compress, add_watermark, ignore_cache, conf)
 
         self.cookie: Optional[str] = None
         self.token: Optional[str] = None
         if self.auth_info:
             self.cookie = self.auth_info["cookie"]
             self.token = self.auth_info["token"]
             self.username = self.auth_info["username"]
@@ -147,14 +143,16 @@
         self.check_login()
 
         url, md5, ok = self._check_cache(image)  # type: ignore
 
         if ok and not self.ignore_cache:
             return url
 
+        logger.debug("uploading", image_path=image)
+
         image = self._compress_image(image)
 
         if isinstance(image, Path):
             image = self._add_watermark(image)
 
         url = self._url("json")
         filename_with_suffix = os.path.basename(str(image))
@@ -201,15 +199,15 @@
             json_resp = resp.json()
         except json.decoder.JSONDecodeError:
             return UploadErrorResponse(resp.status_code, resp.text, str(image))
 
         try:
             uploaded_url: str = json_resp["image"]["image"]["url"]
             logger.info(
-                "uploaded url",
+                "uploaded",
                 target=image,
                 url=uploaded_url,
             )
 
             self.cache.save(
                 md5,
                 IMAGE_BEDS_NAME[self.image_bed_code],
@@ -234,16 +232,14 @@
                 return self.__upload(image, retries + 1)
             else:
                 return UploadErrorResponse(
                     resp.status_code, resp.json()["error"]["message"], str(image)
                 )
 
     def upload_image(self, image_path: ImagePath) -> Union[str, UploadErrorResponse]:
-        logger.debug("uploading", image_path=image_path)
-
         image_path = self._add_watermark(image_path)
 
         if self.auto_compress:
             # 输入的是路径，返回的也必然是路径，忽略 pyright 的错误提示
             image_path = self._compress_image(image_path)  # type: ignore
 
         return self.__upload(image_path)
@@ -332,8 +328,8 @@
         return self.base_url + path
 
     def __repr__(self):
         return "imgtg.com"
 
     @property
     def description(self):
-        return "更适合中国大陆使用，但不支持删除图片"
+        return "中国大陆使用响应较快"
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/imgtu.py` & `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/imgtu.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import json
 import mimetypes
 import requests
 
 from urllib import parse
 from typing import Dict, List, Optional, Set, Tuple, Union
 from up2b.up2b_lib.custom_types import (
+    Config,
     ErrorResponse,
     ImageBedType,
     ImageType,
     ImageStream,
     ImagePath,
     ImgtuResponse,
     UploadErrorResponse,
@@ -45,16 +46,17 @@
     }
 
     def __init__(
         self,
         auto_compress: bool = False,
         add_watermark: bool = False,
         ignore_cache: bool = False,
+        conf: Optional[Config] = None,
     ):
-        super().__init__(auto_compress, add_watermark, ignore_cache)
+        super().__init__(auto_compress, add_watermark, ignore_cache, conf)
 
         self.cookie: Optional[str] = None
         self.token: Optional[str] = None
         if self.auth_info:
             self.cookie = self.auth_info["cookie"]
             self.token = self.auth_info["token"]
             self.username = self.auth_info["username"]
@@ -152,14 +154,16 @@
         self.check_login()
 
         image = self._compress_image(image)
 
         if isinstance(image, Path):
             image = self._add_watermark(image)
 
+        logger.debug("uploading", image_path=image)
+
         url = self._url("json")
         filename_with_suffix = os.path.basename(str(image))
         filename_without_suffix, suffix = os.path.splitext(filename_with_suffix)
         if isinstance(image, Path):
             if suffix.lower() == ".apng":
                 suffix = ".png"
             filename = filename_without_suffix + suffix
@@ -234,23 +238,19 @@
                 return self.__upload(image, retries + 1)
             else:
                 return UploadErrorResponse(
                     resp.status_code, resp.json()["error"]["message"], str(image)
                 )
 
     def upload_image(self, image_path: ImagePath) -> Union[str, UploadErrorResponse]:
-        logger.debug("uploading", image_path=image_path)
-
         return self.__upload(image_path)
 
     def upload_image_stream(
         self, image: ImageStream
     ) -> Union[str, UploadErrorResponse]:
-        logger.debug("uploading:", filename=image.filename)
-
         return self.__upload(image)
 
     def get_all_images(self) -> Union[List[ImgtuResponse], ErrorResponse]:
         self.check_login()
 
         url = self._url(self.username)
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/up2b_api/sm.py` & `up2b-0.7.1a4/up2b/up2b_lib/up2b_api/sm.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 import re
 import requests
 
 from typing import BinaryIO, List, Optional, Dict, Any, Tuple, Union
 from pathlib import Path
 from up2b.up2b_lib.custom_types import (
+    Config,
     ErrorResponse,
     ImageBedType,
     ImagePath,
     ImageStream,
     ImageType,
     SMMSResponse,
     UploadErrorResponse,
@@ -35,16 +36,17 @@
     max_size = 5 * 1024 * 1024
 
     def __init__(
         self,
         auto_compress: bool = False,
         add_watermark: bool = False,
         ignore_cache: bool = False,
+        conf: Optional[Config] = None,
     ):
-        super().__init__(auto_compress, add_watermark, ignore_cache)
+        super().__init__(auto_compress, add_watermark, ignore_cache, conf)
 
         if self.auth_info:
             self.token: str = self.auth_info["token"]
 
             self.headers = {
                 "Authorization": self.token,
             }
@@ -53,15 +55,15 @@
         try:
             token = self._get_api_token(username, password)
             self._save_auth_info(
                 {"token": token, "username": username, "password": password}
             )
             return True
         except Exception as e:
-            logger.error(e)
+            logger.error(e.__str__())
             return False
 
     def _auto_login(self):
         if not self.auth_info:
             raise ValueError("auth info is not found")
 
         username = self.auth_info["username"]
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/utils.py` & `up2b-0.7.1a4/up2b/up2b_lib/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
-# @Author:      thepoy
-# @Email:       thepoy@163.com
-# @File Name:   utils.py
-# @Created At:  2021-02-09 15:17:32
-# @Modified At: 2023-03-09 10:11:26
-# @Modified By: thepoy
 
 import json
 import os
 import locale
 import requests
 
 from typing import List, Sequence, Tuple, Union
 from functools import wraps, partial
 from pathlib import Path
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from urllib.parse import urlparse
+
 from up2b.up2b_lib.constants import (
     CONF_FILE,
     DEFAULT_TIMEOUT,
     IS_MACOS,
     PYTHON_VERSION,
     CACHE_PATH,
+    ImageBedCode,
 )
 from up2b.up2b_lib.custom_types import (
+    Config,
     DownloadErrorResponse,
     ImageType,
-    ConfigFile,
 )
 from up2b.up2b_lib.log import child_logger
 
 
 logger = child_logger(__name__)
 
 
@@ -48,33 +44,41 @@
 
 def check_image_exists(images: Tuple[Union[ImageType, DownloadErrorResponse]]):
     for image in images:
         if isinstance(image, Path) and not image.exists():
             raise FileNotFoundError(image)
 
 
-def read_conf() -> ConfigFile:  # type: ignore
+def read_conf() -> Config:
+    logger.trace("reading configuration file")
+
     if os.getenv("UP2B_TEST"):
-        return {}
+        return Config(None, {}, {})
 
     if not CONF_FILE.exists():
         logger.warning(
             "the configuration file is not found, "
             + "you need to use `--choose-site` or `-c` to select the image bed first."
         )
 
-        return {}
+        return Config(None, {}, {})
 
     try:
         with CONF_FILE.open(encoding="utf-8") as f:
-            conf: ConfigFile = json.loads(f.read())
+            conf = json.loads(f.read())
     except Exception as e:
         logger.fatal("unkown error", err=e)
     else:
-        return conf
+        auth_data = {
+            ImageBedCode(int(k)): v for k, v in conf.get("auth_data", {}).items()
+        }
+
+        return Config(
+            ImageBedCode(conf.get("image_bed")), auth_data, conf.get("watermark", {})
+        )
 
 
 class Login:
     def __init__(self, func):
         wraps(func)(self)
 
     def __call__(self, instance, *args, **kwargs):
@@ -153,18 +157,18 @@
     logger.debug("在线图片已保存到缓存目录", cache_path=cache_path)
 
     return cache_path
 
 
 def check_path(path: Union[Path, str]):
     if not is_url(str(path)):
-        logger.debug("不是在线图片", path=path)
+        logger.debug("本地图片", path=path)
         return Path(path)
 
-    logger.info("是在线图片", path=path)
+    logger.info("在线图片", path=path)
 
     return download_online_image(str(path))
 
 
 def check_paths(paths: Union[Sequence[str], Sequence[Path]]):
     if len(paths) == 1:
         return [check_path(Path(paths[0]))]
```

### Comparing `up2b-0.7.1a3/up2b/up2b_lib/watermark.py` & `up2b-0.7.1a4/up2b/up2b_lib/watermark.py`

 * *Files identical despite different names*

### Comparing `up2b-0.7.1a3/up2b.egg-info/PKG-INFO` & `up2b-0.7.1a4/up2b.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up2b
-Version: 0.7.1a3
+Version: 0.7.1a4
 Summary: 上传图片到图床
 Author-email: thep0y <thepoy@163.com>
 License: MIT License
         
         Copyright (c) 2021 thep0y
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,21 +49,21 @@
 支持 Linux、macOS 和 Windows。
 
 ## 特点
 
 支持以下图床自动上传:
 
 - sm.ms
-- imgse.com(原imgtu.com)
+- imgse.com(原 imgtu.com)
 - github.com
 - imgtg.com
 
-成功上传到`github`后会返回`jsdelivr`的CDN链接，加快在中国境内对图片的访问速度。
+成功上传到`github`后会返回`jsdelivr`的 CDN 链接，加快在中国境内对图片的访问速度。
 
-支持jpeg/jpg和png图片的自动压缩，但仅在测试阶段，可能有些小问题，如果你不想在使用此功能时出现错误或达不到预期则不建议使用。
+支持 jpeg/jpg 和 png 图片的自动压缩，但仅在测试阶段，可能有些小问题，如果你不想在使用此功能时出现错误或达不到预期则不建议使用。
 
 ## 怎么用
 
 安装`up2b`包:
 
 ```shell
 pip install up2b
@@ -102,36 +102,36 @@
 - 4
   - imgtg.com
 
 ```bash
 # 如果你想选择sm.ms
 up2b choose 0
 ```
+
 > 你可能也注意到了，图床的 code 不连续，这是因为最初写这个项目的时候没有考虑到一些图床挂掉的可能性，删掉一些挂掉的图床后，为了使配置文件不冲突，所以图床 code 无法连续。
 >
-> 
->
 > 在 1.0 版本中，将不会再使用数字作为图床的 code，这个问题将会解决，同时会启用全新的配置文件，与 0.X.X 版本的配置文件将不通用。
 
 ### 2 保存认证信息
 
 #### **普通图床：**
 
-git仓库本身并不算是图床，所以git仓库之外的图床都是普通图床。
+git 仓库本身并不算是图床，所以 git 仓库之外的图床都是普通图床。
 
 使用普通图床时，用`login`命令进行认证信息的配置，如：
 
 ```shell
 up2b login username password
 ```
-#### **git仓库：**
 
-此包所指的git仓库包括`github`。
+#### **git 仓库：**
+
+此包所指的 git 仓库包括`github`。
 
-使用git仓库作为图床，需要用或`login-git`命令进行认证信息的配置。
+使用 git 仓库作为图床，需要用或`login-git`命令进行认证信息的配置。
 
 认证信息需要四个参数：
 
 - `ACCESS_TOKEN` 私密令牌
 - `USERNAME` 用户名
 - `REPO` 仓库名
 - `FOLDER` 想要保存在仓库里的哪个文件夹中，会自动创建不存在的文件夹
@@ -154,16 +154,14 @@
 Options:
 	-aw, --add-watermark  对要上传的图片添加文字水印
 	-ac, --auto-compress  允许自动压缩图片
 	-ic, --ignore-cache   忽略数据库缓存，强制上传图片
 	-h, --help            Show this message and exit.
 ```
 
-
-
 将`up2b upload`命令填到`Typora`里，命令里有个参数`-ac`为可选参数，其作用为开启自动压缩功能，如果不加此参数，上传图片时不会自动压缩，超出图床限制大小就会报错。而添加此参数，则会自动将超限图片压缩到限制图片大小或以下，保证顺利上传。
 
 但自动压缩功能当前没有经过严谨地测试，所以不能保证不出问题，有问题请将异常的截图发在电报群里。
 
 开启自动压缩功能：
 
 ```shell
@@ -197,15 +195,15 @@
 ### 创建虚拟环境
 
 如果你不担心对环境中的其他包产生影响，也不介意自己的 Python 库中多一些可能永远用不到的包，则可以忽略此步。
 
 > 如果你使用的环境管理工具为 pthon 内置的 venv，请自行创建环境，这里不多介绍。
 
 ```bash
-conda create -n up2b-temp python=3.10
+conda create -n up2b-temp python=3.11
 conda activate up2b-temp
 ```
 
 ### 安装依赖
 
 ```bash
 pip install build
@@ -230,15 +228,15 @@
 以下是 v1 版本的初步功能设计。
 
 - [ ] 设计通用配置文件规则
 
   - [ ] 图床类型
     - [ ] git
     - [ ] api
-    - [ ] 非api
+    - [ ] 非 api
 
 - [ ] 图床可用性检测及无效标记
 
   - [ ] 对配置文件中的图床进行可达（超时）检测
   - [ ] 对不可达（超时）的图床添加一个无效标记，并记录检测时间
   - [ ] 用户可设置检测周期，在检测周期内不会检测无效图床以节约时间
   - [ ] 用户可设置删除（软删除）无效图床配置的周期次数，当达到或超过此次数的检测周期后，将在配置文件中将此图床标记为永久失效（软删除）
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: up2b Version: 0.7.1a3 Summary:
+Metadata-Version: 2.1 Name: up2b Version: 0.7.1a4 Summary:
 ä¸ä¼ å¾çå°å¾åº Author-email: thep0y
 163.com> License: MIT License Copyright (c) 2021 thep0y Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
@@ -20,41 +20,42 @@
 Description-Content-Type: text/markdown Provides-Extra: mark License-File:
 LICENSE [English](https://github.com/thep0y/up2b) >
 å½ä»¤è¡ç®¡çå¤ªéº»ç¦ï¼è¯è¯[up2b-gui](https://github.com/thep0y/up2b-
 gui)å§ï¼
                               ****** UP2B ******
                                   [Downloads]
 ä¸ä¸ªè½å¨ç»ç«¯ä¸­å°å¾çä¸ä¼ å°å¾åºçåã æ¯æ LinuxãmacOS å
-Windowsã ## ç¹ç¹ æ¯æä»¥ä¸å¾åºèªå¨ä¸ä¼ : - sm.ms - imgse.com
-(åimgtu.com) - github.com - imgtg.com
-æåä¸ä¼ å°`github`åä¼è¿å`jsdelivr`çCDNé¾æ¥ï¼å å¿«å¨ä¸­å½å¢åå¯¹å¾ççè®¿é®éåº¦ã
-æ¯æjpeg/
-jpgåpngå¾ççèªå¨åç¼©ï¼ä½ä»å¨æµè¯é¶æ®µï¼å¯è½æäºå°é®é¢ï¼å¦æä½ ä¸æ³å¨ä½¿ç¨æ­¤åè½æ¶åºç°éè¯¯æè¾¾ä¸å°é¢æåä¸å»ºè®®ä½¿ç¨ã
+Windowsã ## ç¹ç¹ æ¯æä»¥ä¸å¾åºèªå¨ä¸ä¼ : - sm.ms - imgse.com(å
+imgtu.com) - github.com - imgtg.com
+æåä¸ä¼ å°`github`åä¼è¿å`jsdelivr`ç CDN
+é¾æ¥ï¼å å¿«å¨ä¸­å½å¢åå¯¹å¾ççè®¿é®éåº¦ã æ¯æ jpeg/jpg å
+png
+å¾ççèªå¨åç¼©ï¼ä½ä»å¨æµè¯é¶æ®µï¼å¯è½æäºå°é®é¢ï¼å¦æä½ ä¸æ³å¨ä½¿ç¨æ­¤åè½æ¶åºç°éè¯¯æè¾¾ä¸å°é¢æåä¸å»ºè®®ä½¿ç¨ã
 ## æä¹ç¨ å®è£`up2b`å: ```shell pip install up2b ```
 å®è£åï¼ä¼å¤åºä¸æ¡`up2b`å½ä»¤ï¼ ``` Usage: python -m up2b [OPTIONS]
 COMMAND [ARGS]... Options: -h, --help æ¾ç¤ºæ¬å¸®å©ä¿¡æ¯ -v, --version
 æ¾ç¤ºçæ¬ä¿¡æ¯ Commands: choose éæ©å¾åº config-watermark
 éç½®æå­æ°´å° current æ¾ç¤ºæ­£å¨ä½¿ç¨çå¾åº list
 ååºæ¯æçææå¾åº login ä¿å­å¾åºç»å½ä¿¡æ¯ login-git ä¿å­ git
 ç»å½ä¿¡æ¯ upload ä¸ä¼ å¾ç ``` ### 1 éæ©å¾åº
 ç¬¬ä¸æ¬¡ä½¿ç¨æ¶ï¼å¿é¡»åéæ©å¾åºã
 `up2b`ç`choose`å½ä»¤çå¯éå¼ä¸ºï¼ - 0 - sm.ms - 1 - imgse.com - 2 -
 github.com - 4 - imgtg.com ```bash # å¦æä½ æ³éæ©sm.ms up2b choose 0 ```
 > ä½ å¯è½ä¹æ³¨æå°äºï¼å¾åºç code
 ä¸è¿ç»­ï¼è¿æ¯å ä¸ºæååè¿ä¸ªé¡¹ç®çæ¶åæ²¡æèèå°ä¸äºå¾åºææçå¯è½æ§ï¼å æä¸äºææçå¾åºåï¼ä¸ºäºä½¿éç½®æä»¶ä¸å²çªï¼æä»¥å¾åº
-code æ æ³è¿ç»­ã > > > > å¨ 1.0
+code æ æ³è¿ç»­ã > > å¨ 1.0
 çæ¬ä¸­ï¼å°ä¸ä¼åä½¿ç¨æ°å­ä½ä¸ºå¾åºç
 codeï¼è¿ä¸ªé®é¢å°ä¼è§£å³ï¼åæ¶ä¼å¯ç¨å¨æ°çéç½®æä»¶ï¼ä¸
 0.X.X çæ¬çéç½®æä»¶å°ä¸éç¨ã ### 2 ä¿å­è®¤è¯ä¿¡æ¯ ####
-**æ®éå¾åºï¼**
-gitä»åºæ¬èº«å¹¶ä¸ç®æ¯å¾åºï¼æä»¥gitä»åºä¹å¤çå¾åºé½æ¯æ®éå¾åºã
+**æ®éå¾åºï¼** git ä»åºæ¬èº«å¹¶ä¸ç®æ¯å¾åºï¼æä»¥ git
+ä»åºä¹å¤çå¾åºé½æ¯æ®éå¾åºã
 ä½¿ç¨æ®éå¾åºæ¶ï¼ç¨`login`å½ä»¤è¿è¡è®¤è¯ä¿¡æ¯çéç½®ï¼å¦ï¼
-```shell up2b login username password ``` #### **gitä»åºï¼**
-æ­¤åææçgitä»åºåæ¬`github`ã
-ä½¿ç¨gitä»åºä½ä¸ºå¾åºï¼éè¦ç¨æ`login-
+```shell up2b login username password ``` #### **git ä»åºï¼**
+æ­¤åææç git ä»åºåæ¬`github`ã ä½¿ç¨ git
+ä»åºä½ä¸ºå¾åºï¼éè¦ç¨æ`login-
 git`å½ä»¤è¿è¡è®¤è¯ä¿¡æ¯çéç½®ã è®¤è¯ä¿¡æ¯éè¦åä¸ªåæ°ï¼ -
 `ACCESS_TOKEN` ç§å¯ä»¤ç - `USERNAME` ç¨æ·å - `REPO` ä»åºå -
 `FOLDER`
 æ³è¦ä¿å­å¨ä»åºéçåªä¸ªæä»¶å¤¹ä¸­ï¼ä¼èªå¨åå»ºä¸å­å¨çæä»¶å¤¹
 æ¯å¦ï¼ææ³å°å¾çä¿å­å¨`image-
 bed`ä»åºéç`md`æä»¶å¤¹åï¼è¾å¥æ­¤å½ä»¤ï¼ ```shell up2b login-git
 access_token username image-bed md ``` ### 3 (å¯é) å¨ typora
@@ -74,22 +75,22 @@
 /s2.loli.net/2023/03/04/wNqgOpn4Tz5ZUHQ.png) ## èªè¡æå
 å¦ææ­¤é¡¹ç®ä¸­æ´æ°äºæäºç¹æ§å¯¹ä½ æ¥è¯´å¾æç¨ï¼ä½å°æªåå¸æ°ç
 releaseï¼é£ä¹ä½ å¯ä»¥èªè¡æåå®è£ã ### åå»ºèæç¯å¢
 å¦æä½ ä¸æå¿å¯¹ç¯å¢ä¸­çå¶ä»åäº§çå½±åï¼ä¹ä¸ä»æèªå·±ç
 Python åºä¸­å¤ä¸äºå¯è½æ°¸è¿ç¨ä¸å°çåï¼åå¯ä»¥å¿½ç¥æ­¤æ­¥ã >
 å¦æä½ ä½¿ç¨çç¯å¢ç®¡çå·¥å·ä¸º pthon åç½®ç
 venvï¼è¯·èªè¡åå»ºç¯å¢ï¼è¿éä¸å¤ä»ç»ã ```bash conda create -
-n up2b-temp python=3.10 conda activate up2b-temp ``` ### å®è£ä¾èµ ```bash
+n up2b-temp python=3.11 conda activate up2b-temp ``` ### å®è£ä¾èµ ```bash
 pip install build ``` ### æå ```bash python -m build ```
 ä¼å¨é¡¹ç®çæ ¹ç®å½åå»º`dist`ç®å½ï¼éé¢å°±ææåå¥½ç`whl`æä»¶ï¼å®è£å³å¯ï¼
 ``` pip install -U dist/up2b-*-py3-none-any.whl ``` ## TODO
 é´äºå¾åºç½ç«åçéåº¦è¶ä¹æ³è±¡ï¼æä»¥å¨ä¸ä¸ªå¤§çæ¬ä¸­æä¸æç®åå¯¹ä»»ä½å¾åºè¿è¡æ¯æï¼èæ¯ä½¿ç¨éç½®æä»¶çæ¹å¼ç±ç¨æ·èªè¡æ·»å å¾åºï¼å¹¶æ·»å æ£æµå¾åºå¯ç¨æ§çåè½ã
 ä»¥ä¸æ¯ v1 çæ¬çåæ­¥åè½è®¾è®¡ã - [ ]
-è®¾è®¡éç¨éç½®æä»¶è§å - [ ] å¾åºç±»å - [ ] git - [ ] api - [ ]
-éapi - [ ] å¾åºå¯ç¨æ§æ£æµåæ ææ è®° - [ ]
+è®¾è®¡éç¨éç½®æä»¶è§å - [ ] å¾åºç±»å - [ ] git - [ ] api - [ ] é
+api - [ ] å¾åºå¯ç¨æ§æ£æµåæ ææ è®° - [ ]
 å¯¹éç½®æä»¶ä¸­çå¾åºè¿è¡å¯è¾¾ï¼è¶æ¶ï¼æ£æµ - [ ]
 å¯¹ä¸å¯è¾¾ï¼è¶æ¶ï¼çå¾åºæ·»å ä¸ä¸ªæ ææ è®°ï¼å¹¶è®°å½æ£æµæ¶é´
 - [ ]
 ç¨æ·å¯è®¾ç½®æ£æµå¨æï¼å¨æ£æµå¨æåä¸ä¼æ£æµæ æå¾åºä»¥èçº¦æ¶é´
 - [ ]
 ç¨æ·å¯è®¾ç½®å é¤ï¼è½¯å é¤ï¼æ æå¾åºéç½®çå¨ææ¬¡æ°ï¼å½è¾¾å°æè¶è¿æ­¤æ¬¡æ°çæ£æµå¨æåï¼å°å¨éç½®æä»¶ä¸­å°æ­¤å¾åºæ è®°ä¸ºæ°¸ä¹å¤±æï¼è½¯å é¤ï¼
 - [ ] ç¨æ·å¯å¨éç½®æä»¶ä¸­å é¤æ ææ è®° - [ ] æ¬å°ç½é¡µéç½®
```

### Comparing `up2b-0.7.1a3/up2b.egg-info/SOURCES.txt` & `up2b-0.7.1a4/up2b.egg-info/SOURCES.txt`

 * *Files identical despite different names*

