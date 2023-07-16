# Comparing `tmp/pyDecision-2.9.8.tar.gz` & `tmp/pyDecision-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyDecision-2.9.8.tar", last modified: Sat Jul 15 01:33:29 2023, max compression
+gzip compressed data, was "dist\pyDecision-3.0.2.tar", last modified: Sun Jul 16 16:30:04 2023, max compression
```

## Comparing `pyDecision-2.9.8.tar` & `pyDecision-3.0.2.tar`

### file list

```diff
@@ -1,65 +1,69 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/
--rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-2.9.8/LICENSE
--rw-rw-rw-   0        0        0    12577 2023-07-15 01:33:29.000000 pyDecision-2.9.8/PKG-INFO
--rw-rw-rw-   0        0        0    12184 2023-07-15 01:32:45.000000 pyDecision-2.9.8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision/
--rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-2.9.8/pyDecision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision/algorithm/
--rw-rw-rw-   0        0        0     1835 2023-07-14 22:26:21.000000 pyDecision-2.9.8/pyDecision/algorithm/__init__.py
--rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-2.9.8/pyDecision/algorithm/ahp.py
--rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-2.9.8/pyDecision/algorithm/aras.py
--rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-2.9.8/pyDecision/algorithm/borda.py
--rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-2.9.8/pyDecision/algorithm/bwm.py
--rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-2.9.8/pyDecision/algorithm/cocoso.py
--rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-2.9.8/pyDecision/algorithm/codas.py
--rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-2.9.8/pyDecision/algorithm/copras.py
--rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-2.9.8/pyDecision/algorithm/critic.py
--rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-2.9.8/pyDecision/algorithm/dematel.py
--rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-2.9.8/pyDecision/algorithm/e_i.py
--rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-2.9.8/pyDecision/algorithm/e_i_s.py
--rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-2.9.8/pyDecision/algorithm/e_i_v.py
--rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-2.9.8/pyDecision/algorithm/e_ii.py
--rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-2.9.8/pyDecision/algorithm/e_iii.py
--rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-2.9.8/pyDecision/algorithm/e_iv.py
--rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-2.9.8/pyDecision/algorithm/e_tri_b.py
--rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-2.9.8/pyDecision/algorithm/edas.py
--rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_ahp.py
--rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_dematel.py
--rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_edas.py
--rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_topsis.py
--rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-2.9.8/pyDecision/algorithm/fuzzy_vikor.py
--rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-2.9.8/pyDecision/algorithm/gra.py
--rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-2.9.8/pyDecision/algorithm/idocriw.py
--rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-2.9.8/pyDecision/algorithm/mabac.py
--rw-rw-rw-   0        0        0     2998 2023-07-15 01:09:36.000000 pyDecision-2.9.8/pyDecision/algorithm/marcos.py
--rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-2.9.8/pyDecision/algorithm/maut.py
--rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-2.9.8/pyDecision/algorithm/moora.py
--rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-2.9.8/pyDecision/algorithm/moosra.py
--rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-2.9.8/pyDecision/algorithm/multimoora.py
--rw-rw-rw-   0        0        0     2427 2023-07-15 00:38:42.000000 pyDecision-2.9.8/pyDecision/algorithm/ocra.py
--rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-2.9.8/pyDecision/algorithm/p_i.py
--rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-2.9.8/pyDecision/algorithm/p_ii.py
--rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-2.9.8/pyDecision/algorithm/p_iii.py
--rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-2.9.8/pyDecision/algorithm/p_iv.py
--rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-2.9.8/pyDecision/algorithm/p_v.py
--rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-2.9.8/pyDecision/algorithm/p_vi.py
--rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-2.9.8/pyDecision/algorithm/p_xgaia.py
--rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-2.9.8/pyDecision/algorithm/saw.py
--rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-2.9.8/pyDecision/algorithm/smart.py
--rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-2.9.8/pyDecision/algorithm/todim.py
--rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-2.9.8/pyDecision/algorithm/topsis.py
--rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-2.9.8/pyDecision/algorithm/vikor.py
--rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-2.9.8/pyDecision/algorithm/waspas.py
--rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-2.9.8/pyDecision/algorithm/wings.py
-drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision/util/
--rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-2.9.8/pyDecision/util/__init__.py
--rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-2.9.8/pyDecision/util/ga.py
--rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-2.9.8/pyDecision/util/gwo.py
-drwxrwxrwx   0        0        0        0 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision.egg-info/
--rw-rw-rw-   0        0        0    12577 2023-07-15 01:33:28.000000 pyDecision-2.9.8/pyDecision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1701 2023-07-15 01:33:29.000000 pyDecision-2.9.8/pyDecision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 01:33:28.000000 pyDecision-2.9.8/pyDecision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-07-15 01:33:28.000000 pyDecision-2.9.8/pyDecision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-15 01:33:28.000000 pyDecision-2.9.8/pyDecision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 01:33:29.000000 pyDecision-2.9.8/setup.cfg
--rw-rw-rw-   0        0        0      632 2023-07-15 01:32:55.000000 pyDecision-2.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:30:04.000000 pyDecision-3.0.2/
+-rw-rw-rw-   0        0        0      659 2022-03-01 20:02:45.000000 pyDecision-3.0.2/LICENSE
+-rw-rw-rw-   0        0        0    13520 2023-07-16 16:30:04.000000 pyDecision-3.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    13123 2023-07-16 16:23:47.000000 pyDecision-3.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 16:30:03.000000 pyDecision-3.0.2/pyDecision/
+-rw-rw-rw-   0        0        0        1 2022-03-01 07:37:35.000000 pyDecision-3.0.2/pyDecision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:30:04.000000 pyDecision-3.0.2/pyDecision/algorithm/
+-rw-rw-rw-   0        0        0     1994 2023-07-16 16:15:27.000000 pyDecision-3.0.2/pyDecision/algorithm/__init__.py
+-rw-rw-rw-   0        0        0     1079 2022-09-01 20:46:27.000000 pyDecision-3.0.2/pyDecision/algorithm/ahp.py
+-rw-rw-rw-   0        0        0     2536 2021-05-21 16:09:22.000000 pyDecision-3.0.2/pyDecision/algorithm/aras.py
+-rw-rw-rw-   0        0        0     2096 2021-02-04 18:51:35.000000 pyDecision-3.0.2/pyDecision/algorithm/borda.py
+-rw-rw-rw-   0        0        0     1513 2022-03-02 01:40:04.000000 pyDecision-3.0.2/pyDecision/algorithm/bwm.py
+-rw-rw-rw-   0        0        0      801 2023-07-15 20:46:57.000000 pyDecision-3.0.2/pyDecision/algorithm/cilos.py
+-rw-rw-rw-   0        0        0     2606 2023-07-14 19:52:45.000000 pyDecision-3.0.2/pyDecision/algorithm/cocoso.py
+-rw-rw-rw-   0        0        0     2701 2021-05-02 21:48:52.000000 pyDecision-3.0.2/pyDecision/algorithm/codas.py
+-rw-rw-rw-   0        0        0     2420 2021-04-28 14:43:23.000000 pyDecision-3.0.2/pyDecision/algorithm/copras.py
+-rw-rw-rw-   0        0        0     1121 2021-04-26 20:45:47.000000 pyDecision-3.0.2/pyDecision/algorithm/critic.py
+-rw-rw-rw-   0        0        0     3204 2021-02-02 00:46:00.000000 pyDecision-3.0.2/pyDecision/algorithm/dematel.py
+-rw-rw-rw-   0        0        0     9331 2020-01-14 19:04:25.000000 pyDecision-3.0.2/pyDecision/algorithm/e_i.py
+-rw-rw-rw-   0        0        0     9548 2020-01-13 23:26:00.000000 pyDecision-3.0.2/pyDecision/algorithm/e_i_s.py
+-rw-rw-rw-   0        0        0     9225 2020-01-13 23:30:51.000000 pyDecision-3.0.2/pyDecision/algorithm/e_i_v.py
+-rw-rw-rw-   0        0        0    16905 2020-10-26 16:16:05.000000 pyDecision-3.0.2/pyDecision/algorithm/e_ii.py
+-rw-rw-rw-   0        0        0    13823 2020-01-13 22:04:18.000000 pyDecision-3.0.2/pyDecision/algorithm/e_iii.py
+-rw-rw-rw-   0        0        0    14298 2020-01-13 22:04:47.000000 pyDecision-3.0.2/pyDecision/algorithm/e_iv.py
+-rw-rw-rw-   0        0        0    14611 2020-08-10 21:53:58.000000 pyDecision-3.0.2/pyDecision/algorithm/e_tri_b.py
+-rw-rw-rw-   0        0        0     2560 2021-02-02 12:06:30.000000 pyDecision-3.0.2/pyDecision/algorithm/edas.py
+-rw-rw-rw-   0        0        0     1655 2022-09-01 20:46:10.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_ahp.py
+-rw-rw-rw-   0        0        0     3930 2021-02-02 01:12:46.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_dematel.py
+-rw-rw-rw-   0        0        0     4891 2021-02-03 19:17:50.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_edas.py
+-rw-rw-rw-   0        0        0     3935 2021-01-29 16:03:04.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_topsis.py
+-rw-rw-rw-   0        0        0     5943 2021-02-04 16:55:29.000000 pyDecision-3.0.2/pyDecision/algorithm/fuzzy_vikor.py
+-rw-rw-rw-   0        0        0     2330 2021-02-01 19:52:07.000000 pyDecision-3.0.2/pyDecision/algorithm/gra.py
+-rw-rw-rw-   0        0        0     4097 2022-03-20 23:18:57.000000 pyDecision-3.0.2/pyDecision/algorithm/idocriw.py
+-rw-rw-rw-   0        0        0     2534 2022-03-20 23:58:37.000000 pyDecision-3.0.2/pyDecision/algorithm/mabac.py
+-rw-rw-rw-   0        0        0     2551 2023-07-16 13:00:46.000000 pyDecision-3.0.2/pyDecision/algorithm/mairca.py
+-rw-rw-rw-   0        0        0     2998 2023-07-15 01:09:36.000000 pyDecision-3.0.2/pyDecision/algorithm/marcos.py
+-rw-rw-rw-   0        0        0     3759 2023-01-25 00:17:51.000000 pyDecision-3.0.2/pyDecision/algorithm/maut.py
+-rw-rw-rw-   0        0        0      967 2023-07-15 20:29:25.000000 pyDecision-3.0.2/pyDecision/algorithm/merec.py
+-rw-rw-rw-   0        0        0     2490 2021-04-28 17:43:08.000000 pyDecision-3.0.2/pyDecision/algorithm/moora.py
+-rw-rw-rw-   0        0        0     2497 2021-05-20 21:42:55.000000 pyDecision-3.0.2/pyDecision/algorithm/moosra.py
+-rw-rw-rw-   0        0        0     4848 2021-05-21 14:22:41.000000 pyDecision-3.0.2/pyDecision/algorithm/multimoora.py
+-rw-rw-rw-   0        0        0     2427 2023-07-15 00:38:42.000000 pyDecision-3.0.2/pyDecision/algorithm/ocra.py
+-rw-rw-rw-   0        0        0     8518 2020-01-13 22:39:45.000000 pyDecision-3.0.2/pyDecision/algorithm/p_i.py
+-rw-rw-rw-   0        0        0     5836 2020-01-13 23:06:54.000000 pyDecision-3.0.2/pyDecision/algorithm/p_ii.py
+-rw-rw-rw-   0        0        0     8323 2021-01-28 15:26:38.000000 pyDecision-3.0.2/pyDecision/algorithm/p_iii.py
+-rw-rw-rw-   0        0        0     8492 2020-01-13 23:06:54.000000 pyDecision-3.0.2/pyDecision/algorithm/p_iv.py
+-rw-rw-rw-   0        0        0     6437 2022-03-02 01:40:27.000000 pyDecision-3.0.2/pyDecision/algorithm/p_v.py
+-rw-rw-rw-   0        0        0     9325 2020-01-13 23:06:55.000000 pyDecision-3.0.2/pyDecision/algorithm/p_vi.py
+-rw-rw-rw-   0        0        0     7337 2021-01-27 21:21:21.000000 pyDecision-3.0.2/pyDecision/algorithm/p_xgaia.py
+-rw-rw-rw-   0        0        0     2115 2023-07-16 16:14:56.000000 pyDecision-3.0.2/pyDecision/algorithm/piv.py
+-rw-rw-rw-   0        0        0     2079 2021-05-21 01:03:21.000000 pyDecision-3.0.2/pyDecision/algorithm/saw.py
+-rw-rw-rw-   0        0        0     2293 2021-05-21 14:21:59.000000 pyDecision-3.0.2/pyDecision/algorithm/smart.py
+-rw-rw-rw-   0        0        0     2817 2023-07-14 22:25:29.000000 pyDecision-3.0.2/pyDecision/algorithm/todim.py
+-rw-rw-rw-   0        0        0     2549 2021-01-27 13:29:58.000000 pyDecision-3.0.2/pyDecision/algorithm/topsis.py
+-rw-rw-rw-   0        0        0     3619 2021-01-27 16:37:58.000000 pyDecision-3.0.2/pyDecision/algorithm/vikor.py
+-rw-rw-rw-   0        0        0      960 2021-02-02 11:56:42.000000 pyDecision-3.0.2/pyDecision/algorithm/waspas.py
+-rw-rw-rw-   0        0        0     2600 2021-05-20 20:10:59.000000 pyDecision-3.0.2/pyDecision/algorithm/wings.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:30:04.000000 pyDecision-3.0.2/pyDecision/util/
+-rw-rw-rw-   0        0        0       71 2022-03-02 00:42:59.000000 pyDecision-3.0.2/pyDecision/util/__init__.py
+-rw-rw-rw-   0        0        0     6279 2022-03-16 15:18:17.000000 pyDecision-3.0.2/pyDecision/util/ga.py
+-rw-rw-rw-   0        0        0     6126 2022-03-16 15:19:48.000000 pyDecision-3.0.2/pyDecision/util/gwo.py
+drwxrwxrwx   0        0        0        0 2023-07-16 16:30:03.000000 pyDecision-3.0.2/pyDecision.egg-info/
+-rw-rw-rw-   0        0        0    13520 2023-07-16 16:30:01.000000 pyDecision-3.0.2/pyDecision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1820 2023-07-16 16:30:02.000000 pyDecision-3.0.2/pyDecision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 16:30:01.000000 pyDecision-3.0.2/pyDecision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-07-16 16:30:01.000000 pyDecision-3.0.2/pyDecision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-16 16:30:01.000000 pyDecision-3.0.2/pyDecision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 16:30:04.000000 pyDecision-3.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      632 2023-07-16 16:25:42.000000 pyDecision-3.0.2/setup.py
```

### Comparing `pyDecision-2.9.8/LICENSE` & `pyDecision-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/PKG-INFO` & `pyDecision-3.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 2.9.8
+Version: 3.0.2
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making) ;**TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyDecision
 ```
@@ -63,14 +63,15 @@
 3. Try it in **Colab**:
 
 - AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
 - Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://arxiv.org/ftp/arxiv/papers/1311/1311.2886.pdf))
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
+- CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
@@ -81,28 +82,31 @@
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
+- MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
+- MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
```

### Comparing `pyDecision-2.9.8/README.md` & `pyDecision-3.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making) ;**TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyDecision
 ```
@@ -52,14 +52,15 @@
 3. Try it in **Colab**:
 
 - AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
 - Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://arxiv.org/ftp/arxiv/papers/1311/1311.2886.pdf))
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
+- CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
@@ -70,28 +71,31 @@
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
+- MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
+- MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
```

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/__init__.py` & `pyDecision-3.0.2/pyDecision/algorithm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from .ahp           import ahp_method
 from .aras          import aras_method
 from .borda         import borda_method
 from .bwm           import bw_method
+from .cilos         import cilos_method
 from .cocoso        import cocoso_method
 from .codas         import codas_method
 from .copras        import copras_method
 from .critic        import critic_method
 from .dematel       import dematel_method
 from .e_i           import electre_i
 from .e_i_s         import electre_i_s
@@ -19,27 +20,30 @@
 from .fuzzy_dematel import fuzzy_dematel_method
 from .fuzzy_edas    import fuzzy_edas_method
 from .fuzzy_topsis  import fuzzy_topsis_method
 from .fuzzy_vikor   import fuzzy_vikor_method
 from .gra           import gra_method
 from .idocriw       import idocriw_method
 from .mabac         import mabac_method
+from .mairca        import mairca_method
 from .marcos        import marcos_method
 from .maut          import maut_method
+from .merec         import merec_method
 from .moora         import moora_method
 from .moosra        import moosra_method
 from .multimoora    import multimoora_method  
 from .ocra          import ocra_method
 from .p_i           import promethee_i
 from .p_ii          import promethee_ii
 from .p_iii         import promethee_iii
 from .p_iv          import promethee_iv
 from .p_v           import promethee_v
 from .p_vi          import promethee_vi
 from .p_xgaia       import promethee_gaia
+from .piv           import piv_method
 from .saw           import saw_method
 from .smart         import smart_method
 from .todim         import todim_method
 from .topsis        import topsis_method
 from .vikor         import vikor_method, ranking
 from .waspas        import waspas_method
 from .wings         import wings_method
```

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/ahp.py` & `pyDecision-3.0.2/pyDecision/algorithm/ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/aras.py` & `pyDecision-3.0.2/pyDecision/algorithm/aras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/borda.py` & `pyDecision-3.0.2/pyDecision/algorithm/borda.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/bwm.py` & `pyDecision-3.0.2/pyDecision/algorithm/bwm.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/cocoso.py` & `pyDecision-3.0.2/pyDecision/algorithm/cocoso.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/codas.py` & `pyDecision-3.0.2/pyDecision/algorithm/codas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/copras.py` & `pyDecision-3.0.2/pyDecision/algorithm/copras.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/critic.py` & `pyDecision-3.0.2/pyDecision/algorithm/critic.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/dematel.py` & `pyDecision-3.0.2/pyDecision/algorithm/dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/e_i.py` & `pyDecision-3.0.2/pyDecision/algorithm/e_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/e_i_s.py` & `pyDecision-3.0.2/pyDecision/algorithm/e_i_s.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/e_i_v.py` & `pyDecision-3.0.2/pyDecision/algorithm/e_i_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/e_ii.py` & `pyDecision-3.0.2/pyDecision/algorithm/e_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/e_iii.py` & `pyDecision-3.0.2/pyDecision/algorithm/e_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/e_iv.py` & `pyDecision-3.0.2/pyDecision/algorithm/e_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/e_tri_b.py` & `pyDecision-3.0.2/pyDecision/algorithm/e_tri_b.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/edas.py` & `pyDecision-3.0.2/pyDecision/algorithm/edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_ahp.py` & `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_ahp.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_dematel.py` & `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_dematel.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_edas.py` & `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_edas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_topsis.py` & `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/fuzzy_vikor.py` & `pyDecision-3.0.2/pyDecision/algorithm/fuzzy_vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/gra.py` & `pyDecision-3.0.2/pyDecision/algorithm/gra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/idocriw.py` & `pyDecision-3.0.2/pyDecision/algorithm/idocriw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/mabac.py` & `pyDecision-3.0.2/pyDecision/algorithm/mabac.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/marcos.py` & `pyDecision-3.0.2/pyDecision/algorithm/marcos.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/maut.py` & `pyDecision-3.0.2/pyDecision/algorithm/maut.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/moora.py` & `pyDecision-3.0.2/pyDecision/algorithm/moora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/moosra.py` & `pyDecision-3.0.2/pyDecision/algorithm/moosra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/multimoora.py` & `pyDecision-3.0.2/pyDecision/algorithm/multimoora.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/ocra.py` & `pyDecision-3.0.2/pyDecision/algorithm/ocra.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/p_i.py` & `pyDecision-3.0.2/pyDecision/algorithm/p_i.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/p_ii.py` & `pyDecision-3.0.2/pyDecision/algorithm/p_ii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/p_iii.py` & `pyDecision-3.0.2/pyDecision/algorithm/p_iii.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/p_iv.py` & `pyDecision-3.0.2/pyDecision/algorithm/p_iv.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/p_v.py` & `pyDecision-3.0.2/pyDecision/algorithm/p_v.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/p_vi.py` & `pyDecision-3.0.2/pyDecision/algorithm/p_vi.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/p_xgaia.py` & `pyDecision-3.0.2/pyDecision/algorithm/p_xgaia.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/saw.py` & `pyDecision-3.0.2/pyDecision/algorithm/saw.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/smart.py` & `pyDecision-3.0.2/pyDecision/algorithm/smart.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/todim.py` & `pyDecision-3.0.2/pyDecision/algorithm/todim.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/topsis.py` & `pyDecision-3.0.2/pyDecision/algorithm/topsis.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/vikor.py` & `pyDecision-3.0.2/pyDecision/algorithm/vikor.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/waspas.py` & `pyDecision-3.0.2/pyDecision/algorithm/waspas.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/algorithm/wings.py` & `pyDecision-3.0.2/pyDecision/algorithm/wings.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/util/ga.py` & `pyDecision-3.0.2/pyDecision/util/ga.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision/util/gwo.py` & `pyDecision-3.0.2/pyDecision/util/gwo.py`

 * *Files identical despite different names*

### Comparing `pyDecision-2.9.8/pyDecision.egg-info/PKG-INFO` & `pyDecision-3.0.2/pyDecision.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyDecision
-Version: 2.9.8
+Version: 3.0.2
 Summary: A MCDA Library
 Home-page: https://github.com/Valdecy/pyDecisions
 Author: Valdecy Pereira
 Author-email: valdecy.pereira@gmail.com
 License: GNU
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyDecision
 
 ## Introduction
 
-A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making) ;**TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
+A python library with the following MCDA methods: **AHP** (Analytic Hierarchy Process); **Fuzzy AHP**; **ARAS** (Additive Ratio ASsessment); **Borda**; **BWM** (Best-Worst Method); **CODAS** (Combinative Distance-based Assessment); **CILOS** (Criterion Impact LOSs); **CoCoSo** (COmbined COmpromise SOlution); **COPRAS** (Complex PRoportional Assessment); **CRITIC** (CRiteria Importance Through Intercriteria Correlation); **DEMATEL** (DEcision MAking Trial and Evaluation Laboratory); **Fuzzy DEMATEL**; **EDAS** (Evaluation based on Distance from Average Solution); **Fuzzy EDAS**; **ELECTRE** (I, I_s, I_v, II, III, IV, Tri-B); **GRA** (Grey Relational Analysis); **IDOCRIW** (Integrated Determination of Objective CRIteria Weights); **MABAC** (Multi-Attributive Border Approximation area Comparison); **MAIRCA** (Multi-Attributive Ideal-Real Comparative Analysis); **MARCOS** (Measurement of Alternatives and Ranking according to COmpromise Solution); **MAUT** (Multi-attribute Utility Theory); **MEREC** (MEthod based on the Removal Effects of Criteria); **MOORA** (Multi-Objective Optimization on the basis of Ratio Analysis); **MOOSRA** (Multi-Objective Optimisation on the Basis of Simple Ratio Analysis);  **MULTIMOORA** (Multi-Objective Optimization on the basis of Ratio Analisys Multiplicative Form); **OCRA** (Operational Competitiveness RAting); **PROMETHEE** (I, II, III, IV, V, VI, Gaia); **SAW** (Simple Additive Weighting); **SMART** (Simple Multi-Attribute Rating Technique); **TODIM** (TOmada de Decisao Interativa e Multicriterio - Interactive and Multicriteria Decision Making); **PIV** (Proximity Indexed Value); **TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution); **Fuzzy TOPSIS**; **VIKOR** (VIseKriterijumska Optimizacija I Kompromisno Resenje); **Fuzzy VIKOR**; **WINGS** (Weighted Influence Non-linear Gauge System); **WSM** (Weighted Sum Model); **WPM** (Weighted Product Model); **WASPAS** (Weighted Aggregates Sum Product Assessment).
 
 ## Usage
 
 1. Install
 ```bash
 pip install pyDecision
 ```
@@ -63,14 +63,15 @@
 3. Try it in **Colab**:
 
 - AHP ([ Colab Demo ](https://colab.research.google.com/drive/1qwFQs5xkTZ8K-Ul_wWcCtPjLH0QooU9g?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/0377-2217(90)90057-I))
 - Fuzzy AHP ([ Colab Demo ](https://colab.research.google.com/drive/1RtEMOLGL5wtmheMRZv8emcO5wbjYVBCo?usp=sharing)) ( [ Paper ](https://arxiv.org/ftp/arxiv/papers/1311/1311.2886.pdf))
 - ARAS ([ Colab Demo ](https://colab.research.google.com/drive/1rwQgXjvC3E6pRhOs7CkcCV8Vw2bXEPLy?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/pdf/10.3846/tede.2010.10#:~:text=According%20to%20the%20ARAS%20method,criteria%20considered%20in%20a%20project.))
 - Borda ([ Colab Demo ](https://colab.research.google.com/drive/1t5RVtG7_yXK-nPxM0MVd4U01qfTQYW4k?usp=sharing)) ( [ Paper ](http://gerardgreco.free.fr/IMG/pdf/MA_c_moire-Borda-1781.pdf))
 - BWM ([ Colab Demo ](https://colab.research.google.com/drive/1XkacTmtSBvZmx_5K9cfz8t1Ao5j-D-bZ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.omega.2014.11.009))
+- CILOS ([ Colab Demo ](https://colab.research.google.com/drive/1RnSqO_VEPyvXAMHdneloYvA0TzPx55kw?usp=sharing)) ( [ Paper ](https://www.worldscientific.com/doi/10.1142/S0219622016500036))
 - CoCoSo ([ Colab Demo ](https://colab.research.google.com/drive/1U8a3NZzQaxDkJdUT3uKIeeoqFtT_3Mnx?usp=sharing)) ( [ Paper ](https://www.emerald.com/insight/content/doi/10.1108/MD-05-2017-0458/full/html))
 - CODAS ([ Colab Demo ](https://colab.research.google.com/drive/1hm7__urqFeBHM6nVQJcBzGPF72DFuoLr?usp=sharing)) ( [ Paper ](https://EconPapers.repec.org/RePEc:cys:ecocyb:v:50:y:2016:i:3:p:25-44))
 - COPRAS ([ Colab Demo ](https://colab.research.google.com/drive/1TZJtSjXqwYEwuL7-wfLcPQ8ZBtDq3lth?usp=sharing)) ( [ Paper ](https://doi.org/10.3846/20294913.2012.762953))
 - CRITIC ([ Colab Demo ](https://colab.research.google.com/drive/1D5SaBHa1-Eo_KYSXHkFjsHYu29M21l_F?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/0305-0548(94)00059-H))
 - DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/1T04qEft9uwTyQx--gADN6V_vUrT21Xo6?usp=sharing)) ( [ Paper ](https://doi.org/10.1155/2018/3696457))
 - Fuzzy DEMATEL ([ Colab Demo ](https://colab.research.google.com/drive/15e9dMDROr3cxjbWRXg3_t4TScuQtQDpR?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1016/j.eswa.2005.12.005))
 - EDAS ([ Colab Demo ](https://colab.research.google.com/drive/1xsMdwH-IH-zvOW-1kv6ztQnKGt7p5JnY?usp=sharing)) ( [ Paper ](https://doi.org/10.15388/Informatica.2015.57))
@@ -81,28 +82,31 @@
 - ELECTRE II    ([ Colab Demo ](https://colab.research.google.com/drive/1UeAjICH6_tjVr3O9H-fC65HHYMVZgTKc?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE III   ([ Colab Demo ](https://colab.research.google.com/drive/1smeD5ZoPgBnAAUyooAXSrkxHgqZPmUC9?usp=sharing)) ( [ Paper ](https://github.com/Valdecy/Datasets/raw/master/MCDA/E03.pdf))
 - ELECTRE IV    ([ Colab Demo ](https://colab.research.google.com/drive/178x062yC-Es6lstEiFaFprbMsTJZwnC-?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-1-4757-5057-7_3))
 - ELECTRE Tri-B ([ Colab Demo ](https://colab.research.google.com/drive/1hu0fJcxdBAiEDrVngmKQfpINpjTF-osE?usp=sharing)) ( [ Paper ](https://drive.google.com/file/d/1oWOI_sX3EEYdRbavoBTT7vUmPII1yPgE/view?usp=sharing))
 - GRA ([ Colab Demo ](https://colab.research.google.com/drive/1aMMI0Cuo5kpzTDefqEwJhf0wWpBOP_JL?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/S0167-6911(82)80025-X))
 - IDOCRIW ([ Colab Demo ](https://colab.research.google.com/drive/1zt8uPFZGcHaSnpiT7tDnrDjvs0pK_7vS?usp=sharing)) ( [ Paper ](https://link.springer.com/chapter/10.1007/978-3-030-15009-9_19))
 - MABAC ([ Colab Demo ](https://colab.research.google.com/drive/1BMqO-HnBXdcOZfZoULpx1H4MLPoUGucJ?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2014.11.057))
+- MAIRCA ([ Colab Demo ](https://colab.research.google.com/drive/1gfqgrBAFGVygwm1j3lTjfy5wTsLgT_j5?usp=sharing)) ( [ Paper ](https://www.tandfonline.com/doi/full/10.1080/1331677X.2018.1506706))
 - MARCOS ([ Colab Demo ](https://colab.research.google.com/drive/13MI2Qrakm5VzHN3r5O2RqggCzQwRxCs-?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835219307004))
 - MAUT ([ Colab Demo ](https://colab.research.google.com/drive/1qm3ARgQm68GUK2irGiCB-B49vnVHazB7?usp=sharing)) ( [ Paper ](https://apps.dtic.mil/sti/pdfs/AD0770576.pdf))
+- MEREC ([ Colab Demo ](https://colab.research.google.com/drive/1XE3AIzS84w-gw_1MEtV7xvkU1Gj_tRPd?usp=sharing)) ( [ Paper ](https://www.mdpi.com/2073-8994/13/4/525))
 - MOORA ([ Colab Demo ](https://colab.research.google.com/drive/1FpKl0QAdwGgCVvLYsRHvMWhz7yOp17B5?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/228345226_The_MOORA_method_and_its_application_to_privatization_in_a_transition_economy))
 - MOOSRA ([ Colab Demo ](https://colab.research.google.com/drive/1KYyA4f3OsipPA5e63Ja4A0OGmHvNY6dj?usp=sharing)) ( [ Paper ](https://ijret.org/volumes/2014v03/i15/IJRET20140315105.pdf))
 - MULTIMOORA ([ Colab Demo ](https://colab.research.google.com/drive/1JAT8qqHPNoFfMV6a-CzF6BgRwtcUF3-e?usp=sharing)) ( [ Paper ](https://journals.vilniustech.lt/index.php/TEDE/article/view/5832/5078))
 - OCRA ([ Colab Demo ](https://colab.research.google.com/drive/1yQ41lOdjhiANtD1SOXoxA7gVim7A4X4P?usp=sharing)) ( [ Paper ](https://www.researchgate.net/publication/272362515_Selection_of_non-conventional_machining_processes_using_the_OCRA_method))
 - PROMETHEE I    ([ Colab Demo ](https://colab.research.google.com/drive/1WsagC7-Y_5X-Xl90pMz8YwUkKfxf2vol?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE II   ([ Colab Demo ](https://colab.research.google.com/drive/143TUtTBy9y6gW0kMVAfhANBhuw1bKvBB?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE III  ([ Colab Demo ](https://colab.research.google.com/drive/11DBaEBBT8B-B3poXubvZ41HELOHok0Rz?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-030-15009-9_5
 ))
 - PROMETHEE IV   ([ Colab Demo ](https://colab.research.google.com/drive/1X2evE6pIf4F7qiKjt1fSU2PqT-NaA5sJ?usp=sharing)) ( [ Paper ](http://dx.doi.org/10.1007/978-3-319-11949-6_14))
 - PROMETHEE V    ([ Colab Demo ](https://colab.research.google.com/drive/1IaZCCtq5m8vBBxrBLMCp6xB5U2j8ZNRc?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE VI   ([ Colab Demo ](https://colab.research.google.com/drive/14QdhifGitj4GK-QijRr1vj_dmGU2Pfh4?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
 - PROMETHEE Gaia ([ Colab Demo ](https://colab.research.google.com/drive/1lj7IRKXcuRjrpoBp_KmQn_3sI3P_Qxju?usp=sharing)) ( [ Paper ](https://www.cin.ufpe.br/~if703/aulas/promethee.pdf))
+- PIV ([ Colab Demo ](https://colab.research.google.com/drive/1PwJoBqYn1O2s22MqC9euP89Uyv4sedS0?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0360835218301360))
 - SAW ([ Colab Demo ](https://colab.research.google.com/drive/1R4cIsu0jBP9-6zwww_bNxEEnVGrhnS2d?usp=sharing)) ( [ Paper ](https://media.neliti.com/media/publications/326766-simple-additive-weighting-saw-method-in-f8f093e8.pdf))
 - SMART ([ Colab Demo ](https://colab.research.google.com/drive/1K93HXHBR_v2da95Hh_CB6AmTCqta-k3D?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-1-4612-3982-6_4))
 - TODIM ([ Colab Demo ](https://colab.research.google.com/drive/1EQqhhBQHHb8HT0TfuuVeFA2kwezsQYT1?usp=sharing)) ( [ Paper ](https://www.sciencedirect.com/science/article/abs/pii/S0377221707010740))
 - TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1s87DC5_oa9GvgVe98oAP1UIhduac09CB?usp=sharing)) ( [ Paper ](https://doi.org/10.1057/jors.1987.44))
 - Fuzzy TOPSIS ([ Colab Demo ](https://colab.research.google.com/drive/1eKx7AOYrnG-kZcsBt28rMEtCrUO-j3J-?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.procs.2016.07.088))
 - VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1egZiTNvI2eE-tyJ2m85MM6B3-qhiSjPG?usp=sharing)) ( [ Paper ](https://doi.org/10.1007/978-981-33-4745-8_8))
 - Fuzzy VIKOR ([ Colab Demo ](https://colab.research.google.com/drive/1anfCnU2TSrW-Z5vMkS_qXFrYZ0ciQE53?usp=sharing)) ( [ Paper ](https://doi.org/10.1016/j.eswa.2011.04.097))
```

### Comparing `pyDecision-2.9.8/pyDecision.egg-info/SOURCES.txt` & `pyDecision-3.0.2/pyDecision.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 pyDecision.egg-info/requires.txt
 pyDecision.egg-info/top_level.txt
 pyDecision/algorithm/__init__.py
 pyDecision/algorithm/ahp.py
 pyDecision/algorithm/aras.py
 pyDecision/algorithm/borda.py
 pyDecision/algorithm/bwm.py
+pyDecision/algorithm/cilos.py
 pyDecision/algorithm/cocoso.py
 pyDecision/algorithm/codas.py
 pyDecision/algorithm/copras.py
 pyDecision/algorithm/critic.py
 pyDecision/algorithm/dematel.py
 pyDecision/algorithm/e_i.py
 pyDecision/algorithm/e_i_s.py
@@ -29,27 +30,30 @@
 pyDecision/algorithm/fuzzy_dematel.py
 pyDecision/algorithm/fuzzy_edas.py
 pyDecision/algorithm/fuzzy_topsis.py
 pyDecision/algorithm/fuzzy_vikor.py
 pyDecision/algorithm/gra.py
 pyDecision/algorithm/idocriw.py
 pyDecision/algorithm/mabac.py
+pyDecision/algorithm/mairca.py
 pyDecision/algorithm/marcos.py
 pyDecision/algorithm/maut.py
+pyDecision/algorithm/merec.py
 pyDecision/algorithm/moora.py
 pyDecision/algorithm/moosra.py
 pyDecision/algorithm/multimoora.py
 pyDecision/algorithm/ocra.py
 pyDecision/algorithm/p_i.py
 pyDecision/algorithm/p_ii.py
 pyDecision/algorithm/p_iii.py
 pyDecision/algorithm/p_iv.py
 pyDecision/algorithm/p_v.py
 pyDecision/algorithm/p_vi.py
 pyDecision/algorithm/p_xgaia.py
+pyDecision/algorithm/piv.py
 pyDecision/algorithm/saw.py
 pyDecision/algorithm/smart.py
 pyDecision/algorithm/todim.py
 pyDecision/algorithm/topsis.py
 pyDecision/algorithm/vikor.py
 pyDecision/algorithm/waspas.py
 pyDecision/algorithm/wings.py
```

### Comparing `pyDecision-2.9.8/setup.py` & `pyDecision-3.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / 'README.md').read_text()
 
 setup(
     name='pyDecision',
-    version='2.9.8',
+    version='3.0.2',
     license='GNU',
     author='Valdecy Pereira',
     author_email='valdecy.pereira@gmail.com',
     url='https://github.com/Valdecy/pyDecisions',
     packages=find_packages(),
     install_requires=[
         'matplotlib',
```

