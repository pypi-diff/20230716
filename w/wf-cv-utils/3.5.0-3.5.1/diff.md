# Comparing `tmp/wf-cv-utils-3.5.0.tar.gz` & `tmp/wf-cv-utils-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-cv-utils-3.5.0.tar", last modified: Sun Jul 16 13:25:21 2023, max compression
+gzip compressed data, was "wf-cv-utils-3.5.1.tar", last modified: Sun Jul 16 17:55:28 2023, max compression
```

## Comparing `wf-cv-utils-3.5.0.tar` & `wf-cv-utils-3.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/LICENSE
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/MANIFEST.in
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1495 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/README.md
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        5 2023-07-16 13:23:38.000000 wf-cv-utils-3.5.0/VERSION
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/cv_utils/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      197 2023-07-16 13:13:33.000000 wf-cv-utils-3.5.0/cv_utils/__init__.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    34095 2023-07-16 13:13:08.000000 wf-cv-utils-3.5.0/cv_utils/aruco.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      327 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/color.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    32048 2022-12-08 20:56:54.000000 wf-cv-utils-3.5.0/cv_utils/core.py
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/cv_utils/drawing/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        0 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/drawing/__init__.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4150 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/drawing/matplotlib.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    11003 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/drawing/opencv.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4966 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/eager_video_capture.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     7160 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.0/cv_utils/video.py
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/setup.cfg
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1068 2023-07-16 13:14:37.000000 wf-cv-utils-3.5.0/setup.py
-drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 13:25:21.604980 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/PKG-INFO
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      431 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       95 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/requires.txt
--rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        9 2023-07-16 13:25:21.000000 wf-cv-utils-3.5.0/wf_cv_utils.egg-info/top_level.txt
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1088 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/LICENSE
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       34 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/MANIFEST.in
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1495 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/README.md
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        5 2023-07-16 17:54:46.000000 wf-cv-utils-3.5.1/VERSION
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/cv_utils/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      195 2023-07-16 17:52:59.000000 wf-cv-utils-3.5.1/cv_utils/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    34095 2023-07-16 13:26:52.000000 wf-cv-utils-3.5.1/cv_utils/aruco.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      327 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/color.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    24937 2023-07-16 15:43:51.000000 wf-cv-utils-3.5.1/cv_utils/core.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/cv_utils/drawing/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        0 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/drawing/__init__.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4150 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/drawing/matplotlib.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)    11003 2023-07-16 15:40:10.000000 wf-cv-utils-3.5.1/cv_utils/drawing/opencv.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     4966 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/eager_video_capture.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     7160 2022-12-08 20:56:25.000000 wf-cv-utils-3.5.1/cv_utils/video.py
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       38 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/setup.cfg
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1011 2023-07-16 15:40:14.000000 wf-cv-utils-3.5.1/setup.py
+drwxrwxr-x   0 tcquinn   (1001) tcquinn   (1001)        0 2023-07-16 17:55:28.390439 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)     1999 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)      431 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        1 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)       67 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/requires.txt
+-rw-rw-r--   0 tcquinn   (1001) tcquinn   (1001)        9 2023-07-16 17:55:28.000000 wf-cv-utils-3.5.1/wf_cv_utils.egg-info/top_level.txt
```

### Comparing `wf-cv-utils-3.5.0/LICENSE` & `wf-cv-utils-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.0/PKG-INFO` & `wf-cv-utils-3.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-cv-utils
-Version: 3.5.0
+Version: 3.5.1
 Summary: Miscellaneous utilities for working with camera data
 Home-page: https://github.com/WildflowerSchools/wf-cv-utils
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Keywords: cv
 Platform: UNKNOWN
```

### Comparing `wf-cv-utils-3.5.0/README.md` & `wf-cv-utils-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.0/cv_utils/aruco.py` & `wf-cv-utils-3.5.1/cv_utils/aruco.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.0/cv_utils/core.py` & `wf-cv-utils-3.5.1/cv_utils/core.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,9 @@
-import cv_datetime_utils
 import cv2 as cv
 import numpy as np
-# import matplotlib.pyplot as plt
-# import scipy.optimize
-import json
 import os
 
 def termination_criteria(
     max_iterations=10000,
     accuracy=1e-9
 ):
     termination_criteria = (cv.TERM_CRITERIA_COUNT & cv.TERM_CRITERIA_EPS, max_iterations, accuracy)
@@ -232,33 +228,14 @@
     camera_direction = np.matmul(
         cv.Rodrigues(-rotation_vector)[0],
         np.array([[0.0], [0.0], [1.0]]))
     camera_direction = np.squeeze(camera_direction)
     return camera_direction
 
 
-def reconstruct_z_rotation(x, y):
-    if x >= 0.0 and y >= 0.0:
-        return np.arctan(y / x)
-    if x >= 0.0 and y < 0.0:
-        return np.arctan(y / x) + 2 * np.pi
-    return np.arctan(y / x) + np.pi
-
-
-# Currently unused; needs to be fixed up for cases in which x and/or y are close
-# to zero
-def extract_yaw_from_camera_direction(
-        camera_direction):
-    camera_direction = np.asarray(camera_direction).reshape(3)
-    yaw = reconstruct_z_rotation(
-        camera_direction[0],
-        camera_direction[1])
-    return yaw
-
-
 def generate_camera_matrix(
         focal_length,
         principal_point):
     focal_length = np.asarray(focal_length).reshape(2)
     principal_point = np.asarray(principal_point).reshape(2)
     camera_matrix = np.array([
         [focal_length[0], 0, principal_point[0]],
@@ -491,15 +468,14 @@
         (image_points[:, 0] < image_corners[0, 0]) |
         (image_points[:, 0] > image_corners[1, 0]) |
         (image_points[:, 1] < image_corners[0, 1]) |
         (image_points[:, 1] > image_corners[1, 1])
     )
     return outside_frame_boolean
 
-
 def undistort_points(
         image_points,
         camera_matrix,
         distortion_coefficients):
     image_points = np.asarray(image_points)
     camera_matrix = np.asarray(camera_matrix)
     distortion_coefficients = np.asarray(distortion_coefficients)
@@ -681,189 +657,14 @@
         camera_matrix,
         rotation_vector_1,
         translation_vector_1,
         rotation_vector_2,
         translation_vector_2)
     return object_points
 
-
-def estimate_camera_pose_from_plane_object_points(
-        input_object_points,
-        height,
-        origin_index,
-        x_axis_index,
-        y_reference_point,
-        y_reference_point_sign,
-        distance_calibration_indices,
-        calibration_distance):
-    input_object_points = np.asarray(input_object_points)
-    if input_object_points.size == 0:
-        raise ValueError('Obect point array appears to be empty')
-    input_object_points = input_object_points.reshape((-1, 3))
-
-    scale_factor = np.divide(
-        calibration_distance,
-        np.linalg.norm(
-            np.subtract(
-                input_object_points[distance_calibration_indices[0]],
-                input_object_points[distance_calibration_indices[1]])))
-
-    object_points_1 = np.multiply(
-        input_object_points,
-        scale_factor)
-
-    def objective_function(parameters):
-        rotation_x = parameters[0]
-        rotation_y = parameters[1]
-        translation_z = parameters[2]
-        object_points_transformed = transform_object_points(
-            object_points_1,
-            np.array([rotation_x, rotation_y, 0.0]),
-            np.array([0.0, 0.0, translation_z]))
-        return np.sum(np.square(object_points_transformed[:, 2] - height))
-
-    optimization_solution = scipy.optimize.minimize(
-        objective_function,
-        np.array([0.0, 0.0, 0.0]))
-
-    rotation_x_a = optimization_solution['x'][0]
-    rotation_y_a = optimization_solution['x'][1]
-    translation_z_a = optimization_solution['x'][2]
-
-    rotation_x_rotation_y_a_norm = np.linalg.norm([rotation_x_a, rotation_y_a])
-
-    rotation_x_b = rotation_x_a * ((rotation_x_rotation_y_a_norm + np.pi) / rotation_x_rotation_y_a_norm)
-    rotation_y_b = rotation_y_a * ((rotation_x_rotation_y_a_norm + np.pi) / rotation_x_rotation_y_a_norm)
-    translation_z_b = - translation_z_a
-
-    rotation_vector_2_a = np.array([rotation_x_a, rotation_y_a, 0.0])
-    translation_vector_2_a = np.array([0.0, 0.0, translation_z_a])
-    object_points_2_a = transform_object_points(
-        object_points_1,
-        rotation_vector_2_a,
-        translation_vector_2_a)
-
-    rotation_vector_2_b = np.array([rotation_x_b, rotation_y_b, 0.0])
-    translation_vector_2_b = np.array([0.0, 0.0, translation_z_b])
-    object_points_2_b = transform_object_points(
-        object_points_1,
-        rotation_vector_2_b,
-        translation_vector_2_b)
-
-    sign_a = np.sign(
-        np.cross(
-            np.subtract(
-                object_points_2_a[x_axis_index],
-                object_points_2_a[origin_index]),
-            np.subtract(
-                object_points_2_a[y_reference_point],
-                object_points_2_a[origin_index]))[2])
-
-    sign_b = np.sign(
-        np.cross(
-            np.subtract(
-                object_points_2_b[x_axis_index],
-                object_points_2_b[origin_index]),
-            np.subtract(
-                object_points_2_b[y_reference_point],
-                object_points_2_b[origin_index]))[2])
-
-    if sign_a == y_reference_point_sign:
-        rotation_vector_2 = rotation_vector_2_a
-        translation_vector_2 = translation_vector_2_a
-        object_points_2 = object_points_2_a
-    else:
-        rotation_vector_2 = rotation_vector_2_b
-        translation_vector_2 = translation_vector_2_b
-        object_points_2 = object_points_2_b
-
-    xy_shift = - object_points_2[origin_index, :2]
-
-    rotation_vector_3 = np.array([0.0, 0.0, 0.0])
-    translation_vector_3 = np.array([xy_shift[0], xy_shift[1], 0.0])
-    object_points_3 = transform_object_points(
-        object_points_2,
-        rotation_vector_3,
-        translation_vector_3)
-
-    final_z_rotation = - reconstruct_z_rotation(
-        object_points_3[x_axis_index, 0],
-        object_points_3[x_axis_index, 1])
-
-    rotation_vector_4 = np.array([0.0, 0.0, final_z_rotation])
-    translation_vector_4 = np.array([0.0, 0.0, 0.0])
-    object_points_4 = transform_object_points(
-        object_points_3,
-        rotation_vector_4,
-        translation_vector_4)
-
-    rotation_vector_2_3, translation_vector_2_3 = compose_transformations(
-        rotation_vector_2,
-        translation_vector_2,
-        rotation_vector_3,
-        translation_vector_3)
-
-    rotation_vector_2_3_4, translation_vector_2_3_4 = compose_transformations(
-        rotation_vector_2_3,
-        translation_vector_2_3,
-        rotation_vector_4,
-        translation_vector_4)
-
-    camera_rotation_vector, camera_translation_vector = invert_transformation(
-        rotation_vector_2_3_4,
-        translation_vector_2_3_4)
-
-    return camera_rotation_vector, camera_translation_vector, scale_factor, object_points_4
-
-
-def estimate_camera_poses_from_plane_image_points(
-        image_points_1,
-        image_points_2,
-        camera_matrix,
-        height,
-        origin_index,
-        x_axis_index,
-        y_reference_point,
-        y_reference_point_sign,
-        distance_calibration_indices,
-        calibration_distance):
-    image_points_1 = np.asarray(image_points_1)
-    image_points_2 = np.asarray(image_points_2)
-    camera_matrix = np.asarray(camera_matrix)
-    if image_points_1.size == 0 or image_points_2.size == 0:
-        raise ValueError('One or both sets of image points appear to be empty')
-    image_points_1 = image_points_1.reshape((-1, 2))
-    image_points_2 = image_points_2.reshape((-1, 2))
-    if image_points_1.shape != image_points_2.shape:
-        raise ValueError('Sets of image points do not appear to be the same shape')
-    camera_matrix = camera_matrix.reshape((3, 3))
-    relative_rotation_vector, relative_translation_vector = estimate_camera_pose_from_image_points(
-        image_points_1,
-        image_points_2,
-        camera_matrix)
-    input_object_points = reconstruct_object_points_from_image_points(
-        image_points_1,
-        image_points_2,
-        camera_matrix)
-    rotation_vector_1, translation_vector_1, scale_factor = estimate_camera_pose_from_plane_object_points(
-        input_object_points,
-        height,
-        origin_index,
-        x_axis_index,
-        y_reference_point,
-        y_reference_point_sign,
-        distance_calibration_indices,
-        calibration_distance)[:3]
-    rotation_vector_2, translation_vector_2 = compose_transformations(
-        rotation_vector_1,
-        translation_vector_1,
-        relative_rotation_vector,
-        relative_translation_vector * scale_factor)
-    return rotation_vector_1, translation_vector_1, rotation_vector_2, translation_vector_2
-
 def write_image(
     image,
     path
 ):
     image_output_directory, image_output_filename = os.path.split(path)
     if image_output_directory is not None:
         os.makedirs(image_output_directory, exist_ok=True)
```

### Comparing `wf-cv-utils-3.5.0/cv_utils/drawing/matplotlib.py` & `wf-cv-utils-3.5.1/cv_utils/drawing/matplotlib.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.0/cv_utils/drawing/opencv.py` & `wf-cv-utils-3.5.1/cv_utils/drawing/opencv.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.0/cv_utils/eager_video_capture.py` & `wf-cv-utils-3.5.1/cv_utils/eager_video_capture.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.0/cv_utils/video.py` & `wf-cv-utils-3.5.1/cv_utils/video.py`

 * *Files identical despite different names*

### Comparing `wf-cv-utils-3.5.0/setup.py` & `wf-cv-utils-3.5.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import os
 from setuptools import setup, find_packages
 
 BASEDIR = os.path.dirname(os.path.abspath(__file__))
 VERSION = open(os.path.join(BASEDIR, 'VERSION')).read().strip()
 
 BASE_DEPENDENCIES = [
-    'wf-cv-datetime-utils>=0.1.0',
     'opencv-python>=4.5.1',
     'pandas>=1.2.2',
     'numpy>=1.20.1',
-    # 'scipy>=1.6.0',
     'matplotlib>=3.3.4'
 ]
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(BASEDIR))
 
 setup(
```

### Comparing `wf-cv-utils-3.5.0/wf_cv_utils.egg-info/PKG-INFO` & `wf-cv-utils-3.5.1/wf_cv_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-cv-utils
-Version: 3.5.0
+Version: 3.5.1
 Summary: Miscellaneous utilities for working with camera data
 Home-page: https://github.com/WildflowerSchools/wf-cv-utils
 Author: Theodore Quinn
 Author-email: ted.quinn@wildflowerschools.org
 License: UNKNOWN
 Keywords: cv
 Platform: UNKNOWN
```

