# Comparing `tmp/vision6D-0.2.9.tar.gz` & `tmp/vision6D-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-0iowuqvv\vision6D-0.2.9.tar", last modified: Wed Jul  5 00:52:47 2023, max compression
+gzip compressed data, was "E:\GitHub\vision6D\dist\.tmp-kiutxfiz\vision6D-0.3.0.tar", last modified: Sun Jul 16 17:15:01 2023, max compression
```

## Comparing `vision6D-0.2.9.tar` & `vision6D-0.3.0.tar`

### file list

```diff
@@ -1,57 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.878274 vision6D-0.2.9/
--rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.2.9/LICENSE
--rw-rw-rw-   0        0        0       33 2023-07-05 00:49:40.000000 vision6D-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1364 2023-07-05 00:52:47.879274 vision6D-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.2.9/README.md
--rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0     2111 2023-07-05 00:52:47.882274 vision6D-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      445 2023-07-05 00:46:04.000000 vision6D-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.762274 vision6D-0.2.9/test/
--rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.2.9/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.2.9/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.766274 vision6D-0.2.9/vision6D/
--rw-rw-rw-   0        0        0     1050 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.830274 vision6D-0.2.9/vision6D/components/
--rw-rw-rw-   0        0        0      403 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/__init__.py
--rw-rw-rw-   0        0        0     1965 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/camera_store.py
--rw-rw-rw-   0        0        0     2647 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/folder_store.py
--rw-rw-rw-   0        0        0     2229 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/image_store.py
--rw-rw-rw-   0        0        0     2980 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/mask_store.py
--rw-rw-rw-   0        0        0     6567 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/mesh_store.py
--rw-rw-rw-   0        0        0      242 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/singleton.py
--rw-rw-rw-   0        0        0     2206 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/components/video_store.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.845273 vision6D-0.2.9/vision6D/containers/
--rw-rw-rw-   0        0        0      429 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/__init__.py
--rw-rw-rw-   0        0        0     4061 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/camera_container.py
--rw-rw-rw-   0        0        0     4274 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/image_container.py
--rw-rw-rw-   0        0        0     5739 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/mask_container.py
--rw-rw-rw-   0        0        0    17556 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/mesh_container.py
--rw-rw-rw-   0        0        0    11304 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/pnp_container.py
--rw-rw-rw-   0        0        0     9828 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/containers/video_folder_container.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.851272 vision6D-0.2.9/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.2.9/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0    11885 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/data/style.qss
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.855273 vision6D-0.2.9/vision6D/entry/
--rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.2.9/vision6D/entry/__init__.py
--rw-rw-rw-   0        0        0      632 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/entry/main.py
--rw-rw-rw-   0        0        0    35066 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/mainwindow.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.858274 vision6D-0.2.9/vision6D/tools/
--rw-rw-rw-   0        0        0       19 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/tools/__init__.py
--rw-rw-rw-   0        0        0    16464 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/tools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.876274 vision6D-0.2.9/vision6D/widgets/
--rw-rw-rw-   0        0        0      583 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/widgets/__init__.py
--rw-rw-rw-   0        0        0     3443 2023-07-04 17:06:35.000000 vision6D-0.2.9/vision6D/widgets/calibration_pop_window.py
--rw-rw-rw-   0        0        0     2026 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/camera_props_input_dialog.py
--rw-rw-rw-   0        0        0     1722 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/custom_qt_interactor.py
--rw-rw-rw-   0        0        0     2535 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/get_text_dialog.py
--rw-rw-rw-   0        0        0     3766 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/label_window.py
--rw-rw-rw-   0        0        0     1281 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/popup_dialog.py
--rw-rw-rw-   0        0        0     7083 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/video_player.py
--rw-rw-rw-   0        0        0     5718 2023-07-04 17:06:36.000000 vision6D-0.2.9/vision6D/widgets/video_sampler.py
-drwxrwxrwx   0        0        0        0 2023-07-05 00:52:47.807274 vision6D-0.2.9/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1364 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1396 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      284 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-05 00:52:47.000000 vision6D-0.2.9/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.597773 vision6D-0.3.0/
+-rw-rw-rw-   0        0        0     1086 2023-06-02 21:40:49.000000 vision6D-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-07-05 00:49:40.000000 vision6D-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1364 2023-07-16 17:15:01.598770 vision6D-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-06-02 21:40:49.000000 vision6D-0.3.0/README.md
+-rw-rw-rw-   0        0        0      472 2023-06-24 04:23:35.000000 vision6D-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0     2111 2023-07-16 17:15:01.612773 vision6D-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      454 2023-07-07 18:51:59.000000 vision6D-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:00.793629 vision6D-0.3.0/test/
+-rw-rw-rw-   0        0        0    21817 2023-05-30 22:26:10.000000 vision6D-0.3.0/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.3.0/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:00.824629 vision6D-0.3.0/vision6D/
+-rw-rw-rw-   0        0        0     1050 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.089003 vision6D-0.3.0/vision6D/components/
+-rw-rw-rw-   0        0        0      512 2023-07-11 17:34:34.000000 vision6D-0.3.0/vision6D/components/__init__.py
+-rw-rw-rw-   0        0        0     2035 2023-07-13 14:10:02.000000 vision6D-0.3.0/vision6D/components/bbox_store.py
+-rw-rw-rw-   0        0        0     1938 2023-07-11 14:41:41.000000 vision6D-0.3.0/vision6D/components/camera_store.py
+-rw-rw-rw-   0        0        0     2656 2023-07-16 03:30:44.000000 vision6D-0.3.0/vision6D/components/folder_store.py
+-rw-rw-rw-   0        0        0     2648 2023-07-12 18:27:30.000000 vision6D-0.3.0/vision6D/components/image_store.py
+-rw-rw-rw-   0        0        0     3142 2023-07-13 01:57:38.000000 vision6D-0.3.0/vision6D/components/mask_store.py
+-rw-rw-rw-   0        0        0     7354 2023-07-11 17:33:12.000000 vision6D-0.3.0/vision6D/components/mesh_store.py
+-rw-rw-rw-   0        0        0     1580 2023-07-07 15:56:19.000000 vision6D-0.3.0/vision6D/components/point_store.py
+-rw-rw-rw-   0        0        0      242 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/components/singleton.py
+-rw-rw-rw-   0        0        0     2179 2023-07-11 17:33:19.000000 vision6D-0.3.0/vision6D/components/video_store.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.309143 vision6D-0.3.0/vision6D/containers/
+-rw-rw-rw-   0        0        0      614 2023-07-11 18:14:45.000000 vision6D-0.3.0/vision6D/containers/__init__.py
+-rw-rw-rw-   0        0        0     5050 2023-07-16 01:09:17.000000 vision6D-0.3.0/vision6D/containers/bbox_container.py
+-rw-rw-rw-   0        0        0     4027 2023-07-10 17:15:51.000000 vision6D-0.3.0/vision6D/containers/camera_container.py
+-rw-rw-rw-   0        0        0     6131 2023-07-16 03:32:31.000000 vision6D-0.3.0/vision6D/containers/folder_container.py
+-rw-rw-rw-   0        0        0     4372 2023-07-14 15:23:54.000000 vision6D-0.3.0/vision6D/containers/image_container.py
+-rw-rw-rw-   0        0        0     5339 2023-07-16 01:10:24.000000 vision6D-0.3.0/vision6D/containers/mask_container.py
+-rw-rw-rw-   0        0        0    18163 2023-07-13 02:06:31.000000 vision6D-0.3.0/vision6D/containers/mesh_container.py
+-rw-rw-rw-   0        0        0    11304 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/containers/pnp_container.py
+-rw-rw-rw-   0        0        0     1881 2023-07-07 15:47:13.000000 vision6D-0.3.0/vision6D/containers/point_container.py
+-rw-rw-rw-   0        0        0    10367 2023-07-16 03:03:04.000000 vision6D-0.3.0/vision6D/containers/video_container.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.351771 vision6D-0.3.0/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.3.0/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0    11885 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/data/style.qss
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.367772 vision6D-0.3.0/vision6D/entry/
+-rw-rw-rw-   0        0        0        0 2023-06-24 04:11:35.000000 vision6D-0.3.0/vision6D/entry/__init__.py
+-rw-rw-rw-   0        0        0      632 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/entry/main.py
+-rw-rw-rw-   0        0        0    37415 2023-07-16 03:29:17.000000 vision6D-0.3.0/vision6D/mainwindow.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.409770 vision6D-0.3.0/vision6D/tools/
+-rw-rw-rw-   0        0        0       19 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/tools/__init__.py
+-rw-rw-rw-   0        0        0    17321 2023-07-13 01:25:37.000000 vision6D-0.3.0/vision6D/tools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:01.594769 vision6D-0.3.0/vision6D/widgets/
+-rw-rw-rw-   0        0        0      646 2023-07-11 17:29:38.000000 vision6D-0.3.0/vision6D/widgets/__init__.py
+-rw-rw-rw-   0        0        0     3443 2023-07-04 17:06:35.000000 vision6D-0.3.0/vision6D/widgets/calibration_pop_window.py
+-rw-rw-rw-   0        0        0     2026 2023-07-04 17:06:36.000000 vision6D-0.3.0/vision6D/widgets/camera_props_input_dialog.py
+-rw-rw-rw-   0        0        0     1694 2023-07-12 14:56:42.000000 vision6D-0.3.0/vision6D/widgets/custom_qt_interactor.py
+-rw-rw-rw-   0        0        0     5461 2023-07-13 02:49:34.000000 vision6D-0.3.0/vision6D/widgets/draw_bbox_window.py
+-rw-rw-rw-   0        0        0     3882 2023-07-12 15:18:40.000000 vision6D-0.3.0/vision6D/widgets/draw_mask_window.py
+-rw-rw-rw-   0        0        0     2535 2023-07-04 17:06:36.000000 vision6D-0.3.0/vision6D/widgets/get_text_dialog.py
+-rw-rw-rw-   0        0        0     1281 2023-07-04 17:06:36.000000 vision6D-0.3.0/vision6D/widgets/popup_dialog.py
+-rw-rw-rw-   0        0        0     7083 2023-07-10 15:16:47.000000 vision6D-0.3.0/vision6D/widgets/video_player.py
+-rw-rw-rw-   0        0        0     5718 2023-07-04 17:06:36.000000 vision6D-0.3.0/vision6D/widgets/video_sampler.py
+drwxrwxrwx   0        0        0        0 2023-07-16 17:15:00.906629 vision6D-0.3.0/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1364 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1616 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      284 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 17:15:00.000000 vision6D-0.3.0/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.2.9/LICENSE` & `vision6D-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/PKG-INFO` & `vision6D-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.9
+Version: 0.3.0
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
 Project-URL: Documentation, https://vision6d.readthedocs.io/en/latest/
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.9/README.md` & `vision6D-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/setup.cfg` & `vision6D-0.3.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e32 2e39 0d0a 7572  sion = 0.2.9..ur
+00000020: 7369 6f6e 203d 2030 2e33 2e30 0d0a 7572  sion = 0.3.0..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.2.9/test/test_create_dataset.py` & `vision6D-0.3.0/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/test/test_projection.py` & `vision6D-0.3.0/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/__init__.py` & `vision6D-0.3.0/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/components/camera_store.py` & `vision6D-0.3.0/vision6D/components/camera_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,14 @@
 '''
 
 import math
 import pyvista as pv
 import numpy as np
 from . import Singleton
 
-# contains mesh objects
-
 class CameraStore(metaclass=Singleton):
     def __init__(self, window_size):
         self.window_size = window_size
         self.reset()
         
     def reset(self):
         self.camera = pv.Camera()
```

### Comparing `vision6D-0.2.9/vision6D/components/folder_store.py` & `vision6D-0.3.0/vision6D/components/folder_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,63 +12,60 @@
 import re
 import pathlib
 
 import numpy as np
 
 from . import Singleton
 
-
-# contains mesh objects
-
 class FolderStore(metaclass=Singleton):
     def __init__(self):
         self.reset()
 
     def reset(self):
         self.folder_path = None
-        self.current_frame = 0
+        self.current_image = 0
 
     def get_files_from_folder(self, category):
         dir = pathlib.Path(self.folder_path) / category
         folders = [d for d in os.listdir(dir) if os.path.isdir(os.path.join(dir, d))]
         if len(folders) == 1: dir = pathlib.Path(self.folder_path) / category / folders[0]
         # Retrieve files
         files = [f for f in os.listdir(dir) if os.path.isfile(os.path.join(dir, f))]
-        self.total_frame = len(files)
+        self.total_image = len(files)
         # Sort files
         files.sort(key=lambda f: int(re.sub('\D', '', f)))
         return files, dir
 
-    def add_folder(self, folder_path):
+    def add_folder(self, folder_path, mesh_actors):
         self.folder_path = folder_path
         folders = [d for d in os.listdir(self.folder_path) if os.path.isdir(os.path.join(self.folder_path, d))] 
         image_path = ''
         mask_path = ''
         pose_path = ''
         mesh_path = ''
         if 'images' in folders:
             image_files, image_dir = self.get_files_from_folder('images')
-            path = str(image_dir / image_files[self.current_frame])
+            path = str(image_dir / image_files[self.current_image])
             if os.path.isfile(path): image_path = path
         if 'masks' in folders:
             mask_files, mask_dir = self.get_files_from_folder('masks')
-            path = str(mask_dir / mask_files[self.current_frame])
+            path = str(mask_dir / mask_files[self.current_image])
             if os.path.isfile(path): mask_path = path
         if 'poses' in folders:
             pose_files, pose_dir = self.get_files_from_folder('poses')
-            path = str(pose_dir / pose_files[self.current_frame])
+            path = str(pose_dir / pose_files[self.current_image])
             if os.path.isfile(path): pose_path = path
-        if self.current_frame == 0:
+        if self.current_image == 0 or len(mesh_actors) == 0:
             if 'meshes' in folders:
                 dir = pathlib.Path(self.folder_path) / "meshes"
                 path = dir / 'mesh_path.txt'
                 if os.path.isfile(path): mesh_path = path
 
         return image_path, mask_path, pose_path, mesh_path
     
-    def prev_frame(self):
-        self.current_frame -= 1
-        self.current_frame = np.clip(self.current_frame, 0, self.total_frame)
+    def prev_image(self):
+        self.current_image -= 1
+        self.current_image = np.clip(self.current_image, 0, self.total_image)
         
-    def next_frame(self):
-        self.current_frame += 1
-        self.current_frame = np.clip(self.current_frame, 0, self.total_frame)
+    def next_image(self):
+        self.current_image += 1
+        self.current_image = np.clip(self.current_image, 0, self.total_image)
```

### Comparing `vision6D-0.2.9/vision6D/components/image_store.py` & `vision6D-0.3.0/vision6D/components/image_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,56 +3,63 @@
 @license: (C) Copyright.
 @contact: yike.zhang@vanderbilt.edu
 @software: Vision6D
 @file: image_store.py
 @time: 2023-07-03 20:23
 @desc: create store for image related base functions
 '''
+import copy
 
 import numpy as np
 import pathlib
 import pyvista as pv
 import PIL.Image
 
 
 from . import Singleton
 from ..tools import utils
 
-# contains mesh objects
-
 class ImageStore(metaclass=Singleton):
     def __init__(self):
         self.reset()
         self.mirror_x = False
         self.mirror_y = False
 
     def reset(self):
         self.image_path = None
+        self.image_source = None
         self.image_actor = None
         self.image_opacity = 0.8
+        self.width = None
+        self.height = None
 
     def add_image(self, image_source):
         if isinstance(image_source, pathlib.WindowsPath) or isinstance(image_source, str):
             self.image_path = str(image_source)
             image_source = np.array(PIL.Image.open(image_source), dtype='uint8')
+        
+        #^ save the image_source for mirroring image in the video
+        self.image_source = copy.deepcopy(image_source)
+
         if len(image_source.shape) == 2: image_source = image_source[..., None]
+        dim = image_source.shape
+        self.height, self.width, channel = dim[0], dim[1], dim[2]
 
         if self.mirror_x: image_source = image_source[:, ::-1, :]
         if self.mirror_y: image_source = image_source[::-1, :, :]
 
-        dim = image_source.shape
-        h, w, channel = dim[0], dim[1], dim[2]
-
-        self.render = utils.create_render(w, h)
-
-        image = pv.UniformGrid(dimensions=(w, h, 1), spacing=[0.01, 0.01, 1], origin=(0.0, 0.0, 0.0))
-        image.point_data["values"] = image_source.reshape((w * h, channel)) # order = 'C
-        image = image.translate(-1 * np.array(image.center), inplace=False)
-
+        self.render = utils.create_render(self.width, self.height)
+        image = self.update_image(image_source, channel)
         return image, image_source, channel
+    
+    def update_image(self, image_source, channel):
+        image = pv.UniformGrid(dimensions=(self.width, self.height, 1), spacing=[0.01, 0.01, 1], origin=(0.0, 0.0, 0.0))
+        image.point_data["values"] = image_source.reshape((self.width * self.height, channel)) # order = 'C
+        image = image.translate(-1 * np.array(image.center), inplace=False)
+        return image
         
     def update_opacity(self, delta):
         self.image_opacity += delta
         self.image_opacity = np.clip(self.image_opacity, 0, 1)
         self.image_actor.GetProperty().opacity = self.image_opacity
         
     def render_image(self, camera):
```

### Comparing `vision6D-0.2.9/vision6D/components/mask_store.py` & `vision6D-0.3.0/vision6D/components/mask_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 import PIL.Image
 import numpy as np
 import pyvista as pv
 
 from . import Singleton
 from ..tools import utils
 
-# contains mesh objects
-
 class MaskStore(metaclass=Singleton):
     def __init__(self):
         self.reset()
         self.mirror_x = False
         self.mirror_y = False
 
     def reset(self):
@@ -37,47 +35,48 @@
             mask_source = np.array(PIL.Image.open(mask_source), dtype='uint8')
 
         # if len(mask_source.shape) == 2: mask_source = mask_source[..., None]
         if mask_source.shape[-1] == 3: mask_source = cv2.cvtColor(mask_source, cv2.COLOR_RGB2GRAY)
 
         # Get the segmentation contour points
         contours, _ = cv2.findContours(mask_source, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
-        points2d = contours[0].squeeze()
+        points = contours[0].squeeze()
+        points = points * 0.01
+        points = np.hstack((points, np.zeros(points.shape[0]).reshape((-1, 1))))
         
         # Mirror points
         h, w = mask_source.shape[0], mask_source.shape[1]
         
         self.render = utils.create_render(w, h)
         
-        if self.mirror_x: points2d[:, 0] = w - points2d[:, 0]
-        if self.mirror_y: points2d[:, 1] = h - points2d[:, 1]
-
-        bottom_point = points2d[np.argmax(points2d[:, 1])]
-
-        mask_center = (mask_source.shape[1] // 2, mask_source.shape[0] // 2)
+        if self.mirror_x: points[:, 0] = w*0.01 - points[:, 0]
+        if self.mirror_y: points[:, 1] = h*0.01 - points[:, 1]
 
-        self.mask_offset = np.hstack(((bottom_point - mask_center)*0.01, 0))
-
-        # Pad points a z dimension
-        points = np.hstack((points2d*0.01, np.zeros(points2d.shape[0]).reshape((-1, 1))))
-        # Find the bottom point on mask
         self.mask_bottom_point = points[np.argmax(points[:, 1])]
+        mask_center = np.array([mask_source.shape[1] // 2, mask_source.shape[0] // 2, 0]) * 0.01
+        self.mask_offset = self.mask_bottom_point - mask_center
 
         # Create the mesh surface object
         cells = np.hstack([[points.shape[0]], np.arange(points.shape[0]), 0])
         mask_surface = pv.PolyData(points, cells).triangulate()
         mask_surface = mask_surface.translate(-self.mask_bottom_point+self.mask_offset, inplace=False)
 
-        return mask_surface, points
+        return mask_surface
 
     def update_opacity(self, delta):
         self.mask_opacity += delta
         self.mask_opacity = np.clip(self.mask_opacity, 0, 1)
         self.mask_actor.GetProperty().opacity = self.mask_opacity
 
+    def update_mask(self):
+        tranformed_points = utils.get_mask_actor_points(self.mask_actor)
+        cells = np.hstack([[tranformed_points.shape[0]], np.arange(tranformed_points.shape[0]), 0])
+        mask_surface = pv.PolyData(tranformed_points, cells).triangulate()
+        return mask_surface
+
     def render_mask(self, camera):
         self.render.clear()
         render_actor = self.mask_actor.copy(deep=True)
         render_actor.GetProperty().opacity = 1
         self.render.add_actor(render_actor, pickable=False)
         self.render.camera = camera
         self.render.disable()
```

### Comparing `vision6D-0.2.9/vision6D/components/mesh_store.py` & `vision6D-0.3.0/vision6D/components/mesh_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,25 +13,20 @@
 import trimesh
 import pyvista as pv
 import numpy as np
 
 from . import Singleton
 from ..tools import utils
 
-# contains mesh objects
-
 class MeshStore(metaclass=Singleton):
     def __init__(self, window_size):
-        self.reset()
-        self.render = utils.create_render(window_size[0], window_size[1])
-
-    def reset(self):
         self.reference = None
         self.mesh_path = None
         self.mesh_name = None
+        self.mesh_info = None
         self.mirror_x = False
         self.mirror_y = False
         self.mesh_actors = {}
         self.meshdict = {}
         self.latlon = utils.load_latitude_longitude()
         
         self.colors = ["cyan", "magenta", "yellow", "lime", "dodgerblue", "darkviolet", "darkorange", "darkgrey"]
@@ -47,61 +42,85 @@
 
         # Pose as meshes' attributes
         self.pose_path = None
         self.transformation_matrix = np.eye(4)
         self.initial_pose = None
         self.undo_poses = {}
 
+        self.render = utils.create_render(window_size[0], window_size[1])
+
+    def reset(self):
+        self.reference = None
+        self.mesh_path = None
+        self.mesh_name = None
+        self.mesh_info = None
+        self.mirror_x = False
+        self.mirror_y = False
+        self.mesh_actors.clear()
+        self.meshdict.clear()
+        self.latlon = utils.load_latitude_longitude()
+        
+        self.colors = ["cyan", "magenta", "yellow", "lime", "dodgerblue", "darkviolet", "darkorange", "darkgrey"]
+        self.used_colors.clear()
+        self.mesh_colors.clear()
+
+        self.surface_opacity = 0.3
+        self.mesh_opacity.clear()
+        self.store_mesh_opacity.clear()
+        
+        # Set mesh spacing
+        self.mesh_spacing = [1, 1, 1]
+
+        # Pose as meshes' attributes
+        self.pose_path = None
+        self.transformation_matrix = np.eye(4)
+        self.initial_pose = None
+        self.undo_poses.clear()
+
     #^ Mesh related
-    def add_mesh(self, mesh_source):
-        flag = False
-                              
+    def add_mesh(self, mesh_source):                        
         if isinstance(mesh_source, pathlib.WindowsPath) or isinstance(mesh_source, str):
             self.mesh_path = str(mesh_source)
             if pathlib.Path(mesh_source).suffix == '.mesh': mesh_source = utils.load_trimesh(mesh_source)
             else: mesh_source = pv.read(mesh_source)
 
-        self.mesh_name = pathlib.Path(self.mesh_path).stem
-        self.meshdict[self.mesh_name] = self.mesh_path
-        self.mesh_opacity[self.mesh_name] = self.surface_opacity
-
         if isinstance(mesh_source, trimesh.Trimesh):
             assert (mesh_source.vertices.shape[1] == 3 and mesh_source.faces.shape[1] == 3), "it should be N by 3 matrix"
-            mesh_data = pv.wrap(mesh_source)
+            self.mesh_info = pv.wrap(mesh_source)
             source_verts = mesh_source.vertices * self.mesh_spacing
             source_faces = mesh_source.faces
-            flag = True
 
         if isinstance(mesh_source, pv.PolyData):
-            mesh_data = mesh_source
+            self.mesh_info = mesh_source
             source_verts = mesh_source.points * self.mesh_spacing
             source_faces = mesh_source.faces.reshape((-1, 4))[:, 1:]
-            flag = True
 
-        if flag:
-            # consider the mesh verts spacing
-            mesh_data.points = mesh_data.points * self.mesh_spacing
+        if self.mesh_info is not None:
+            # set mesh attributes
+            self.mesh_name = pathlib.Path(self.mesh_path).stem + "_mesh"
+            self.meshdict[self.mesh_name] = self.mesh_path
+            self.mesh_opacity[self.mesh_name] = self.surface_opacity
+            self.mesh_info.points = self.mesh_info.points * self.mesh_spacing
             if self.initial_pose is None: self.initial_pose = self.transformation_matrix
 
             # assign a color to every mesh
             if len(self.colors) != 0: 
                 mesh_color = self.colors.pop(0)
             else:
                 self.colors = self.used_colors
                 mesh_color = self.colors.pop(0)
                 self.used_colors = []
 
             self.used_colors.append(mesh_color)
             # store neccessary attributes
             self.mesh_colors[self.mesh_name] = mesh_color
-                        
-            return mesh_data, source_verts, source_faces
+            return source_verts, source_faces
         else:
             self.reset()
-            return None, None, None
+            return None, None
 
     def remove_mesh(self, name):
         del self.mesh_actors[name] # remove the item from the mesh dictionary
         del self.mesh_colors[name]
         del self.mesh_opacity[name]
         del self.meshdict[name]
         self.reference = None
```

### Comparing `vision6D-0.2.9/vision6D/components/video_store.py` & `vision6D-0.3.0/vision6D/components/video_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,14 @@
 
 from . import Singleton
 from ..widgets import VideoPlayer
 from ..widgets import VideoSampler
 
 from PyQt5 import QtWidgets
 
-# contains mesh objects
-
 class VideoStore(metaclass=Singleton):
     def __init__(self):
         self.reset()
 
     def reset(self):
         self.video_path = None
         self.current_frame = 0
```

### Comparing `vision6D-0.2.9/vision6D/containers/camera_container.py` & `vision6D-0.3.0/vision6D/containers/camera_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,21 @@
 
 class CameraContainer:
     def __init__(self, plotter):
         self.plotter = plotter
         self.camera_store = CameraStore()
         self.image_store = ImageStore()
 
+    def reset_camera(self):
+        self.plotter.camera = self.camera_store.camera.copy()
+
     def set_camera_props(self):
         self.camera_store.set_camera_intrinsics()
         self.camera_store.set_camera_extrinsics()
-        self.plotter.camera = self.camera_store.camera.copy()
+        self.reset_camera()
 
     def camera_calibrate(self):
         if self.image_store.image_path:
             original_image = np.array(PIL.Image.open(self.image_store.image_path), dtype='uint8')
             # make the the original image shape is [h, w, 3] to match with the rendered calibrated_image
             original_image = original_image[..., :3]
             if len(original_image.shape) == 2: original_image = original_image[..., None]
@@ -64,15 +67,12 @@
                 try:
                     self.camera_store.fx, self.camera_store.fy, self.camera_store.cx, self.camera_store.cy, self.camera_store.cam_viewup, self.camera_store.cam_position = ast.literal_eval(fx), ast.literal_eval(fy), ast.literal_eval(cx), ast.literal_eval(cy), ast.literal_eval(cam_viewup), ast.literal_eval(cam_position)
                     self.set_camera_props()
                 except:
                     self.camera_store.fx, self.camera_store.fy, self.camera_store.cx, self.camera_store.cy, self.camera_store.cam_viewup, self.camera_store.cam_position = pre_fx, pre_fy, pre_cx, pre_cy, pre_cam_viewup, pre_cam_position
                     QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Error occured, check the format of the input values", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
-    def reset_camera(self):
-        self.plotter.camera = self.camera_store.camera.copy()
-
     def zoom_in(self):
         self.plotter.camera.zoom(2)
 
     def zoom_out(self):
         self.plotter.camera.zoom(0.5)
```

### Comparing `vision6D-0.2.9/vision6D/containers/image_container.py` & `vision6D-0.3.0/vision6D/containers/image_container.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         if image_path:
             self.hintLabel.hide()
             self.add_image(image_path)
 
     def mirror_image(self, direction):
         if direction == 'x': self.image_store.mirror_x = not self.image_store.mirror_x
         elif direction == 'y': self.image_store.mirror_y = not self.image_store.mirror_y
-        self.add_image(self.image_store.image_path)
+        self.add_image(self.image_store.image_source)
 
     def add_image(self, image_source):
 
         image, original_image, channel = self.image_store.add_image(image_source)
 
         # Then add it to the plotter
         if channel == 1: 
@@ -81,18 +81,19 @@
         if not up: change *= -1
         self.image_store.update_opacity(change)
         self.plotter.add_actor(self.image_store.image_actor, pickable=False, name="image")
         self.check_button(actor_name='image')
 
     def export_image(self):
         if self.image_store.image_actor:
-            image = self.image_store.render_image(camera=self.plotter.camera.copy())
+            image_rendered = self.image_store.render_image(camera=self.plotter.camera.copy())
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Image Files (*.png)")
             if output_path:
-                if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.png')
-                rendered_image = PIL.Image.fromarray(image)
+                if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
+                rendered_image = PIL.Image.fromarray(image_rendered)
                 rendered_image.save(output_path)
-                self.output_text.append(f"-> Export image render to:\n {str(output_path)}")
+                self.output_text.append(f"-> Export image render to:\n {output_path}")
                 self.output_text.append(f"\n************************************************************\n")
+            self.image_store.image_path = output_path
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.2.9/vision6D/containers/mask_container.py` & `vision6D-0.3.0/vision6D/containers/mask_container.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 @time: 2023-07-03 20:26
 @desc: create container for mask related actions in application
 '''
 
 import pathlib
 
 import numpy as np
-import pyvista as pv
 import PIL.Image
 
 from PyQt5 import QtWidgets
 
 from ..tools import utils
 from ..components import CameraStore
 from ..components import ImageStore
 from ..components import MaskStore
-from ..widgets import LabelWindow
+from ..widgets import MaskWindow
 
 class MaskContainer:
     def __init__(self, 
                 plotter, 
                 hintLabel, 
                 track_actors_names, 
                 add_button_actor_name, 
@@ -50,35 +49,35 @@
             self.add_mask(mask_path)
 
     def mirror_mask(self, direction):
         if direction == 'x': self.mask_store.mirror_x = not self.mask_store.mirror_x
         elif direction == 'y': self.mask_store.mirror_y = not self.mask_store.mirror_y
         self.add_mask(self.mask_store.mask_path)
 
-    def load_mask(self, mask_surface, points):
+    def load_mask(self, mask_surface):
         # Add mask surface object to the plot
         mask_mesh = self.plotter.add_mesh(mask_surface, color="white", style='surface', opacity=self.mask_store.mask_opacity)
         actor, _ = self.plotter.add_actor(mask_mesh, pickable=True, name='mask')
         self.mask_store.mask_actor = actor
-        mask_point_data = utils.get_mask_actor_points(self.mask_store.mask_actor)
-        assert np.isclose(((mask_point_data+self.mask_store.mask_bottom_point-self.mask_store.mask_offset) - points), 0).all(), "mask_point_data and points should be equal"
-
+        
     def add_mask(self, mask_source):
-        mask_surface, points = self.mask_store.add_mask(mask_source)
-        self.load_mask(mask_surface, points)
+        mask_surface = self.mask_store.add_mask(mask_source)
+        self.load_mask(mask_surface)
         
         # Add remove current image to removeMenu
         if 'mask' not in self.track_actors_names:
             self.track_actors_names.append('mask')
             self.add_button_actor_name('mask')
     
     def reset_mask(self):
         if self.mask_store.mask_path:
-            mask_surface, points = self.mask_store.add_mask(self.mask_store.mask_path)
-            self.load_mask(mask_surface, points)
+            self.mask_store.mirror_x = False
+            self.mask_store.mirror_y = False
+            mask_surface = self.mask_store.add_mask(self.mask_store.mask_path)
+            self.load_mask(mask_surface)
 
     def set_mask_opacity(self, mask_opacity: float):
         self.mask_store.mask_opacity = mask_opacity
         self.mask_store.mask_actor.GetProperty().opacity = mask_opacity
         self.plotter.add_actor(self.mask_store.mask_actor, pickable=True, name='mask')
     
     def toggle_mask_opacity(self, up):
@@ -90,35 +89,33 @@
     
     def draw_mask(self):
         def handle_output_path_change(output_path):
             if output_path:
                 self.mask_store.mask_path = output_path
                 self.add_mask(self.mask_store.mask_path)
         if self.image_store.image_path:
-            self.label_window = LabelWindow(self.image_store.image_path)
-            self.label_window.show()
-            self.label_window.image_label.output_path_changed.connect(handle_output_path_change)
+            self.mask_window = MaskWindow(self.image_store.image_path)
+            self.mask_window.mask_label.output_path_changed.connect(handle_output_path_change)
+        elif self.image_store.image_source is not None:
+            self.mask_window = MaskWindow(self.image_store.image_source)
+            self.mask_window.mask_label.output_path_changed.connect(handle_output_path_change)
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
     def export_mask(self):
         if self.mask_store.mask_actor:
             # Store the transformed mask actor if there is any transformation
-            tranformed_points = utils.get_mask_actor_points(self.mask_store.mask_actor)
-            cells = np.hstack([[tranformed_points.shape[0]], np.arange(tranformed_points.shape[0]), 0])
-            mask_surface = pv.PolyData(tranformed_points, cells).triangulate()
-            mask_mesh = self.plotter.add_mesh(mask_surface, color="white", style='surface', opacity=self.mask_store.mask_opacity)
-            actor, _ = self.plotter.add_actor(mask_mesh, pickable=True, name='mask')
-            self.mask_store.mask_actor = actor
-
+            mask_surface = self.mask_store.update_mask()
+            self.load_mask(mask_surface)
             image = self.mask_store.render_mask(camera=self.plotter.camera.copy())
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Mask Files (*.png)")
             if output_path:
-                if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.png')
+                if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
-                self.output_text.append(f"-> Export mask render to:\n {str(output_path)}")
+                self.output_text.append(f"-> Export mask render to:\n {output_path}")
                 self.output_text.append(f"\n************************************************************\n")
+            self.mask_store.mask_path = output_path
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a mask first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.2.9/vision6D/containers/mesh_container.py` & `vision6D-0.3.0/vision6D/containers/mesh_container.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
                 button_group_actors_names,
                 check_button,
                 opacity_spinbox, 
                 opacity_value_change,
                 reset_camera,
                 current_pose,
                 register_pose,
+                load_mask,
                 output_text):
         
         self.ignore_opacity_change = False
         self.toggle_hide_meshes_flag = False
 
         self.color_button = color_button
         self.plotter = plotter
@@ -50,16 +51,17 @@
         self.track_actors_names = track_actors_names
         self.add_button_actor_name = add_button_actor_name
         self.button_group_actors_names = button_group_actors_names
         self.check_button = check_button
         self.opacity_spinbox = opacity_spinbox
         self.opacity_value_change = opacity_value_change
         self.reset_camera = reset_camera
-        self.register_pose = register_pose
         self.current_pose = current_pose
+        self.register_pose = register_pose
+        self.load_mask = load_mask
         self.output_text = output_text
         
         self.camera_store = CameraStore()
         self.mask_store = MaskStore()
         self.mesh_store = MeshStore()
 
     def add_mesh_file(self, mesh_path='', prompt=False):
@@ -78,18 +80,17 @@
         self.add_mesh(self.mesh_store.meshdict[self.mesh_store.reference], transformation_matrix)
         self.mesh_store.undo_poses.clear()
         self.output_text.append(f"-> Mirrored transformation matrix is: \n{transformation_matrix}")
         self.output_text.append(f"\n************************************************************\n")
 
     def add_mesh(self, mesh_source, transformation_matrix=None):
         """ add a mesh to the pyqt frame """
-        mesh_data, source_verts, source_faces = self.mesh_store.add_mesh(mesh_source)
-
-        if mesh_data:      
-            mesh = self.plotter.add_mesh(mesh_data, color=self.mesh_store.mesh_colors[self.mesh_store.mesh_name], opacity=self.mesh_store.mesh_opacity[self.mesh_store.mesh_name], name=self.mesh_store.mesh_name)
+        source_verts, source_faces = self.mesh_store.add_mesh(mesh_source)
+        if self.mesh_store.mesh_info:
+            mesh = self.plotter.add_mesh(self.mesh_store.mesh_info, color=self.mesh_store.mesh_colors[self.mesh_store.mesh_name], opacity=self.mesh_store.mesh_opacity[self.mesh_store.mesh_name], name=self.mesh_store.mesh_name)
             mesh.user_matrix = self.mesh_store.transformation_matrix if transformation_matrix is None else transformation_matrix
             actor, _ = self.plotter.add_actor(mesh, pickable=True, name=self.mesh_store.mesh_name)
 
             actor_vertices, actor_faces = utils.get_mesh_actor_vertices_faces(actor)
             assert (actor_vertices == source_verts).all(), "vertices should be the same"
             assert (actor_faces == source_faces).all(), "faces should be the same"
             assert actor.name == self.mesh_store.mesh_name, "actor's name should equal to mesh_name"
@@ -169,26 +170,28 @@
             checked_button = self.button_group_actors_names.checkedButton()
             if checked_button: self.checked_button_name = checked_button.text()
             else: self.checked_button_name = None
 
             for button in self.button_group_actors_names.buttons():
                 actor_name = button.text()
                 if actor_name in self.mesh_store.mesh_actors:
-                    if actor_name == self.checked_button_name: continue
+                    if len(self.mesh_store.mesh_actors) != 1 and actor_name == self.checked_button_name: 
+                        continue
                     self.ignore_opacity_change = True
                     self.opacity_spinbox.setValue(0)
                     self.ignore_opacity_change = False
                     self.mesh_store.store_mesh_opacity[actor_name] = copy.deepcopy(self.mesh_store.mesh_opacity[actor_name])
                     self.mesh_store.mesh_opacity[actor_name] = 0
                     self.set_mesh_opacity(actor_name, self.mesh_store.mesh_opacity[actor_name])
         else:
             for button in self.button_group_actors_names.buttons():
                 actor_name = button.text()
                 if actor_name in self.mesh_store.mesh_actors:
-                    if actor_name == self.checked_button_name: continue
+                    if len(self.mesh_store.mesh_actors) != 1 and actor_name == self.checked_button_name: 
+                        continue
                     self.ignore_opacity_change = True
                     self.opacity_spinbox.setValue(self.mesh_store.store_mesh_opacity[actor_name])
                     self.ignore_opacity_change = False
                     self.set_mesh_opacity(actor_name, self.mesh_store.store_mesh_opacity[actor_name])
                     self.mesh_store.store_mesh_opacity[actor_name] = copy.deepcopy(self.mesh_store.mesh_opacity[actor_name])
                             
     def add_pose_file(self, pose_path):
@@ -203,16 +206,17 @@
 
     def add_pose(self, matrix:np.ndarray=None, rot:np.ndarray=None, trans:np.ndarray=None):
         if matrix is not None: 
             self.mesh_store.initial_pose = matrix
             self.reset_gt_pose()
         else:
             if (rot and trans): matrix = np.vstack((np.hstack((rot, trans)), [0, 0, 0, 1]))
-        self.reset_camera()
-
+            self.mesh_store.initial_pose = matrix
+            self.reset_gt_pose()
+        
     def set_pose(self):
         # get the gt pose
         get_text_dialog = GetTextDialog()
         res = get_text_dialog.exec_()
         if res == QtWidgets.QDialog.Accepted:
             try:
                 gt_pose = ast.literal_eval(get_text_dialog.user_text)
@@ -230,69 +234,74 @@
                 QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
     
     def reset_gt_pose(self):
         if self.mesh_store.initial_pose is not None:
             self.output_text.append(f"-> Reset the GT pose to: \n{self.mesh_store.initial_pose}")
             self.output_text.append(f"\n************************************************************\n")
             self.register_pose(self.mesh_store.initial_pose)
+            self.reset_camera()
 
     def update_gt_pose(self):
         if self.mesh_store.initial_pose is not None:
             self.mesh_store.initial_pose = self.mesh_store.transformation_matrix
             self.current_pose()
             self.output_text.append(f"-> Update the GT pose to: \n{self.mesh_store.initial_pose}")
             self.output_text.append(f"\n************************************************************\n")
 
     def undo_pose(self):
         if self.button_group_actors_names.checkedButton():
             actor_name = self.button_group_actors_names.checkedButton().text()
-            if self.mesh_store.undo_poses and len(self.mesh_store.undo_poses[actor_name]) != 0: 
-                self.mesh_store.undo_pose(actor_name)
-                # register the rest meshes' pose to current undoed pose
-                self.check_button(actor_name=actor_name)
+            if actor_name in self.mesh_store.mesh_actors:
+                if self.mesh_store.undo_poses and len(self.mesh_store.undo_poses[actor_name]) != 0: 
+                    self.mesh_store.undo_pose(actor_name)
+                    # register the rest meshes' pose to current undoed pose
+                    self.check_button(actor_name=actor_name)
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Choose a mesh actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def export_pose(self):
         if self.mesh_store.reference: 
             self.update_gt_pose()
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Pose Files (*.npy)")
             if output_path:
-                if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.npy')
+                if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.npy')
                 np.save(output_path, self.mesh_store.transformation_matrix)
-                self.output_text.append(f"-> Saved:\n{self.mesh_store.transformation_matrix}\nExport to:\n {str(output_path)}")
+                self.output_text.append(f"-> Saved:\n{self.mesh_store.transformation_matrix}\nExport to:\n {output_path}")
                 self.output_text.append(f"\n************************************************************\n")
+            self.mesh_store.pose_path = output_path
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
     
     def export_mesh_render(self, save_render=True):
         image = None
         if self.mesh_store.reference:
             image = self.mesh_store.render_mesh(camera=self.plotter.camera.copy())
             if save_render:
                 output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "Mesh Files (*.png)")
                 if output_path:
-                    if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.png')
+                    if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
                     rendered_image = PIL.Image.fromarray(image)
                     rendered_image.save(output_path)
-                    self.output_text.append(f"-> Export mesh render to:\n {str(output_path)}")
+                    self.output_text.append(f"-> Export mesh render to:\n {output_path}")
                     self.output_text.append(f"\n************************************************************\n")
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
         return image
 
     def export_segmesh_render(self):
         if self.mesh_store.reference and self.mask_store.mask_actor:
+            mask_surface = self.mask_store.update_mask()
+            self.load_mask(mask_surface)
             segmask = self.mask_store.render_mask(camera=self.plotter.camera.copy())
             if np.max(segmask) > 1: segmask = segmask / 255
             image = self.mesh_store.render_mesh(camera=self.plotter.camera.copy())
             image = (image * segmask).astype(np.uint8)
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(QtWidgets.QMainWindow(), "Save File", "", "SegMesh Files (*.png)")
             if output_path:
-                if pathlib.Path(output_path).suffix == '': output_path = output_path.parent / (output_path.stem + '.png')
+                if pathlib.Path(output_path).suffix == '': output_path = pathlib.Path(output_path).parent / (pathlib.Path(output_path).stem + '.png')
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
-                self.output_text.append(f"-> Export segmask render:\n to {str(output_path)}")
+                self.output_text.append(f"-> Export segmask render:\n to {output_path}")
                 self.output_text.append(f"\n************************************************************\n")
         else:
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a mesh or mask first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.2.9/vision6D/containers/pnp_container.py` & `vision6D-0.3.0/vision6D/containers/pnp_container.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/containers/video_folder_container.py` & `vision6D-0.3.0/vision6D/containers/video_container.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,164 +1,175 @@
 '''
 @author: Yike (Nicole) Zhang
 @license: (C) Copyright.
 @contact: yike.zhang@vanderbilt.edu
 @software: Vision6D
-@file: video_folder_container.py
+@file: video_container.py
 @time: 2023-07-03 20:28
-@desc: create container for video/folder related actions in application
+@desc: create container for video related actions in application
 '''
 
 import os
 import pathlib
 
 import numpy as np
 import PIL.Image
 
 from PyQt5 import QtWidgets
 
 from ..components import ImageStore
+from ..components import MaskStore
+from ..components import BboxStore
 from ..components import MeshStore
 from ..components import VideoStore
 from ..components import FolderStore
 
-class VideoFolderContainer:
+from ..tools import utils
+
+class VideoContainer:
     def __init__(self,
-                play_video_button, 
-                sample_video_button, 
+                plotter,
+                play_video_button,
                 hintLabel, 
                 register_pose,
                 current_pose,
                 add_image,
-                add_folder,
+                load_mask,
                 clear_plot,
                 output_text):
         
+        self.plotter = plotter
         self.play_video_button = play_video_button
-        self.sample_video_button = sample_video_button
         self.hintLabel = hintLabel
         self.register_pose = register_pose
         self.current_pose = current_pose
         self.add_image = add_image
-        self.add_folder = add_folder
+        self.load_mask = load_mask
         self.clear_plot = clear_plot
         self.output_text = output_text
         
         self.image_store = ImageStore()
+        self.mask_store = MaskStore()
+        self.bbox_store = BboxStore()
         self.mesh_store = MeshStore()
         self.video_store = VideoStore()
         self.folder_store = FolderStore()
   
     def add_video_file(self, video_path='', prompt=False):
         if prompt:
             video_path, _ = QtWidgets.QFileDialog().getOpenFileName(None, "Open file", "", "Files (*.avi *.mp4 *.mkv *.mov *.fly *.wmv *.mpeg *.asf *.webm)")
         if video_path:
             if self.folder_store.folder_path: self.clear_plot() # main goal is to set folder_path to None
             self.hintLabel.hide()
             self.video_store.add_video(video_path)
             self.play_video_button.setEnabled(True)
-            self.sample_video_button.setEnabled(True)
             self.play_video_button.setText(f"Play ({self.video_store.current_frame}/{self.video_store.total_frame})")
             self.output_text.append(f"-> Load video {self.video_store.video_path} into vision6D")
             self.output_text.append(f"\n************************************************************\n")
             self.load_per_frame_info()
             self.sample_video()
 
     def load_per_frame_info(self):
         video_frame = self.video_store.load_per_frame_info()
         if video_frame is not None: 
             self.add_image(video_frame)
             return video_frame
         else: 
             return None
                 
-    def save_frame(self):
+    def sample_video(self):
+        if self.video_store.video_path: 
+            self.video_store.sample_video()
+        else: 
+            QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+
+    def play_video(self):
         if self.video_store.video_path:
-            video_frame = self.load_per_frame_info()
-            if video_frame is not None:
-                os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D", exist_ok=True)
+            self.video_store.play_video()
+            self.play_video_button.setText(f"Play ({self.video_store.current_frame}/{self.video_store.total_frame})")
+            self.load_per_frame_info()
+        else: QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+    
+    def save_info(self):
+        if self.video_store.video_path:
+            os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D", exist_ok=True)
+            # save each frame
+            if self.image_store.image_actor is not None:
                 os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "frames", exist_ok=True)
                 output_frame_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "frames" / f"frame_{self.video_store.current_frame}.png"
-                save_frame = PIL.Image.fromarray(video_frame)
-                
-                # save each frame
+                image_rendered = self.image_store.render_image(camera=self.plotter.camera.copy())
+                save_frame = PIL.Image.fromarray(image_rendered)
                 save_frame.save(output_frame_path)
-                self.output_text.append(f"-> Save frame {self.video_store.current_frame}: ({self.video_store.current_frame}/{self.video_store.total_frame}) to <span style='background-color:yellow; color:black;'>{str(output_frame_path)}</span>")
-                self.output_text.append(f"\n************************************************************\n")
                 self.image_store.image_path = str(output_frame_path)
-
-                # save gt_pose for each frame
+                self.output_text.append(f"-> Save frame {self.video_store.current_frame} to {str(output_frame_path)}")
+                self.output_text.append(f"\n************************************************************\n")
+        
+            # save gt_pose for each frame if there are any meshes
+            if len(self.mesh_store.mesh_actors) > 0:
                 os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "poses", exist_ok=True)
                 output_pose_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "poses" / f"pose_{self.video_store.current_frame}.npy"
                 self.current_pose()
                 np.save(output_pose_path, self.mesh_store.transformation_matrix)
-                self.output_text.append(f"-> Save frame {self.video_store.current_frame} pose to <span style='background-color:yellow; color:black;'>{str(output_pose_path)}</span>:")
+                self.output_text.append(f"-> Save frame {self.video_store.current_frame} pose to {str(output_pose_path)}:")
                 self.output_text.append(f"{self.mesh_store.transformation_matrix}")
                 self.output_text.append(f"\n************************************************************\n")
-        elif self.folder_store.folder_path:
-            # save gt_pose for specific frame
-            os.makedirs(pathlib.Path(self.folder_store.folder_path) / "vision6D", exist_ok=True)
-            os.makedirs(pathlib.Path(self.folder_store.folder_path) / "vision6D" / "poses", exist_ok=True)
-            output_pose_path = pathlib.Path(self.folder_store.folder_path) / "vision6D" / "poses" / f"{pathlib.Path(self.mesh_store.pose_path).stem}.npy"
-            self.current_pose()
-            np.save(output_pose_path, self.mesh_store.transformation_matrix)
-            self.output_text.append(f"-> Save frame {pathlib.Path(self.mesh_store.pose_path).stem} pose to <span style='background-color:yellow; color:black;'>{str(output_pose_path)}</span>:")
-            self.output_text.append(f"{self.mesh_store.transformation_matrix}")
-            self.output_text.append(f"\n************************************************************\n")
-        else: 
-            QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video or a folder!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
-    def sample_video(self):
-        if self.video_store.video_path: 
-            self.video_store.sample_video()
+            # save mask if there is a mask  
+            if self.mask_store.mask_actor is not None:
+                os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "masks", exist_ok=True)
+                output_mask_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "masks" / f"mask_{self.video_store.current_frame}.png"
+                mask_surface = self.mask_store.update_mask()
+                self.load_mask(mask_surface)
+                image = self.mask_store.render_mask(camera=self.plotter.camera.copy())
+                rendered_image = PIL.Image.fromarray(image)
+                rendered_image.save(output_mask_path)
+                self.mask_store.mask_path = output_mask_path
+                self.output_text.append(f"-> Save frame {self.video_store.current_frame} mask render to {output_mask_path}")
+                self.output_text.append(f"\n************************************************************\n")
+
+            # save bbox if there is a bbox  
+            if self.bbox_store.bbox_actor is not None:
+                os.makedirs(pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "bboxs", exist_ok=True)
+                output_bbox_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "bboxs" / f"bbox_{self.video_store.current_frame}.npy"
+                points = utils.get_bbox_actor_points(self.bbox_store.bbox_actor, self.bbox_store.bbox_bottom_point, self.bbox_store.bbox_offset)
+                np.save(output_bbox_path, points)
+                self.bbox_store.bbox_path = output_bbox_path
+                self.output_text.append(f"-> Save frame {self.video_store.current_frame} bbox points to {output_bbox_path}")
+                self.output_text.append(f"\n************************************************************\n")
+    
         else: 
             QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
-    def play_video(self):
-        if self.video_store.video_path:
-            self.video_store.play_video()
-            self.play_video_button.setText(f"Play ({self.video_store.current_frame}/{self.video_store.total_frame})")
-            self.load_per_frame_info()
-        else: QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-    
-    def prev_frame(self):
+    def prev_info(self):
         if self.video_store.video_path:
             self.video_store.prev_frame()
             pose_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "poses" / f"pose_{self.video_store.current_frame}.npy"
             if os.path.isfile(pose_path): 
                 self.mesh_store.transformation_matrix = np.load(pose_path)
                 self.register_pose(self.mesh_store.transformation_matrix)
                 self.output_text.append(f"-> Load saved frame {self.video_store.current_frame} pose: \n{self.mesh_store.transformation_matrix}")
                 self.output_text.append(f"\n************************************************************\n")
             else: 
                 self.output_text.append(f"-> No saved pose for frame {self.video_store.current_frame}")
                 self.output_text.append(f"\n************************************************************\n")
             self.play_video_button.setText(f"Play ({self.video_store.current_frame}/{self.video_store.total_frame})")
             self.load_per_frame_info()
-        elif self.folder_store.folder_path:
-            self.folder_store.prev_frame()
-            self.play_video_button.setText(f"Frame ({self.folder_store.current_frame}/{self.folder_store.total_frame})")
-            self.add_folder(self.folder_store.folder_path)
         else:
-            QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video or folder!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
-    def next_frame(self):
+    def next_info(self):
         if self.video_store.video_path:
-            self.save_frame()
+            self.save_info()
             self.video_store.next_frame()
             # load pose for the current frame if the pose exist
             pose_path = pathlib.Path(self.video_store.video_path).parent / f"{pathlib.Path(self.video_store.video_path).stem}_vision6D" / "poses" / f"pose_{self.video_store.current_frame}.npy"
             if os.path.isfile(pose_path): 
                 self.mesh_store.transformation_matrix = np.load(pose_path)
                 self.register_pose(self.mesh_store.transformation_matrix)
                 self.output_text.append(f"-> Load saved frame {self.video_store.current_frame} pose: \n{self.mesh_store.transformation_matrix}")
                 self.output_text.append(f"\n************************************************************\n")
             self.play_video_button.setText(f"Play ({self.video_store.current_frame}/{self.video_store.total_frame})")
             self.load_per_frame_info()
-        elif self.folder_store.folder_path:
-            self.folder_store.next_frame()
-            self.play_video_button.setText(f"Frame ({self.folder_store.current_frame}/{self.folder_store.total_frame})")
-            self.add_folder(self.folder_store.folder_path)
         else:
-            QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video or folder!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            QtWidgets.QMessageBox.warning(QtWidgets.QMainWindow(), 'vision6D', "Need to load a video!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
```

### Comparing `vision6D-0.2.9/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.3.0/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/data/style.qss` & `vision6D-0.3.0/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/entry/main.py` & `vision6D-0.3.0/vision6D/entry/main.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/mainwindow.py` & `vision6D-0.3.0/vision6D/mainwindow.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,27 +23,32 @@
 from pyvistaqt import MainWindow
 from PyQt5.QtCore import Qt, QPoint
 
 # self defined package import
 from .widgets import CustomQtInteractor
 from .widgets import PopUpDialog
 
+from .components import CameraStore
 from .components import ImageStore
 from .components import MaskStore
-from .components import CameraStore
+from .components import BboxStore
 from .components import MeshStore
+from .components import PointStore
 from .components import VideoStore
 from .components import FolderStore
 
 from .containers import CameraContainer
 from .containers import ImageContainer
 from .containers import MaskContainer
+from .containers import BboxContainer
 from .containers import MeshContainer
+from .containers import PointContainer
 from .containers import PnPContainer
-from .containers import VideoFolderContainer
+from .containers import VideoContainer
+from .containers import FolderContainer
 
 np.set_printoptions(suppress=True)
 
 class MyMainWindow(MainWindow):
     def __init__(self, parent=None):
         QtWidgets.QMainWindow.__init__(self, parent)
         
@@ -55,26 +60,27 @@
         self.setAcceptDrops(True)
 
         # Initialize
         self.workspace_path = ''
         self.track_actors_names = []
         self.button_group_actors_names = QtWidgets.QButtonGroup(self)
 
+        self.camera_store = CameraStore(self.window_size)
         self.image_store = ImageStore()
         self.mask_store = MaskStore()
-        self.camera_store = CameraStore(self.window_size)
+        self.bbox_store = BboxStore()
         self.mesh_store = MeshStore(self.window_size)
+        self.point_store = PointStore()
         self.video_store = VideoStore()
         self.folder_store = FolderStore()
 
         # Create widgets
         self.color_button = QtWidgets.QPushButton("Color")
         self.color_button.clicked.connect(self.show_color_popup)
         self.play_video_button = QtWidgets.QPushButton("Play Video")
-        self.sample_video_button = QtWidgets.QPushButton("Sample Video")
         self.opacity_spinbox = QtWidgets.QDoubleSpinBox()
         self.opacity_spinbox.setMinimum(0.0)
         self.opacity_spinbox.setMaximum(1.0)
         self.opacity_spinbox.setDecimals(2)
         self.opacity_spinbox.setSingleStep(0.05)
         self.opacity_spinbox.setValue(0.3)
         self.opacity_spinbox.valueChanged.connect(self.opacity_value_change)
@@ -132,41 +138,63 @@
         self.mask_container = MaskContainer(plotter=self.plotter,
                                             hintLabel=self.hintLabel, 
                                             track_actors_names=self.track_actors_names, 
                                             add_button_actor_name=self.add_button_actor_name, 
                                             check_button=self.check_button, 
                                             output_text=self.output_text)
         
+        self.point_container = PointContainer(plotter=self.plotter,
+                                            hintLabel=self.hintLabel,
+                                            track_actors_names=self.track_actors_names, 
+                                            add_button_actor_name=self.add_button_actor_name,
+                                            output_text=self.output_text,
+                                            )
+        
         self.mesh_container = MeshContainer(color_button=self.color_button,
                                             plotter=self.plotter,
                                             hintLabel=self.hintLabel,
                                             track_actors_names=self.track_actors_names,
                                             add_button_actor_name=self.add_button_actor_name,
                                             button_group_actors_names=self.button_group_actors_names,
                                             check_button=self.check_button,
                                             opacity_spinbox=self.opacity_spinbox,
                                             opacity_value_change=self.opacity_value_change,
                                             reset_camera=self.camera_container.reset_camera,
                                             current_pose=self.current_pose,
                                             register_pose=self.register_pose,
+                                            load_mask = self.mask_container.load_mask,
                                             output_text=self.output_text)
         
         self.pnp_container = PnPContainer(plotter=self.plotter,
                                         export_mesh_render=self.mesh_container.export_mesh_render,
                                         output_text=self.output_text)
         
-        self.video_folder_container = VideoFolderContainer(play_video_button=self.play_video_button, 
-                                                        sample_video_button=self.sample_video_button, 
-                                                        hintLabel=self.hintLabel, 
-                                                        register_pose=self.register_pose,
-                                                        current_pose=self.current_pose,
-                                                        add_image=self.image_container.add_image,
-                                                        add_folder=self.add_folder,
-                                                        clear_plot=self.clear_plot,
-                                                        output_text=self.output_text)
+        self.video_container = VideoContainer(plotter=self.plotter,
+                                            play_video_button=self.play_video_button, 
+                                            hintLabel=self.hintLabel, 
+                                            register_pose=self.register_pose,
+                                            current_pose=self.current_pose,
+                                            add_image=self.image_container.add_image,
+                                            load_mask=self.mask_container.load_mask,
+                                            clear_plot=self.clear_plot,
+                                            output_text=self.output_text)
+        
+        self.folder_container = FolderContainer(plotter=self.plotter,
+                                                play_video_button=self.play_video_button, 
+                                                current_pose=self.current_pose,
+                                                add_folder=self.add_folder,
+                                                load_mask=self.mask_container.load_mask,
+                                                output_text=self.output_text)
+        
+        self.bbox_container = BboxContainer(plotter=self.plotter,
+                                            hintLabel=self.hintLabel, 
+                                            track_actors_names=self.track_actors_names, 
+                                            add_button_actor_name=self.add_button_actor_name, 
+                                            check_button=self.check_button, 
+                                            output_text=self.output_text)
 
     def key_bindings(self):
         # Camera related key bindings
         QtWidgets.QShortcut(QtGui.QKeySequence("c"), self).activated.connect(self.camera_container.reset_camera)
         QtWidgets.QShortcut(QtGui.QKeySequence("z"), self).activated.connect(self.camera_container.zoom_out)
         QtWidgets.QShortcut(QtGui.QKeySequence("x"), self).activated.connect(self.camera_container.zoom_in)
 
@@ -179,25 +207,32 @@
         QtWidgets.QShortcut(QtGui.QKeySequence("n"), self).activated.connect(lambda up=False: self.image_container.toggle_image_opacity(up))
 
         # Mask related key bindings
         QtWidgets.QShortcut(QtGui.QKeySequence("t"), self).activated.connect(self.mask_container.reset_mask)
         QtWidgets.QShortcut(QtGui.QKeySequence("g"), self).activated.connect(lambda up=True: self.mask_container.toggle_mask_opacity(up))
         QtWidgets.QShortcut(QtGui.QKeySequence("h"), self).activated.connect(lambda up=False: self.mask_container.toggle_mask_opacity(up))
 
+        # Bbox related key bindings
+        QtWidgets.QShortcut(QtGui.QKeySequence("f"), self).activated.connect(self.bbox_container.reset_bbox)
+
         # Mesh related key bindings 
         QtWidgets.QShortcut(QtGui.QKeySequence("k"), self).activated.connect(self.mesh_container.reset_gt_pose)
         QtWidgets.QShortcut(QtGui.QKeySequence("l"), self).activated.connect(self.mesh_container.update_gt_pose)
         QtWidgets.QShortcut(QtGui.QKeySequence("s"), self).activated.connect(self.mesh_container.undo_pose)
         QtWidgets.QShortcut(QtGui.QKeySequence("y"), self).activated.connect(lambda up=True: self.mesh_container.toggle_surface_opacity(up))
         QtWidgets.QShortcut(QtGui.QKeySequence("u"), self).activated.connect(lambda up=False: self.mesh_container.toggle_surface_opacity(up))
 
-        # Video Folder related key bindings 
-        QtWidgets.QShortcut(QtGui.QKeySequence("Right"), self).activated.connect(self.video_folder_container.next_frame)
-        QtWidgets.QShortcut(QtGui.QKeySequence("Left"), self).activated.connect(self.video_folder_container.prev_frame)
-        QtWidgets.QShortcut(QtGui.QKeySequence("Space"), self).activated.connect(self.video_folder_container.play_video)
+        # Video related key bindings 
+        QtWidgets.QShortcut(QtGui.QKeySequence("Right"), self).activated.connect(self.video_container.next_info)
+        QtWidgets.QShortcut(QtGui.QKeySequence("Left"), self).activated.connect(self.video_container.prev_info)
+        QtWidgets.QShortcut(QtGui.QKeySequence("Space"), self).activated.connect(self.video_container.play_video)
+
+        # Folder related key bindings 
+        QtWidgets.QShortcut(QtGui.QKeySequence("a"), self).activated.connect(self.folder_container.prev_info)
+        QtWidgets.QShortcut(QtGui.QKeySequence("d"), self).activated.connect(self.folder_container.next_info)
 
     def showMaximized(self):
         super(MyMainWindow, self).showMaximized()
 
     def dragEnterEvent(self, e):
         if e.mimeData().hasUrls():
             e.accept()
@@ -213,15 +248,15 @@
                 # Load workspace json file
                 if file_path.endswith(('.json')): self.add_workspace(workspace_path=file_path)
                 # Load mesh file
                 elif file_path.endswith(('.mesh', '.ply', '.stl', '.obj', '.off', '.dae', '.fbx', '.3ds', '.x3d')):
                     self.mesh_container.add_mesh_file(mesh_path=file_path)
                 # Load video file
                 elif file_path.endswith(('.avi', '.mp4', '.mkv', '.mov', '.fly', '.wmv', '.mpeg', '.asf', '.webm')):
-                    self.video_folder_container.add_video_file(video_path=file_path)
+                    self.video_container.add_video_file(video_path=file_path)
                 # Load image/mask file
                 elif file_path.endswith(('.png', '.jpg', 'jpeg', '.tiff', '.bmp', '.webp', '.ico')):  # add image/mask
                     file_data = np.array(PIL.Image.open(file_path).convert('L'), dtype='uint8')
                     unique, _ = np.unique(file_data, return_counts=True)
                     if len(unique) == 2: self.mask_container.add_mask_file(mask_path=file_path)
                     else: self.image_container.add_image_file(image_path=file_path) 
                         
@@ -240,50 +275,66 @@
     def set_menu_bars(self):
         mainMenu = self.menuBar()
         
         # allow to add files
         fileMenu = mainMenu.addMenu('File')
         fileMenu.addAction('Add Workspace', functools.partial(self.add_workspace, prompt=True))
         fileMenu.addAction('Add Folder', functools.partial(self.add_folder, prompt=True))
-        fileMenu.addAction('Add Video', functools.partial(self.video_folder_container.add_video_file, prompt=True))
+        fileMenu.addAction('Add Video', functools.partial(self.video_container.add_video_file, prompt=True))
         fileMenu.addAction('Add Image', functools.partial(self.image_container.add_image_file, prompt=True))
         fileMenu.addAction('Add Mask', functools.partial(self.mask_container.add_mask_file, prompt=True))
+        fileMenu.addAction('Add Bbox', functools.partial(self.bbox_container.add_bbox_file, prompt=True))
         fileMenu.addAction('Add Mesh', functools.partial(self.mesh_container.add_mesh_file, prompt=True))
-        fileMenu.addAction('Draw Mask', self.mask_container.draw_mask)
+        fileMenu.addAction('Add Points', functools.partial(self.point_container.load_points_file, prompt=True))
         fileMenu.addAction('Clear', self.clear_plot)
 
         # allow to export files
         exportMenu = mainMenu.addMenu('Export')
         exportMenu.addAction('Image', self.image_container.export_image)
         exportMenu.addAction('Mask', self.mask_container.export_mask)
+        exportMenu.addAction('Bbox', self.bbox_container.export_bbox)
         exportMenu.addAction('Pose', self.mesh_container.export_pose)
         exportMenu.addAction('Mesh Render', self.mesh_container.export_mesh_render)
         exportMenu.addAction('SegMesh Render', self.mesh_container.export_segmesh_render)
+
+        # Add draw related actions
+        DrawMenu = mainMenu.addMenu('Draw')
+        DrawMenu.addAction('Mask', self.mask_container.draw_mask)
+        DrawMenu.addAction('BBox', self.bbox_container.draw_bbox)
+        # DrawMenu.addAction('Points', self.point_container.draw_point)
+        DrawMenu.addAction('Reset Mask (t)', self.mask_container.reset_mask)
+        DrawMenu.addAction('Reset Bbox (f)', self.bbox_container.reset_bbox)
         
         # Add video related actions
-        VideoFolderMenu = mainMenu.addMenu('Video/Folder')
-        VideoFolderMenu.addAction('Play', self.video_folder_container.play_video)
-        VideoFolderMenu.addAction('Sample', self.video_folder_container.sample_video)
-        VideoFolderMenu.addAction('Save Frame', self.video_folder_container.save_frame)
-        VideoFolderMenu.addAction('Prev Frame', self.video_folder_container.prev_frame)
-        VideoFolderMenu.addAction('Next Frame', self.video_folder_container.next_frame)
+        VideoMenu = mainMenu.addMenu('Video')
+        VideoMenu.addAction('Play', self.video_container.play_video)
+        VideoMenu.addAction('Sample', self.video_container.sample_video)
+        VideoMenu.addAction('Save', self.video_container.save_info)
+        VideoMenu.addAction('Prev', self.video_container.prev_info)
+        VideoMenu.addAction('Next', self.video_container.next_info)
+
+        # Add folder related actions
+        FolderMenu = mainMenu.addMenu('Folder')
+        FolderMenu.addAction('Save', self.folder_container.save_info)
+        FolderMenu.addAction('Prev', self.folder_container.prev_info)
+        FolderMenu.addAction('Next', self.folder_container.next_info)
 
         # Add camera related actions
         CameraMenu = mainMenu.addMenu('Camera')
         CameraMenu.addAction('Calibrate', self.camera_container.camera_calibrate)
+        CameraMenu.addAction('Set Camera', self.camera_container.set_camera)
         CameraMenu.addAction('Reset Camera (d)', self.camera_container.reset_camera)
         CameraMenu.addAction('Zoom In (x)', self.camera_container.zoom_in)
         CameraMenu.addAction('Zoom Out (z)', self.camera_container.zoom_out)
         
-        # Add register related actions
-        RegisterMenu = mainMenu.addMenu('Register')
-        RegisterMenu.addAction('Reset GT Pose (k)', self.mesh_container.reset_gt_pose)
-        RegisterMenu.addAction('Reset Mask (t)', self.mask_container.reset_mask)
-        RegisterMenu.addAction('Update GT Pose (l)', self.mesh_container.update_gt_pose)
-        RegisterMenu.addAction('Undo Pose (s)', self.mesh_container.undo_pose)
+        # Add pose related actions
+        PoseMenu = mainMenu.addMenu('Pose')
+        PoseMenu.addAction('Reset GT Pose (k)', self.mesh_container.reset_gt_pose)
+        PoseMenu.addAction('Update GT Pose (l)', self.mesh_container.update_gt_pose)
+        PoseMenu.addAction('Undo Pose (s)', self.mesh_container.undo_pose)
 
         # Add pnp algorithm related actions
         PnPMenu = mainMenu.addMenu('PnP')
         PnPMenu.addAction('EPnP with mesh', self.pnp_container.epnp_mesh)
         PnPMenu.addAction('EPnP with nocs mask', functools.partial(self.pnp_container.epnp_mask, True))
         PnPMenu.addAction('EPnP with latlon mask', functools.partial(self.pnp_container.epnp_mask, False))
 
@@ -329,92 +380,60 @@
 
         #* Create the top widgets (layout)
         top_layout = QtWidgets.QHBoxLayout()
         top_layout.setContentsMargins(0, 0, 0, 0)
 
         # Create Grid layout for function buttons
         top_grid_layout = QtWidgets.QGridLayout()
-
-        # Create the set camera button
-        set_camera_button = QtWidgets.QPushButton("Set Camera")
-        set_camera_button.clicked.connect(self.camera_container.set_camera)
-        top_grid_layout.addWidget(set_camera_button, 0, 0)
+        top_grid_layout.addWidget(self.color_button, 0, 0)
+        top_grid_layout.addWidget(self.opacity_spinbox, 0, 1)
 
         # Create the actor pose button
         actor_pose_button = QtWidgets.QPushButton("Set Pose")
         actor_pose_button.clicked.connect(self.mesh_container.set_pose)
-        top_grid_layout.addWidget(actor_pose_button, 0, 1)
+        top_grid_layout.addWidget(actor_pose_button, 0, 2)
 
-        # Create the draw mask button
-        draw_mask_button = QtWidgets.QPushButton("Draw Mask")
-        draw_mask_button.clicked.connect(self.mask_container.draw_mask)
-        top_grid_layout.addWidget(draw_mask_button, 0, 2)
+        # Create the spacing button
+        self.spacing_button = QtWidgets.QPushButton("Spacing")
+        self.spacing_button.clicked.connect(self.mesh_container.set_spacing)
+        top_grid_layout.addWidget(self.spacing_button, 0, 3)
 
-        # Create the video related button
-        self.play_video_button.clicked.connect(self.video_folder_container.play_video)
-        top_grid_layout.addWidget(self.play_video_button, 0, 3)
+        # Create the hide button
+        hide_button = QtWidgets.QPushButton("Toggle Meshes")
+        hide_button.clicked.connect(self.mesh_container.toggle_hide_meshes_button)
+        top_grid_layout.addWidget(hide_button, 1, 0)
+
+        # Create the mirror x button
+        self.mirror_x_button = QtWidgets.QPushButton("Mirror X")
+        self.mirror_x_button.clicked.connect(lambda _, direction="x": self.mirror_actors(direction))
+        top_grid_layout.addWidget(self.mirror_x_button, 1, 1)
+
+        # Create the mirror y button
+        self.mirror_y_button = QtWidgets.QPushButton("Mirror Y")
+        self.mirror_y_button.clicked.connect(lambda _, direction="y": self.mirror_actors(direction))
+        top_grid_layout.addWidget(self.mirror_y_button, 1, 2)
 
-        self.sample_video_button.clicked.connect(self.video_folder_container.sample_video)
-        top_grid_layout.addWidget(self.sample_video_button, 1, 0)
+        # Create the remove button
+        remove_button = QtWidgets.QPushButton("Remove Actor")
+        remove_button.clicked.connect(self.remove_actors_button)
+        top_grid_layout.addWidget(remove_button, 1, 3)
 
-        self.save_frame_button = QtWidgets.QPushButton("Save Frame")
-        self.save_frame_button.clicked.connect(self.video_folder_container.save_frame)
-        top_grid_layout.addWidget(self.save_frame_button, 1, 1)
-
-        self.prev_frame_button = QtWidgets.QPushButton("Prev Frame")
-        self.prev_frame_button.clicked.connect(self.video_folder_container.prev_frame)
-        top_grid_layout.addWidget(self.prev_frame_button, 1, 2)
-
-        self.next_frame_button = QtWidgets.QPushButton("Next Frame")
-        self.next_frame_button.clicked.connect(self.video_folder_container.next_frame)
-        top_grid_layout.addWidget(self.next_frame_button, 1, 3)
+        # Create the video related button
+        self.play_video_button.clicked.connect(self.video_container.play_video)
+        top_grid_layout.addWidget(self.play_video_button, 2, 0)
 
         top_grid_widget = QtWidgets.QWidget()
         top_grid_widget.setLayout(top_grid_layout)
         top_layout.addWidget(top_grid_widget)
         display_layout.addLayout(top_layout)
 
         #* Create the bottom widgets
         actor_widget = QtWidgets.QLabel("Actors")
         display_layout.addWidget(actor_widget)
 
-        actor_grid_layout = QtWidgets.QGridLayout()
-        actor_grid_layout.setContentsMargins(10, 5, 10, 10)
-
-        # Create the color dropdown menu
-        actor_grid_layout.addWidget(self.color_button, 0, 0)
-        
-        actor_grid_layout.addWidget(self.opacity_spinbox, 0, 1)
-
-        # Create the hide button
-        hide_button = QtWidgets.QPushButton("toggle meshes")
-        hide_button.clicked.connect(self.mesh_container.toggle_hide_meshes_button)
-        actor_grid_layout.addWidget(hide_button, 0, 2)
-
-        # Create the remove button
-        remove_button = QtWidgets.QPushButton("Remove Actor")
-        remove_button.clicked.connect(self.remove_actors_button)
-        actor_grid_layout.addWidget(remove_button, 0, 3)
-        display_layout.addLayout(actor_grid_layout)
-
-        # Create the spacing button
-        self.spacing_button = QtWidgets.QPushButton("Spacing")
-        self.spacing_button.clicked.connect(self.mesh_container.set_spacing)
-        actor_grid_layout.addWidget(self.spacing_button, 1, 0)
-
-        # Create the mirror x button
-        self.mirror_x_button = QtWidgets.QPushButton("Mirror X")
-        self.mirror_x_button.clicked.connect(lambda _, direction="x": self.mirror_actors(direction))
-        actor_grid_layout.addWidget(self.mirror_x_button, 1, 1)
-
-        # Create the mirror y button
-        self.mirror_y_button = QtWidgets.QPushButton("Mirror Y")
-        self.mirror_y_button.clicked.connect(lambda _, direction="y": self.mirror_actors(direction))
-        actor_grid_layout.addWidget(self.mirror_y_button, 1, 2)
-
         # Create a scroll area for the buttons
         scroll_area = QtWidgets.QScrollArea()
         scroll_area.setWidgetResizable(True)
         display_layout.addWidget(scroll_area)
 
         # Create a container widget for the buttons
         button_container = QtWidgets.QWidget()
@@ -478,15 +497,15 @@
         self.plotter.enable_trackball_actor_style()
         
         self.plotter.add_axes()
         self.plotter.add_camera_orientation_widget()
 
         self.plotter.show()
         self.show()
-   
+
     def register_pose(self, pose):
         for actor_name, actor in self.mesh_store.mesh_actors.items():
             actor.user_matrix = pose
             self.plotter.add_actor(actor, pickable=True, name=actor_name)
 
     def current_pose(self, text=None, output_text=True):
         self.mesh_store.current_pose()
@@ -504,14 +523,15 @@
             curr_opacity = self.mesh_store.mesh_actors[self.mesh_store.reference].GetProperty().opacity
             self.opacity_spinbox.setValue(curr_opacity)
         else:
             self.color_button.setText("Color")
             if text == 'image': curr_opacity = self.image_store.image_opacity
             elif text == 'mask': curr_opacity = self.mask_store.mask_opacity
             else: curr_opacity = self.opacity_spinbox.value()
+            self.mesh_store.reference = None #* For fixing some bugs in segmesh render function
             self.opacity_spinbox.setValue(curr_opacity)
             
     def check_button(self, actor_name, output_text=True):
         for button in self.button_group_actors_names.buttons():
             if button.text() == actor_name: 
                 button.setChecked(True)
                 self.button_actor_name_clicked(text=actor_name, output_text=output_text)
@@ -575,125 +595,141 @@
             workspace_path, _ = QtWidgets.QFileDialog().getOpenFileName(None, "Open file", "", "Files (*.json)")
         if workspace_path:
             if self.workspace_path: self.clear_plot()
             self.workspace_path = workspace_path
             self.hintLabel.hide()
             with open(str(self.workspace_path), 'r') as f: workspace = json.load(f)
             if 'image_path' in workspace: self.image_container.add_image_file(image_path=workspace['image_path'])
-            if 'video_path' in workspace: self.video_folder_container.add_video_file(video_path=workspace['video_path'])
+            if 'video_path' in workspace: self.video_container.add_video_file(video_path=workspace['video_path'])
             if 'mask_path' in workspace: self.mask_container.add_mask_file(mask_path=workspace['mask_path'])
+            if 'bbox_path' in workspace: self.bbox_container.add_bbox_file(bbox_path=workspace['bbox_path'])
             # need to load pose before loading meshes
             if 'pose_path' in workspace: self.mesh_container.add_pose_file(pose_path=workspace['pose_path'])
             if 'mesh_path' in workspace:
                 mesh_paths = workspace['mesh_path']
                 for path in mesh_paths: self.mesh_container.add_mesh_file(mesh_path=path)
             
             # reset camera
             self.camera_container.reset_camera()
 
     def add_folder(self, folder_path='', prompt=False):
         if prompt: 
             folder_path = QtWidgets.QFileDialog.getExistingDirectory(self, "Select Folder")
         if folder_path:
             if self.video_store.video_path or self.workspace_path: self.clear_plot() # main goal is to set video_path to None
-            image_path, mask_path, pose_path, mesh_path = self.folder_store.add_folder(folder_path=folder_path)
+            image_path, mask_path, pose_path, mesh_path = self.folder_store.add_folder(folder_path=folder_path, mesh_actors=self.mesh_store.mesh_actors)
             if image_path or mask_path or pose_path or mesh_path:
                 if image_path: self.image_container.add_image_file(image_path=image_path)
                 if mask_path: self.mask_container.add_mask_file(mask_path=mask_path)
                 if pose_path: self.mesh_container.add_pose_file(pose_path=pose_path)
                 if mesh_path: 
                     with open(mesh_path, 'r') as f: mesh_path = f.read().splitlines()
                     for path in mesh_path: self.mesh_container.add_mesh_file(path)
                 self.play_video_button.setEnabled(False)
-                self.sample_video_button.setEnabled(False)
-                self.play_video_button.setText(f"Frame ({self.folder_store.current_frame}/{self.folder_store.total_frame})")
+                self.play_video_button.setText(f"Image ({self.folder_store.current_image}/{self.folder_store.total_image})")
                 self.camera_container.reset_camera()
             else:
                 self.folder_store.reset()
                 QtWidgets.QMessageBox.warning(self, 'vision6D', "Not a valid folder, please reload a folder", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def mirror_actors(self, direction):
         checked_button = self.button_group_actors_names.checkedButton()
         if checked_button:
             actor_name = checked_button.text()
             if actor_name == 'image':
                 self.image_container.mirror_image(direction)
             elif actor_name == 'mask':
                 self.mask_container.mirror_mask(direction)
+            elif actor_name == 'bbox':
+                self.bbox_container.mirror_bbox(direction)
             elif actor_name in self.mesh_store.mesh_actors:
                 self.mesh_container.mirror_mesh(direction)
         else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def remove_actor(self, button):
         name = button.text()
         if name == 'image': 
             actor = self.image_store.image_actor
             self.image_store.reset()
         elif name == 'mask':
             actor = self.mask_store.mask_actor
             self.mask_store.reset()
+        elif name == 'bbox':
+            actor = self.bbox_store.bbox_actor
+            self.bbox_store.reset()
         elif name in self.mesh_store.mesh_actors: 
             actor = self.mesh_store.mesh_actors[name]
             self.mesh_store.remove_mesh(name)
             self.color_button.setText("Color")
+        elif name in self.point_store.point_actors:
+            actor = self.point_store.point_actors[name]
+            self.point_store.remove_point(name)
 
         self.plotter.remove_actor(actor)
         self.track_actors_names.remove(name)
         # remove the button from the button group
         self.button_group_actors_names.removeButton(button)
         # remove the button from the self.button_layout widget
         self.button_layout.removeWidget(button)
         # offically delete the button
         button.deleteLater()
 
         # clear out the plot if there is no actor
-        if self.image_store.image_actor is None and self.mask_store.mask_actor is None and len(self.mesh_store.mesh_actors) == 0: self.clear_plot()
+        if (self.image_store.image_actor is None) and (self.mask_store.mask_actor is None) and (len(self.mesh_store.mesh_actors) == 0) and (len(self.point_store.point_actors) == 0): 
+            self.clear_plot()
 
     def remove_actors_button(self):
         checked_button = self.button_group_actors_names.checkedButton()
         if checked_button: self.remove_actor(checked_button)
         else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
     def clear_plot(self):
         # Clear out everything in the remove menu
         for button in self.button_group_actors_names.buttons():
             name = button.text()
-            if name == 'image': actor = self.image_store.image_actor
-            elif name == 'mask': actor = self.mask_store.mask_actor
+            if name == 'image': 
+                actor = self.image_store.image_actor
+                self.image_store.reset()
+                self.image_store.mirror_x = False
+                self.image_store.mirror_y = False
+            elif name == 'mask': 
+                actor = self.mask_store.mask_actor
+                self.mask_store.reset()
+                self.mask_store.mirror_x = False
+                self.mask_store.mirror_y = False
+            elif name == 'bbox':
+                actor = self.bbox_store.bbox_actor
+                self.bbox_store.reset()
+                self.bbox_store.mirror_x = False
+                self.bbox_store.mirror_y = False
             elif name in self.mesh_store.mesh_actors: 
                 actor = self.mesh_store.mesh_actors[name]
                 self.mesh_store.remove_mesh(name)
                 self.color_button.setText("Color")
+            elif name in self.point_store.point_actors:
+                actor = self.point_store.point_actors[name]
+                self.point_store.remove_point(name)
+
             self.plotter.remove_actor(actor)
             # remove the button from the button group
             self.button_group_actors_names.removeButton(button)
             # remove the button from the self.button_layout widget
             self.button_layout.removeWidget(button)
             # offically delete the button
             button.deleteLater()
 
-        self.image_store.reset()
-        self.image_store.mirror_x = False
-        self.image_store.mirror_y = False
-
-        self.mask_store.reset()
-        self.mask_store.mirror_x = False
-        self.mask_store.mirror_y = False
-
         self.mesh_store.reset()
-
+        self.point_store.reset()
         self.video_store.reset()
         self.folder_store.reset()
-
-        # Re-initial the dictionaries
         self.workspace_path = ''
         self.track_actors_names.clear()
+        self.clear_output_text()
 
         self.color_button.setText("Color")
         self.play_video_button.setText("Play Video")
         self.opacity_spinbox.setValue(0.3)
-        self.clear_output_text()
-
+        
         self.hintLabel.show()
```

### Comparing `vision6D-0.2.9/vision6D/tools/utils.py` & `vision6D-0.3.0/vision6D/tools/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -380,14 +380,29 @@
     points = (matrix[:3, :3] @ points_array.T).T + matrix[:3, 3:].T
     # Calculate points with homogeneous coordinates
     homogeneous_points = np.hstack((points_array, np.ones((points_array.shape[0], 1))))
     transformed_points = ((matrix @ homogeneous_points.T).T)[:, :3]
     assert np.isclose(transformed_points, points).all(), "points and transformed_points should be very very close!"
     return transformed_points
 
+def get_bbox_actor_points(actor, bbox_bottom_point, bbox_offset):
+    input = actor.GetMapper().GetInput()
+    point_data = input.GetPoints().GetData()
+    points_array = vtknp.vtk_to_numpy(point_data)
+    vtk_matrix = actor.GetMatrix()
+    matrix = np.array([[vtk_matrix.GetElement(i, j) for j in range(4)] for i in range(4)])
+    # Calculate points not with homogeneous form
+    points = (matrix[:3, :3] @ points_array.T).T + matrix[:3, 3:].T
+    # Calculate points with homogeneous coordinates
+    homogeneous_points = np.hstack((points_array, np.ones((points_array.shape[0], 1))))
+    transformed_points = ((matrix @ homogeneous_points.T).T)[:, :3]
+    assert np.isclose(transformed_points, points).all(), "points and transformed_points should be very very close!"
+    points = points + bbox_bottom_point - bbox_offset
+    return points
+
 def get_mesh_actor_vertices_faces(actor):
     input = actor.GetMapper().GetInput()
     points = input.GetPoints().GetData()
     cells = input.GetPolys().GetData()
     vertices = vtknp.vtk_to_numpy(points)
     """
     # popular presentation
```

### Comparing `vision6D-0.2.9/vision6D/widgets/__init__.py` & `vision6D-0.3.0/vision6D/widgets/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from .calibration_pop_window import CalibrationPopWindow
 from .camera_props_input_dialog import CameraPropsInputDialog
 from .custom_qt_interactor import CustomQtInteractor
 from .get_text_dialog import GetTextDialog
-from .label_window import LabelWindow
+from .draw_mask_window import MaskWindow
+from .draw_bbox_window import BboxWindow
 from .popup_dialog import PopUpDialog
 from .video_player import VideoPlayer
 from .video_sampler import VideoSampler
 
 __all__ = [
     'CalibrationPopWindow',
     'CameraPropsInputDialog',
     'CustomQtInteractor',
     'GetTextDialog',
-    'LabelWindow',
+    'MaskWindow',
+    'BboxWindow',
     'PopUpDialog',
     'VideoPlayer',
     'VideoSampler',
 ]
```

### Comparing `vision6D-0.2.9/vision6D/widgets/calibration_pop_window.py` & `vision6D-0.3.0/vision6D/widgets/calibration_pop_window.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/widgets/camera_props_input_dialog.py` & `vision6D-0.3.0/vision6D/widgets/camera_props_input_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/widgets/custom_qt_interactor.py` & `vision6D-0.3.0/vision6D/widgets/custom_qt_interactor.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,35 +10,36 @@
 
 import vtk
 from pyvistaqt import QtInteractor
 
 class CustomQtInteractor(QtInteractor):
     def __init__(self, parent=None, main_window=None):
         super().__init__(parent)
-        # Save main_window
         self.main_window = main_window
+        self.cell_picker = None
 
     def mousePressEvent(self, event):
         super().mousePressEvent(event)
         if event.button() == 1 or event.button() == 4:  # Left or middle mouse button
             self.press_callback(self.iren.interactor)
 
     def mouseReleaseEvent(self, event):
         super().mouseReleaseEvent(event)
         if event.button() == 1 or event.button() == 4:  # Left or middle mouse button
-            if self.picker: self.release_callback()
+            self.release_callback()
             
     def press_callback(self, obj, *args):
         x, y = obj.GetEventPosition()
-        picker = vtk.vtkCellPicker()
-        if picker.Pick(x, y, 0, self.renderer): self.picker = picker
-        else: 
-            self.picker = None
+        cell_picker = vtk.vtkCellPicker()
+        if cell_picker.Pick(x, y, 0, self.renderer): 
+            self.cell_picker = cell_picker
+        else:
             if self.main_window.image_store.image_actor: 
                 self.main_window.check_button('image')
 
     def release_callback(self):
-        picked_actor = self.picker.GetActor()
-        actor_name = picked_actor.name
-        if (actor_name in self.main_window.mesh_store.mesh_actors) or (actor_name == 'mask'):
-            # check the picked mesh button and register the rest to the mesh reference's current pose
-            self.main_window.check_button(actor_name)
+        if self.cell_picker: 
+            picked_actor = self.cell_picker.GetActor()
+            actor_name = picked_actor.name
+            if (actor_name in self.main_window.mesh_store.mesh_actors) or (actor_name == 'mask'):
+                self.main_window.check_button(actor_name)
+        self.cell_picker = None
```

### Comparing `vision6D-0.2.9/vision6D/widgets/get_text_dialog.py` & `vision6D-0.3.0/vision6D/widgets/get_text_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/widgets/label_window.py` & `vision6D-0.3.0/vision6D/widgets/draw_mask_window.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
 @author: Yike (Nicole) Zhang
 @license: (C) Copyright.
 @contact: yike.zhang@vanderbilt.edu
 @software: Vision6D
-@file: label_window.py
+@file: draw_mask_window.py
 @time: 2023-07-03 20:32
 @desc: create the window for mask labeling/drawing
 '''
 
 # General import
 import numpy as np
 import cv2
@@ -17,15 +17,15 @@
 # Qt5 import
 from PyQt5 import QtWidgets, QtGui, QtCore
 from PyQt5.QtCore import Qt
 
 # self defined package import
 np.set_printoptions(suppress=True)
 
-class LabelImage(QtWidgets.QLabel):
+class MaskLabel(QtWidgets.QLabel):
     output_path_changed = QtCore.pyqtSignal(str)
     def __init__(self, pixmap):
         super().__init__()
         self.setFocusPolicy(Qt.StrongFocus)
         self.setPixmap(pixmap)
         self.setContentsMargins(0, 0, 0, 0)
         
@@ -70,26 +70,28 @@
             if (QtCore.QLineF(self.points.first(), self.points.last()).length() < 10) and (self.points.first() != self.points.last()):
                 complete_points.append(self.points.first())
             # Draw the first point with a larger radius
             painter.setBrush(QtGui.QBrush(QtGui.QColor(0, 0, 255)))
             painter.drawEllipse(self.points.point(0), 2, 2)
             painter.drawPolyline(complete_points)
 
-class LabelWindow(QtWidgets.QWidget):
+class MaskWindow(QtWidgets.QWidget):
     def __init__(self, image_source):
         super().__init__()
-        image_source = np.array(PIL.Image.open(image_source), dtype='uint8')
+        if isinstance(image_source, pathlib.WindowsPath) or isinstance(image_source, str):
+            image_source = np.array(PIL.Image.open(image_source), dtype='uint8')
         image = QtGui.QImage(image_source.tobytes(), image_source.shape[1], image_source.shape[0], image_source.shape[2]*image_source.shape[1], QtGui.QImage.Format_RGB888)
         pixmap = QtGui.QPixmap.fromImage(image)
         self.setFixedSize(pixmap.size())
 
         layout = QtWidgets.QVBoxLayout()
 
         #* setContentsMargins sets the width of the outside border around the layout
         layout.setContentsMargins(0, 0, 0, 0)
         #* setSpacing sets the width of the inside border between widgets in the layout.
         layout.setSpacing(0)
         #* Both are set to zero to eliminate any space between the widgets and the layout border.
 
-        self.image_label = LabelImage(pixmap)
-        layout.addWidget(self.image_label)
-        self.setLayout(layout)
+        self.mask_label = MaskLabel(pixmap)
+        layout.addWidget(self.mask_label)
+        self.setLayout(layout)
+        self.show()
```

### Comparing `vision6D-0.2.9/vision6D/widgets/popup_dialog.py` & `vision6D-0.3.0/vision6D/widgets/popup_dialog.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/widgets/video_player.py` & `vision6D-0.3.0/vision6D/widgets/video_player.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D/widgets/video_sampler.py` & `vision6D-0.3.0/vision6D/widgets/video_sampler.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.2.9/vision6D.egg-info/PKG-INFO` & `vision6D-0.3.0/vision6D.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.2.9
+Version: 0.3.0
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzyk/vision6D
 License: GNU GENERAL Public License
 Project-URL: Documentation, https://vision6d.readthedocs.io/en/latest/
 Keywords: 6D,pose estimation,registration,segmentation,tool
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.2.9/vision6D.egg-info/SOURCES.txt` & `vision6D-0.3.0/vision6D.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,42 @@
 vision6D.egg-info/PKG-INFO
 vision6D.egg-info/SOURCES.txt
 vision6D.egg-info/dependency_links.txt
 vision6D.egg-info/entry_points.txt
 vision6D.egg-info/requires.txt
 vision6D.egg-info/top_level.txt
 vision6D/components/__init__.py
+vision6D/components/bbox_store.py
 vision6D/components/camera_store.py
 vision6D/components/folder_store.py
 vision6D/components/image_store.py
 vision6D/components/mask_store.py
 vision6D/components/mesh_store.py
+vision6D/components/point_store.py
 vision6D/components/singleton.py
 vision6D/components/video_store.py
 vision6D/containers/__init__.py
+vision6D/containers/bbox_container.py
 vision6D/containers/camera_container.py
+vision6D/containers/folder_container.py
 vision6D/containers/image_container.py
 vision6D/containers/mask_container.py
 vision6D/containers/mesh_container.py
 vision6D/containers/pnp_container.py
-vision6D/containers/video_folder_container.py
+vision6D/containers/point_container.py
+vision6D/containers/video_container.py
 vision6D/data/ossiclesCoordinateMapping.json
 vision6D/data/style.qss
 vision6D/entry/__init__.py
 vision6D/entry/main.py
 vision6D/tools/__init__.py
 vision6D/tools/utils.py
 vision6D/widgets/__init__.py
 vision6D/widgets/calibration_pop_window.py
 vision6D/widgets/camera_props_input_dialog.py
 vision6D/widgets/custom_qt_interactor.py
+vision6D/widgets/draw_bbox_window.py
+vision6D/widgets/draw_mask_window.py
 vision6D/widgets/get_text_dialog.py
-vision6D/widgets/label_window.py
 vision6D/widgets/popup_dialog.py
 vision6D/widgets/video_player.py
 vision6D/widgets/video_sampler.py
```

