# Comparing `tmp/CASCADe-spectroscopy-1.2.2.tar.gz` & `tmp/CASCADe-spectroscopy-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CASCADe-spectroscopy-1.2.2.tar", last modified: Thu Feb  9 17:59:46 2023, max compression
+gzip compressed data, was "CASCADe-spectroscopy-1.2.3.tar", last modified: Sun Jul 16 10:35:58 2023, max compression
```

## Comparing `CASCADe-spectroscopy-1.2.2.tar` & `CASCADe-spectroscopy-1.2.3.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/CASCADe_spectroscopy.egg-info/
--rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-02-09 17:59:46.000000 CASCADe-spectroscopy-1.2.2/CASCADe_spectroscopy.egg-info/PKG-INFO
--rw-r--r--   0 bouwman  (10420) users      (100)     1604 2023-02-09 17:59:46.000000 CASCADe-spectroscopy-1.2.2/CASCADe_spectroscopy.egg-info/SOURCES.txt
--rw-r--r--   0 bouwman  (10420) users      (100)        1 2023-02-09 17:59:46.000000 CASCADe-spectroscopy-1.2.2/CASCADe_spectroscopy.egg-info/dependency_links.txt
--rw-r--r--   0 bouwman  (10420) users      (100)      241 2023-02-09 17:59:46.000000 CASCADe-spectroscopy-1.2.2/CASCADe_spectroscopy.egg-info/requires.txt
--rw-r--r--   0 bouwman  (10420) users      (100)       14 2023-02-09 17:59:46.000000 CASCADe-spectroscopy-1.2.2/CASCADe_spectroscopy.egg-info/top_level.txt
--rw-r--r--   0 bouwman  (10420) users      (100)    35149 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.2/LICENSE.txt
--rw-rw-r--   0 bouwman  (10420) users      (100)      146 2022-01-29 13:05:24.000000 CASCADe-spectroscopy-1.2.2/MANIFEST.in
--rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/PKG-INFO
--rw-r--r--   0 bouwman  (10420) users      (100)    20448 2022-05-04 13:20:33.000000 CASCADe-spectroscopy-1.2.2/README.md
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/cascade/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/cascade/TSO/
--rw-r--r--   0 bouwman  (10420) users      (100)   111340 2023-02-01 18:11:59.000000 CASCADe-spectroscopy-1.2.2/cascade/TSO/TSO.py
--rw-r--r--   0 bouwman  (10420) users      (100)      118 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.2/cascade/TSO/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      534 2023-02-09 17:18:52.000000 CASCADe-spectroscopy-1.2.2/cascade/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/cascade/build_archive/
--rw-r--r--   0 bouwman  (10420) users      (100)      150 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.2/cascade/build_archive/__init__.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    26971 2023-01-19 10:42:28.000000 CASCADe-spectroscopy-1.2.2/cascade/build_archive/build_archive.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/cascade/cpm_model/
--rw-r--r--   0 bouwman  (10420) users      (100)      138 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.2/cascade/cpm_model/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   142804 2023-02-09 17:12:56.000000 CASCADe-spectroscopy-1.2.2/cascade/cpm_model/cpm_model.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/cascade/data_model/
--rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.2/cascade/data_model/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    33058 2022-12-13 22:35:41.000000 CASCADe-spectroscopy-1.2.2/cascade/data_model/data_model.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/cascade/exoplanet_tools/
--rw-r--r--   0 bouwman  (10420) users      (100)      157 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.2/cascade/exoplanet_tools/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   106159 2023-01-19 14:45:52.000000 CASCADe-spectroscopy-1.2.2/cascade/exoplanet_tools/exoplanet_tools.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/cascade/initialize/
--rw-r--r--   0 bouwman  (10420) users      (100)      142 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.2/cascade/initialize/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    33472 2023-01-23 08:17:03.000000 CASCADe-spectroscopy-1.2.2/cascade/initialize/initialize.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.038492 CASCADe-spectroscopy-1.2.2/cascade/instruments/
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/cascade/instruments/Generic/
--rw-r--r--   0 bouwman  (10420) users      (100)    16487 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/Generic/Generic.py
--rw-r--r--   0 bouwman  (10420) users      (100)       67 2019-07-02 16:36:37.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/Generic/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/cascade/instruments/HST/
--rw-r--r--   0 bouwman  (10420) users      (100)    97326 2023-01-23 08:09:03.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/HST/HST.py
--rw-r--r--   0 bouwman  (10420) users      (100)      123 2019-07-01 18:06:29.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/HST/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)     2577 2019-07-02 16:05:13.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/InstrumentsBaseClasses.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/cascade/instruments/JWST/
--rw-r--r--   0 bouwman  (10420) users      (100)    61037 2022-12-13 19:34:07.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/JWST/JWST.py
--rw-r--r--   0 bouwman  (10420) users      (100)       68 2019-07-02 16:14:39.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/JWST/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)     5048 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/ObservationGenerator.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/cascade/instruments/Spitzer/
--rw-r--r--   0 bouwman  (10420) users      (100)    46648 2022-01-30 23:14:50.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/Spitzer/Spitzer.py
--rw-r--r--   0 bouwman  (10420) users      (100)      135 2019-07-01 18:06:42.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/Spitzer/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      614 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.2/cascade/instruments/__init__.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/cascade/spectral_extraction/
--rw-r--r--   0 bouwman  (10420) users      (100)      169 2019-07-23 14:55:38.000000 CASCADe-spectroscopy-1.2.2/cascade/spectral_extraction/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)   108152 2022-07-25 12:36:07.000000 CASCADe-spectroscopy-1.2.2/cascade/spectral_extraction/spectral_extraction.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/cascade/utilities/
--rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.2/cascade/utilities/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)    10685 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.2/cascade/utilities/readwrite_spectra.py
--rw-r--r--   0 bouwman  (10420) users      (100)    27545 2022-07-25 12:33:13.000000 CASCADe-spectroscopy-1.2.2/cascade/utilities/utilities.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/cascade/verbose/
--rw-r--r--   0 bouwman  (10420) users      (100)      132 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.2/cascade/verbose/__init__.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    40342 2022-07-23 06:59:01.000000 CASCADe-spectroscopy-1.2.2/cascade/verbose/verbose.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/scripts/
--rwxr-xr-x   0 bouwman  (10420) users      (100)    23962 2022-01-30 20:40:13.000000 CASCADe-spectroscopy-1.2.2/scripts/build_local_hst_archive.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)     7757 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.2/scripts/run_cascade.py
--rwxr-xr-x   0 bouwman  (10420) users      (100)    12362 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.2/scripts/run_cascade.sh
--rwxr-xr-x   0 bouwman  (10420) users      (100)     4042 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.2/scripts/run_stats.sh
--rwxrwxr-x   0 bouwman  (10420) users      (100)     1927 2022-02-02 15:07:16.000000 CASCADe-spectroscopy-1.2.2/scripts/setup_cascade.py
--rw-r--r--   0 bouwman  (10420) users      (100)       38 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/setup.cfg
--rw-r--r--   0 bouwman  (10420) users      (100)     2671 2023-02-09 17:18:52.000000 CASCADe-spectroscopy-1.2.2/setup.py
-drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-02-09 17:59:46.042492 CASCADe-spectroscopy-1.2.2/tests/
--rw-r--r--   0 bouwman  (10420) users      (100)        0 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.2/tests/__init__.py
--rw-r--r--   0 bouwman  (10420) users      (100)      491 2019-02-17 14:49:38.000000 CASCADe-spectroscopy-1.2.2/tests/cascade_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     1212 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.2/tests/cpm_model_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     4940 2019-02-17 14:50:18.000000 CASCADe-spectroscopy-1.2.2/tests/data_model_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     5889 2022-01-31 10:08:59.000000 CASCADe-spectroscopy-1.2.2/tests/exoplanet_tools_tests.py
--rw-r--r--   0 bouwman  (10420) users      (100)     2054 2022-01-25 23:52:24.000000 CASCADe-spectroscopy-1.2.2/tests/initialize_tests.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.819157 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/
+-rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/PKG-INFO
+-rw-r--r--   0 bouwman  (10420) users      (100)     1604 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/SOURCES.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)        1 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/dependency_links.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)      241 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/requires.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)       14 2023-07-16 10:35:58.000000 CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/top_level.txt
+-rw-r--r--   0 bouwman  (10420) users      (100)    35149 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/LICENSE.txt
+-rw-rw-r--   0 bouwman  (10420) users      (100)      146 2022-01-29 13:05:24.000000 CASCADe-spectroscopy-1.2.3/MANIFEST.in
+-rw-r--r--   0 bouwman  (10420) users      (100)    21158 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/PKG-INFO
+-rw-r--r--   0 bouwman  (10420) users      (100)    20448 2022-05-04 13:20:33.000000 CASCADe-spectroscopy-1.2.3/README.md
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.819157 CASCADe-spectroscopy-1.2.3/cascade/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.819157 CASCADe-spectroscopy-1.2.3/cascade/TSO/
+-rw-r--r--   0 bouwman  (10420) users      (100)   111340 2023-02-01 18:11:59.000000 CASCADe-spectroscopy-1.2.3/cascade/TSO/TSO.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      118 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/TSO/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      534 2023-07-16 10:27:24.000000 CASCADe-spectroscopy-1.2.3/cascade/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.819157 CASCADe-spectroscopy-1.2.3/cascade/build_archive/
+-rw-r--r--   0 bouwman  (10420) users      (100)      150 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.3/cascade/build_archive/__init__.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    26971 2023-01-19 10:42:28.000000 CASCADe-spectroscopy-1.2.3/cascade/build_archive/build_archive.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.823157 CASCADe-spectroscopy-1.2.3/cascade/cpm_model/
+-rw-r--r--   0 bouwman  (10420) users      (100)      138 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/cpm_model/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   143269 2023-02-09 20:42:11.000000 CASCADe-spectroscopy-1.2.3/cascade/cpm_model/cpm_model.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.823157 CASCADe-spectroscopy-1.2.3/cascade/data_model/
+-rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/data_model/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    33058 2022-12-13 22:35:41.000000 CASCADe-spectroscopy-1.2.3/cascade/data_model/data_model.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.823157 CASCADe-spectroscopy-1.2.3/cascade/exoplanet_tools/
+-rw-r--r--   0 bouwman  (10420) users      (100)      157 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/exoplanet_tools/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   106303 2023-07-16 10:10:15.000000 CASCADe-spectroscopy-1.2.3/cascade/exoplanet_tools/exoplanet_tools.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.823157 CASCADe-spectroscopy-1.2.3/cascade/initialize/
+-rw-r--r--   0 bouwman  (10420) users      (100)      142 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/initialize/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    33472 2023-01-23 08:17:03.000000 CASCADe-spectroscopy-1.2.3/cascade/initialize/initialize.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.827157 CASCADe-spectroscopy-1.2.3/cascade/instruments/
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.827157 CASCADe-spectroscopy-1.2.3/cascade/instruments/Generic/
+-rw-r--r--   0 bouwman  (10420) users      (100)    16487 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/Generic/Generic.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       67 2019-07-02 16:36:37.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/Generic/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.827157 CASCADe-spectroscopy-1.2.3/cascade/instruments/HST/
+-rw-r--r--   0 bouwman  (10420) users      (100)    97326 2023-01-23 08:09:03.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/HST/HST.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      123 2019-07-01 18:06:29.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/HST/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     2577 2019-07-02 16:05:13.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/InstrumentsBaseClasses.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/instruments/JWST/
+-rw-r--r--   0 bouwman  (10420) users      (100)    61037 2022-12-13 19:34:07.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/JWST/JWST.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       68 2019-07-02 16:14:39.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/JWST/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     5048 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/ObservationGenerator.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/instruments/Spitzer/
+-rw-r--r--   0 bouwman  (10420) users      (100)    46648 2022-01-30 23:14:50.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/Spitzer/Spitzer.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      135 2019-07-01 18:06:42.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/Spitzer/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      614 2022-04-20 16:22:53.000000 CASCADe-spectroscopy-1.2.3/cascade/instruments/__init__.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/spectral_extraction/
+-rw-r--r--   0 bouwman  (10420) users      (100)      169 2019-07-23 14:55:38.000000 CASCADe-spectroscopy-1.2.3/cascade/spectral_extraction/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)   108152 2022-07-25 12:36:07.000000 CASCADe-spectroscopy-1.2.3/cascade/spectral_extraction/spectral_extraction.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/utilities/
+-rw-r--r--   0 bouwman  (10420) users      (100)      139 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/cascade/utilities/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    10685 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.3/cascade/utilities/readwrite_spectra.py
+-rw-r--r--   0 bouwman  (10420) users      (100)    27545 2022-07-25 12:33:13.000000 CASCADe-spectroscopy-1.2.3/cascade/utilities/utilities.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.831157 CASCADe-spectroscopy-1.2.3/cascade/verbose/
+-rw-r--r--   0 bouwman  (10420) users      (100)      132 2020-11-16 11:16:32.000000 CASCADe-spectroscopy-1.2.3/cascade/verbose/__init__.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    40342 2022-07-23 06:59:01.000000 CASCADe-spectroscopy-1.2.3/cascade/verbose/verbose.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/scripts/
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    23962 2022-01-30 20:40:13.000000 CASCADe-spectroscopy-1.2.3/scripts/build_local_hst_archive.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)     7757 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.3/scripts/run_cascade.py
+-rwxr-xr-x   0 bouwman  (10420) users      (100)    12362 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.3/scripts/run_cascade.sh
+-rwxr-xr-x   0 bouwman  (10420) users      (100)     4042 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.3/scripts/run_stats.sh
+-rwxrwxr-x   0 bouwman  (10420) users      (100)     1927 2022-02-02 15:07:16.000000 CASCADe-spectroscopy-1.2.3/scripts/setup_cascade.py
+-rw-r--r--   0 bouwman  (10420) users      (100)       38 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/setup.cfg
+-rw-r--r--   0 bouwman  (10420) users      (100)     2671 2023-07-16 10:27:24.000000 CASCADe-spectroscopy-1.2.3/setup.py
+drwxr-xr-x   0 bouwman  (10420) users      (100)        0 2023-07-16 10:35:58.835157 CASCADe-spectroscopy-1.2.3/tests/
+-rw-r--r--   0 bouwman  (10420) users      (100)        0 2019-02-08 13:35:07.000000 CASCADe-spectroscopy-1.2.3/tests/__init__.py
+-rw-r--r--   0 bouwman  (10420) users      (100)      491 2019-02-17 14:49:38.000000 CASCADe-spectroscopy-1.2.3/tests/cascade_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     1212 2020-11-16 11:16:33.000000 CASCADe-spectroscopy-1.2.3/tests/cpm_model_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     4940 2019-02-17 14:50:18.000000 CASCADe-spectroscopy-1.2.3/tests/data_model_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     5889 2022-01-31 10:08:59.000000 CASCADe-spectroscopy-1.2.3/tests/exoplanet_tools_tests.py
+-rw-r--r--   0 bouwman  (10420) users      (100)     2054 2022-01-25 23:52:24.000000 CASCADe-spectroscopy-1.2.3/tests/initialize_tests.py
```

### Comparing `CASCADe-spectroscopy-1.2.2/CASCADe_spectroscopy.egg-info/PKG-INFO` & `CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: CASCADe-spectroscopy
-Version: 1.2.2
+Version: 1.2.3
 Summary: CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data
 Home-page: https://jbouwman.gitlab.io/CASCADe/
 Download-URL: https://gitlab.com/jbouwman/CASCADe
 Author: Jeroen Bouwman
 Author-email: bouwman@mpia.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.7, <3.10
+Requires-Python: >=3.8, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 [![pipeline status](https://gitlab.com/jbouwman/CASCADe/badges/master/pipeline.svg)](https://gitlab.com/jbouwman/CASCADe/commits/master)
 
 #  <span style="color:#1F618D">CASCADe </span>: <span style="color:#1F618D">C</span>alibration of tr<span style="color:#1F618D">A</span>nsit <span style="color:#1F618D">S</span>pectroscopy using <span style="color:#1F618D">CA</span>usal <span style="color:#1F618D">D</span>ata
```

### Comparing `CASCADe-spectroscopy-1.2.2/CASCADe_spectroscopy.egg-info/SOURCES.txt` & `CASCADe-spectroscopy-1.2.3/CASCADe_spectroscopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/LICENSE.txt` & `CASCADe-spectroscopy-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/PKG-INFO` & `CASCADe-spectroscopy-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: CASCADe-spectroscopy
-Version: 1.2.2
+Version: 1.2.3
 Summary: CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data
 Home-page: https://jbouwman.gitlab.io/CASCADe/
 Download-URL: https://gitlab.com/jbouwman/CASCADe
 Author: Jeroen Bouwman
 Author-email: bouwman@mpia.de
 License: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
-Requires-Python: >=3.7, <3.10
+Requires-Python: >=3.8, <3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 [![pipeline status](https://gitlab.com/jbouwman/CASCADe/badges/master/pipeline.svg)](https://gitlab.com/jbouwman/CASCADe/commits/master)
 
 #  <span style="color:#1F618D">CASCADe </span>: <span style="color:#1F618D">C</span>alibration of tr<span style="color:#1F618D">A</span>nsit <span style="color:#1F618D">S</span>pectroscopy using <span style="color:#1F618D">CA</span>usal <span style="color:#1F618D">D</span>ata
```

### Comparing `CASCADe-spectroscopy-1.2.2/README.md` & `CASCADe-spectroscopy-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/TSO/TSO.py` & `CASCADe-spectroscopy-1.2.3/cascade/TSO/TSO.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/__init__.py` & `CASCADe-spectroscopy-1.2.3/cascade/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*
 """
 CASCADe init file.
 
 @author: Jeroen Bouwman
 """
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 __all__ = ['data_model', 'TSO', 'instruments', 'cpm_model',
            'initialize', 'exoplanet_tools', 'utilities',
            'spectral_extraction', 'build_archive', 'verbose']
 
 from . import data_model
 from . import TSO
 from . import instruments
```

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/build_archive/build_archive.py` & `CASCADe-spectroscopy-1.2.3/cascade/build_archive/build_archive.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/cpm_model/cpm_model.py` & `CASCADe-spectroscopy-1.2.3/cascade/cpm_model/cpm_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1451,44 +1451,44 @@
             DESCRIPTION. The default is None.
 
         Returns
         -------
         None.
 
         """
-        processed_parameters = copy.deepcopy(self.processed_parameters)
+        #processed_parameters = copy.deepcopy(self.processed_parameters)
 
         if bootstrap_chunk is None:
             bootstrap_chunk = list(
-                np.arange(processed_parameters.corrected_fitted_spectrum.shape[0])
+                np.arange(self.processed_parameters.corrected_fitted_spectrum.shape[0])
                 )
             bootstrap_sample_counter = list(
-                np.arange(processed_parameters.corrected_fitted_spectrum.shape[0])
+                np.arange(self.processed_parameters.corrected_fitted_spectrum.shape[0])
                 )
         else:
             bootstrap_chunk, bootstrap_sample_counter = bootstrap_chunk
 
-        processed_parameters.corrected_fitted_spectrum[bootstrap_chunk, ...] +=\
+        self.processed_parameters.corrected_fitted_spectrum[bootstrap_chunk, ...] =\
             new_parameters.corrected_fitted_spectrum[bootstrap_sample_counter, ...]
-        processed_parameters.fitted_baseline[bootstrap_chunk, ...] +=\
+        self.processed_parameters.fitted_baseline[bootstrap_chunk, ...] =\
             new_parameters.fitted_baseline
-        processed_parameters.fit_residuals[bootstrap_chunk, ...] +=\
+        self.processed_parameters.fit_residuals[bootstrap_chunk, ...] =\
             new_parameters.fit_residuals
-        processed_parameters.normed_fit_residuals[bootstrap_chunk, ...] +=\
+        self.processed_parameters.normed_fit_residuals[bootstrap_chunk, ...] =\
             new_parameters.normed_fit_residuals
-        processed_parameters.normed_fitted_spectrum[bootstrap_chunk, ...] +=\
+        self.processed_parameters.normed_fitted_spectrum[bootstrap_chunk, ...] =\
             new_parameters.normed_fitted_spectrum
-        processed_parameters.error_normed_fitted_spectrum[bootstrap_chunk, ...] +=\
+        self.processed_parameters.error_normed_fitted_spectrum[bootstrap_chunk, ...] =\
             new_parameters.error_normed_fitted_spectrum
-        processed_parameters.wavelength_normed_fitted_spectrum[bootstrap_chunk, ...] +=\
+        self.processed_parameters.wavelength_normed_fitted_spectrum[bootstrap_chunk, ...] =\
             new_parameters.wavelength_normed_fitted_spectrum
-        processed_parameters.stellar_spectrum[bootstrap_chunk, ...] +=\
+        self.processed_parameters.stellar_spectrum[bootstrap_chunk, ...] =\
             new_parameters.stellar_spectrum
 
-        self.processed_parameters = processed_parameters
+        #self.processed_parameters = processed_parameters
 
     def get_fitted_parameters(self, bootstrap_chunk=None):
         """
         Return the fitted parameters.
 
         Parameters
         ----------
@@ -2602,19 +2602,19 @@
 
         Returns
         -------
         TYPE
             DESCRIPTION.
 
         """
-        return ray.get(
+        return copy.deepcopy(ray.get(
             self.parameter_server_handle.get_fitted_parameters.remote(
                 bootstrap_chunk=bootstrap_chunk
                 )
-                       )
+                       ))
 
     def get_processed_parameters_from_server(self, bootstrap_chunk=None):
         """
         Grab fitted regression parameters from the parameter server.
 
         Parameters
         ----------
@@ -2622,19 +2622,19 @@
 
         Returns
         -------
         Simplenamespace
             Simple namespace containing all processed parameters.
 
         """
-        return ray.get(
+        return copy.deepcopy(ray.get(
             self.parameter_server_handle.get_processed_parameters.remote(
                 bootstrap_chunk=bootstrap_chunk
                 )
-                       )
+                       ))
 
     def get_regularization_parameters_from_server(self):
         """
         Get the regularization parameters from the parameter server.
 
         Returns
         -------
@@ -2971,15 +2971,15 @@
     def __init__(self, #initial_processed_parameters,
                  control_parameters,
                  fit_parameters, lightcurve_model,  correction_matrix,
                  bootsptrap_indici, boostrap_sample_index_chunk):
         #self.processed_parameters= copy.deepcopy(initial_processed_parameters)
         self.control_parameters = control_parameters
         self.bootsptrap_indici = bootsptrap_indici
-        self.boostrap_sample_index_chunk = copy.deepcopy(boostrap_sample_index_chunk)
+        self.boostrap_sample_index_chunk = boostrap_sample_index_chunk
         self.regression_results = fit_parameters.regression_results
         self.fitted_spectrum = fit_parameters.fitted_spectrum
         self.fitted_model = fit_parameters.fitted_model
         self.lightcurve_model = lightcurve_model
         self.correction_matrix = correction_matrix
 
         self.processed_parameters=SimpleNamespace()
@@ -3101,28 +3101,27 @@
         #    corrected_spectrum = \
         #        self.processed_parameters.corrected_fitted_spectrum[iboot,:]
         for bootstrap_counter, (iboot, bootstrap_selection, models, corrected_spectrum) in enumerate(
                 zip(self.boostrap_sample_index_chunk, self.bootsptrap_indici, self.fitted_model,
                     self.processed_parameters.corrected_fitted_spectrum
                     )
                 ):
-
-            baseline_model = np.zeros(
+            self.processed_parameters.fitted_baseline = np.zeros(
                 self.control_parameters.data_parameters.shape)
-            residual = np.ma.zeros(
+            self.processed_parameters.fit_residuals = np.ma.zeros(
                 self.control_parameters.data_parameters.shape)
-            normed_residual = np.ma.zeros(
+            self.processed_parameters.normed_fit_residuals = np.ma.zeros(
                 self.control_parameters.data_parameters.shape)
             lc_model = \
                 self.lightcurve_model.lightcurve_model[..., bootstrap_selection]
-            normed_spectrum = np.zeros((
+            self.processed_parameters.normed_fitted_spectrum = np.zeros((
                 self.control_parameters.data_parameters.max_spectral_points))
-            error_normed_spectrum = np.zeros(
+            self.processed_parameters.error_normed_fitted_spectrum = np.zeros(
                 self.control_parameters.data_parameters.max_spectral_points)
-            wavelength_normed_spectrum = np.zeros((
+            self.processed_parameters.wavelength_normed_fitted_spectrum = np.zeros((
                 self.control_parameters.data_parameters.max_spectral_points))
 
             regression_data_selections = \
                self.get_data_per_bootstrap_step(data_server_handle,
                                                  regressor_indici,
                                                  bootstrap_selection)
 
@@ -3132,30 +3131,30 @@
 
                 (il, _), (_, _), nwave = regression_selection
 
                 data_unscaled, wavelength, phase, covariance, mask= \
                     regression_data_selection
                 lc = lc_model[il, :]
                 base = models[ipixel] - (corrected_spectrum)[ipixel]*lc
-                baseline_model[il, :] = base
-                residual[il, :] = np.ma.array(data_unscaled - models[ipixel],
-                                  mask=mask)
+                self.processed_parameters.fitted_baseline[il, :] = base
+                self.processed_parameters.fit_residuals[il, :] = \
+                    np.ma.array(data_unscaled - models[ipixel], mask=mask)
 
                 data_normed = data_unscaled/base
                 covariance_normed = covariance*np.diag(base**-2)
                 normed_depth, error_normed_depth, sigma_hat = \
                     ols(lc[:, np.newaxis], data_normed-1.0,
                         covariance=covariance_normed)
-                normed_residual[il, :] = \
+                self.processed_parameters.normed_fit_residuals[il, :] = \
                     np.ma.array(data_normed-1.0-normed_depth*lc, mask=mask)
-                normed_spectrum[ipixel] = \
+                self.processed_parameters.normed_fitted_spectrum[ipixel] = \
                     normed_depth*self.lightcurve_model.dilution_correction[il, 0]
-                error_normed_spectrum[ipixel] = \
+                self.processed_parameters.error_normed_fitted_spectrum[ipixel] = \
                     error_normed_depth*self.lightcurve_model.dilution_correction[il, 0]
-                wavelength_normed_spectrum[ipixel] = wavelength
+                self.processed_parameters.wavelength_normed_fitted_spectrum[ipixel] = wavelength
 
             del regression_data_selections, regression_selection, regression_data_selection
             del data_unscaled, wavelength, phase, covariance, mask, il, nwave
             gc.collect()
             # self.processed_parameters.fitted_baseline[iboot,:] = baseline_model
             # self.processed_parameters.fit_residuals[iboot,:] = residual
             # self.processed_parameters.normed_fit_residuals[iboot,:] = \
@@ -3166,26 +3165,26 @@
             #     error_normed_spectrum
             # self.processed_parameters.wavelength_normed_fitted_spectrum[iboot,:] = \
             #     wavelength_normed_spectrum
             # self.processed_parameters.stellar_spectrum[iboot,:] = \
             #     corrected_spectrum/normed_spectrum
 
 
-            self.processed_parameters.fitted_baseline = baseline_model
-            self.processed_parameters.fit_residuals = residual
-            self.processed_parameters.normed_fit_residuals = \
-                normed_residual
-            self.processed_parameters.normed_fitted_spectrum = \
-                normed_spectrum
-            self.processed_parameters.error_normed_fitted_spectrum = \
-                error_normed_spectrum
-            self.processed_parameters.wavelength_normed_fitted_spectrum = \
-                wavelength_normed_spectrum
+            #self.processed_parameters.fitted_baseline = baseline_model
+            #self.processed_parameters.fit_residuals = residual
+            #self.processed_parameters.normed_fit_residuals = \
+            #    normed_residual
+            #self.processed_parameters.normed_fitted_spectrum = \
+            #    normed_spectrum
+            #self.processed_parameters.error_normed_fitted_spectrum = \
+            #    error_normed_spectrum
+            #self.processed_parameters.wavelength_normed_fitted_spectrum = \
+            #    wavelength_normed_spectrum
             self.processed_parameters.stellar_spectrum = \
-                corrected_spectrum/normed_spectrum
+                corrected_spectrum/self.processed_parameters.normed_fitted_spectrum
 
             self.update_parameters_on_server(parameter_server_handle,
                                              bootstrap_chunk=([iboot,], [bootstrap_counter,]))
             #bootstrap_counter += 1
         gc.collect()
```

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/data_model/data_model.py` & `CASCADe-spectroscopy-1.2.3/cascade/data_model/data_model.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/exoplanet_tools/exoplanet_tools.py` & `CASCADe-spectroscopy-1.2.3/cascade/exoplanet_tools/exoplanet_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1457,15 +1457,16 @@
     References
     ----------
     .. [2] Morello et al. 2019, (arXiv:1908.09599)
     """
 
     __valid_ld_laws = {'linear', 'quadratic', 'nonlinear'}
     __valid_model_grid = {'Atlas_2000', 'Phoenix_2012_13', 'Phoenix_2018',
-                          'Stagger_2015', 'Stagger_2018', 'Phoenix_drift_2012'}
+                          'Stagger_2015', 'Stagger_2018', 'Phoenix_drift_2012',
+                          'MPS_Atlas_set1_2023', 'MPS_Atlas_set2_2023'}
 
     def __init__(self, cascade_configuration):
         self.cascade_configuration = cascade_configuration
         if ast.literal_eval(self.cascade_configuration.catalog_use_catalog):
             self.par = self.return_par_from_db()
         else:
             self.par = self.return_par_from_ini()
@@ -2039,15 +2040,16 @@
 
     This class usines the Exotethys package to read a stellar model from
     a grid of stellar models and an instrument passband to create a
     simple simulated spectrum of the observed star.
     """
 
     __valid_model_grid = {'Atlas_2000', 'Phoenix_2012_13', 'Phoenix_2018',
-                          'Stagger_2015', 'Stagger_2018', 'Phoenix_drift_2012'}
+                          'Stagger_2015', 'Stagger_2018', 'Phoenix_drift_2012',
+                          'MPS_Atlas_set1_2023', 'MPS_Atlas_set2_2023'}
 
     def __init__(self, cascade_configuration):
         self.cascade_configuration = cascade_configuration
         if ast.literal_eval(self.cascade_configuration.catalog_use_catalog):
             self.par = self.return_par_from_db()
         else:
             self.par = self.return_par_from_ini()
```

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/initialize/initialize.py` & `CASCADe-spectroscopy-1.2.3/cascade/initialize/initialize.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/instruments/Generic/Generic.py` & `CASCADe-spectroscopy-1.2.3/cascade/instruments/Generic/Generic.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/instruments/HST/HST.py` & `CASCADe-spectroscopy-1.2.3/cascade/instruments/HST/HST.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/instruments/InstrumentsBaseClasses.py` & `CASCADe-spectroscopy-1.2.3/cascade/instruments/InstrumentsBaseClasses.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/instruments/JWST/JWST.py` & `CASCADe-spectroscopy-1.2.3/cascade/instruments/JWST/JWST.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/instruments/ObservationGenerator.py` & `CASCADe-spectroscopy-1.2.3/cascade/instruments/ObservationGenerator.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/instruments/Spitzer/Spitzer.py` & `CASCADe-spectroscopy-1.2.3/cascade/instruments/Spitzer/Spitzer.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/instruments/__init__.py` & `CASCADe-spectroscopy-1.2.3/cascade/instruments/__init__.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/spectral_extraction/spectral_extraction.py` & `CASCADe-spectroscopy-1.2.3/cascade/spectral_extraction/spectral_extraction.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/utilities/readwrite_spectra.py` & `CASCADe-spectroscopy-1.2.3/cascade/utilities/readwrite_spectra.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/utilities/utilities.py` & `CASCADe-spectroscopy-1.2.3/cascade/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/cascade/verbose/verbose.py` & `CASCADe-spectroscopy-1.2.3/cascade/verbose/verbose.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/scripts/build_local_hst_archive.py` & `CASCADe-spectroscopy-1.2.3/scripts/build_local_hst_archive.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/scripts/run_cascade.py` & `CASCADe-spectroscopy-1.2.3/scripts/run_cascade.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/scripts/run_cascade.sh` & `CASCADe-spectroscopy-1.2.3/scripts/run_cascade.sh`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/scripts/run_stats.sh` & `CASCADe-spectroscopy-1.2.3/scripts/run_stats.sh`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/scripts/setup_cascade.py` & `CASCADe-spectroscopy-1.2.3/scripts/setup_cascade.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/setup.py` & `CASCADe-spectroscopy-1.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     'description': 'CASCADe : Calibration of trAnsit Spectroscopy using CAusal Data',
     'long_description': README,
     'long_description_content_type': "text/markdown",
     'author': 'Jeroen Bouwman',
     'url': 'https://jbouwman.gitlab.io/CASCADe/',
     'download_url': 'https://gitlab.com/jbouwman/CASCADe',
     'author_email': 'bouwman@mpia.de',
-    'version': '1.2.2',
-    'python_requires': '>=3.7, <3.10',
+    'version': '1.2.3',
+    'python_requires': '>=3.8, <3.10',
     'license': 'GNU General Public License v3 (GPLv3)',
     'classifiers': ["Programming Language :: Python :: 3",
                     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
                     "Operating System :: OS Independent",
                     'Intended Audience :: Science/Research',
                     'Topic :: Scientific/Engineering :: Astronomy',
                     ],
```

### Comparing `CASCADe-spectroscopy-1.2.2/tests/cpm_model_tests.py` & `CASCADe-spectroscopy-1.2.3/tests/cpm_model_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/tests/data_model_tests.py` & `CASCADe-spectroscopy-1.2.3/tests/data_model_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/tests/exoplanet_tools_tests.py` & `CASCADe-spectroscopy-1.2.3/tests/exoplanet_tools_tests.py`

 * *Files identical despite different names*

### Comparing `CASCADe-spectroscopy-1.2.2/tests/initialize_tests.py` & `CASCADe-spectroscopy-1.2.3/tests/initialize_tests.py`

 * *Files identical despite different names*

