# Comparing `tmp/wf-cv-utils-3.4.0.tar.gz` & `tmp/wf-cv-utils-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-cv-utils-3.4.0.tar", last modified: Mon Jan 31 20:43:53 2022, max compression
+gzip compressed data, was "wf-cv-utils-3.5.0.tar", last modified: Sun Jul 16 13:25:21 2023, max compression
```

## Comparing `wf-cv-utils-3.4.0.tar` & `wf-cv-utils-3.5.0.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 btalberg   (501) staff       (20)        0 2022-01-31 20:43:53.164087 wf-cv-utils-3.4.0/
--rw-r--r--   0 btalberg   (501) staff       (20)      273 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/.gitignore
--rw-r--r--   0 btalberg   (501) staff       (20)     1088 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/LICENSE
--rw-r--r--   0 btalberg   (501) staff       (20)       34 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/MANIFEST.in
--rw-r--r--   0 btalberg   (501) staff       (20)      426 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/Makefile
--rw-r--r--   0 btalberg   (501) staff       (20)     1999 2022-01-31 20:43:53.163947 wf-cv-utils-3.4.0/PKG-INFO
--rw-r--r--   0 btalberg   (501) staff       (20)     1495 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/README.md
--rw-r--r--   0 btalberg   (501) staff       (20)        5 2022-01-31 20:41:30.000000 wf-cv-utils-3.4.0/VERSION
-drwxr-xr-x   0 btalberg   (501) staff       (20)        0 2022-01-31 20:43:53.159832 wf-cv-utils-3.4.0/cv_utils/
--rw-r--r--   0 btalberg   (501) staff       (20)      168 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/cv_utils/__init__.py
--rw-r--r--   0 btalberg   (501) staff       (20)      327 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/cv_utils/color.py
--rw-r--r--   0 btalberg   (501) staff       (20)    29498 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/cv_utils/core.py
-drwxr-xr-x   0 btalberg   (501) staff       (20)        0 2022-01-31 20:43:53.161836 wf-cv-utils-3.4.0/cv_utils/drawing/
--rw-r--r--   0 btalberg   (501) staff       (20)        0 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/cv_utils/drawing/__init__.py
--rw-r--r--   0 btalberg   (501) staff       (20)     4150 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/cv_utils/drawing/matplotlib.py
--rw-r--r--   0 btalberg   (501) staff       (20)    11003 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/cv_utils/drawing/opencv.py
--rw-r--r--   0 btalberg   (501) staff       (20)     4966 2022-01-31 20:35:59.000000 wf-cv-utils-3.4.0/cv_utils/eager_video_capture.py
--rw-r--r--   0 btalberg   (501) staff       (20)     7160 2022-01-31 20:35:59.000000 wf-cv-utils-3.4.0/cv_utils/video.py
--rw-r--r--   0 btalberg   (501) staff       (20)       38 2022-01-31 20:43:53.164535 wf-cv-utils-3.4.0/setup.cfg
--rw-r--r--   0 btalberg   (501) staff       (20)     1070 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/setup.py
-drwxr-xr-x   0 btalberg   (501) staff       (20)        0 2022-01-31 20:43:53.162763 wf-cv-utils-3.4.0/tests/
--rw-r--r--   0 btalberg   (501) staff       (20)      483 2022-01-03 22:41:31.000000 wf-cv-utils-3.4.0/tests/test_color.py
-drwxr-xr-x   0 btalberg   (501) staff       (20)        0 2022-01-31 20:43:53.163760 wf-cv-utils-3.4.0/wf_cv_utils.egg-info/
--rw-r--r--   0 btalberg   (501) staff       (20)     1999 2022-01-31 20:43:53.000000 wf-cv-utils-3.4.0/wf_cv_utils.egg-info/PKG-INFO
--rw-r--r--   0 btalberg   (501) staff       (20)      453 2022-01-31 20:43:53.000000 wf-cv-utils-3.4.0/wf_cv_utils.egg-info/SOURCES.txt
--rw-r--r--   0 btalberg   (501) staff       (20)        1 2022-01-31 20:43:53.000000 wf-cv-utils-3.4.0/wf_cv_utils.egg-info/dependency_links.txt
--rw-r--r--   0 btalberg   (501) staff       (20)       77 2022-01-31 20:43:53.000000 wf-cv-utils-3.4.0/wf_cv_utils.egg-info/requires.txt
--rw-r--r--   0 btalberg   (501) staff       (20)        9 2022-01-31 20:43:53.000000 wf-cv-utils-3.4.0/wf_cv_utils.egg-info/top_level.txt
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/LICENSE
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/MANIFEST.in
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1495 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/README.md
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        5 2023-07-16 13:23:38.000000 wf-cv-utils-3.5.0/VERSION
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/cv_utils/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      197 2023-07-16 13:13:33.000000 wf-cv-utils-3.5.0/cv_utils/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    34095 2023-07-16 13:13:08.000000 wf-cv-utils-3.5.0/cv_utils/aruco.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      327 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/color.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    32048 2022-12-08 20:56:54.000000 wf-cv-utils-3.5.0/cv_utils/core.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/cv_utils/drawing/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        0 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/drawing/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4150 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/drawing/matplotlib.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    11003 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/drawing/opencv.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4966 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/eager_video_capture.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     7160 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/video.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/setup.cfg
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1068 2023-07-16 13:14:37.000000 wf-cv-utils-3.5.0/setup.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      431 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       95 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/requires.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        9 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/top_level.txt
```

### Comparing `wf-cv-utils-3.4.0/LICENSE` & `wf-cv-utils-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.4.0/PKG-INFO` & `wf-cv-utils-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-cv-utils
-Version: 3.4.0
+Version: 3.5.0
 Summary: Miscellaneous utilities for working with camera data
 Home-page: https://github.com/WildflowerSchools/wf-cv-utils
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Keywords: cv
 Platform: UNKNOWN
```

### Comparing `wf-cv-utils-3.4.0/README.md` & `wf-cv-utils-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.4.0/cv_utils/core.py` & `wf-cv-utils-3.5.0/cv_utils/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,91 @@
 import cv2 as cv
 import numpy as np
 # import matplotlib.pyplot as plt
 # import scipy.optimize
 import json
 import os
 
+def termination_criteria(
+    max_iterations=10000,
+    accuracy=1e-9
+):
+    termination_criteria = (cv.TERM_CRITERIA_COUNT & cv.TERM_CRITERIA_EPS, max_iterations, accuracy)
+    return termination_criteria
+
+def camera_calibration_flags(
+    use_intrinsic_guess=False,
+    fix_principal_point=False,
+    fix_aspect_ratio=False,
+    zero_tangent_distortion=False,
+    fix_focal_length=False,
+    fix_k1=False,
+    fix_k2=False,
+    fix_k3=False,
+    fix_k4=False,
+    fix_k5=False,
+    fix_k6=False,
+    rational_model=False,
+    thin_prism_model=False,
+    fix_s1_s2_s3_s4=False,
+    tilted_model=False,
+    fix_taux_tauy=False,
+):
+    flags = 0
+    flag_descriptions=list()
+    if use_intrinsic_guess:
+        flags += cv.CALIB_USE_INTRINSIC_GUESS
+        flag_descriptions.append('use intrinsic guess')
+    if fix_principal_point:
+        flags += cv.CALIB_FIX_PRINCIPAL_POINT
+        flag_descriptions.append('fix principal point')
+    if fix_aspect_ratio:
+        flags += cv.CALIB_FIX_ASPECT_RATIO
+        flag_descriptions.append('fix aspect ratio')
+    if zero_tangent_distortion:
+        flags += cv.CALIB_ZERO_TANGENT_DIST
+        flag_descriptions.append('zero tangent distortion')
+    if fix_focal_length:
+        flags += cv.CALIB_FIX_FOCAL_LENGTH
+        flag_descriptions.append('fix focal length')
+    if fix_k1:
+        flags += cv.CALIB_FIX_K1
+        flag_descriptions.append('fix k_1')
+    if fix_k2:
+        flags += cv.CALIB_FIX_K2
+        flag_descriptions.append('fix k_2')
+    if fix_k3:
+        flags += cv.CALIB_FIX_K3
+        flag_descriptions.append('fix k_3')
+    if fix_k4:
+        flags += cv.CALIB_FIX_K4
+        flag_descriptions.append('fix k_4')
+    if fix_k5:
+        flags += cv.CALIB_FIX_K5
+        flag_descriptions.append('fix k_5')
+    if fix_k6:
+        flags += cv.CALIB_FIX_K6
+        flag_descriptions.append('fix k_6')
+    if rational_model:
+        flags += cv.CALIB_RATIONAL_MODEL
+        flag_descriptions.append('rational model')
+    if thin_prism_model:
+        flags += cv.CALIB_THIN_PRISM_MODEL
+        flag_descriptions.append('thin prism model')
+    if fix_s1_s2_s3_s4:
+        flags += cv.CALIB_FIX_S1_S2_S3_S4
+        flag_descriptions.append('fix s_1/s_2/s_3/s_4')
+    if tilted_model:
+        flags += cv.CALIB_TILTED_MODEL
+        flag_descriptions.append('tilted model')
+    if fix_taux_tauy:
+        flags += cv.CALIB_FIX_TAUX_TAUY
+        flag_descriptions.append('fix tau_x/tau_y')
+    return flags, flag_descriptions
+
 def compose_transformations(
         rotation_vector_1,
         translation_vector_1,
         rotation_vector_2,
         translation_vector_2):
     rotation_vector_1 = np.asarray(rotation_vector_1).reshape(3)
     translation_vector_1 = np.asarray(translation_vector_1).reshape(3)
@@ -790,7 +867,11 @@
     image_output_directory, image_output_filename = os.path.split(path)
     if image_output_directory is not None:
         os.makedirs(image_output_directory, exist_ok=True)
     cv.imwrite(
         filename=path,
         img=image
     )
+
+def read_image(path):
+    image = cv.imread(path)
+    return image
```

### Comparing `wf-cv-utils-3.4.0/cv_utils/drawing/matplotlib.py` & `wf-cv-utils-3.5.0/cv_utils/drawing/matplotlib.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.4.0/cv_utils/drawing/opencv.py` & `wf-cv-utils-3.5.0/cv_utils/drawing/opencv.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.4.0/cv_utils/eager_video_capture.py` & `wf-cv-utils-3.5.0/cv_utils/eager_video_capture.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.4.0/cv_utils/video.py` & `wf-cv-utils-3.5.0/cv_utils/video.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.4.0/setup.py` & `wf-cv-utils-3.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 BASE_DEPENDENCIES = [
     'wf-cv-datetime-utils>=0.1.0',
     'opencv-python>=4.5.1',
     'pandas>=1.2.2',
     'numpy>=1.20.1',
     # 'scipy>=1.6.0',
-    # 'matplotlib>=3.3.4'
+    'matplotlib>=3.3.4'
 ]
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(BASEDIR))
 
 setup(
     name='wf-cv-utils',
```

### Comparing `wf-cv-utils-3.4.0/wf_cv_utils.egg-info/PKG-INFO` & `wf-cv-utils-3.5.0/wf_cv_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-cv-utils
-Version: 3.4.0
+Version: 3.5.0
 Summary: Miscellaneous utilities for working with camera data
 Home-page: https://github.com/WildflowerSchools/wf-cv-utils
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Keywords: cv
 Platform: UNKNOWN
```

