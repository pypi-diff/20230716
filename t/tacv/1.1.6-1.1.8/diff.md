# Comparing `tmp/tacv-1.1.6.tar.gz` & `tmp/tacv-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tacv-1.1.6.tar", last modified: Fri Jun  2 03:26:12 2023, max compression
+gzip compressed data, was "tacv-1.1.8.tar", last modified: Sun Jul 16 10:25:09 2023, max compression
```

## Comparing `tacv-1.1.6.tar` & `tacv-1.1.8.tar`

### file list

```diff
@@ -1,60 +1,62 @@
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.551066 tacv-1.1.6/
--rw-rw-r--   0 tu        (1000) tu        (1000)     1065 2022-07-26 16:30:33.000000 tacv-1.1.6/LICENSE
--rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2023-06-02 03:26:12.551066 tacv-1.1.6/PKG-INFO
--rw-rw-r--   0 tu        (1000) tu        (1000)     6908 2022-07-29 02:23:53.000000 tacv-1.1.6/README.md
--rw-rw-r--   0 tu        (1000) tu        (1000)      105 2022-07-26 16:30:33.000000 tacv-1.1.6/pyproject.toml
--rw-rw-r--   0 tu        (1000) tu        (1000)       32 2022-07-26 16:30:33.000000 tacv-1.1.6/requirements.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)      200 2023-06-02 03:26:12.551066 tacv-1.1.6/setup.cfg
--rw-rw-r--   0 tu        (1000) tu        (1000)     1838 2023-06-02 03:25:44.000000 tacv-1.1.6/setup.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/cli/
--rw-rw-r--   0 tu        (1000) tu        (1000)       63 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/cli/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      206 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/cli/cli.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/
--rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-28 14:56:31.000000 tacv-1.1.6/tacv/detection/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/
--rw-rw-r--   0 tu        (1000) tu        (1000)     9698 2022-07-29 02:23:53.000000 tacv-1.1.6/tacv/detection/centernet/CenterNet.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     4429 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/Trainer.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      130 2022-07-28 14:56:31.000000 tacv-1.1.6/tacv/detection/centernet/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/backbones/
--rw-rw-r--   0 tu        (1000) tu        (1000)      100 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/backbones/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)    10067 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/backbones/resnet.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/heads/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/heads/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/losses/
--rw-rw-r--   0 tu        (1000) tu        (1000)       35 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/losses/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1363 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/losses/losses.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/detection/centernet/utils/
--rw-rw-r--   0 tu        (1000) tu        (1000)       90 2022-07-28 14:56:31.000000 tacv-1.1.6/tacv/detection/centernet/utils/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      261 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/common.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2448 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/data_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     3031 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/geometry_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2345 2022-07-29 02:21:21.000000 tacv-1.1.6/tacv/detection/centernet/utils/infer.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      189 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/lightning_utils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.6/tacv/detection/centernet/utils/pytorch_model_utils.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/fileUtils/
--rw-rw-r--   0 tu        (1000) tu        (1000)       72 2023-04-21 02:49:52.000000 tacv-1.1.6/tacv/fileUtils/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1577 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/fileUtils/fileutils.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     5573 2023-06-02 03:21:52.000000 tacv-1.1.6/tacv/fileUtils/thread_downloader.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/geometry/
--rw-rw-r--   0 tu        (1000) tu        (1000)       18 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/geometry/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      782 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/geometry/iou.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv/resources/
--rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/resources/__init__.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.551066 tacv-1.1.6/tacv/torch/
--rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/torch/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     1046 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/torch/model_utils.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.551066 tacv-1.1.6/tacv/video/
--rw-rw-r--   0 tu        (1000) tu        (1000)       25 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/video/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)     2710 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/video/video_proc.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.551066 tacv-1.1.6/tacv/visual/
--rw-rw-r--   0 tu        (1000) tu        (1000)       21 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/visual/__init__.py
--rw-rw-r--   0 tu        (1000) tu        (1000)      558 2022-07-26 16:30:33.000000 tacv-1.1.6/tacv/visual/draw2d.py
-drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-06-02 03:26:12.547066 tacv-1.1.6/tacv.egg-info/
--rw-rw-r--   0 tu        (1000) tu        (1000)     7323 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/PKG-INFO
--rw-rw-r--   0 tu        (1000) tu        (1000)     1281 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/SOURCES.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)        1 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/dependency_links.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)       92 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/entry_points.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)       33 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/requires.txt
--rw-rw-r--   0 tu        (1000) tu        (1000)        5 2023-06-02 03:26:12.000000 tacv-1.1.6/tacv.egg-info/top_level.txt
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1065 2022-07-26 16:30:33.000000 tacv-1.1.8/LICENSE
+-rw-rw-r--   0 tu        (1000) tu        (1000)     9642 2023-07-16 10:25:09.437906 tacv-1.1.8/PKG-INFO
+-rw-rw-r--   0 tu        (1000) tu        (1000)     9226 2023-07-16 10:24:20.000000 tacv-1.1.8/README.md
+-rw-rw-r--   0 tu        (1000) tu        (1000)      105 2022-07-26 16:30:33.000000 tacv-1.1.8/pyproject.toml
+-rw-rw-r--   0 tu        (1000) tu        (1000)       39 2023-07-16 09:24:56.000000 tacv-1.1.8/requirements.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)      200 2023-07-16 10:25:09.437906 tacv-1.1.8/setup.cfg
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1839 2023-07-16 09:17:53.000000 tacv-1.1.8/setup.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.433905 tacv-1.1.8/tacv/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.433905 tacv-1.1.8/tacv/cli/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       63 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/cli/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      206 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/cli/cli.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.433905 tacv-1.1.8/tacv/detection/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       26 2022-07-28 14:56:31.000000 tacv-1.1.8/tacv/detection/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/detection/centernet/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     9698 2022-07-29 02:23:53.000000 tacv-1.1.8/tacv/detection/centernet/CenterNet.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     4429 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/Trainer.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      130 2022-07-28 14:56:31.000000 tacv-1.1.8/tacv/detection/centernet/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/detection/centernet/backbones/
+-rw-rw-r--   0 tu        (1000) tu        (1000)      100 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/backbones/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)    10067 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/backbones/resnet.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/detection/centernet/heads/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/heads/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/detection/centernet/losses/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       35 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/losses/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1363 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/losses/losses.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/detection/centernet/utils/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       90 2022-07-28 14:56:31.000000 tacv-1.1.8/tacv/detection/centernet/utils/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      261 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/utils/common.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2448 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/utils/data_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     3031 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/utils/geometry_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2345 2022-07-29 02:21:21.000000 tacv-1.1.8/tacv/detection/centernet/utils/infer.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      189 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/utils/lightning_utils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-28 10:48:47.000000 tacv-1.1.8/tacv/detection/centernet/utils/pytorch_model_utils.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/fileUtils/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       72 2023-04-21 02:49:52.000000 tacv-1.1.8/tacv/fileUtils/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1577 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/fileUtils/fileutils.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     5573 2023-06-02 03:21:52.000000 tacv-1.1.8/tacv/fileUtils/thread_downloader.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/geometry/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       18 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/geometry/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      782 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/geometry/iou.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/resources/
+-rw-rw-r--   0 tu        (1000) tu        (1000)        0 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/resources/__init__.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/torch/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       56 2023-07-16 10:13:47.000000 tacv-1.1.8/tacv/torch/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     8040 2023-07-16 09:58:44.000000 tacv-1.1.8/tacv/torch/example_lora.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     5408 2023-07-16 09:24:56.000000 tacv-1.1.8/tacv/torch/lora_any.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1046 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/torch/model_utils.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/video/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       25 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/video/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)     2710 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/video/video_proc.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.437906 tacv-1.1.8/tacv/visual/
+-rw-rw-r--   0 tu        (1000) tu        (1000)       21 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/visual/__init__.py
+-rw-rw-r--   0 tu        (1000) tu        (1000)      558 2022-07-26 16:30:33.000000 tacv-1.1.8/tacv/visual/draw2d.py
+drwxrwxr-x   0 tu        (1000) tu        (1000)        0 2023-07-16 10:25:09.433905 tacv-1.1.8/tacv.egg-info/
+-rw-rw-r--   0 tu        (1000) tu        (1000)     9642 2023-07-16 10:25:09.000000 tacv-1.1.8/tacv.egg-info/PKG-INFO
+-rw-rw-r--   0 tu        (1000) tu        (1000)     1331 2023-07-16 10:25:09.000000 tacv-1.1.8/tacv.egg-info/SOURCES.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)        1 2023-07-16 10:25:09.000000 tacv-1.1.8/tacv.egg-info/dependency_links.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)       92 2023-07-16 10:25:09.000000 tacv-1.1.8/tacv.egg-info/entry_points.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)       40 2023-07-16 10:25:09.000000 tacv-1.1.8/tacv.egg-info/requires.txt
+-rw-rw-r--   0 tu        (1000) tu        (1000)        5 2023-07-16 10:25:09.000000 tacv-1.1.8/tacv.egg-info/top_level.txt
```

### Comparing `tacv-1.1.6/LICENSE` & `tacv-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/PKG-INFO` & `tacv-1.1.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,92 @@
 Metadata-Version: 2.1
 Name: tacv
-Version: 1.1.6
+Version: 1.1.8
 Summary: A mini package for daily tasks
 Home-page: https://github.com/TaQuangTu/TaCV
-Author: TaQuangTu
+Author: QuangTu-Ta
 Author-email: taquangtu132@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# TACV - A mini package for daily tasks
+from tacv.fileUtils import ThreadedDownload# TACV - A mini package for daily tasks
 
 ## Installation
+
 ```bash
 pip install tacv
 ```
 
+Some specific functions depend on other libraries (.e.g `mlflow`, `torch`, `pytorch-lightning`). Be forgiving and install the necessary libraries if required.
+
 ## Examples
 
 <details>
+<summary> <b>LoRA training</b></summary>
+
+Adding LoRA to your model and start training as usual with minimal code changes.
+
+1. Define a boilerplate class that inherit both AnyLoRA and the model you want to play, in this case GPTNeoForCausalLM
+
+```python
+from tacv.torch import AnyLoRA
+from transformers import GPTNeoForCausalLM
+
+
+class GPTNeoLoRA(GPTNeoForCausalLM, AnyLoRA):
+    def __init__(self, config):
+        GPTNeoForCausalLM.__init__(self, config)
+```
+
+2. Add LoRA to layers that you think it could bring the training benefit, here we choose the Key and Value matrices in
+   all self-attention blocks
+
+```python
+# init your LoRA model
+model = GPTNeoLoRA.from_pretrained("EleutherAI/gpt-neo-1.3B", low_cpu_mem_usage=True)
+
+model.init_lora(rank=8, layers_contain=["k_proj", "v_proj"])
+
+# Also give "layers_end_with" and "layers_start_with" a try
+model.init_lora(rank=4, layers_end_with="q_proj", layers_start_with="wte")
+
+# drop grad of all other layers before training
+model.mark_only_lora_as_trainable(bias="none")
+```
+
+3. The rest of training is as usual, just as you have done before using AnyLoRA.
+4. Save and load LoRA weights.
+
+```python
+# save LoRA
+model.save_lora("lora.pth")
+# load LoRA for inference
+model.load_lora("lora.pth")
+```
+
+Want more control over the training and mode behavior, visit my example of fine-tuning a GPT-Neo model for Vietnamese
+at `tacv/torch/example_lora.py`
+
+
+</details>
+
+
+<details>
 <summary> <b>2D Object Detection</b></summary>
 
 For now, CenterNet is supported. However, use it as prototype purpose only, there is no official benchmark on accuracy.
 
 #### Train with your own dataset
 
 * First, create a config file for training/model config, see full config at `tacv/detection/sample_config.yml`.
+
 ```yaml
 input_size: &input_size [ 224,448 ]
 max_object: &max_obj 16
 num_classes: &num_classes 5
 train_config:
   gpus: 0 # 0 means CPU, N means using N available GPU(s) for training
   epoch: 600
@@ -59,51 +113,60 @@
 model:
   num_classes: *num_classes
   backbone_layers: 18
   head_conv_channel: 64
   max_object: *max_obj
   input_shape: *input_size
 ```
-* Second, create your own Dataset class that returns data as described in the `__getitem__()` method, see following example:
+
+* Second, create your own Dataset class that returns data as described in the `__getitem__()` method, see following
+  example:
+
 ```python
 from torch.utils.data import Dataset
 import torch
 
+
 class MockDataset(Dataset):
     def __init__(self, max_objs, input_shape_HW):
         self.max_objs = max_objs
         self.input_shape_HW = input_shape_HW
+
     def __getitem__(self, item):
         # read your image
         # image = cv2.imread(your image path)
         # do any transform operation, then return a tensor
-        image = torch.rand(3, self.input_shape_HW[0],self.input_shape_HW[1])  # Shape = (3, InputShape, W)
-        annos = torch.rand(self.max_objs, 5)  # Shape = (MaxObjs x 5) , each row presents for (x,y,w,h,class_id) relative to input shape
+        image = torch.rand(3, self.input_shape_HW[0], self.input_shape_HW[1])  # Shape = (3, InputShape, W)
+        annos = torch.rand(self.max_objs,
+                           5)  # Shape = (MaxObjs x 5) , each row presents for (x,y,w,h,class_id) relative to input shape
         masks = torch.zeros(
             self.max_objs)  # Shape = (MaxObjs,)  each value is False or True (1 indicates having object)
         masks[0:3] = True
         return {"image": image, "annos": annos, "masks": masks}
 
     def __len__(self):
         return 1000
 ```
+
 * Init `CenterNetTrainer` and here we go
+
 ```python
 from tacv.detection import CenterNetTrainer
 from torch.utils.data import random_split
 
 config_path = "tacv/detection/sample_config.yml"
-max_objs = 16 # read from config file
-input_shape = (224,448) # read from config file
-dataset = MockDataset(max_objs=max_objs,input_shape_HW = input_shape)  # Replace with your custom dataset
+max_objs = 16  # read from config file
+input_shape = (224, 448)  # read from config file
+dataset = MockDataset(max_objs=max_objs, input_shape_HW=input_shape)  # Replace with your custom dataset
 train_set, val_set = random_split(dataset, [900, 100])
 
 trainer = CenterNetTrainer(train_set, val_set, config_path)
 trainer.train()
 ```
+
 #### Inference on single image
 
 ```python
 import cv2
 import torch
 from tacv.detection import load_centernet_model_with_config
 from tacv.detection import infer
@@ -115,107 +178,158 @@
     model = load_centernet_model_with_config(config_path, load_bbone_pretrained=False)
     model.load_state_dict("your_checkpoint.pth")
     model.eval()
     model.to(device)
 
     image = cv2.imread("your_image.png")
     bboxes = infer(model, image, device)
-    print(bboxes) # list of detections in format (xc,yc,w,h,class_id,confidence_score)
+    print(bboxes)  # list of detections in format (xc,yc,w,h,class_id,confidence_score)
 ```
 
 </details>
 
 <details>
 <summary> <b>File utils</b></summary>
 
 ### File utils
+
 #### Get all file paths from a directory
+
 ```python
 from tacv.fileUtils import get_all_files
+
 file_paths = get_all_files("dir_name")
 ```
+
 Returns a list of file absolute paths, for example
+
 ```
 ['./venvCondaTest/x86_64-conda_cos6-linux-gnu/bin/ld', './venvCondaTest/conda-meta/_libgcc_mutex-0.1-main.json', './venvCondaTest/conda-meta/xz-5.2.5-h7b6447c_0.json', './venvCondaTest/conda-meta/wheel-0.37.1-pyhd3eb1b0_0.json', './venvCondaTest/conda-meta/setuptools-58.0.4-py36h06a4308_0.json', './venvCondaTest/conda-meta/ca-certificates-2021.10.26-h06a4308_2.json', './venvCondaTest/conda-meta/readline-8.1.2-h7f8727e_1.json', './venvCondaTest/conda-meta/sqlite-3.37.2-hc218d9a_0.json', './venvCondaTest/conda-meta/libgcc-ng-9.3.0-h5101ec6_17.json', './venvCondaTest/conda-meta/ncurses-6.3-h7f8727e_2.json']
 ```
+
 #### Save/load json data to/from file
+
 ```python
-from tacv.fileUtils import save_json,load_json
+from tacv.fileUtils import save_json, load_json
 
 json_file = "myfile.json"
-json_data = {"name":"Ta","age":100}
+json_data = {"name": "Ta", "age": 100}
 # save json
-save_json(json_file,json_data)
+save_json(json_file, json_data)
 # load json
 json_data = load_json(json_file)
 ```
+
+#### Multi-threaded file downloader
+
+```python
+from tacv.fileUtils import ThreadedDownload
+
+urls = [
+    'http://localhost:11223/210207000111980_3_124202.jpg',
+    'http://localhost:11223/210430000373373_3_407200.jpg',
+    'http://localhost:11223/210426000324979_3_356188.jpg',
+    'http://localhost:11223/200819000060994_3_78314.png'
+]
+downloader = ThreadedDownload(urls, "/home/tu/Desktop/LabelStudio", False, thread_count=3, url_tries=3)
+
+print(f'Downloading {len(urls)} files')
+downloader.run()
+print(f'Downloaded {len(downloader.report["success"])} of {len(urls)}')
+```
+
 </details>
 
 <details>
 <summary> <b>CV2 Visualization</b></summary>
 
 #### Draw 2D points onto an image
+
 ```python
 import cv2
 from tacv.visual import draw_points
+
 image = cv2.imread("myimage.jpg")
-points = [(18,19),(55,55),(102,22),(66,22)]
-draw_points(image,points,circular=True,color=(0,255,0),thickness=2)
-cv2.imwrite("new_image.jpg",image)
+points = [(18, 19), (55, 55), (102, 22), (66, 22)]
+draw_points(image, points, circular=True, color=(0, 255, 0), thickness=2)
+cv2.imwrite("new_image.jpg", image)
 ```
+
 </details>
 
 <details>
 <summary> <b>Video and image utils</b></summary>
 
 #### Synthesize a video from images
+
 ```python
 from tacv.video import images2video
-image_dir = "my_images" #directory containing images in the same format
-video_path = "tacv_test.mp4" #path to save the synthesized video
+
+image_dir = "my_images"  # directory containing images in the same format
+video_path = "tacv_test.mp4"  # path to save the synthesized video
 # common use case
-images2video(image_dir,video_path,fps=24, image_ext = None, sort=False)
+images2video(image_dir, video_path, fps=24, image_ext=None, sort=False)
 ```
+
 Parameters:
+
 * `fps`: default = 24
-* `image_ext`: a string, specify image extension to synthesize the video, for example (`jpg`, `png`,...). If it is `None`. All images will be grabbed. Default is `None`.
-* `sort`: `True` or `False`. Indicate if the images should be sorted by name before synthesizing the video. Default is `True`.
+* `image_ext`: a string, specify image extension to synthesize the video, for example (`jpg`, `png`,...). If it
+  is `None`. All images will be grabbed. Default is `None`.
+* `sort`: `True` or `False`. Indicate if the images should be sorted by name before synthesizing the video. Default
+  is `True`.
+
 #### Extract images from a video
+
 ```python
 from tacv.video import video2images
-video_path = "tacv_test.mp4" #path to video to be extracted to images
-image_dir = "my_images" #directory to save the extracted images
-video2images(video_path,image_dir,exist_ok=False, image_ext="jpg", verbose=True)
+
+video_path = "tacv_test.mp4"  # path to video to be extracted to images
+image_dir = "my_images"  # directory to save the extracted images
+video2images(video_path, image_dir, exist_ok=False, image_ext="jpg", verbose=True)
 ```
+
 Parameters:
-* `exist_ok`: default is False. If `image_dir` already contains images and this flag is `False`. The process will be cancel, otherwise it continues.
-* `image_ext`: a string, specify image extension, for example (`jpg`, `png`,...). If it is `None`. All images will be grabbed. Default is `None`.
+
+* `exist_ok`: default is False. If `image_dir` already contains images and this flag is `False`. The process will be
+  cancel, otherwise it continues.
+* `image_ext`: a string, specify image extension, for example (`jpg`, `png`,...). If it is `None`. All images will be
+  grabbed. Default is `None`.
 * `verbose`: `True` or `False`. Set it to `True` to view the extracting process. Default is `True`.
+
 </details>
 
 <details>
 <summary> <b>Geometry utils</b></summary>
 
 #### Calculate 2D IOU of two polygons
+
 ```python
 from tacv.geometry import iou_2d
-polygon_1 = [[0,0],[10,10],[0,10]]
+
+polygon_1 = [[0, 0], [10, 10], [0, 10]]
 polygon_2 = [[0, 20], [10, 10], [0, 0]]
-print(iou_2d(polygon_1,polygon_2))
+print(iou_2d(polygon_1, polygon_2))
 ```
+
 </details>
 <details>
 <summary> <b>Command Line Interface</b></summary>
 
 #### Synthesize a video from images
+
 ```bash
 tacv_i2v image_dir video_path [optional: fps image_ext]
 ```
+
 #### Extract images from a video
+
 ```bash
 tacv_v2i video_path image_dir
 ```
+
 </details>
 
 ### For more
-* Visit args description in source code 
+
+* Visit args description in source code
 * Visit `test.py` file
```

### Comparing `tacv-1.1.6/README.md` & `tacv-1.1.8/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,78 @@
-# TACV - A mini package for daily tasks
+from tacv.fileUtils import ThreadedDownload# TACV - A mini package for daily tasks
 
 ## Installation
+
 ```bash
 pip install tacv
 ```
 
+Some specific functions depend on other libraries (.e.g `mlflow`, `torch`, `pytorch-lightning`). Be forgiving and install the necessary libraries if required.
+
 ## Examples
 
 <details>
+<summary> <b>LoRA training</b></summary>
+
+Adding LoRA to your model and start training as usual with minimal code changes.
+
+1. Define a boilerplate class that inherit both AnyLoRA and the model you want to play, in this case GPTNeoForCausalLM
+
+```python
+from tacv.torch import AnyLoRA
+from transformers import GPTNeoForCausalLM
+
+
+class GPTNeoLoRA(GPTNeoForCausalLM, AnyLoRA):
+    def __init__(self, config):
+        GPTNeoForCausalLM.__init__(self, config)
+```
+
+2. Add LoRA to layers that you think it could bring the training benefit, here we choose the Key and Value matrices in
+   all self-attention blocks
+
+```python
+# init your LoRA model
+model = GPTNeoLoRA.from_pretrained("EleutherAI/gpt-neo-1.3B", low_cpu_mem_usage=True)
+
+model.init_lora(rank=8, layers_contain=["k_proj", "v_proj"])
+
+# Also give "layers_end_with" and "layers_start_with" a try
+model.init_lora(rank=4, layers_end_with="q_proj", layers_start_with="wte")
+
+# drop grad of all other layers before training
+model.mark_only_lora_as_trainable(bias="none")
+```
+
+3. The rest of training is as usual, just as you have done before using AnyLoRA.
+4. Save and load LoRA weights.
+
+```python
+# save LoRA
+model.save_lora("lora.pth")
+# load LoRA for inference
+model.load_lora("lora.pth")
+```
+
+Want more control over the training and mode behavior, visit my example of fine-tuning a GPT-Neo model for Vietnamese
+at `tacv/torch/example_lora.py`
+
+
+</details>
+
+
+<details>
 <summary> <b>2D Object Detection</b></summary>
 
 For now, CenterNet is supported. However, use it as prototype purpose only, there is no official benchmark on accuracy.
 
 #### Train with your own dataset
 
 * First, create a config file for training/model config, see full config at `tacv/detection/sample_config.yml`.
+
 ```yaml
 input_size: &input_size [ 224,448 ]
 max_object: &max_obj 16
 num_classes: &num_classes 5
 train_config:
   gpus: 0 # 0 means CPU, N means using N available GPU(s) for training
   epoch: 600
@@ -45,51 +99,60 @@
 model:
   num_classes: *num_classes
   backbone_layers: 18
   head_conv_channel: 64
   max_object: *max_obj
   input_shape: *input_size
 ```
-* Second, create your own Dataset class that returns data as described in the `__getitem__()` method, see following example:
+
+* Second, create your own Dataset class that returns data as described in the `__getitem__()` method, see following
+  example:
+
 ```python
 from torch.utils.data import Dataset
 import torch
 
+
 class MockDataset(Dataset):
     def __init__(self, max_objs, input_shape_HW):
         self.max_objs = max_objs
         self.input_shape_HW = input_shape_HW
+
     def __getitem__(self, item):
         # read your image
         # image = cv2.imread(your image path)
         # do any transform operation, then return a tensor
-        image = torch.rand(3, self.input_shape_HW[0],self.input_shape_HW[1])  # Shape = (3, InputShape, W)
-        annos = torch.rand(self.max_objs, 5)  # Shape = (MaxObjs x 5) , each row presents for (x,y,w,h,class_id) relative to input shape
+        image = torch.rand(3, self.input_shape_HW[0], self.input_shape_HW[1])  # Shape = (3, InputShape, W)
+        annos = torch.rand(self.max_objs,
+                           5)  # Shape = (MaxObjs x 5) , each row presents for (x,y,w,h,class_id) relative to input shape
         masks = torch.zeros(
             self.max_objs)  # Shape = (MaxObjs,)  each value is False or True (1 indicates having object)
         masks[0:3] = True
         return {"image": image, "annos": annos, "masks": masks}
 
     def __len__(self):
         return 1000
 ```
+
 * Init `CenterNetTrainer` and here we go
+
 ```python
 from tacv.detection import CenterNetTrainer
 from torch.utils.data import random_split
 
 config_path = "tacv/detection/sample_config.yml"
-max_objs = 16 # read from config file
-input_shape = (224,448) # read from config file
-dataset = MockDataset(max_objs=max_objs,input_shape_HW = input_shape)  # Replace with your custom dataset
+max_objs = 16  # read from config file
+input_shape = (224, 448)  # read from config file
+dataset = MockDataset(max_objs=max_objs, input_shape_HW=input_shape)  # Replace with your custom dataset
 train_set, val_set = random_split(dataset, [900, 100])
 
 trainer = CenterNetTrainer(train_set, val_set, config_path)
 trainer.train()
 ```
+
 #### Inference on single image
 
 ```python
 import cv2
 import torch
 from tacv.detection import load_centernet_model_with_config
 from tacv.detection import infer
@@ -101,107 +164,158 @@
     model = load_centernet_model_with_config(config_path, load_bbone_pretrained=False)
     model.load_state_dict("your_checkpoint.pth")
     model.eval()
     model.to(device)
 
     image = cv2.imread("your_image.png")
     bboxes = infer(model, image, device)
-    print(bboxes) # list of detections in format (xc,yc,w,h,class_id,confidence_score)
+    print(bboxes)  # list of detections in format (xc,yc,w,h,class_id,confidence_score)
 ```
 
 </details>
 
 <details>
 <summary> <b>File utils</b></summary>
 
 ### File utils
+
 #### Get all file paths from a directory
+
 ```python
 from tacv.fileUtils import get_all_files
+
 file_paths = get_all_files("dir_name")
 ```
+
 Returns a list of file absolute paths, for example
+
 ```
 ['./venvCondaTest/x86_64-conda_cos6-linux-gnu/bin/ld', './venvCondaTest/conda-meta/_libgcc_mutex-0.1-main.json', './venvCondaTest/conda-meta/xz-5.2.5-h7b6447c_0.json', './venvCondaTest/conda-meta/wheel-0.37.1-pyhd3eb1b0_0.json', './venvCondaTest/conda-meta/setuptools-58.0.4-py36h06a4308_0.json', './venvCondaTest/conda-meta/ca-certificates-2021.10.26-h06a4308_2.json', './venvCondaTest/conda-meta/readline-8.1.2-h7f8727e_1.json', './venvCondaTest/conda-meta/sqlite-3.37.2-hc218d9a_0.json', './venvCondaTest/conda-meta/libgcc-ng-9.3.0-h5101ec6_17.json', './venvCondaTest/conda-meta/ncurses-6.3-h7f8727e_2.json']
 ```
+
 #### Save/load json data to/from file
+
 ```python
-from tacv.fileUtils import save_json,load_json
+from tacv.fileUtils import save_json, load_json
 
 json_file = "myfile.json"
-json_data = {"name":"Ta","age":100}
+json_data = {"name": "Ta", "age": 100}
 # save json
-save_json(json_file,json_data)
+save_json(json_file, json_data)
 # load json
 json_data = load_json(json_file)
 ```
+
+#### Multi-threaded file downloader
+
+```python
+from tacv.fileUtils import ThreadedDownload
+
+urls = [
+    'http://localhost:11223/210207000111980_3_124202.jpg',
+    'http://localhost:11223/210430000373373_3_407200.jpg',
+    'http://localhost:11223/210426000324979_3_356188.jpg',
+    'http://localhost:11223/200819000060994_3_78314.png'
+]
+downloader = ThreadedDownload(urls, "/home/tu/Desktop/LabelStudio", False, thread_count=3, url_tries=3)
+
+print(f'Downloading {len(urls)} files')
+downloader.run()
+print(f'Downloaded {len(downloader.report["success"])} of {len(urls)}')
+```
+
 </details>
 
 <details>
 <summary> <b>CV2 Visualization</b></summary>
 
 #### Draw 2D points onto an image
+
 ```python
 import cv2
 from tacv.visual import draw_points
+
 image = cv2.imread("myimage.jpg")
-points = [(18,19),(55,55),(102,22),(66,22)]
-draw_points(image,points,circular=True,color=(0,255,0),thickness=2)
-cv2.imwrite("new_image.jpg",image)
+points = [(18, 19), (55, 55), (102, 22), (66, 22)]
+draw_points(image, points, circular=True, color=(0, 255, 0), thickness=2)
+cv2.imwrite("new_image.jpg", image)
 ```
+
 </details>
 
 <details>
 <summary> <b>Video and image utils</b></summary>
 
 #### Synthesize a video from images
+
 ```python
 from tacv.video import images2video
-image_dir = "my_images" #directory containing images in the same format
-video_path = "tacv_test.mp4" #path to save the synthesized video
+
+image_dir = "my_images"  # directory containing images in the same format
+video_path = "tacv_test.mp4"  # path to save the synthesized video
 # common use case
-images2video(image_dir,video_path,fps=24, image_ext = None, sort=False)
+images2video(image_dir, video_path, fps=24, image_ext=None, sort=False)
 ```
+
 Parameters:
+
 * `fps`: default = 24
-* `image_ext`: a string, specify image extension to synthesize the video, for example (`jpg`, `png`,...). If it is `None`. All images will be grabbed. Default is `None`.
-* `sort`: `True` or `False`. Indicate if the images should be sorted by name before synthesizing the video. Default is `True`.
+* `image_ext`: a string, specify image extension to synthesize the video, for example (`jpg`, `png`,...). If it
+  is `None`. All images will be grabbed. Default is `None`.
+* `sort`: `True` or `False`. Indicate if the images should be sorted by name before synthesizing the video. Default
+  is `True`.
+
 #### Extract images from a video
+
 ```python
 from tacv.video import video2images
-video_path = "tacv_test.mp4" #path to video to be extracted to images
-image_dir = "my_images" #directory to save the extracted images
-video2images(video_path,image_dir,exist_ok=False, image_ext="jpg", verbose=True)
+
+video_path = "tacv_test.mp4"  # path to video to be extracted to images
+image_dir = "my_images"  # directory to save the extracted images
+video2images(video_path, image_dir, exist_ok=False, image_ext="jpg", verbose=True)
 ```
+
 Parameters:
-* `exist_ok`: default is False. If `image_dir` already contains images and this flag is `False`. The process will be cancel, otherwise it continues.
-* `image_ext`: a string, specify image extension, for example (`jpg`, `png`,...). If it is `None`. All images will be grabbed. Default is `None`.
+
+* `exist_ok`: default is False. If `image_dir` already contains images and this flag is `False`. The process will be
+  cancel, otherwise it continues.
+* `image_ext`: a string, specify image extension, for example (`jpg`, `png`,...). If it is `None`. All images will be
+  grabbed. Default is `None`.
 * `verbose`: `True` or `False`. Set it to `True` to view the extracting process. Default is `True`.
+
 </details>
 
 <details>
 <summary> <b>Geometry utils</b></summary>
 
 #### Calculate 2D IOU of two polygons
+
 ```python
 from tacv.geometry import iou_2d
-polygon_1 = [[0,0],[10,10],[0,10]]
+
+polygon_1 = [[0, 0], [10, 10], [0, 10]]
 polygon_2 = [[0, 20], [10, 10], [0, 0]]
-print(iou_2d(polygon_1,polygon_2))
+print(iou_2d(polygon_1, polygon_2))
 ```
+
 </details>
 <details>
 <summary> <b>Command Line Interface</b></summary>
 
 #### Synthesize a video from images
+
 ```bash
 tacv_i2v image_dir video_path [optional: fps image_ext]
 ```
+
 #### Extract images from a video
+
 ```bash
 tacv_v2i video_path image_dir
 ```
+
 </details>
 
 ### For more
-* Visit args description in source code 
+
+* Visit args description in source code
 * Visit `test.py` file
```

### Comparing `tacv-1.1.6/setup.py` & `tacv-1.1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,23 +35,23 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r") as f:
     lines = f.readlines()
     required_pkgs = [item.strip() for item in lines]
 
 # version_file = "tacv/resources/version.txt"
-new_ver = "1.1.6"  # increase_version_by_one(version_file)
+new_ver = "1.1.8"  # increase_version_by_one(version_file)
 print(f"Building {new_ver}")
 setup(
     name='tacv',
     version=new_ver,
     packages=setuptools.find_packages(where="."),
     url='https://github.com/TaQuangTu/TaCV',
     license='LICENSE',
-    author='TaQuangTu',
+    author='QuangTu-Ta',
     install_requires=required_pkgs,
     author_email='taquangtu132@gmail.com',
     description='A mini package for daily tasks',
     long_description_content_type="text/markdown",
     long_description=long_description,
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `tacv-1.1.6/tacv/detection/centernet/CenterNet.py` & `tacv-1.1.8/tacv/detection/centernet/CenterNet.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/detection/centernet/Trainer.py` & `tacv-1.1.8/tacv/detection/centernet/Trainer.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/detection/centernet/backbones/resnet.py` & `tacv-1.1.8/tacv/detection/centernet/backbones/resnet.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/detection/centernet/losses/losses.py` & `tacv-1.1.8/tacv/detection/centernet/losses/losses.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/detection/centernet/utils/data_utils.py` & `tacv-1.1.8/tacv/detection/centernet/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/detection/centernet/utils/geometry_utils.py` & `tacv-1.1.8/tacv/detection/centernet/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/detection/centernet/utils/infer.py` & `tacv-1.1.8/tacv/detection/centernet/utils/infer.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/fileUtils/fileutils.py` & `tacv-1.1.8/tacv/fileUtils/fileutils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/fileUtils/thread_downloader.py` & `tacv-1.1.8/tacv/fileUtils/thread_downloader.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/geometry/iou.py` & `tacv-1.1.8/tacv/geometry/iou.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/torch/model_utils.py` & `tacv-1.1.8/tacv/torch/model_utils.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/video/video_proc.py` & `tacv-1.1.8/tacv/video/video_proc.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv/visual/draw2d.py` & `tacv-1.1.8/tacv/visual/draw2d.py`

 * *Files identical despite different names*

### Comparing `tacv-1.1.6/tacv.egg-info/PKG-INFO` & `tacv-1.1.8/tacv.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,92 @@
 Metadata-Version: 2.1
 Name: tacv
-Version: 1.1.6
+Version: 1.1.8
 Summary: A mini package for daily tasks
 Home-page: https://github.com/TaQuangTu/TaCV
-Author: TaQuangTu
+Author: QuangTu-Ta
 Author-email: taquangtu132@gmail.com
 License: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# TACV - A mini package for daily tasks
+from tacv.fileUtils import ThreadedDownload# TACV - A mini package for daily tasks
 
 ## Installation
+
 ```bash
 pip install tacv
 ```
 
+Some specific functions depend on other libraries (.e.g `mlflow`, `torch`, `pytorch-lightning`). Be forgiving and install the necessary libraries if required.
+
 ## Examples
 
 <details>
+<summary> <b>LoRA training</b></summary>
+
+Adding LoRA to your model and start training as usual with minimal code changes.
+
+1. Define a boilerplate class that inherit both AnyLoRA and the model you want to play, in this case GPTNeoForCausalLM
+
+```python
+from tacv.torch import AnyLoRA
+from transformers import GPTNeoForCausalLM
+
+
+class GPTNeoLoRA(GPTNeoForCausalLM, AnyLoRA):
+    def __init__(self, config):
+        GPTNeoForCausalLM.__init__(self, config)
+```
+
+2. Add LoRA to layers that you think it could bring the training benefit, here we choose the Key and Value matrices in
+   all self-attention blocks
+
+```python
+# init your LoRA model
+model = GPTNeoLoRA.from_pretrained("EleutherAI/gpt-neo-1.3B", low_cpu_mem_usage=True)
+
+model.init_lora(rank=8, layers_contain=["k_proj", "v_proj"])
+
+# Also give "layers_end_with" and "layers_start_with" a try
+model.init_lora(rank=4, layers_end_with="q_proj", layers_start_with="wte")
+
+# drop grad of all other layers before training
+model.mark_only_lora_as_trainable(bias="none")
+```
+
+3. The rest of training is as usual, just as you have done before using AnyLoRA.
+4. Save and load LoRA weights.
+
+```python
+# save LoRA
+model.save_lora("lora.pth")
+# load LoRA for inference
+model.load_lora("lora.pth")
+```
+
+Want more control over the training and mode behavior, visit my example of fine-tuning a GPT-Neo model for Vietnamese
+at `tacv/torch/example_lora.py`
+
+
+</details>
+
+
+<details>
 <summary> <b>2D Object Detection</b></summary>
 
 For now, CenterNet is supported. However, use it as prototype purpose only, there is no official benchmark on accuracy.
 
 #### Train with your own dataset
 
 * First, create a config file for training/model config, see full config at `tacv/detection/sample_config.yml`.
+
 ```yaml
 input_size: &input_size [ 224,448 ]
 max_object: &max_obj 16
 num_classes: &num_classes 5
 train_config:
   gpus: 0 # 0 means CPU, N means using N available GPU(s) for training
   epoch: 600
@@ -59,51 +113,60 @@
 model:
   num_classes: *num_classes
   backbone_layers: 18
   head_conv_channel: 64
   max_object: *max_obj
   input_shape: *input_size
 ```
-* Second, create your own Dataset class that returns data as described in the `__getitem__()` method, see following example:
+
+* Second, create your own Dataset class that returns data as described in the `__getitem__()` method, see following
+  example:
+
 ```python
 from torch.utils.data import Dataset
 import torch
 
+
 class MockDataset(Dataset):
     def __init__(self, max_objs, input_shape_HW):
         self.max_objs = max_objs
         self.input_shape_HW = input_shape_HW
+
     def __getitem__(self, item):
         # read your image
         # image = cv2.imread(your image path)
         # do any transform operation, then return a tensor
-        image = torch.rand(3, self.input_shape_HW[0],self.input_shape_HW[1])  # Shape = (3, InputShape, W)
-        annos = torch.rand(self.max_objs, 5)  # Shape = (MaxObjs x 5) , each row presents for (x,y,w,h,class_id) relative to input shape
+        image = torch.rand(3, self.input_shape_HW[0], self.input_shape_HW[1])  # Shape = (3, InputShape, W)
+        annos = torch.rand(self.max_objs,
+                           5)  # Shape = (MaxObjs x 5) , each row presents for (x,y,w,h,class_id) relative to input shape
         masks = torch.zeros(
             self.max_objs)  # Shape = (MaxObjs,)  each value is False or True (1 indicates having object)
         masks[0:3] = True
         return {"image": image, "annos": annos, "masks": masks}
 
     def __len__(self):
         return 1000
 ```
+
 * Init `CenterNetTrainer` and here we go
+
 ```python
 from tacv.detection import CenterNetTrainer
 from torch.utils.data import random_split
 
 config_path = "tacv/detection/sample_config.yml"
-max_objs = 16 # read from config file
-input_shape = (224,448) # read from config file
-dataset = MockDataset(max_objs=max_objs,input_shape_HW = input_shape)  # Replace with your custom dataset
+max_objs = 16  # read from config file
+input_shape = (224, 448)  # read from config file
+dataset = MockDataset(max_objs=max_objs, input_shape_HW=input_shape)  # Replace with your custom dataset
 train_set, val_set = random_split(dataset, [900, 100])
 
 trainer = CenterNetTrainer(train_set, val_set, config_path)
 trainer.train()
 ```
+
 #### Inference on single image
 
 ```python
 import cv2
 import torch
 from tacv.detection import load_centernet_model_with_config
 from tacv.detection import infer
@@ -115,107 +178,158 @@
     model = load_centernet_model_with_config(config_path, load_bbone_pretrained=False)
     model.load_state_dict("your_checkpoint.pth")
     model.eval()
     model.to(device)
 
     image = cv2.imread("your_image.png")
     bboxes = infer(model, image, device)
-    print(bboxes) # list of detections in format (xc,yc,w,h,class_id,confidence_score)
+    print(bboxes)  # list of detections in format (xc,yc,w,h,class_id,confidence_score)
 ```
 
 </details>
 
 <details>
 <summary> <b>File utils</b></summary>
 
 ### File utils
+
 #### Get all file paths from a directory
+
 ```python
 from tacv.fileUtils import get_all_files
+
 file_paths = get_all_files("dir_name")
 ```
+
 Returns a list of file absolute paths, for example
+
 ```
 ['./venvCondaTest/x86_64-conda_cos6-linux-gnu/bin/ld', './venvCondaTest/conda-meta/_libgcc_mutex-0.1-main.json', './venvCondaTest/conda-meta/xz-5.2.5-h7b6447c_0.json', './venvCondaTest/conda-meta/wheel-0.37.1-pyhd3eb1b0_0.json', './venvCondaTest/conda-meta/setuptools-58.0.4-py36h06a4308_0.json', './venvCondaTest/conda-meta/ca-certificates-2021.10.26-h06a4308_2.json', './venvCondaTest/conda-meta/readline-8.1.2-h7f8727e_1.json', './venvCondaTest/conda-meta/sqlite-3.37.2-hc218d9a_0.json', './venvCondaTest/conda-meta/libgcc-ng-9.3.0-h5101ec6_17.json', './venvCondaTest/conda-meta/ncurses-6.3-h7f8727e_2.json']
 ```
+
 #### Save/load json data to/from file
+
 ```python
-from tacv.fileUtils import save_json,load_json
+from tacv.fileUtils import save_json, load_json
 
 json_file = "myfile.json"
-json_data = {"name":"Ta","age":100}
+json_data = {"name": "Ta", "age": 100}
 # save json
-save_json(json_file,json_data)
+save_json(json_file, json_data)
 # load json
 json_data = load_json(json_file)
 ```
+
+#### Multi-threaded file downloader
+
+```python
+from tacv.fileUtils import ThreadedDownload
+
+urls = [
+    'http://localhost:11223/210207000111980_3_124202.jpg',
+    'http://localhost:11223/210430000373373_3_407200.jpg',
+    'http://localhost:11223/210426000324979_3_356188.jpg',
+    'http://localhost:11223/200819000060994_3_78314.png'
+]
+downloader = ThreadedDownload(urls, "/home/tu/Desktop/LabelStudio", False, thread_count=3, url_tries=3)
+
+print(f'Downloading {len(urls)} files')
+downloader.run()
+print(f'Downloaded {len(downloader.report["success"])} of {len(urls)}')
+```
+
 </details>
 
 <details>
 <summary> <b>CV2 Visualization</b></summary>
 
 #### Draw 2D points onto an image
+
 ```python
 import cv2
 from tacv.visual import draw_points
+
 image = cv2.imread("myimage.jpg")
-points = [(18,19),(55,55),(102,22),(66,22)]
-draw_points(image,points,circular=True,color=(0,255,0),thickness=2)
-cv2.imwrite("new_image.jpg",image)
+points = [(18, 19), (55, 55), (102, 22), (66, 22)]
+draw_points(image, points, circular=True, color=(0, 255, 0), thickness=2)
+cv2.imwrite("new_image.jpg", image)
 ```
+
 </details>
 
 <details>
 <summary> <b>Video and image utils</b></summary>
 
 #### Synthesize a video from images
+
 ```python
 from tacv.video import images2video
-image_dir = "my_images" #directory containing images in the same format
-video_path = "tacv_test.mp4" #path to save the synthesized video
+
+image_dir = "my_images"  # directory containing images in the same format
+video_path = "tacv_test.mp4"  # path to save the synthesized video
 # common use case
-images2video(image_dir,video_path,fps=24, image_ext = None, sort=False)
+images2video(image_dir, video_path, fps=24, image_ext=None, sort=False)
 ```
+
 Parameters:
+
 * `fps`: default = 24
-* `image_ext`: a string, specify image extension to synthesize the video, for example (`jpg`, `png`,...). If it is `None`. All images will be grabbed. Default is `None`.
-* `sort`: `True` or `False`. Indicate if the images should be sorted by name before synthesizing the video. Default is `True`.
+* `image_ext`: a string, specify image extension to synthesize the video, for example (`jpg`, `png`,...). If it
+  is `None`. All images will be grabbed. Default is `None`.
+* `sort`: `True` or `False`. Indicate if the images should be sorted by name before synthesizing the video. Default
+  is `True`.
+
 #### Extract images from a video
+
 ```python
 from tacv.video import video2images
-video_path = "tacv_test.mp4" #path to video to be extracted to images
-image_dir = "my_images" #directory to save the extracted images
-video2images(video_path,image_dir,exist_ok=False, image_ext="jpg", verbose=True)
+
+video_path = "tacv_test.mp4"  # path to video to be extracted to images
+image_dir = "my_images"  # directory to save the extracted images
+video2images(video_path, image_dir, exist_ok=False, image_ext="jpg", verbose=True)
 ```
+
 Parameters:
-* `exist_ok`: default is False. If `image_dir` already contains images and this flag is `False`. The process will be cancel, otherwise it continues.
-* `image_ext`: a string, specify image extension, for example (`jpg`, `png`,...). If it is `None`. All images will be grabbed. Default is `None`.
+
+* `exist_ok`: default is False. If `image_dir` already contains images and this flag is `False`. The process will be
+  cancel, otherwise it continues.
+* `image_ext`: a string, specify image extension, for example (`jpg`, `png`,...). If it is `None`. All images will be
+  grabbed. Default is `None`.
 * `verbose`: `True` or `False`. Set it to `True` to view the extracting process. Default is `True`.
+
 </details>
 
 <details>
 <summary> <b>Geometry utils</b></summary>
 
 #### Calculate 2D IOU of two polygons
+
 ```python
 from tacv.geometry import iou_2d
-polygon_1 = [[0,0],[10,10],[0,10]]
+
+polygon_1 = [[0, 0], [10, 10], [0, 10]]
 polygon_2 = [[0, 20], [10, 10], [0, 0]]
-print(iou_2d(polygon_1,polygon_2))
+print(iou_2d(polygon_1, polygon_2))
 ```
+
 </details>
 <details>
 <summary> <b>Command Line Interface</b></summary>
 
 #### Synthesize a video from images
+
 ```bash
 tacv_i2v image_dir video_path [optional: fps image_ext]
 ```
+
 #### Extract images from a video
+
 ```bash
 tacv_v2i video_path image_dir
 ```
+
 </details>
 
 ### For more
-* Visit args description in source code 
+
+* Visit args description in source code
 * Visit `test.py` file
```

### Comparing `tacv-1.1.6/tacv.egg-info/SOURCES.txt` & `tacv-1.1.8/tacv.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,12 +32,14 @@
 tacv/fileUtils/__init__.py
 tacv/fileUtils/fileutils.py
 tacv/fileUtils/thread_downloader.py
 tacv/geometry/__init__.py
 tacv/geometry/iou.py
 tacv/resources/__init__.py
 tacv/torch/__init__.py
+tacv/torch/example_lora.py
+tacv/torch/lora_any.py
 tacv/torch/model_utils.py
 tacv/video/__init__.py
 tacv/video/video_proc.py
 tacv/visual/__init__.py
 tacv/visual/draw2d.py
```

