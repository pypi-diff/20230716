# Comparing `tmp/pyote-5.3.1.tar.gz` & `tmp/pyote-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyote-5.3.1.tar", last modified: Mon Jul 10 20:53:54 2023, max compression
+gzip compressed data, was "pyote-5.3.2.tar", last modified: Sun Jul 16 03:15:08 2023, max compression
```

## Comparing `pyote-5.3.1.tar` & `pyote-5.3.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 20:53:54.771696 pyote-5.3.1/
--rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.1/LICENSE
--rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-07-10 20:53:54.771696 pyote-5.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.1/README.rst
--rw-rw-rw-   0        0        0       80 2023-07-10 20:53:54.772697 pyote-5.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2922 2023-06-06 20:30:01.000000 pyote-5.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:53:54.604154 pyote-5.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-10 20:53:54.614300 pyote-5.3.1/src/pyote.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-07-10 20:53:54.000000 pyote-5.3.1/src/pyote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2023-07-10 20:53:54.000000 pyote-5.3.1/src/pyote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 20:53:54.000000 pyote-5.3.1/src/pyote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.1/src/pyote.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      257 2023-07-10 20:53:54.000000 pyote-5.3.1/src/pyote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-10 20:53:54.000000 pyote-5.3.1/src/pyote.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-10 20:53:54.731266 pyote-5.3.1/src/pyoteapp/
--rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.1/src/pyoteapp/PYOTE.bat
--rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.1/src/pyoteapp/SER.py
--rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.1/src/pyoteapp/__init__.py
--rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.1/src/pyoteapp/autocorrtools.py
--rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.1/src/pyoteapp/blockIntegrateUtils.py
--rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.1/src/pyoteapp/checkForNewerVersion.py
--rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.1/src/pyoteapp/csvreader.py
--rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.1/src/pyoteapp/diffraction-table.p
--rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.1/src/pyoteapp/errorBarUtils.py
--rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.1/src/pyoteapp/example-penumbral.csv
--rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.1/src/pyoteapp/exponentialEdgeUtilities.py
--rw-rw-rw-   0        0        0     6850 2023-07-06 22:29:01.000000 pyote-5.3.1/src/pyoteapp/false_positive.py
--rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.1/src/pyoteapp/fixedPrecision.py
--rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.1/src/pyoteapp/genDiffraction.py
--rw-rw-rw-   0        0        0   386870 2023-07-10 15:37:00.000000 pyote-5.3.1/src/pyoteapp/gui.py
--rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.1/src/pyoteapp/helpDialog.py
--rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.1/src/pyoteapp/iterative_logl_functions.py
--rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.1/src/pyoteapp/likelihood_calculations.py
-drwxrwxrwx   0        0        0        0 2023-07-10 20:53:54.770696 pyote-5.3.1/src/pyoteapp/model-examples/
--rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.1/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
--rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.1/src/pyoteapp/model-examples/LCP_penumbral.p
--rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.1/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.1/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.1/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.1/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
--rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.1/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.1/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.1/src/pyoteapp/model-help.pdf
--rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.1/src/pyoteapp/noiseUtils.py
--rw-rw-rw-   0        0        0   458476 2023-07-10 20:51:28.000000 pyote-5.3.1/src/pyoteapp/pyote-info.pdf
--rw-rw-rw-   0        0        0   447259 2023-07-08 20:11:39.000000 pyote-5.3.1/src/pyoteapp/pyote.py
--rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.1/src/pyoteapp/pyote_modelling_utility_functions.py
--rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.1/src/pyoteapp/run-pyote-mac.bat
--rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.1/src/pyoteapp/showVideoFrames.py
--rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.1/src/pyoteapp/solverUtils.py
--rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.1/src/pyoteapp/subframe_timing_utilities.py
--rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.1/src/pyoteapp/timestampDialog.py
--rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.1/src/pyoteapp/timestampUtils.py
--rw-rw-rw-   0        0        0       34 2023-07-10 20:52:14.000000 pyote-5.3.1/src/pyoteapp/version.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.833435 pyote-5.3.2/
+-rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.2/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1190 2023-07-16 03:15:08.833435 pyote-5.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.2/README.rst
+-rw-rw-rw-   0        0        0       80 2023-07-16 03:15:08.834467 pyote-5.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2922 2023-06-06 20:30:01.000000 pyote-5.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.648538 pyote-5.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.659622 pyote-5.3.2/src/pyote.egg-info/
+-rw-rw-rw-   0        0        0     1190 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.2/src/pyote.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      257 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 03:15:08.000000 pyote-5.3.2/src/pyote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.795839 pyote-5.3.2/src/pyoteapp/
+-rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.2/src/pyoteapp/PYOTE.bat
+-rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.2/src/pyoteapp/SER.py
+-rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.2/src/pyoteapp/__init__.py
+-rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.2/src/pyoteapp/autocorrtools.py
+-rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.2/src/pyoteapp/blockIntegrateUtils.py
+-rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.2/src/pyoteapp/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.2/src/pyoteapp/csvreader.py
+-rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.2/src/pyoteapp/diffraction-table.p
+-rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.2/src/pyoteapp/errorBarUtils.py
+-rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.2/src/pyoteapp/example-penumbral.csv
+-rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.2/src/pyoteapp/exponentialEdgeUtilities.py
+-rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.2/src/pyoteapp/false_positive.py
+-rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.2/src/pyoteapp/fixedPrecision.py
+-rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.2/src/pyoteapp/genDiffraction.py
+-rw-rw-rw-   0        0        0   386870 2023-07-10 15:37:00.000000 pyote-5.3.2/src/pyoteapp/gui.py
+-rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.2/src/pyoteapp/helpDialog.py
+-rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.2/src/pyoteapp/iterative_logl_functions.py
+-rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.2/src/pyoteapp/likelihood_calculations.py
+drwxrwxrwx   0        0        0        0 2023-07-16 03:15:08.833435 pyote-5.3.2/src/pyoteapp/model-examples/
+-rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.2/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
+-rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.2/src/pyoteapp/model-examples/LCP_penumbral.p
+-rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.2/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.2/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.2/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.2/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
+-rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.2/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.2/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.2/src/pyoteapp/model-help.pdf
+-rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.2/src/pyoteapp/noiseUtils.py
+-rw-rw-rw-   0        0        0   459582 2023-07-16 02:51:18.000000 pyote-5.3.2/src/pyoteapp/pyote-info.pdf
+-rw-rw-rw-   0        0        0   449634 2023-07-16 02:45:25.000000 pyote-5.3.2/src/pyoteapp/pyote.py
+-rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.2/src/pyoteapp/pyote_modelling_utility_functions.py
+-rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.2/src/pyoteapp/run-pyote-mac.bat
+-rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.2/src/pyoteapp/showVideoFrames.py
+-rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.2/src/pyoteapp/solverUtils.py
+-rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.2/src/pyoteapp/subframe_timing_utilities.py
+-rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.2/src/pyoteapp/timestampDialog.py
+-rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.2/src/pyoteapp/timestampUtils.py
+-rw-rw-rw-   0        0        0       34 2023-07-14 17:15:17.000000 pyote-5.3.2/src/pyoteapp/version.py
```

### Comparing `pyote-5.3.1/LICENSE` & `pyote-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/PKG-INFO` & `pyote-5.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.1
+Version: 5.3.2
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.1/setup.py` & `pyote-5.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyote.egg-info/PKG-INFO` & `pyote-5.3.2/src/pyote.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.1
+Version: 5.3.2
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.1/src/pyote.egg-info/SOURCES.txt` & `pyote-5.3.2/src/pyote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/SER.py` & `pyote-5.3.2/src/pyoteapp/SER.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/autocorrtools.py` & `pyote-5.3.2/src/pyoteapp/autocorrtools.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/blockIntegrateUtils.py` & `pyote-5.3.2/src/pyoteapp/blockIntegrateUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/checkForNewerVersion.py` & `pyote-5.3.2/src/pyoteapp/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/csvreader.py` & `pyote-5.3.2/src/pyoteapp/csvreader.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/diffraction-table.p` & `pyote-5.3.2/src/pyoteapp/diffraction-table.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/errorBarUtils.py` & `pyote-5.3.2/src/pyoteapp/errorBarUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/example-penumbral.csv` & `pyote-5.3.2/src/pyoteapp/example-penumbral.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/exponentialEdgeUtilities.py` & `pyote-5.3.2/src/pyoteapp/exponentialEdgeUtilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/false_positive.py` & `pyote-5.3.2/src/pyoteapp/false_positive.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         A = cumA / numA
         B = cumB / numB
 
         drop = B - A
         if drop > best_drop_so_far:
             best_drop_so_far = drop
 
-    obs = None
     return best_drop_so_far
 
 
 @njit(parallel=True)
 def compute_drops(event_duration: int,
                   observation_size: int,
                   noise_sigma: float,
```

### Comparing `pyote-5.3.1/src/pyoteapp/fixedPrecision.py` & `pyote-5.3.2/src/pyoteapp/fixedPrecision.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/genDiffraction.py` & `pyote-5.3.2/src/pyoteapp/genDiffraction.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/gui.py` & `pyote-5.3.2/src/pyoteapp/gui.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/helpDialog.py` & `pyote-5.3.2/src/pyoteapp/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/iterative_logl_functions.py` & `pyote-5.3.2/src/pyoteapp/iterative_logl_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/likelihood_calculations.py` & `pyote-5.3.2/src/pyoteapp/likelihood_calculations.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p` & `pyote-5.3.2/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-examples/LCP_penumbral.p` & `pyote-5.3.2/src/pyoteapp/model-examples/LCP_penumbral.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.2/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.2/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.2/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv` & `pyote-5.3.2/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.2/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.2/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/model-help.pdf` & `pyote-5.3.2/src/pyoteapp/model-help.pdf`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/noiseUtils.py` & `pyote-5.3.2/src/pyoteapp/noiseUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/pyote-info.pdf` & `pyote-5.3.2/src/pyoteapp/pyote-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 3% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,8 +1,18 @@
 Version history (PyOTE description – out of date - is at end)
+Version 5.3.2
+15 July 2023
+• Fixes a bug in the calculation of the duration fit metric when an already integrated csv
+file is in use.
+•
+
+Added specialized folders inside an observation folder to reduce clutter. There are new
+folders titled: FP-plots, Detectability, Normalization, ApertureGroups, OCR, and Finders
+inside an observation folder
+
 Version 5.3.1
 10 July 2023
 • Squeezed the lightcurves tab to allow a little more space for the plot for those that
 need to run PyOTE on a small laptop screen
 To deal with pixel-challenged laptop screens --1: the plot can be made to span the entire width of the GUI by dragging splitter all the
 way to the left
 2: or you can change your pixel resolution to 150% instead of the default 200%
@@ -32,23 +42,22 @@
 That would be very wrong if the user is stepping through multiple light-curves in search
 of the “best” as they would all use the same baseline numbers (B and sigmaB).
 
 •
 
 Added false-positive metric to fit-metrics and rearranged output order.
 
-Version 5.2.7
+Version 5.2.7
 24 June 2023
 • Minor change: corrected titles in fit-metric file from D frame to D reading num and R
 frame to R reading num
 Version 5.2.6
 17 June 2023
 • Changed order of buttons on Noise analysis/Detectability tab to better reflect work flow
-
-•
+•
 
 If a minEvent of 1 is entered for the min/max search, it is automatically changed to 2
 (with an advisory message to this effect) to ease work flow.
 
 •
 
 Added buttons to Lightcurves tab to make it more convenient to calculate and
@@ -93,25 +102,25 @@
 
 Version 5.2.2
 13 April 2023
 • Adds diffraction modelling of an elliptical asteroid shape
 Version 5.2.1 27 March 2023
 • Fixed problem with VizieR loading from North American .xlsx caused by Occult
 sometimes putting a string in the asteroid field and sometimes an integer.
-•
+
+•
 
 SER files with colorCode other than mono are now accepted.
 
 Version 5.2.0 17 March 2023
 • Fixes a bug in code introduced in version 5.1.0 where dropped frames are detected –
 that code did not handle an observation that passed through midnight (23:59:59)
 Version 5.1.9 10 March 2023
 • Fixes issues involving Tangra light curve names
-
-•
+•
 
 Clears previous light curves names when reading a new csv file.
 
 Version 5.1.8
 9 March 2023
 • Fixed GUI problem that just keeps re-occurring behind the scenes – frustrating.
 Version 5.1.7
@@ -144,27 +153,23 @@
 performed). Simply display the ‘signal’ and ‘appsum’ versions of a target lightcurve and
 use the y position spinBox on one of the curves until they overlap. This should show
 that during the event, the points almost exactly overlap, so event timing will be the
 same.
 •
 
 Added a button to the VizieR tab that will fill most of the entry boxes in the VizieR form
-from a North American .xlsx file for that event (derived from OW/Occult 4), if one is
-available.
 
+from a North American .xlsx file for that event (derived from OW/Occult 4), if one is
+available.
 Version 5.0.8 1 February 2023
 • Changed the VizieR form filling requirements to allow for all star catalog entries to
 remain unfilled.
 Version 5.0.7 22 January 2023
-
-•
-
-Fixed insidious and dangerous bug in VizieR tab that caused site coordinates to be
+• Fixed insidious and dangerous bug in VizieR tab that caused site coordinates to be
 saved and restored incorrectly.
-
 Version 5.0.6 19 January 2023
 • Fixed some data entry/edit issues in the new Other models tab.
 •
 
 Fixed a bug in the edge-on-disk model that was causing edges to be misplaced when
 D and R limb angles were unequal and the D angle was not 90 degrees. This was
 noticeable in the model-example provided for testing/training.
@@ -198,23 +203,22 @@
 When a block size is entered, the program will determine the best offset value to use
 for the integration.
 •
 
 Added a comprehensive set of lightcurve models together with tools to help automate
 the fitting of the new models to observation data. Models included:
 o Diffraction (including central spot for low rho events) using physical optics
-o Disk on disk (geometrical optics) for large stars
-o Edge on disk (geometrical optics) for large stars and limb angles on asteroid
 
+o Disk on disk (geometrical optics) for large stars
+o Edge on disk (geometrical optics) for large stars and limb angles on asteroid
 Version 4.9.2 14 August 2022
 • Added various tests involving the penumbral fit process to gently lead the user back to
 the path of rightness should that user try to do a ‘fit’ without loading a light-curve and/or
 not marking D and R regions.
-
-Version 4.9.1 10 August 2022
+Version 4.9.1 10 August 2022
 • In the diffraction tab, added a selection box so that asteroid distance can be entered
 either in parallax (arcseconds) or AU. Also reviewed and added to the context help on
 this tab to be more explanatory.
 Version 4.9.0 9 August 2022
 • Added a button to the diffraction tab for use during penumbral fits to do a re-fit.
 Improved (hopefully) the context help regarding the selection of D and R regions for a
 penumbral fit (cautioning the user to only include points from the penumbral transition).
@@ -236,23 +240,26 @@
 Version 4.8.7 29 July 2022
 • changed numpy version requirement to match that of PyMovie so that ultimately the
 two programs can share a virtual environment, thus saving much space.
 Version 4.8.6 23 July 2022
 • added instructions telling the user how to install a new version when one is found.
 There are instructions for pip based installations and pipenv installations
 Version 4.8.4
-• there are no changes. This is a new version just to test the change introduced in 4.8.3
+
+•
+
+there are no changes. This is a new version just to test the change introduced in 4.8.3
 about version detection and handling thereof.
+
 Version 4.8.3
 • this version removes the offer to update to a newer version when one is found. This
 has been done primarily to allow an easy transition to a distribution method that does
 not require the installation of Anaconda3, but it also gives the user more control. When
 a newer version is available, a message to that effect will be shown but otherwise the
-
-user’s workflow is not interrupted by a ‘nag’ about ‘do you want to download the newer
+user’s workflow is not interrupted by a ‘nag’ about ‘do you want to download the newer
 version?’.
 Version 4.8.2
 • changed the format of the false-positive probability report because very small but nonzero values were showing (confusingly) as probability 0.0000 That no longer can
 happen.
 Version 4.8.1
 • fixes automatic block integration failure under Win11.
 •
@@ -282,22 +289,22 @@
 •
 
 corrected the log messaging about Donly, Ronly, DandR, and min/max directions to the
 solver consistent
 
 version 4.6.3
 • in detectability: logged new 'drop message' to the detectability.log
-version 4.6.2
+
+version 4.6.2
 • in detectability: when event duration is or becomes less than the camera exposure
 time, the observed drop is reduced proportionately
 version 4.6.1
 • in detectability: changed calculation of number of event points from
 ceiling(dur/rdgTime) to round(dur/rdgTime)
-
-•
+•
 
 in detectability: allow a single point event.
 
 •
 
 In detectability: stop stepping down duration when calculation of number of event
 points reaches zero
@@ -324,22 +331,22 @@
 • fixes a bug where transition points (only present in high SNR light-curves) were not
 properly ignored during calculation of event noise. This manifested itself most clearly in
 too large error bars for magDrop
 version 4.5.0
 • fixes a bug introduced with the NE3 code changes that inhibited sub-frame timing
 adjustments.
 version 4.4.9
-• fixed yet another manisfestation of the bug introduced in version 4.2.1
+
+• fixed yet another manisfestation of the bug introduced in version 4.2.1
 version 4.4.8
 • fixed another manifestation of the bug introduced in version 4.2.1
 version 4.4.7
 • fixes a bug introduced in version 4.2.1 (February 8, 2022) that caused D values to be
 calculated as occurring 1 reading early
-
-version 4.4.5
+version 4.4.5
 • added a checkbox to enable selection of whether or not the camera response curve is
 shown on the lightcurve plot
 version 4.4.4
 • detectability and normalization activities are written to dedicated log files:
 *.detectability.PYOTE.log
 *.normalization.PYOTE.log
 version 4.3.8
@@ -365,32 +372,29 @@
 The red metric is the Pearson R value of the correlation between the target lightcurve
 and the reference lightcurve; it should be maximized (using the X offset spinbox of the
 reference curve) at the point where the two curves are properly time-aligned. It is also
 affected by the smoothing interval, but this connection should be ignored.
 The green metric is the standard deviation of the target lightcurve – it is lowered when
 the target lightcurve has a minimum slope and the fewest and shallowest bumps. Use
 the spinbox for the number of readings in the smoothing interval to minimize this
-number.
+
+number.
 version 4.3.5
 • made the 'step-by' buttons radio buttons so that it is clear what the current step size is.
 •
 
 removed the automatic switch to the Lightcurve panel
 
 version 4.3.3
-
-•
-
-added a Pearson R calculation whenever normalization is being performed. This may
+• added a Pearson R calculation whenever normalization is being performed. This may
 be an aid in aligning time shifts between the target lightcurve and the reference
 lightcurve.
 The idea is that the user will observe this value as left and right (X offset) shifts are
 performed and choose the position that gives the highest positive value for this number
 (it will always be between 1.0 and -1.0).
-
 version 4.3.2
 • adds step size selection for the Y offset spinboxes
 •
 
 activates the 'show' checkbox on reference curves so that the reference curve display
 can be turned off – but it will still be active behind the scenes, just not visible.
 
@@ -415,26 +419,27 @@
 
 version 4.2.6
 • tidies up the lightcurve panel a bit and changes color samples for target and reference
 curves.
 version 4.2.5
 • completes implementation of the time shift (left/right shift) of the reference curve for
 normalization.
-•
+
+•
 
 adds dot color samples next to the lightcurve titles.
 
 version 4.2.4
 • makes tab/panel order sticky
 •
 
 analysis tab always opens first, but automatic switch to Lightcurves tab occurs upon
 file read.
 
-•
+•
 
 'target' lightcurve cannot no longer be moved up or down. If there is an overlapping
 lightcurve, move the non-target lightcurve to clear the overlap.
 
 version 4.2.3
 • fixes block integration that was broken by the new lightcurve selection code.
 •
@@ -465,25 +470,26 @@
 affected. This facility was added to allow the separation of lightcurves that would
 otherwise overlap in a confusing manner.
 There can only be one lightcurve selected as target.
 There can be either 0 or 1 lightcurve selected as a reference for normalization.
 Normalization is applied whenever the normalization reference curve smoothing
 interval spinbox is changed from 0. Whenever this number is changed, a new
 normalization will result. If this number is returned to zero, all normalization is removed
-and the original values restored.
+
+and the original values restored.
 The X offset spinbox is not yet implemented. Its (future) purpose is to allow the
 reference curve used for normalization to be 'time shifted' for those cases where a
 drifting cloud affects lightcurves at slightly different times.
 •
 
 the normalization itself has been simplified so that no user input is needed other than
 the number of readings to be used in the smoothing procedure. The smoothing
 procedure is a double application of a first order Savitzky-Golay filter (a straight line) to
+the points included with extrapolation.
 
-the points included with extrapolation.
 •
 
 added (back again) a spinbox on the Setting/Misc. Tab that allows the dot size used in
 lightcurve plots to be changed.
 
 version 4.2.1
 • fixed final report showing NE3 stuff even when NE3 not in use was checked.
@@ -515,25 +521,26 @@
 Adds test to detectability routine so that the user cannot give an event duration that
 requires more points than are available in the observation.
 
 version 4.1.5
 • changed error bar calculation reporting so that the the value reported in the
 containment interval report matches that reported in the Excel final report when there is
 no asymmetry present.
-version 4.1.4
+
+version 4.1.4
 • This version adds tools needed to make best use of the Night Eagle 3 camera, the
 successor to the Night Eagle Astro camera (which is no longer in production). They are
 all grouped on a new tab page titled Night Eagle 3.
 •
 
 The Night Eagle 3 is a rolling shutter CMOS camera. As a result, with this camera, the
 timing of an occultation depends on which row the occulted star is at when the
 occultation occurs. PyOTE will automatically calculate the needed time correction from
+the y (row) position that you enter in the spin/entry box at the bottom of this tab.
 
-the y (row) position that you enter in the spin/entry box at the bottom of this tab.
 •
 
 For the Night Eagle 3, times extracted by PyOTE require only a VTI correction (if you
 use an IOTA VTI, there is no correction at all needed).
 
 •
 
@@ -581,29 +588,25 @@
 
 You will probably want to use the most aggressive noise reduction in most cases, but
 make sure that your expected event duration is long enough that the D transition
 exponential curve has time to settle to the bottom event plus some time to allow a good
 determination of the event bottom intensity. At DNR:HIGH, your expected event time
 should be greater than 30 frames (1 second) to use this setting.
 
-•
+•
 
 I suggest the following rules-of-thumb: can use DNR:HIGH for events 2 seconds and
 longer; can use DNR:MIDDLE for events 1 second and longer; can use DNR:LOW for
 events 0.5 seconds and longer.
 
 version 4.1.2
 • fixes bug when D only search has been selected
 version 4.1.1
-
-•
-
-fixes bug where signal columns beyond four were being read as duplicates of column
+• fixes bug where signal columns beyond four were being read as duplicates of column
 5.
-
 version 4.1.0
 • adds error bars to reported magDrop values.
 This was an interesting exercise in the propagation of errors because the magDrop
 calculation involves ln(A/B) where we know the error bars for A and B but have to
 propagate those errors through the ratio A/B to get its error bars and then through the
 ln() function to get the final error bars. The equations I use were verified through
 simulations.
@@ -627,28 +630,24 @@
 • if you click outside the light-curve, the closest point will be toggled (so you don't have
 to zoom in to select the leftmost or rightmost point in a light-curve.
 •
 
 When baseline statistics are calculated, they are reported as baseline mean and
 baseline snr (instead of just snr, which is the term we use when a drop is present).
 
-version 4.0.4
+version 4.0.4
 • a few GUI changes
 •
 
 removed the Use as secondary check box. Now if secondary curve is selected (spinner
 is non-zero), it will be used automatically.
 
 version 4.0.3
-
-•
-
-implements a major GUI change: uses tabbed folders to group buttons and other
+• implements a major GUI change: uses tabbed folders to group buttons and other
 controls.
-
 •
 
 Removes radio buttons that indicated a D and R solution wanted, or a D-only solution,
 or an R-only solution. The type of solution is now inferred from D and R region setting.
 When min/max event size is used as the search criteria, then a D and R solution is
 assumed and found. This type of search criteria does not make sense for a D-only or
 an R-only solution. Use a D region or R region selection for these cases
@@ -675,23 +674,24 @@
 calculator to step from the given duration down until an event of that duration fails the
 False-positive test, only the final plot (where False-positive became non-zero) will be
 plotted.
 All of the above is just to cut down on clutter in the light-curve directory and to only plot
 meaningful graphics generated during the minimum duration search.
 version 3.9.9
 • whew! 3.9.8 did solve the sizing issue. So it is safe to get back in the water so...
-This version just improves the right-click context help for buttons in the new
+
+This version just improves the right-click context help for buttons in the new
 Detectibility calculator.
 version 3.9.8
 • one more attempt to solve the gui sizing issue.
 •
 
 'sticky' settings are back but are now stored in pyote.ini instead of the
+obscure simple-ote.ini
 
-obscure simple-ote.ini
 version 3.9.7
 • Something inexplicable has happened regarding gui size. Suddenly, the gui size is too
 large for many people – but I have set the gui size smaller than it has ever been. So,
 best guess is that an overly large gui size got distributed once (there was a strange
 event where an extremely large gui size appeared) and is being 'remembered' in the
 simple-ote-ini file that preserves the 'sticky' values like size and position of the gui and
 a few other things.
@@ -712,24 +712,25 @@
 plot where detection failed will be left on-screen.
 If the duration step size is left unfilled or is zero, a single 'detectibility' calculation will be
 made as before.
 version 3.9.4
 • attempts to fix over-size initial gui.
 version 3.9.3
 • makes various improvements to the 'detectability' calculator to make it easier to use.
-version 3.9.2
+
+version 3.9.2
 • adds a 'detectability' calculator for use in pre-planning event observation.
 •
 
 'scrunched' the left panel buttons together to make more room for the user to move the
 horizontal splitter up (which gives more room to view the lower right panel where the
 report gets printed).
 I think that this is kind of ugly, and it can be easily returned to the more spacious format
+if users would prefer the old look over more view space for the report.
 
-if users would prefer the old look over more view space for the report.
 version 3.9.1
 • adds an snr calculation to the Calc baseline stats button.
 version 3.9.0
 • restored the right-click help to the Mark baseline region | Clear baseline region |
 Calc baseline mean/sigma/corr coeffs buttons that got lost during the scrollable gui
 experiment.
 version 3.8.9
@@ -752,24 +753,25 @@
 version 3.8.4
 • changed the way QTableWidgetItem and QApplication were referenced to
 accommodate the latest Anaconda version, which has reorganized where those
 modules are stored. A similar change was made in version 3.7.6 and I do not know
 how this has gone uncorrected for so long – I hope that I have not missed something.
 version 3.8.3
 • adds display of light-curve name (if available in the csv file) to the curve-to-be-analyzed
-and the normalization curve next to their selection spinners.
+
+and the normalization curve next to their selection spinners.
 version 3.8.2
 • 3.7.5 introduced a scrollable GUI for small screens. Unfortunately, that caused resizing
 problem for all users. The version reverts back to the original GUI design.
 •
 
 Added a print to the command window of the version number for diagnostic purposes.
 It will help clarify the situation when an installation has somehow managed to have
+multiple locations for PyOTE storage as to exactly what version is running.
 
-multiple locations for PyOTE storage as to exactly what version is running.
 version 3.8.1
 • adds a checkbox to use reading number to annotate the x-axis, even when timestamps
 are available to use for this annotation. The setting is 'sticky', so your last preference
 will be remembered and used in the next run.
 version 3.8.0
 • adds a tutorial button to supply a quick-start for new or infrequent users.
 version 3.7.9
@@ -793,24 +795,24 @@
 • changed the way QMainWindow and Qapplication were referenced to accommodate
 the latest Anaconda version, which has reorganized where those modules are stored.
 This was causing a fatal startup error.
 version 3.7.5
 • changes the routine that looks for the latest version of PyOTE to one provided by Kia
 Getrost. His version contacts the PyPI repository via a json query and is the officially
 supported way to get version info. My version was based on a 'hack' that depended on
-a special feature of pip (the loader that get programs from the PyPI repository) that was
+
+a special feature of pip (the loader that get programs from the PyPI repository) that was
 marked as 'unsupported'. That worked for many years until the pip programmers
 removed the 'special feature' as was their right (and the implicit promise/warning, I
 guess). This caused several users to always get a message that they were not running
 the most recent version of PyOTE, even though they were. Again: thanks to Kia
 Getrost for researching the problem and even supplying correct code (worked first
 time!) for me to use.
 • The GUI has been changed so that scroll bars will appear when the standard GUI size
-
-exceeds your screen dimensions. THIS IS EXPERIMENTAL BECAUSE I DO NOT
+exceeds your screen dimensions. THIS IS EXPERIMENTAL BECAUSE I DO NOT
 HAVE SUCH A SMALL SCREEN TO TEST WITH. If this does not work for you, please
 let me know immediately!
 version 3.7.4
 • fixed issue with ‘save main plot’ that caused the graphic to sometimes be written
 to a previous folder rather than the current folder containing the csv file (FYI: it
 was a ‘feature’ of the routine that saved this information that, in the interest of
 efficiency, it would sometimes not write a new folder name to the ‘sticky file’ until
@@ -835,23 +837,23 @@
 generation
 version 3.6.7
 • clarified the location of the Enable Manual Timestamp Entry checkbox in the
 pop-up message appears when there are no timestamps in the csv file.
 version 3.6.6
 • modified the lightcurve demo to show more clearly the camera exposure
 function and the star intensity function that are convolved with the diffraction
-lightcurve to produce the lightcurve as seen by the camera.
+
+lightcurve to produce the lightcurve as seen by the camera.
 The right-click help connected to the Demo button has been expanded to
 include a discussion of the convolution operation and hopefully provide some
 context to aid in understanding the star and camera function plots.
 version 3.6.5
 • added advisory message when False Positive probability plot appears in hopes
 of stemming in-discriminant use of this number as a 'decider' between a 'miss'
-
-and a 'positive' for an observation.
+and a 'positive' for an observation.
 version 3.6.4
 • version 3.6.2 would open .xlsx Report file on Mac, but not Windows. This
 version attempts to fix that (Windows needs a different command to open a file).
 version 3.6.2
 • In Excel report:
 … at end of filling, I call the OS to open the file. Requires correct association
 of .xlsx file type with Excel or LibreOffice, or whatever you use to examine
@@ -869,22 +871,22 @@
 • provides the ability to fill entries in the Excel spreadsheet Asteroid Occultation
 Report Form from PyOTE results, thus eliminating transcription errors.
 A button to allow the user to activate this 'fill' has been added just to the right of
 
 the … write report button
 NOTE: the normal .xls report form that OccultWatcher creates and prefills (when
 requested) during your report to OccultWatcher ...
-… MUST BE CONVERTED to .xlsx for use by PyOTE!
+
+… MUST BE CONVERTED to .xlsx for use by PyOTE!
 … For Windows users, Excel will read an .xls file and save it as .xlsx
 … For Mac/Linux users, LibreOffice will read an .xls file and save it as .xlsx
 Sorry about this extra step, but it was necessary. The downstream tools used by area
 coordinators work equally well with the .xls and .xlsx forms of the spreadsheet, so there is no
 problem sending in the .xlsx version.
-
-What gets filled in for you is:
+What gets filled in for you is:
 ...D/R uncorrected times
 ...D/R error bars
 ...SNR
 …OTA used
 ...nominal magDrop (entered in Comments cell of the spreadsheet).
 NOTE: you must still open the spreadsheet and enter the exposure setting used for your
 camera; it was not possible to do this from PyOTE.
@@ -905,24 +907,27 @@
 started from PyMovie. Previously, it had only reopened the same file instead of
 giving the user a file select dialog to choose from.
 version 3.5.5
 • fixed a bug that kept occultations from being extracted from lightcurves 5 and
 up. The lightcurves above 4 could be viewed --- they just couldn't be processed
 through the event finder because they were a different type (coding error)
 version 3.5.4
-• made the 'get newest version' code identical to that in PyMovie in hopes that
+
+•
+
+made the 'get newest version' code identical to that in PyMovie in hopes that
 that will resolve the issue that some people experience with pip (or python)
 installing downloaded pyote in a directory where it subsequently cannot be
 discovered. The change is minute, so I'm not optimistic, but it's worth a shot.
+
 version 3.5.3
 • removed the blank lines between header lines extracted from the csv file and
 placed in the log file --- this makes it easier to look at the newly added aperture
 settings (so just a tiny cosmetic change).
-
-version 3.5.2
+version 3.5.2
 • Changed the 'smooth reference star procedure' to no longer display the points at
 the left and right ends; such points are actually extrapolated points with all the
 hazards that extrapolation can engender. Smoothing functions that use sliding
 windows always have a problem at either the left edge, the right edge, or both
 (when a symmetrical smoothing algorithm is employed). They run out of points
 and have to extrapolate/fake a number of points equal to the window size. Such
 extrapolated points can exhibit extreme behavior, zooming up or down
@@ -954,23 +959,22 @@
 to the data table where, once again, a 'write csv' process will capture the results.
 
 •
 
 Added additional reminders that the start-of-exposure timestamp/timing
 convention is employed.
 
-version 3.4.9
+version 3.4.9
 • Added some explanatory language to the “Excel report” section regarding the
 proper interpretation of the 'false positive probability' number.
 version 3.4.8
 • This version deals more realistically with high magDrop lightcurves by defining a
 'limiting magDrop' as:
 limMagDrop = 2.5 * log10( B / std(A) )
-
-std(A) is the noise level of A.
+std(A) is the noise level of A.
 B = average baseline intensity
 A = average event intensity
 Normally, we report/calculate magDrop = 2.5 * log10( B / A ), but this calculation becomes
 increasingly unreliable as the value for A gets very small. And when A is noisy, it is even
 possible to statistically have A become negative for large mag drop lightcurves. This happens
 more and more as A approaches and then becomes smaller than std(A). For example, if A
 happened to be equal to std(A), the normal distribution of A values tells us that 84% of
@@ -994,29 +998,26 @@
 
 Made use diff and Do OCR checkboxes sticky.
 
 version 3.4.4
 • PyMovie files can have lightcurves extracted from more than 4 apertures (with
 user supplied names). This version allows all lightcurves from PyMovie files to
 be read and made available for processing. Prior to this change, only the first 4
-lightcurves were read.
+
+lightcurves were read.
 Note: when you change the lightcurve to be analyzed (with the spinner), the log
 panel will show the aperture name for that lightcurve. That happens when the
 reference lightcurve is changed as well.
 These changes are to PyMovie file treatment ONLY.
 version 3.4.3
-
-•
-
-Fixed bug that required an entry in dist(AU) and speed(km/sec) edit boxes for a
+• Fixed bug that required an entry in dist(AU) and speed(km/sec) edit boxes for a
 solution to be found (the empty entries were causing an uncaught exception).
 The intention is that PyOTE should work as it always did if a user ignores the
 new lightcurve parameter panel and makes no entries. This 'fix' was required to
 make that happen.
-
 version 3.4.2
 • Cosmetic change again: added a spinner to control line widths in plots so that a
 user can adjust for the resolution of the screen in use. I design on a 5120x2880
 screen and needed lines to be 3 pixel wide to suit my taste. But some users
 have screens with 1280 horizontal resolution and those same 3 pixels became
 unsightly fat lines --- now there's a choice.
 version 3.4.1
@@ -1041,27 +1042,25 @@
 it resides, other files will get added in your installation directory --- we really don't
 want extraneous non-program files floating around in your installation directory.
 To learn how to use the new procedure (which is a bit 'fiddly'), right-click on the
 penumbral fit checkbox --- be patient; play around.
 
 version 3.4.0
 • Adds the ability to specify a diffraction lightcurve for use in timing the event. A
-new panel with edit boxes for asteroid/occulting body distance (in AU --astronomical units) and asteroid/shadow speed (in km per second) has been
+new panel with edit boxes for asteroid/occulting body distance (in AU ---
+
+astronomical units) and asteroid/shadow speed (in km per second) has been
 added. These values are needed in order to calculate a diffraction light curve.
 In addition to modeling diffraction effects, one can add the effect of a finite star
 disk to produce a penumbral curve. NOTE: PyOTE does not yet have the ability
 to correctly analyze a penumbral curve where it takes more than 1 or 2 readings
 for the transition. That project is under way and will be in the next version.
 version 3.3.9
-
-•
-
-Automatically installs cv2 if not already present. This package is needed for the
+• Automatically installs cv2 if not already present. This package is needed for the
 new frame view feature.
-
 version 3.3.8
 • If the video referenced in the csv file can be found, there is now an automatic
 display of the D and R frames relevant to calculating correct D and R times so
 that the user can verify that timestamp OCR extracted the correct timestamp
 values.
 version 3.3.7
 • A new button (View frame) with an associated spinner for entry of a frame
@@ -1086,22 +1085,22 @@
 Another use for this feature is to handle the case where there is a visual timestamp, but
 either OCR was not activated during the .csv preparation, or the timestamp overlay
 came from an unsupported VTI type. The workflow would be to let PyOTE find the D
 and R frame values, but before pressing ... write report, do a Manual timestamp
 entry for the D and R frame entries found by viewing the relevant frames and entering
 the correct times in the Manual timestamp dialog.
 It should be noted that the manual timestamp entry can be performed even when
-timestamps were already present in the file --- your manual entries will cause all the
+
+timestamps were already present in the file --- your manual entries will cause all the
 timestamps to be recalculated.
 version 3.3.5:
 • Changed usage of max([a, b ,c]) to max(a, b, c) to see if this allows the Numba
 JIT compiler to work for one user that found version 3.3.4 failed to load/compile.
 This should have no effect on users that already have version 3.3.4 working.
-
-version 3.3.4:
+version 3.3.4:
 • To shorten the time to find 'solutions', I used the Numba JIT (just-in-time)
 platform independent compiler that produces machine code from Python bytecode. You may notice a very slight increase in the time to start-up PyOTE
 because I do those compile operations while PyOTE is being loaded.
 version 3.3.2:
 • Adds a false-positive probability calculation and printout in the final report. This
 number is the fraction of 'false drops' found during the 50,000 tests that are
 greater than or equal to the drop value extracted from the actual observation.
@@ -1125,25 +1124,29 @@
 help. This scheme was introduced in PyMovie and I found it easier to use than
 the 'hover' scheme. In practice, the 'hover' popped up when it was not needed,
 so most users eventually disabled it. As a result, it became so tedious to look at
 help --- enable hover; hover; read; disable hover --- that the help system was
 used less and less. The right-click-for-help is always available and easily
 invoked --- hopefully this will encourage more frequent reference to it.
 version 3.2.6
-• This is a 'cosmetic' release --- there should be NO detectable differences from
+
+•
+•
+•
+
+•
+
+This is a 'cosmetic' release --- there should be NO detectable differences from
 version 3.2.5 in terms of functionality.
-• All python files were brought into compliance with PEP 8 coding standards.
+All python files were brought into compliance with PEP 8 coding standards.
 Only I care about that.
-• More significantly, I removed the dependency on C code by using Numba as a
+More significantly, I removed the dependency on C code by using Numba as a
 code accelerator instead of Cython. As a result, I no longer need to compile
 separate code versions for Mac, Windows, and Linux. That makes my life
 easier, but you should experience no operational changes.
-
-•
-
 All this 'cosmetic' work is in preparation for working on PyOTE issues again.
 
 version 3.2.5
 • Added special test for Tangra files to detect the empty fields (which MUST be
 fixed) that Tangra outputs whenever it has trouble extracted a value from an
 aperture. It prints a message and stops all further processing, forcing the user
 to attend to and deal with the missing values.
@@ -1173,22 +1176,22 @@
 superfluous commas at the end of data lines (that Tangra did NOT put there).
 Until this version, that 'butchered' file could not be read. This version adds code
 to parse data lines only up to the first non-empty column. Hopefully this will not
 have ramifications in the future (like a format change that has empty fields
 followed by non-empty fields --- not a likely expectation).
 version 3.2.0
 • Changed GUI to better align text on min max edit boxes to avoid confusion.
-version 3.1.9
+
+version 3.1.9
 • Fixed a bug in the test for a min/max solution search being constrained by a too
 large min value.
 version 3.1.8
 • version 3.1.7 was released without an updated version history. Here is what
 was changed in 3.1.7:
-
-•
+•
 
 Added the ability to write the data table that is displayed in the lower left corner
 of the GUI out as a csv file. Now, if timestamps and block integration operations
 are performed on the input file, those results can be preserved in a csv file.
 A 'file save' dialog is provided should you wish to change the default name and
 location of the resulting file. The default name is that of the input file with the
 text .PYOTE inserted to the left of the .csv extension. The default location is the
@@ -1218,28 +1221,29 @@
 •
 
 Cleaned up some language in tooltips.
 
 version 3.1.3:
 • Expanded manual timestamp preset time deltas to include NTSC and PAL field
 times. Also added ability to evaluate numeric expressions entered in the
-'Custom time' box: now you can type 1.001/60.0 in that box if you wish.
+
+'Custom time' box: now you can type 1.001/60.0 in that box if you wish.
 •
 
 Eliminated the 'entry num' column in the data matrix at the lower left of the GUI.
 The 'entry num' is unused and a possible source of confusion with the frame or
 field number for the unwary.
 
 •
 
 Added all the light curves read from the input file to the data matrix display.
 Previously, only the first light curve values were displayed. This is done in
-
-anticipation of adding a 'write csv' button to memorialize the result of a manual
+anticipation of adding a 'write csv' button to memorialize the result of a manual
 timestamp entry.
+
 version 3.1.2:
 • Added a test for possible dropped frames identical to that done in R-OTE when
 manual timestamp is utilized. The test is to calculate the expected number of
 frames based on standard NTSC/PAL frame times and compare that number
 with the count of frames enclosed by the early and late timestamps. If there is a
 mismatch of more than 0.12 frames, a warning is popped up and a log entry
 made. It is possible to use a 'custom' frame time if your camera differs from
@@ -1270,22 +1274,22 @@
 Desktop the first time pyote is run. Double-clicking on that Desktop file icon will
 start pyote thereafter.
 version 3.0.8:
 • Added a Windows batch file to the distribution that, when executed, will startup
 pyote. The file is called PYOTE.bat and is automatically copied to
 C:\Anaconda3 (if it is not already there) when pyote is first run. Now, to create a
 clickable desktop icon for starting up pyote, a user need only go to the
-C:\Anaconda3 directory, locate the PYOTE.bat file, create a shortcut to it, and
+
+C:\Anaconda3 directory, locate the PYOTE.bat file, create a shortcut to it, and
 drag the shortcut to the desktop. Remember, that file does not appear until the
 first run of pyote.
 The ‘skipped’ version numbers were caused by the need for repeated testing of
 this new feature, each test requiring a new version, even though functionality did
 not change,
-
-version 3.0.1:
+version 3.0.1:
 • Restored the vertical splitter between the command/plot area and the
 table/report area. Somewhere along the line this capability was accidentally
 removed, and the lack of the splitter was not noticed. Now it’s back.
 version 3.0.0:
 • No code changes. This version is the same as 2.1.6 except that it is built on
 python 3.7. The previous versions used python 3.6. This allows new users to
 install the latest Anaconda3 version (which installs python 3.7) without fiddling
@@ -1310,23 +1314,23 @@
 • To ease usage of the automatic block integration feature, accepting the
 automatically determined block integration parameters no longer uses a modal
 query box, which interfered with the ability to explore/expand the light curve plot.
 Now there is separate button which gets enabled after an automatic block
 integration completes.
 version 2.1.1
 • Added progress bar tracking of block integration analysis because it can take an
-extended amount of time to complete the analysis when the light curve has
+
+extended amount of time to complete the analysis when the light curve has
 many points.
 version 2.1.0
 • Added automatic determination of 'correct' block size and offset for block
 integration when user clicks Block integrate button without selecting the two
 points normally required to specify integration block beginning and end. The
 user can choose to accept or reject pyote's opinion of the correct parameters to
-
-use when the automation determination is invoked.
+use when the automation determination is invoked.
 version 2.0.9
 • Made the selection of Tooltip display 'sticky'
 • Duration calculation when D and R span midnight now handled correctly
 version 2.0.8
 • toolTips changed to invoke and display in a custom dialog box that can be
 moved and resized to better accommodate legacy displays
 • Calc flash timing calculation fixed to properly deal with the non-integer frame
@@ -1361,24 +1365,25 @@
 During the error bar calculation, it is possible for the Cholesky decomposition
 needed for treating correlated noise to fail. Previous versions treated this as a
 fatal error and would not produce a final report. This version instead treats the
 noise as uncorrelated and continues processing to produce a final report.
 
 version 2.0.6
 • Added additional instruction in the popup that appears when no timestamps are
-found in the csv file. This will give casual users additional guidance and
+
+found in the csv file. This will give casual users additional guidance and
 clarification for the manual timestamp entry process.
 version 2.0.5
 • files generated by pyote now contain PYOTE in the filename.
 •
 
 Timestamps can be corrupted to the point that a timeDelta of 0.0 can result.
 This version traps that event and reports it clearly --- 2.0.4 failed silently with a
+divide by zero exception
 
-divide by zero exception
 version 2.0.4
 • improves the handling of errors during the reading of Tangra files by showing
 the offending line in the report panel. Tangra, if it has a tracking problem (i.e.,
 loses it) will emit an empty field for that measurement, leaving it up to the user
 to decide how to fill in the missing value. Prior pyote versions simply reported
 'format error' without providing a printout of the offending line. This version fixes
 that.
@@ -1411,27 +1416,27 @@
 
 version 1.47
 • adds bold red highlighting to message:
 ! There is something wrong with timestamps at D and/or R or frames have been dropped !
 
 so that it is harder to miss.
 
-version 1.46
+version 1.46
 • adds automatic recalculation of baseline and event noise parameters utilizing all
 available data points during a second solution pass; this removes the variability
 in calculated error bars due to user selection of a necessarily less complete set
 of data points for noise analysis during the first solution pass.
 •
 
 adds bold blue text in the 'Excel' portion of the final report to indicate whether or
 not the light curve was block integrated, trimmed, or normalized. Failing to block
-
-integrate a light curve that needed it is a common error. Highlighting the
+integrate a light curve that needed it is a common error. Highlighting the
 presence or absence of block integration in the most looked at portion of the
 final report will hopefully help reduce the number of such errors.
+
 Version 1.45
 • the initial fully functional release of pyote.
 
 Introduction to pyote
 Bob Anderson (bob.anderson.ok@gmail.com)
 pyote is an occultation timing extraction utility program written primarily in python and
 distributed through PyPI (the python package repository).
```

### Comparing `pyote-5.3.1/src/pyoteapp/pyote.py` & `pyote-5.3.2/src/pyoteapp/pyote.py`

 * *Files 1% similar despite different names*

```diff
@@ -5522,15 +5522,22 @@
         mousePoint = self.mainPlotViewBox.mapSceneToView(pos)
         self.verticalCursor.setPos(round(mousePoint.x()))
 
     def writeDefaultGraphicsPlots(self, error_bar_plots_available=True):
         if not error_bar_plots_available:
             return
 
-        self.graphicFile, _ = os.path.splitext(self.csvFilePath)
+        lightCurveDir = os.path.dirname(self.csvFilePath)  # This gets the folder where the light-curve.csv is located
+        self.graphicFile = os.path.join(lightCurveDir, 'FP-plots')
+        if not os.path.exists(self.graphicFile):
+            os.mkdir(self.graphicFile)
+        head, tail = os.path.split(self.csvFilePath)
+        name_to_use, _ = os.path.splitext(tail)
+
+        self.graphicFile = os.path.join(self.graphicFile, name_to_use)
 
         exporter = FixedImageExporter(self.dBarPlotItem)
         exporter.makeWidthHeightInts()
         targetFileD = self.graphicFile + '.D_pyote.png'
         exporter.export(targetFileD)
 
         exporter = FixedImageExporter(self.durBarPlotItem)
@@ -7152,19 +7159,19 @@
 
         if self.targetKey == '':
             self.targetKey = self.lightcurveTitles[0].text()
 
         self.showMsg(f'fit metrics for {self.targetKey}', blankLine=False, bold=True)
 
         # Calculate false-positive ratio
-        margin = self.observedDrop - self.maxNoiseInducedDrop
+        # margin = self.observedDrop - self.maxNoiseInducedDrop
         # false_positive_ratio = margin / self.maxNoiseInducedDrop
+
         false_positive_metric = self.observedDrop / self.maxNoiseInducedDrop - 1.0
 
-        time_uncertainty = (self.deltaDhi95 - self.deltaDlo95) / 2.0 * self.timeDelta
         time_uncertainty = max(abs(self.deltaDhi95), abs(self.deltaDlo95)) * self.timeDelta
 
         stats_msg = f'\nfit metrics === false-positive metric: {false_positive_metric:0.3f} ' \
                     f'time error bar: +/- {time_uncertainty:0.4f} seconds' \
                     f'   DNR: {self.snrB:0.2f}  '
         self.showMsg(stats_msg, blankLine=False, bold=True)
 
@@ -7188,15 +7195,18 @@
             self.showMsg(stats_msg, blankLine=False, bold=True)
 
         if self.eventType == 'Ronly' or self.eventType == 'DandR':
             stats_msg = f'\nfit metrics === R frame number: {self.Rframe:0.4f}'
             self.showMsg(stats_msg, blankLine=False, bold=True)
 
         if self.eventType == 'DandR':
-            duration = (self.Rframe - self.Dframe) * (self.timeDelta / self.blockSize)
+            time_at_R = convertTimeStringToTime(self.Rtimestring)
+            time_at_D = convertTimeStringToTime(self.Dtimestring)
+            duration = time_at_R - time_at_D
+            # duration = (self.Rframe - self.Dframe) * (self.timeDelta / self.blockSize)
             stats_msg = f'\nfit metrics === duration: {duration:0.4f} seconds'
             self.showMsg(stats_msg, blankLine=False, bold=True)
 
         if self.eventType == 'Donly' or self.eventType == 'DandR':
             stats_msg = f'\nfit metrics === D time: {self.Dtimestring}'
             self.showMsg(stats_msg, blankLine=False, bold=True)
 
@@ -7948,18 +7958,42 @@
 
             # 4.6.1 change
             # obs[eventStart:eventStart+event_duration+1] -= observed_drop
             obs[eventStart:eventStart + event_duration] -= redDrop
 
             pw.plot(obs)
             pw.plot(obs, pen=None, symbol='o', symbolBrush=(0, 0, 255), symbolSize=6)
-            left_marker = pg.InfiniteLine(pos=eventStart, pen='r')
-            pw.addItem(left_marker)
-            right_marker = pg.InfiniteLine(pos=eventStart + event_duration, pen='g')
-            pw.addItem(right_marker)
+
+            # left_marker = pg.InfiniteLine(pos=eventStart, pen='r')
+            # pw.addItem(left_marker)
+            # right_marker = pg.InfiniteLine(pos=eventStart + event_duration, pen='g')
+            # pw.addItem(right_marker)
+
+            # Plot the square wave
+            x_vals = []
+            y_vals = []
+            x_vals.append(0)
+            y_vals.append(self.B)
+
+            x_vals.append(eventStart - 1)
+            y_vals.append(self.B)
+
+            x_vals.append(eventStart)
+            y_vals.append(self.A)
+
+            x_vals.append(eventStart+event_duration)
+            y_vals.append(self.A)
+
+            x_vals.append(eventStart+event_duration + 1)
+            y_vals.append(self.B)
+
+            x_vals.append(len(obs)-1)
+            y_vals.append(self.B)
+
+            pw.plot(x_vals, y_vals, pen=pg.mkPen([255, 0, 0], width=4))
 
             if self.writeExampleLightcurveCheckBox.isChecked():
                 # Write the example lightcurve (obs) to a csv file
                 self.writeExampleLightcurveToFile(obs, self.timeDelta)
 
         return
 
@@ -8967,18 +9001,37 @@
             self.userDeterminedBaselineStats = False
             self.userDeterminedEventStats = False
             self.setWindowTitle('PYOTE Version: ' + version.version() + '  File being processed: ' + self.csvFilePath)
             dirpath, _ = os.path.split(self.csvFilePath)
             self.logFile, _ = os.path.splitext(self.csvFilePath)
             self.logFile = self.logFile + '.pyote_log.txt'
 
-            self.detectabilityLogFile, _ = os.path.splitext(self.csvFilePath)
+            # self.detectabilityLogFile, _ = os.path.splitext(self.csvFilePath)
+            # self.detectabilityLogFile = self.detectabilityLogFile + '.pyote_detectability.txt'
+
+            lightCurveDir = os.path.dirname(self.csvFilePath)  # This gets the folder where the light-curve.csv is located
+            self.detectabilityLogFile = os.path.join(lightCurveDir, 'Detectability')
+            if not os.path.exists(self.detectabilityLogFile):
+                os.mkdir(self.detectabilityLogFile)
+            head, tail = os.path.split(self.csvFilePath)
+            name_to_use, _ = os.path.splitext(tail)
+            self.detectabilityLogFile = os.path.join(self.detectabilityLogFile, name_to_use)
             self.detectabilityLogFile = self.detectabilityLogFile + '.pyote_detectability.txt'
 
-            self.normalizationLogFile, _ = os.path.splitext(self.csvFilePath)
+            # self.normalizationLogFile, _ = os.path.splitext(self.csvFilePath)
+            # self.normalizationLogFile = self.normalizationLogFile + '.pyote_normalization.txt'
+
+            lightCurveDir = os.path.dirname(
+                self.csvFilePath)  # This gets the folder where the light-curve.csv is located
+            self.normalizationLogFile = os.path.join(lightCurveDir, 'Normalization')
+            if not os.path.exists(self.normalizationLogFile):
+                os.mkdir(self.normalizationLogFile)
+            head, tail = os.path.split(self.csvFilePath)
+            name_to_use, _ = os.path.splitext(tail)
+            self.normalizationLogFile = os.path.join(self.normalizationLogFile, name_to_use)
             self.normalizationLogFile = self.normalizationLogFile + '.pyote_normalization.txt'
 
             curDateTime = datetime.datetime.today().ctime()
             self.showMsg('')
             self.showMsg(
                 '#' * 20 + ' PYOTE ' + version.version() + '  session started: ' + curDateTime + '  ' + '#' * 20)
```

### Comparing `pyote-5.3.1/src/pyoteapp/pyote_modelling_utility_functions.py` & `pyote-5.3.2/src/pyoteapp/pyote_modelling_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/showVideoFrames.py` & `pyote-5.3.2/src/pyoteapp/showVideoFrames.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/solverUtils.py` & `pyote-5.3.2/src/pyoteapp/solverUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/subframe_timing_utilities.py` & `pyote-5.3.2/src/pyoteapp/subframe_timing_utilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/timestampDialog.py` & `pyote-5.3.2/src/pyoteapp/timestampDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.1/src/pyoteapp/timestampUtils.py` & `pyote-5.3.2/src/pyoteapp/timestampUtils.py`

 * *Files identical despite different names*

