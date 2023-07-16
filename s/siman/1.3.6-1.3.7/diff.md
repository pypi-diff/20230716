# Comparing `tmp/siman-1.3.6.tar.gz` & `tmp/siman-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.3.6.tar", last modified: Fri Jul 14 10:44:46 2023, max compression
+gzip compressed data, was "dist/siman-1.3.7.tar", last modified: Sun Jul 16 18:08:18 2023, max compression
```

## Comparing `siman-1.3.6.tar` & `siman-1.3.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-14 10:44:46.419551 siman-1.3.6/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.6/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.6/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-14 10:44:46.419551 siman-1.3.6/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.6/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-14 10:44:46.420551 siman-1.3.6/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-14 10:44:42.000000 siman-1.3.6/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-14 10:44:46.417551 siman-1.3.6/siman/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.3.6/siman/3d_plot.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.3.6/siman/SSHTools.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.3.6/siman/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50661 2023-07-14 09:47:42.000000 siman-1.3.6/siman/analysis.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.3.6/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-14 10:44:46.418551 siman-1.3.6/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.6/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.6/siman/analyze/segregation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.3.6/siman/approximation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.3.6/siman/bands.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120936 2023-07-14 10:44:19.000000 siman-1.3.6/siman/calc_manage.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.3.6/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-14 10:44:46.418551 siman-1.3.6/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.6/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.6/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.6/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.6/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56581 2023-07-14 10:44:19.000000 siman-1.3.6/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.6/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-14 10:44:46.418551 siman-1.3.6/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.6/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.6/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.6/siman/chg/vasputil_chgarith_module.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11095 2023-07-14 10:44:19.000000 siman-1.3.6/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-14 10:44:46.419551 siman-1.3.6/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.6/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53424 2023-07-14 09:47:42.000000 siman-1.3.6/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.6/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.3.6/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.6/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.3.6/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119501 2023-07-14 09:47:42.000000 siman-1.3.6/siman/core/structure.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-07-14 10:44:19.000000 siman-1.3.6/siman/database.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.3.6/siman/default_project_conf.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.3.6/siman/dev_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.3.6/siman/dos_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.3.6/siman/fit_hex.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.3.6/siman/functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.3.6/siman/geo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    14653 2023-07-14 10:44:19.000000 siman-1.3.6/siman/header.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.3.6/siman/helper_for_writing_beatiful_code.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.3.6/siman/impurity.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    87526 2023-07-14 10:44:19.000000 siman-1.3.6/siman/inout.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.3.6/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-14 10:44:46.419551 siman-1.3.6/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.6/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.6/siman/mat_prop/mat_prop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.3.6/siman/matproj_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.3.6/siman/monte.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.3.6/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.3.6/siman/neb.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.3.6/siman/pairs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    49764 2023-07-14 10:44:19.000000 siman-1.3.6/siman/picture_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.3.6/siman/plot_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.3.6/siman/polaron.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.3.6/siman/polaron_hop.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.3.6/siman/polaron_mod.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194610 2023-07-14 10:44:19.000000 siman-1.3.6/siman/project_funcs.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.3.6/siman/properties_2d.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.3.6/siman/properties_energy.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.3.6/siman/properties_lattice.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.3.6/siman/set_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.3.6/siman/simanrc.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.3.6/siman/small_classes.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.3.6/siman/small_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.3.6/siman/structure_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.3.6/siman/table_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.3.6/siman/thermo.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.3.6/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-14 10:44:46.418551 siman-1.3.6/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-14 10:44:46.000000 siman-1.3.6/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-14 10:44:46.000000 siman-1.3.6/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-14 10:44:46.000000 siman-1.3.6/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-14 10:44:46.000000 siman-1.3.6/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-14 10:44:46.000000 siman-1.3.6/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.454508 siman-1.3.7/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.7/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.7/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-16 18:08:18.454508 siman-1.3.7/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.7/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-07-16 18:08:18.454508 siman-1.3.7/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-07-16 18:08:14.000000 siman-1.3.7/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.452508 siman-1.3.7/siman/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2023-07-14 10:44:19.000000 siman-1.3.7/siman/3d_plot.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2023-07-14 10:44:19.000000 siman-1.3.7/siman/SSHTools.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       32 2023-07-14 10:44:19.000000 siman-1.3.7/siman/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50708 2023-07-16 18:04:57.000000 siman-1.3.7/siman/analysis.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2023-07-14 10:44:19.000000 siman-1.3.7/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.452508 siman-1.3.7/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.7/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.7/siman/analyze/segregation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2023-07-14 10:44:19.000000 siman-1.3.7/siman/approximation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2023-07-14 10:44:19.000000 siman-1.3.7/siman/bands.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   120786 2023-07-16 18:04:57.000000 siman-1.3.7/siman/calc_manage.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2023-07-14 10:44:19.000000 siman-1.3.7/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.453508 siman-1.3.7/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56599 2023-07-16 18:04:57.000000 siman-1.3.7/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.7/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.453508 siman-1.3.7/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.7/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.7/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.7/siman/chg/vasputil_chgarith_module.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    11041 2023-07-16 18:04:57.000000 siman-1.3.7/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.454508 siman-1.3.7/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.7/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53318 2023-07-16 18:04:57.000000 siman-1.3.7/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.7/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33350 2023-07-14 09:47:42.000000 siman-1.3.7/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.7/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2122 2023-07-16 18:04:57.000000 siman-1.3.7/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   119405 2023-07-16 18:04:57.000000 siman-1.3.7/siman/core/structure.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    20203 2023-07-14 10:44:19.000000 siman-1.3.7/siman/database.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2023-07-14 10:44:19.000000 siman-1.3.7/siman/default_project_conf.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2023-07-14 10:44:19.000000 siman-1.3.7/siman/dev_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33287 2023-07-14 10:44:19.000000 siman-1.3.7/siman/dos_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2023-07-14 10:44:19.000000 siman-1.3.7/siman/fit_hex.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-07-14 10:44:19.000000 siman-1.3.7/siman/functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   113839 2023-07-14 10:44:19.000000 siman-1.3.7/siman/geo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    16289 2023-07-16 18:04:57.000000 siman-1.3.7/siman/header.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      286 2023-07-14 10:44:19.000000 siman-1.3.7/siman/helper_for_writing_beatiful_code.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    40269 2023-07-14 10:44:19.000000 siman-1.3.7/siman/impurity.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    87557 2023-07-16 18:04:57.000000 siman-1.3.7/siman/inout.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2023-07-14 10:44:19.000000 siman-1.3.7/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.454508 siman-1.3.7/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.7/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.7/siman/mat_prop/mat_prop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    46189 2023-07-14 10:44:19.000000 siman-1.3.7/siman/matproj_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2023-07-14 10:44:19.000000 siman-1.3.7/siman/monte.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      980 2023-07-14 10:44:19.000000 siman-1.3.7/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31637 2023-07-14 10:44:19.000000 siman-1.3.7/siman/neb.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2023-07-14 10:44:19.000000 siman-1.3.7/siman/pairs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    50657 2023-07-16 18:04:57.000000 siman-1.3.7/siman/picture_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2023-07-14 10:44:19.000000 siman-1.3.7/siman/plot_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-07-14 10:44:19.000000 siman-1.3.7/siman/polaron.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2023-07-14 10:44:19.000000 siman-1.3.7/siman/polaron_hop.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2023-07-14 10:44:19.000000 siman-1.3.7/siman/polaron_mod.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   194610 2023-07-14 10:44:19.000000 siman-1.3.7/siman/project_funcs.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2023-07-14 10:44:19.000000 siman-1.3.7/siman/properties_2d.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2023-07-14 10:44:19.000000 siman-1.3.7/siman/properties_energy.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2023-07-14 10:44:19.000000 siman-1.3.7/siman/properties_lattice.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    30687 2023-07-14 10:44:19.000000 siman-1.3.7/siman/set_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2023-07-14 10:44:19.000000 siman-1.3.7/siman/simanrc.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      174 2023-07-14 10:44:19.000000 siman-1.3.7/siman/small_classes.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6663 2023-07-14 10:44:19.000000 siman-1.3.7/siman/small_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2023-07-14 10:44:19.000000 siman-1.3.7/siman/structure_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2023-07-14 10:44:19.000000 siman-1.3.7/siman/table_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2023-07-14 10:44:19.000000 siman-1.3.7/siman/thermo.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2023-07-14 10:44:19.000000 siman-1.3.7/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-07-16 18:08:18.452508 siman-1.3.7/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-07-16 18:08:18.000000 siman-1.3.7/siman.egg-info/top_level.txt
```

### Comparing `siman-1.3.6/LICENSE` & `siman-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/PKG-INFO` & `siman-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.6
+Version: 1.3.7
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.6/setup.py` & `siman-1.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.3.6",
+    version="1.3.7",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.3.6/siman/3d_plot.py` & `siman-1.3.7/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/SSHTools.py` & `siman-1.3.7/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/analysis.py` & `siman-1.3.7/siman/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     from pymatgen.analysis.ewald import EwaldSummation
 
 except:
     print('analysis.py: pymatgen is not avail; run   pip install pymatgen')
 
 
 from siman import header
-from siman.header import printlog, print_and_log, mpl, db
+from siman.header import printlog, db
 from siman.functions import element_name_inv, invert, get_from_server
 from siman.picture_functions import plot_mep, fit_and_plot
 from siman.geo import determine_symmetry_positions, local_surrounding, find_moving_atom, image_distance, rms_pos_diff, interpolate
 from siman.database import push_figure_to_archive
 from siman.small_functions import is_list_like, makedir
 from siman.inout import write_xyz, read_xyz, write_occmatrix
 from siman.calcul import site_repulsive_e
@@ -149,15 +149,15 @@
             critical_point_type = 'undefined'
 
         # print(type(r_de_max), type(e), critical_point_type)
         print('Saddle point at {:.2f} {:.2f} is a local {:}'.format(r_de_max, float(e), critical_point_type)  )
 
 
     else:
-        print_and_log('Warning! no roots')
+        printlog('Warning! no roots')
         # diff_barrier = 0
         sign = 1
 
 
     mine = min(energies)
     maxe = max(energies)
     de = abs(mine - maxe)
@@ -365,14 +365,16 @@
     exclude - list of objects to skip
 
     formula - chemical formula used to calculate capacity in mAh/g
 
     fit_power - power of fit polynomial
     """
 
+    from siman.picture_functions import mpl
+
     if xs is None:
         xs = sorted(objs.keys())
 
     es2 = []
     xs2 = []
     x_prev = None
     V_prev = None
@@ -437,15 +439,15 @@
     es_inv.insert(0, 2.75)
 
 
     font = {'family' : 'Arial',
             # 'weight' : 'boolld',
             'size'   : 14}
 
-    header.mpl.rc('font', **font)
+    mpl.rc('font', **font)
 
     xi = [f(xi) for xi in x]
     print(xi )
 
     print('Full capacity is ', g(1)  )
 
     for i in range(len(x)):
@@ -660,14 +662,15 @@
            eos = EquationOfState(volumes, energies, eos='sjeos')
            v0, e0, B = eos.fit()
            eos.plot()
 
     """
     # e, v, emin, vmin       = plot_conv( conv[n], calc,  "fit_gb_volume2")
 
+    from siman.picture_functions import mpl
 
 
     alist = []
     vlist = []
     etotlist  = []
     magn1 = []
     magn2 = []
@@ -977,20 +980,20 @@
             cl_i.state = '2. Ready to read outcar'
             # if not os.path.exists(cl_i.path["output"]):
             #     load = 'o'
             outst2 = ("%s"%cl_i.name).ljust(name_field_length)
             if readfiles:
                 print(outst2+'|'+cl_i.read_results(loadflag, show = show, choose_outcar = choose_outcar) )
             else:
-                print_and_log(outst2+' | File was not read')
+                printlog(outst2+' | File was not read')
             
 
             if cl_i.id in calc: #move creation of calcs with images to add_neb
                 ''
-                # print_and_log('Please test code below this message to save prev calcs')
+                # printlog('Please test code below this message to save prev calcs')
                 # if cl_i != calc[cl_i.id]
                 #     if hasattr(calc[cl_i.id], 'prev') and calc[cl_i.id].prev:
                 #         prevlist = calc[cl_i.id].prev
                 #     else:
                 #         prevlist = [calc[cl_i.id]]
                 #     cl_i.prev = prevlist
                 #     calc[cl_i.id] = cl_i
```

### Comparing `siman-1.3.6/siman/analysis_functions.py` & `siman-1.3.7/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/analyze/segregation.py` & `siman-1.3.7/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/approximation.py` & `siman-1.3.7/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/bands.py` & `siman-1.3.7/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/calc_manage.py` & `siman-1.3.7/siman/calc_manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 if pymatgen_flag:
     from pymatgen.ext.matproj import MPRester
     from pymatgen.io.vasp.inputs import Poscar
 
 import siman
 from siman import header
-from siman.header import print_and_log, runBash, mpl, plt
+from siman.header import printlog, runBash
 from siman.small_functions import is_list_like, makedir, list2string, calc_ngkpt, setting_sshpass
 from siman.classes import Description
 from siman.core.structure import Structure
 from siman.calculators.vasp import CalculationVasp
 from siman.calculators.aims import CalculationAims
 from siman.calculators.gaussian import CalculationGaussian
 from siman.core.molecule import Molecule
@@ -44,16 +44,14 @@
 from siman.geo import interpolate, replic, image_distance, scale_cell_uniformly, scale_cell_by_matrix, remove_atoms, create_deintercalated_structure, create_antisite_defect, create_antisite_defect2, local_surrounding, find_moving_atom
 from siman.set_functions import init_default_sets
 from siman.database import push_figure_to_archive
 
 from siman.calculators.qe import CalculationQE
 
 
-printlog = print_and_log
-
 
 # Check the default parameters
 
 # Default savefile
 try:
     printlog('calc_manage.py, string 41, header.default_savefile ', header.default_savefile)
 except AttributeError:
@@ -126,19 +124,19 @@
         # hstring = ("%s    #on %s"% (traceback.extract_stack(None, 2)[0][3],   datetime.date.today() ) )
         hstring = 'add_des("{:s}", "{:s}", "{:s}")    #on {:})'.format(it, it_folder, des, datetime.date.today())
 
         try:
             if hstring != header.history[-1]: header.history.append( hstring  )
         except:
             header.history.append( hstring  )
-        print_and_log("New structure name "+it+ " added to struct_des dict"+"\n")
+        printlog("New structure name "+it+ " added to struct_des dict"+"\n")
 
 
     else:
-        print_and_log("Attention! "+it+' already exist in struct_des, skipping; use override = True if you really need it; or first remove using manually_remove_from_struct_des()')
+        printlog("Attention! "+it+' already exist in struct_des, skipping; use override = True if you really need it; or first remove using manually_remove_from_struct_des()')
         # raise RuntimeError
 
 
     return
 
 
 
@@ -543,15 +541,15 @@
 
 
 
 
 
         if ifolder: 
             if it not in ifolder: # just to be consistent with names
-                print_and_log('Check ifolder !!! it is not in ifolder')
+                printlog('Check ifolder !!! it is not in ifolder')
                 raise RuntimeError
 
 
         return
 
 
     def add_loop_inherit():
@@ -627,20 +625,20 @@
                 
                     if inherit_option in inh_opt_ngkpt:
                         inherit_ngkpt(it_new, it, varset[inputset]) # 
 
 
 
             if ise_new:
-                print_and_log('Inherited calculation uses set', ise_new)
+                printlog('Inherited calculation uses set', ise_new)
 
                 setlist = [ise_new,]
 
             else:
-                print_and_log('Inherited calculation uses the same sets', setlist)
+                printlog('Inherited calculation uses the same sets', setlist)
 
 
             it = it_new
         return
 
 
     def add_loop_modify():
@@ -863,23 +861,23 @@
 
             v = verlist[0]
             # printlog('add_loop_scale(): version is ', v)
             # sys.exit()
 
 
             # if up != 'up3':
-            print_and_log('add_loop_scale(): Preparing   scale  calculation ... ', imp = 'Y')
+            printlog('add_loop_scale(): Preparing   scale  calculation ... ', imp = 'Y')
 
             if len(verlist) > 1:
-                print_and_log('Error! Currently   scale  is allowed only for one version')
+                printlog('Error! Currently   scale  is allowed only for one version')
             
 
 
             if it_new not in struct_des:
-                if it_folder:
+                if it_folder is not None:
                     section_folder = it_folder
                 else:
                     section_folder = struct_des[it].sfolder
 
                 add_des(struct_des, it_new, section_folder, 'scale: scaled "images" for '+it+'.'+str(setlist)+'.'+str(v)   )
 
 
@@ -897,23 +895,28 @@
 
                 id_s = (it,inputset,v)
                 
                 if input_st:
                     it_l = it_new
                 else:
                     it_l = it 
+                
+                # print(header.SIMAN_WEB)
+
                 if header.SIMAN_WEB:
                     suf = '.'+id_s[1]
                     input_folder = struct_des[it_l].sfolder+'/'+it_l+suf
                     xyz_folder = struct_des[it_l].sfolder+'/'+it_new+suf
-                
+                    # print(xyz_folder)
+                    # sys.exit()
                 else:
                     suf = ''
                     input_folder = struct_des[it_l].sfolder+'/'+it_l+suf
                     xyz_folder = None
+                    # sys.exit()
 
 
                 if input_st:
                     st = input_st
                     pname = st.name
                     printlog('add_loop_scale():using input_st', pname)
                     input_st = None
@@ -1012,15 +1015,15 @@
 
                     # cl_temp.init = None
                     fitted_v100_id = cl_temp.id
 
 
                 verlist = verlist_new
 
-                print_and_log(len(sts), 'scale images have been created.', imp = 'y')
+                printlog(len(sts), 'scale images have been created.', imp = 'y')
             
 
 
 
 
             it      = it_new
             if ise_new:
@@ -1040,27 +1043,27 @@
         nonlocal input_geo_format, it
 
         mat_proj_st_id = None
         if mat_proj_id:
             input_geo_format = 'mat_proj'
 
         if input_geo_format == 'mat_proj':
-            print_and_log("Taking structure "+it+" from materialsproject.org ...", imp = 'Y')
+            printlog("Taking structure "+it+" from materialsproject.org ...", imp = 'Y')
             if it_folder == None:
-                print_and_log('Error! Please provide local folder for new ', it, 'structure using *it_folder* argument! ', imp = 'Y')
+                printlog('Error! Please provide local folder for new ', it, 'structure using *it_folder* argument! ', imp = 'Y')
             
             st = get_structure_from_matproj(it, it_folder, verlist[0], mat_proj_cell, mat_proj_id)
             mat_proj_st_id = st.mat_proj_st_id
             input_geo_file = st.input_geo_file
             input_geo_format = 'vasp'
 
         elif input_geo_format == 'cee_database':
             
             if it_folder == None:
-                print_and_log('Error! Please provide local folder for new ', it, 'structure using *it_folder* argument! ', imp = 'Y')
+                printlog('Error! Please provide local folder for new ', it, 'structure using *it_folder* argument! ', imp = 'Y')
 
             get_structure_from_cee_database(it, it_folder, verlist[0], **cee_args) #will transform it to vasp
             input_geo_format = 'vasp'
         return mat_proj_st_id
 
 
     def add_loop_neb():
@@ -1070,44 +1073,44 @@
         neb_flag = calc_method and not set(['neb', 'only_neb']).isdisjoint(calc_method)
         if neb_flag: #put nimage values for set_sequence
             curset = varset[ setlist[0] ]
             if not n_neb_images:
                 n_neb_images = varset[curset.vasp_params['IMAGES']]
 
             if not n_neb_images:
-                print_and_log('Error! You did not provide number of NEB images nor in *n_neb_images* nor in your set!')
+                printlog('Error! You did not provide number of NEB images nor in *n_neb_images* nor in your set!')
                 raise RuntimeError
 
 
             if header.corenum % n_neb_images > 0:
-                print_and_log('Error! add_loop_neb(): Number of cores should be dividable by number of IMAGES', header.corenum, n_neb_images)
+                printlog('Error! add_loop_neb(): Number of cores should be dividable by number of IMAGES', header.corenum, n_neb_images)
                 raise RuntimeError
 
             nebsets = [curset]
             
             if hasattr(curset, 'set_sequence') and curset.set_sequence:
                 for s in curset.set_sequence:
                     nebsets.append(s)
 
             for s in nebsets:
                 s.init_images_value = copy.deepcopy(s.vasp_params['IMAGES'])
                 s.vasp_params['IMAGES'] = n_neb_images
             #     print s.vasp_params['IMAGES']
             # sys.exit()
-            print_and_log('Attention, I update number of images in the set to', n_neb_images, 'for this calculation; ', imp = 'y')
+            printlog('Attention, I update number of images in the set to', n_neb_images, 'for this calculation; ', imp = 'y')
         return neb_flag, nebsets
 
 
     def add_loop_neb2(neb_flag, nebsets):
         if neb_flag:
 
             if len(setlist) > 1:
-                print_and_log('In "neb" mode only one set is allowed' )
+                printlog('In "neb" mode only one set is allowed' )
                 raise RuntimeError
-            print_and_log('Preparing   neb  calculation ... ')
+            printlog('Preparing   neb  calculation ... ')
 
             #create necessary calculations without
             nimages = varset[setlist[0]].vasp_params['IMAGES']
             # verlist+=[ 3+v for v in range(nimages)  ] #list of images starts from 3 (1 and 2 are final and start)
 
             # write_batch_list+=[False for v in range(nimages)] #not used now
 
@@ -1127,27 +1130,27 @@
                 if n < 10:
                     n_st = '0'+str(n)
                 elif n < 100:
                     n_st = str(n)
 
 
                 cl_i.path["output"] = cl_i.dir + n_st + "/OUTCAR"
-                print_and_log(i , cl_i.path["output"], 'overwritten in database')
+                printlog(i , cl_i.path["output"], 'overwritten in database')
 
                 cl_i.associated_outcars = list([a.replace('2.', '', 1) for a in cl.associated_outcars])
 
 
 
 
                 cl_i.state = '2. Ready to read outcar'
 
                 if cl_i.id in calc: # for 'continue' mode the add_calculation() takes care, but here it should be
                                     # repeated. Again think about using only add_calculation and  write_batch_list
                     ''
-                    # print_and_log('Please test code below this message to save prev calcs')
+                    # printlog('Please test code below this message to save prev calcs')
                     # if cl_i != calc[cl_i.id]
                     #     if hasattr(calc[cl_i.id], 'prev') and calc[cl_i.id].prev:
                     #         prevlist = calc[cl_i.id].prev
                     #     else:
                     #         prevlist = [calc[cl_i.id]]
                     #     cl_i.prev = prevlist
                     #     calc[cl_i.id] = cl_i
@@ -1282,15 +1285,15 @@
 
         if hstring != header.history[-1]: 
             header.history.append( hstring  )
 
 
 
         if up not in ('up1','up2','up3'): 
-            print_and_log("Warning! You are in the test mode, to add please change up to up1; "); 
+            printlog("Warning! You are in the test mode, to add please change up to up1; "); 
             sys.exit()
         
         if run: #
             complete_run() # for IPython notebook
             printlog(run_on_server('./run', header.CLUSTER_ADDRESS), imp= 'Y' )
             printlog('To read results use ', hstring, '; possible options for show: fit, fo, fop, en, mag, magp, smag, maga, occ, occ1, mep, mepp', imp = 'Y')
 
@@ -1589,29 +1592,29 @@
 
                 if up != 'up2':
                     return
 
 
     else:
         status = "new"
-        print_and_log( "There is no calculation with id "+ str(id)+". I create new with set "+str(inputset)+"\n" )        
+        printlog( "There is no calculation with id "+ str(id)+". I create new with set "+str(inputset)+"\n" )        
 
 
 
 
     if "up" in up:
 
         header.close_run = True
 
 
         if status in ["exist","compl"]: 
-            print_and_log("You asked to update existing calculation with id "+ str(id)+"; results are overwritten" )         
+            printlog("You asked to update existing calculation with id "+ str(id)+"; results are overwritten" )         
 
         if status == 'compl' and inherit_option == 'continue':
-            print_and_log(id, 'is completed, I will make its copy in self.prev[]', imp = 'Y' )         
+            printlog(id, 'is completed, I will make its copy in self.prev[]', imp = 'Y' )         
 
             cl_prev = copy.deepcopy(calc[id])
 
 
 
 
         if params.get('calculator'):
@@ -1681,19 +1684,19 @@
         if hasattr(cl.set, 'savefile'):
             for s in cl.set.savefile:
                 if s not in savefile:
                     savefile+=s
 
 
         if hasattr(cl.set, 'u_ramping_nstep') and cl.set.u_ramping_nstep:
-            print_and_log("Attention! U ramping method is detected from set\n\n")
+            printlog("Attention! U ramping method is detected from set\n\n")
             cl.calc_method.append('u_ramping')
 
         if hasattr(cl.set, 'afm_ordering'):
-            print_and_log("Attention! afm_ordering method is detected from set\n\n")
+            printlog("Attention! afm_ordering method is detected from set\n\n")
             cl.calc_method.append('afm_ordering')
 
 
 
         #pass using object
         # if header.copy_to_cluster_flag:
         cl.cluster_address      = header.cluster_address
@@ -1882,15 +1885,15 @@
 
 
 
         if status == "compl": 
             cl.state = '2. Can be completed but was reinitialized' #new behavior 30.08.2016
 
 
-        print_and_log("\nCalculation db["+str(id)+"] successfully created\n\n", imp = 'Y')
+        printlog("\nCalculation db["+str(id)+"] successfully created\n\n", imp = 'Y')
 
 
 
 
     return
 
 
@@ -2035,44 +2038,44 @@
 
 
 
 
 
     if id_from:
         if type(id_from) == str: # if string - treated like file name
-            print_and_log("I detect *id_from* path provided; taking some information from:", id_from)
+            printlog("I detect *id_from* path provided; taking some information from:", id_from)
 
             calc_from = CalculationVasp();
             calc_from.read_geometry(id_from)
             calc_from.end = calc_from.init
             calc_from_name = id_from
         else:
-            print_and_log("I detect *id_from* Calculation(); taking some information from:", id_from, id_from_st_type)
+            printlog("I detect *id_from* Calculation(); taking some information from:", id_from, id_from_st_type)
             
 
             calc_from = calc[id_from]
             calc_from_name = calc_from.name
 
         if id_from_st_type == 'end':
             st_from = calc_from.end
         elif id_from_st_type == 'init':
             st_from = calc_from.init
 
 
 
         if cl_base.len_units != calc_from.len_units:
-            print_and_log("Calculations have different len_units"); raise RuntimeError
+            printlog("Calculations have different len_units"); raise RuntimeError
 
         if it_new == id_from[0] and ver_new == id_from[2]:
-            print_and_log("Warning! check your versions, you are trying to overwrite existing from structures, nothing done")
+            printlog("Warning! check your versions, you are trying to overwrite existing from structures, nothing done")
             raise RuntimeError 
 
 
     if it_new == cl_base.id[0] and ver_new == cl_base.id[2]:
-        print_and_log("Warning! check your versions, you are trying to overwrite existing base structures, nothing done")
+        printlog("Warning! check your versions, you are trying to overwrite existing base structures, nothing done")
         raise RuntimeError
   
 
 
 
     new = copy.deepcopy(  cl_base  )
 
@@ -2116,15 +2119,15 @@
     if geo_folder == '':
         new.path["input_geo"] = it_new_folder + '/' +it_new+'.inherit.'+inherit_type+'.'+str(ver_new)+'.'+'geo'
     else:
         new.path["input_geo"] = geo_folder + '/' + it_new+"/"+it_new+'.inherit.'+inherit_type+'.'+str(ver_new)+'.'+'geo'
 
     
     makedir(new.path["input_geo"])
-    print_and_log('Path for inherited calc =', it_new_folder)
+    printlog('Path for inherited calc =', it_new_folder)
 
 
 
 
     if inherit_type == "r2r3":
         des = ' Partly inherited from the final state of '+cl_base.name+'; r2 and r3 from '+calc_from_name
         st.rprimd[1] = st_from.rprimd[1].copy()
@@ -2171,68 +2174,68 @@
         except:
             printlog('Attention! hex_a and hex_c were not found')
 
         st.update_xcart() #calculate new xcart from xred, because rprimd was changed
 
 
     elif inherit_type in ["full", ]:
-        # print_and_log("Warning! final xred and xcart was used from OUTCAR and have low precision. Please use CONTCAR file \n");
+        # printlog("Warning! final xred and xcart was used from OUTCAR and have low precision. Please use CONTCAR file \n");
         des = 'Fully inherited from the final state of '+cl_base.name
 
 
     elif inherit_type  == 'full_chg':
 
         des = 'Fully inherited (including chg file ) from the final state of '+cl_base.name
 
         # The file is copied in add_loop_finalize !!!
 
     elif inherit_type == "full_nomag":
-        # print_and_log("Warning! final xred and xcart was used from OUTCAR and have low precision. Please use CONTCAR file \n");
+        # printlog("Warning! final xred and xcart was used from OUTCAR and have low precision. Please use CONTCAR file \n");
         des = 'Fully inherited from the final state of '+cl_base.name+'; "magmom" set to [None]'
         st.magmom = [None]
 
     elif inherit_type == "occ":
         des = 'Fully inherited from the final state of '+cl_base.name+'; occupation matrix is taken from '+calc_from_name
 
-        print_and_log('Inherit option: "occ", reading occupation matrices from',calc_from_name)
+        printlog('Inherit option: "occ", reading occupation matrices from',calc_from_name)
         
         if not calc_from.occ_matrices:
-            print_and_log('Error! calc_from.occ_matrices is empty')
+            printlog('Error! calc_from.occ_matrices is empty')
             raise RuntimeError
 
 
         #additional control to which atoms should be applied
         #if cells are different
-        print_and_log('You can use *occ_atom_coressp* to control for which atoms you inherit occupations')
+        printlog('You can use *occ_atom_coressp* to control for which atoms you inherit occupations')
 
 
 
         if calc_from.end.natom != new.natom or occ_atom_coressp:
             
             if calc_from.end.natom != new.natom:
-                print_and_log('Attention! Numbers of atoms are different. Please use *occ_atom_coressp* or I will try to use most closest to alkali ion d-atoms ')
+                printlog('Attention! Numbers of atoms are different. Please use *occ_atom_coressp* or I will try to use most closest to alkali ion d-atoms ')
 
             if not occ_atom_coressp:
                 # raise RuntimeError
-                print_and_log('Please run res_loop(show = "occ") for *id_base*=',id_base, ' and *id_from*=',id_from, 'to save self.dist_numb')
+                printlog('Please run res_loop(show = "occ") for *id_base*=',id_base, ' and *id_from*=',id_from, 'to save self.dist_numb')
 
 
                 occ_atom_coressp = {}
                 occ_atom_coressp[calc_from.dist_numb[0][1] ] = new.dist_numb[0][1] 
             
             
-            print_and_log('The occ matrices will be inherited from atom # in id_from to atom # in id_base:', end = '\n')
+            printlog('The occ matrices will be inherited from atom # in id_from to atom # in id_base:', end = '\n')
             occs = {}
                 
             for iat_from in occ_atom_coressp: # key is atom number in id_from 
                 iat_new = occ_atom_coressp[iat_from] #new is based on id_base
                 occs[ iat_new ] = calc_from.occ_matrices[iat_from]
-                print_and_log('        occ:',iat_from+1,'-->', iat_new+1)
+                printlog('        occ:',iat_from+1,'-->', iat_new+1)
         else:
-            print_and_log('The cells seems to be consistent; full inheritence of occ_matrices')
+            printlog('The cells seems to be consistent; full inheritence of occ_matrices')
             occs = calc_from.occ_matrices
         
         # sys.exit()
 
         write_occmatrix(occs, it_new_folder)
 
 
@@ -2241,24 +2244,24 @@
 
 
 
         # sys.exit()
 
     elif inherit_type == 'supercell':
         from siman.geo import ortho_vec, create_supercell
-        print_and_log('       inherit_icalc(): starting supercell mode ...', imp = 'Y')
-        # print_and_log('rprimd is \n', st.rprimd)
+        printlog('       inherit_icalc(): starting supercell mode ...', imp = 'Y')
+        # printlog('rprimd is \n', st.rprimd)
         
         if mul_matrix is None: #if *mul_matrix* is not provided, try to use *ortho*
             mul_matrix = ortho_vec(st.rprimd, ortho_sizes = ortho)
             printlog('*mul_matrix* was calculated from *ortho*')
         else:
             printlog('*mul_matrix* was explicitly provided')
 
-        print_and_log('Mul matrix is\n',mul_matrix)
+        printlog('Mul matrix is\n',mul_matrix)
         st = create_supercell(st, mul_matrix)
         # sc.mul_matrix = mul_matrix.copy()
         # new.init = sc
         # new.end  = sc
         des = 'obtained from '+cl_base.name+' by creating supercell '+str(ortho)
         override = True
     
@@ -2303,15 +2306,15 @@
 
 
 
     elif inherit_type == "make_vacancy":
         """Remove  atom 'i_atom_to_remove' from final state of id_base"""
 
 
-        print_and_log('Warning! Please check inherit_type == "make_vacancy", typat can be wrong  if more than one element present in the system\n ',
+        printlog('Warning! Please check inherit_type == "make_vacancy", typat can be wrong  if more than one element present in the system\n ',
             'Use del_atom() method ')
         # raise RuntimeError
 
         des = 'Atom '+str(i_atom_to_remove)+' removed from  '+cl_base.name
 
         del st.typat[i_atom_to_remove]
         del st.xcart[i_atom_to_remove]
@@ -2343,33 +2346,33 @@
 
 
 
 
         znucl = st.znucl
         
         if z_replace not in znucl: 
-            print_and_log("Error! Calc "+new.name+" does not have atoms of this type")
+            printlog("Error! Calc "+new.name+" does not have atoms of this type")
             raise RuntimeError
 
         if atom_to_replace not in id_base[0] or atom_new not in it_new:
-            print_and_log("Error! inherit_icalc(): Something wrong with names of atom types")
+            printlog("Error! inherit_icalc(): Something wrong with names of atom types")
             raise RuntimeError            
-        print_and_log( "replace ", z_replace, "by", z_new)
+        printlog( "replace ", z_replace, "by", z_new)
 
         znucl = [int(z) for z in znucl] # convert to int
         i_r = znucl.index(z_replace)
-        print_and_log( "index ", i_r)
+        printlog( "index ", i_r)
         znucl[i_r] = z_new
 
         if znucl[-2] == znucl[-1]: #just for special case
             del znucl[-1]
 
             for i, t in enumerate(st.typat):
                 if t == st.ntypat:
-                    print_and_log( "found ntypat" ,t)
+                    printlog( "found ntypat" ,t)
                     st.typat[i]-=1
                     #print t
             st.ntypat-=1
             #print st.typat
             #print new.end.typat
         
         st.znucl = znucl
@@ -2407,15 +2410,15 @@
         des = 'Inherited from the final state of '+cl_base.name+' with the copying the wave function and waveder files'
 
 
 
 
 
     else:
-        print_and_log("Error! Unknown type of Calculation inheritance")
+        printlog("Error! Unknown type of Calculation inheritance")
 
 
 
     
 
 
 
@@ -2604,14 +2607,16 @@
 
 
     """
 
 
     """Setup"""
 
+    from siman.picture_functions import plt
+
 
 
     if not is_list_like(verlist):
         verlist = [verlist]
 
     if not is_list_like(setlist):
         setlist = [setlist]
@@ -2692,28 +2697,28 @@
                     calc[b_id].read_results(loadflag, choose_outcar = choose_outcar)
                 
                 e_b = 1e10; v_b = 1e10
                 if '4' in calc[b_id].state:
                     e_b = calc[b_id].energy_sigma0
                     v_b = calc[b_id].end.vol
                 else:
-                    print_and_log('Warning! Calculation ',b_id, 'was not finished; please check, now skipping ...', important = 'y')
+                    printlog('Warning! Calculation ',b_id, 'was not finished; please check, now skipping ...', important = 'y')
         else:
             printlog('Attention! res_loop(): b_id', b_id, 'does not exist. return {} []')
             # return {}, []
 
     #define reference values
     e1_r = 0
     if type(r_id) in (float, int):
         e1_r = r_id
     elif type(r_id) == tuple:
         # if '4' not in calc[r_id].state:
         #     print "Start to read reference:"
         if readfiles:
-            print_and_log( calc[r_id].read_results(loadflag, choose_outcar = choose_outcar)  )
+            printlog( calc[r_id].read_results(loadflag, choose_outcar = choose_outcar)  )
         e_r = calc[r_id].energy_sigma0 #reference calc
         nat_r = calc[r_id].end.natom # reference calc
         e1_r = e_r/nat_r # energy per one atom
         # print e1_r
 
 
     """Amendmend required before main loop """
@@ -3003,28 +3008,28 @@
 
         if id not in calc or '4' not in calc[id].state:
             # printlog(calc[id].state, imp = 'Y')
             try:
                 dire = cl.dir
             except:
                 dire = ''
-            print_and_log( "res_loop(): Calculation ",id, 'is unfinished; return \{\} []',dire, imp = 'Y')
+            printlog( "res_loop(): Calculation ",id, 'is unfinished; return \{\} []',dire, imp = 'Y')
             return {}, []
         
         outloop_segreg_analysis(b_id, analys_type, conv, n, description_for_archive, show, push2archive)
 
         
 
 
 
 
         if analys_type == 'redox_pot':
             
             if '4' not in bcl.state:
-                print_and_log("res_loop: Calculation ",bcl.id, 'is unfinished; return', imp = 'Y')
+                printlog("res_loop: Calculation ",bcl.id, 'is unfinished; return', imp = 'Y')
                 return {}, []
 
             results_dic = calc_redox(cl, bcl, energy_ref)
             
 
         if analys_type == 'neb':
             results_dic = neb_analysis(cl, show, up, push2archive, old_behaviour, results_dic, fitplot_args, style_dic, params)
@@ -3153,15 +3158,15 @@
     coeffs1 = np.polyfit(T, F, 8)
     fit_func = np.poly1d(coeffs1)
     T_range = np.linspace(min(T), max(T))
     
 
     fit_and_plot(d1 = (T, F, 'b-', 'orig'), d2 = (T_range, fit_func(T_range), 'r--', 'fit'), show = 1)
 
-    print_and_log( 'I return', key)
+    printlog( 'I return', key)
 
     return T_range, fit_func
 
 
 
 
 def for_phonopy(new_id, from_id = None, calctype = 'read', mp = [10, 10, 10], additional = None):
@@ -3210,15 +3215,15 @@
                 el = element_name_inv(z)
                 f.write(el+' ')
             f.write("\nDIAG = .TRUE.\n")
             f.write("DISPLACEMENT_DISTANCE = 0.03\n")
 
          
         #run phonopy
-        print_and_log(
+        printlog(
             runBash('export PYTHONPATH=~/installed/phonopy-1.9.5/lib/python:$PYTHONPATH; rm POSCAR-*;'+header.path_to_phonopy 
             +confname+' -c '+posname+' -d --tolerance=0.01'), imp = 'y' )
 
         ndis = len( glob.glob('POSCAR-*') )
         print( ndis, ' displacement files was created\n\n\n\n', )
 
         os.chdir(savedPath)
@@ -3277,24 +3282,24 @@
                 f.write("\nMP = {:}\n".format( mpstr ))
                 f.write("\nTSTEP = {:}\n".format( 1 ))
                 f.write("\nTMAX = {:}\n".format( 1155 ))
 
             if not os.path.exists("FORCE_SETS"):
                 #run phonopy; read forces
                 ndis = len( glob.glob('*.vasprun.xml') )
-                print_and_log( ndis, ' displacement files was Found')
-                print_and_log( runBash('export PYTHONPATH=~/installed/phonopy-1.9.5/lib/python:$PYTHONPATH; '+header.path_to_phonopy 
+                printlog( ndis, ' displacement files was Found')
+                printlog( runBash('export PYTHONPATH=~/installed/phonopy-1.9.5/lib/python:$PYTHONPATH; '+header.path_to_phonopy 
                     +'  -f {1..'+str(ndis)+'}.vasprun.xml --tolerance=0.01'), imp = 'Y' )
 
             #calculate thermal prop
             result = 'thermal_properties_'+mpstr.replace(" ", "_")+'.yaml'
             if not os.path.exists(result):
 
                 posname = 'SPOSCAR'
-                print_and_log( runBash('export PYTHONPATH=~/installed/phonopy-1.9.5/lib/python:$PYTHONPATH; '+header.path_to_phonopy 
+                printlog( runBash('export PYTHONPATH=~/installed/phonopy-1.9.5/lib/python:$PYTHONPATH; '+header.path_to_phonopy 
                     +confname+' -c '+posname+' -t -p -s --tolerance=0.01'), imp = 'y' )
 
                 shutil.copyfile('thermal_properties.yaml', result)
     
 
             T_range, fit_func = read_phonopy_data(result)
 
@@ -3318,15 +3323,15 @@
     """
     cee_struct_type (str) - 
         'exp' - experimental structures
         '' - all
 
     """
     it_base = it.split('.')[0]
-    print_and_log("Taking structure "+it_base+" from CEE CREI database of Skoltech ...", imp = 'Y')
+    printlog("Taking structure "+it_base+" from CEE CREI database of Skoltech ...", imp = 'Y')
 
     # database_server = 'aksenov@10.30.100.28'
     database_server = 'sd'
     # database_path   = '/home/Data/CEStorage/'
     database_path   = '/home/Data/'+section+'/'
 
     if 'exp' in cee_struct_type:
@@ -3443,15 +3448,15 @@
         makedir(path2poscar)
     else:
         # path2poscar = groundstate_st_id+".POSCAR"
         path2poscar = it_folder+'/'+groundstate_st_id+".POSCAR" if it_folder else groundstate_st_id+".POSCAR"
 
     
     Poscar(st_pmg).write_file(path2poscar, direct=True, vasp4_compatible=True, )
-    print_and_log('Structure', groundstate_st_id, 'downloaded from materialsproject.org\n',
+    printlog('Structure', groundstate_st_id, 'downloaded from materialsproject.org\n',
         'File '+path2poscar+" was written", imp = 'y')
 
     st = smart_structure_read(input_geo_file = path2poscar)
     st.groundstate_st_id = groundstate_st_id
     st.mat_proj_st_id    = groundstate_st_id
     st.input_geo_file    = path2poscar
 
@@ -3488,15 +3493,15 @@
 
 
 def manually_remove_from_struct_des(struct_des, key):
     """
     
     """
     del struct_des[key]
-    print_and_log('Attention! Entry '+key+' was removed from struct_des dict/\n')
+    printlog('Attention! Entry '+key+' was removed from struct_des dict/\n')
```

### Comparing `siman-1.3.6/siman/calcul.py` & `siman-1.3.7/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/calculators/aims.py` & `siman-1.3.7/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/calculators/gaussian.py` & `siman-1.3.7/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/calculators/qe.py` & `siman-1.3.7/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/calculators/vasp.py` & `siman-1.3.7/siman/calculators/vasp.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os, math, copy, glob, shutil, sys
 import numpy as np
 from siman import header
 from siman.core.calculation import Calculation
 from siman.core.structure import Structure
 from siman.header import runBash
 
-from siman.header import printlog, print_and_log, runBash, plt
+from siman.header import printlog, runBash
 
 from siman import set_functions
 # from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.functions import (read_vectors, read_list, words, read_string,
      element_name_inv, invert, calculate_voronoi, 
     get_from_server, push_to_server, run_on_server, smoother, file_exists_on_server, check_output)
@@ -68,28 +68,28 @@
         self.gbpos = None
 
 
         #Determine version
         if version:
             self.version = version
         else:
-            print_and_log('Trying to find version at the end of filename POSCAR-v ...')
+            printlog('Trying to find version at the end of filename POSCAR-v ...')
             try:
                 ver = int(filename.split('-')[-1])
-                print_and_log('OK\n')
+                printlog('OK\n')
 
             except:
-                print_and_log('\nTrying to find version at the begenning of filename v.POSCAR...')
+                printlog('\nTrying to find version at the begenning of filename v.POSCAR...')
 
                 try:
                     ver = int(os.path.basename(filename).split('.')[0] )
-                    print_and_log('OK\n')
+                    printlog('OK\n')
                
                 except:
-                    print_and_log('No version, using 1\n')
+                    printlog('No version, using 1\n')
                     ver = 1
 
             self.version = ver
 
         self.init = Structure()
         self.init = read_poscar(self.init, filename)
         self.des = self.init.des
@@ -105,15 +105,15 @@
            option -inheritance option
            prevcalcver - ver of first calc in calc list; for first None
            state - 'init' or 'end' 
         """
         #units
         # try:
         #     if "ang" in self.len_units or "Ang" in self.len_units: 
-        #         global to_ang; to_ang = 1.0; print_and_log("Conversion multiplier to_ang is "+str(to_ang) )
+        #         global to_ang; to_ang = 1.0; printlog("Conversion multiplier to_ang is "+str(to_ang) )
         # except AttributeError:
         #     pass
 
         if option == 'inherit_xred' and 'car' in type_of_coordinates: 
             raise RuntimeError 
 
         if option == 'inherit_xred' and prevcalcver: 
@@ -322,15 +322,15 @@
                
 
                 f.write("\n")
 
 
 
 
-            print_and_log(incar_filename, "was generated\n")
+            printlog(incar_filename, "was generated\n")
         
             incar_list.append(incar_filename)
         
 
         return incar_list
 
 
@@ -426,65 +426,65 @@
 
 
 
 
         elif self.set.kpoints_file:
             if self.set.kpoints_file is True:
 
-                print_and_log( "You said to generate KPOINTS file. set.kpoints_file =",self.set.kpoints_file," \n")
+                printlog( "You said to generate KPOINTS file. set.kpoints_file =",self.set.kpoints_file," \n")
                 self.calc_kspacings()
                 #Generate kpoints file
 
                 #
                 if hasattr(struct_des[it], 'ngkpt_dict_for_kspacings') and kspacing in struct_des[it].ngkpt_dict_for_kspacings:
                     N =    struct_des[it].ngkpt_dict_for_kspacings[kspacing]
-                    print_and_log( 'Attention! ngkpt = ',N, 
+                    printlog( 'Attention! ngkpt = ',N, 
                         ' is adopted from struct_des which you provided for it ',it, ' and kspacing = ',kspacing)
                     nk1 = N[0]; nk2 = N[1]; nk3 = N[2]
                     self.set.ngkpt = N
 
                 elif self.set.ngkpt:
                     nk1 = self.set.ngkpt[0]; nk2 = self.set.ngkpt[1]; nk3 = self.set.ngkpt[2];
-                    print_and_log( "Attention! ngkpt was used for kpoints file\n")
+                    printlog( "Attention! ngkpt was used for kpoints file\n")
 
                 
                 elif kspacing:
-                    print_and_log( "Attention! ngkpt for kpoints file are created from kspacing; ngkpt is empty\n")
+                    printlog( "Attention! ngkpt for kpoints file are created from kspacing; ngkpt is empty\n")
                     N = self.check_kpoints()
                     self.set.ngkpt = N
                     nk1 = N[0]; nk2 = N[1]; nk3 = N[2]
                 
                 else:
-                    print_and_log( "Error! could not find information about k-points\n")
+                    printlog( "Error! could not find information about k-points\n")
 
 
 
                 with open(filename,'w', newline = '') as f:
 
                     f.write("Automatic Mesh\n") #Comment
                     f.write("0 \n")#Number of points; 0-Auto
                     if 'KGAMMA' in self.set.vasp_params and self.set.vasp_params["KGAMMA"] in (1,'.TRUE.', 'True', '1'): 
                         f.write("Gamma\n")
                     else: 
                         f.write("Monkhorst Pack\n")
                     f.write('%i %i %i \n'%(nk1, nk2, nk3) )
                     f.write("0 0 0\n") # optional shift
 
-                print_and_log( "KPOINTS was generated\n")
+                printlog( "KPOINTS was generated\n")
             
             else:
                 # print()
                 shutil.copyfile(self.set.kpoints_file, filename)
-                print_and_log( "KPOINTS was copied from"+self.set.kpoints_file+"\n")
+                printlog( "KPOINTS was copied from"+self.set.kpoints_file+"\n")
 
             self.path['kpoints'] = filename 
 
 
         else:
-            print_and_log( "This set is without KPOINTS file.\n")
+            printlog( "This set is without KPOINTS file.\n")
             filename = ''
 
 
 
         return [filename]
 
 
@@ -657,19 +657,19 @@
 
         # print(hasattr(self.init, 'magmom') and hasattr(self.init.magmom, '__iter__') and not None in self.init.magmom)
         # print(self.init.magmom)
         # print(None in self.init.magmom)
         # sys.exit()
         if hasattr(self.init, 'magmom') and hasattr(self.init.magmom, '__iter__') and not None in self.init.magmom and bool(self.init.magmom):
 
-            print_and_log('actualize_set(): Magnetic moments are determined from self.init.magmom:',self.init.magmom, imp = 'y')
+            printlog('actualize_set(): Magnetic moments are determined from self.init.magmom:',self.init.magmom, imp = 'y')
 
         elif hasattr(curset, 'magnetic_moments') and curset.magnetic_moments:
-            print_and_log('actualize_set(): Magnetic moments are determined using siman key "magnetic_moments" and corresponding dict in set', end = '\n')
-            print_and_log('curset.magnetic_moments = ', curset.magnetic_moments)
+            printlog('actualize_set(): Magnetic moments are determined using siman key "magnetic_moments" and corresponding dict in set', end = '\n')
+            printlog('curset.magnetic_moments = ', curset.magnetic_moments)
             
             mag_mom_other = 0.6 # magnetic moment for all other elements
             magmom = []
             for el in curset.magnetic_moments.keys():
                 if '/' in el and ldau == False:
                     # if ldau is true and multitype regime is true then everything is updated above
                     # if ldau is true and multitype is false than we cant use multitype here because LDAUL will become incompatible with POSCAR 
@@ -714,28 +714,28 @@
             #check possible antiferromagnetic configurations:
             spec_mom_is = []
             for i, m in enumerate(magmom):
                 if m != mag_mom_other: #detected some specific moment
                     spec_mom_is.append(i)
 
             if len(spec_mom_is) % 2 == 0 and len(spec_mom_is) > 0:
-                print_and_log('Number of elements is even! trying to find all antiferromagnetic orderings:', imp = 'y')
+                printlog('Number of elements is even! trying to find all antiferromagnetic orderings:', imp = 'y')
                 ns = len(spec_mom_is); 
                 number_of_ord = int(math.factorial(ns) / math.factorial(0.5 * ns)**2)
                 
                 if number_of_ord > 10000:
                     printlog('Attention! Too much orderings (1000), skipping ...')
                 else:
                     nords = 71
                     use_each = number_of_ord // nords  # spin() should be improved to find the AFM state based on the number of configuration 
                     if use_each == 0:
                         use_each = 1
 
                     if number_of_ord > nords:
-                        print_and_log('Attention! Number of orderings is', number_of_ord, ' more than', nords, ' - I will check only each first ', imp = 'y')
+                        printlog('Attention! Number of orderings is', number_of_ord, ' more than', nords, ' - I will check only each first ', imp = 'y')
                 # else:
 
                     ls = [0]*len(spec_mom_is)
                     # print ls
                     orderings = []
                     
 
@@ -791,24 +791,24 @@
                         
 
                         printlog(j, new_magmom,)
                         
                         mag_orderings.append(new_magmom)
 
                     # print orderings
-                    print_and_log('Total number of orderings is ', len(orderings),imp = 'y')
+                    printlog('Total number of orderings is ', len(orderings),imp = 'y')
                     
                     if self.calc_method and 'afm_ordering' in self.calc_method:
                         self.magnetic_orderings = mag_orderings
                   
             self.init.magmom = magmom # the order is the same as for other lists in init
 
         
         elif 'MAGMOM' in vp and vp['MAGMOM']: #just add * to magmom tag if it is provided without it
-            print_and_log('Magnetic moments from vasp_params["MAGMOM"] are used\n')
+            printlog('Magnetic moments from vasp_params["MAGMOM"] are used\n')
             
             # if "*" not in vp['MAGMOM']:
             #     vp['MAGMOM'] = str(natom) +"*"+ vp['MAGMOM']
         
 
 
         # print (self.init.magmom, 'asdfaaaaaaaaaaaa')
@@ -923,28 +923,31 @@
 
         return
 
     def plot_energy_step(self,):
         # print(self.maxforce)
         # maxf = [m[1] for m in self.maxforce_list ]
         # print(maxf)
+        from siman.picture_functions import plt
         steps = range(len(self.list_e_sigma0))
         plt.plot(steps, 1000*(np.array(self.list_e_sigma0)-self.energy_sigma0) , '-o')
         # plt.xlabel('MD step')
         # plt.ylabel('Energy per cell (eV')
         plt.xlabel('Step')
         plt.ylabel('Energy per cell relative to min (meV)')
 
         plt.show()
         return
 
     def plot_energy_conv(self,):
         # print(self.maxforce)
         # maxf = [m[1] for m in self.maxforce_list ]
         # print(maxf)
+        from siman.picture_functions import plt
+
         en = self.list_e_conv[10:]
         steps = range(len(en))
         plt.plot(steps, (np.array(en)-self.energy_sigma0) , '-o')
         # plt.xlabel('MD step')
         # plt.ylabel('Energy per cell (eV')
         plt.xlabel('SCF Step')
         plt.ylabel('Energy per cell relative to min (eV)')
@@ -1039,15 +1042,15 @@
             # print "ssh "+self.cluster_address+" cat "+self.dir+"ENERGIES"
             # print (  energies_str )
             # if not 'cat' in energies_str:
             #     self.associated_energies = [float(e) for e in energies_str.split()]
             
             # self.u_ramping_u_values = np.arange(*self.u_ramping_list)
             # print 'associated_energies:', self.associated_energies
-        print_and_log('read_results() path to outcar', path_to_outcar)
+        printlog('read_results() path to outcar', self.project_path_cluster+path_to_outcar)
         # sys.exit()
 
 
 
         if not os.path.exists(path_to_outcar):
             load = load+'o'
 
@@ -1435,19 +1438,19 @@
 
         local_atoms = local_surrounding(self.xcart[-1], self.end, 6, control = 'atoms')
         numbers = local_atoms[2] # first atom is impurity
         # print numbers
         imp_partial_chg = imp_valence_chg - float(ACF[numbers[0]].split()[4])
 
         mat_partial_chg = [mat_valence_chg - float(ACF[i].split()[4]) for i in numbers[1:] ]
-        print_and_log( "Partial charge of impurity ", imp_partial_chg, imp = 'Y' )
-        print_and_log( "Partial charges of neibouring Ti atoms", " ".join("{:.2f}".format(m) for m in mat_partial_chg), imp = 'Y' )
-        print_and_log( "Partial charge of matrix", sum(mat_partial_chg), imp = 'Y' )
+        printlog( "Partial charge of impurity ", imp_partial_chg, imp = 'Y' )
+        printlog( "Partial charges of neibouring Ti atoms", " ".join("{:.2f}".format(m) for m in mat_partial_chg), imp = 'Y' )
+        printlog( "Partial charge of matrix", sum(mat_partial_chg), imp = 'Y' )
         
-        print_and_log( "Sum of mat and imp charges:", sum(mat_partial_chg)+imp_partial_chg, imp = 'Y' )
+        printlog( "Sum of mat and imp charges:", sum(mat_partial_chg)+imp_partial_chg, imp = 'Y' )
 
         return path_to_file
 
 
 
 
 
@@ -1542,14 +1545,17 @@
         INPUT:
             - ylim (2*tuple of float)
         """
 
         from pymatgen.io.vasp import Vasprun, BSVasprun
         from pymatgen.electronic_structure.plotter import BSPlotter
 
+        from siman.picture_functions import plt
+
+
         xml_file = self.get_file('vasprun.xml', nametype = 'asoutcar')
         # print(xml_file)
         # print(self.path['kpoints']) #os.getcwd()+'/'+
         if ylim is None:
             ylim = (-12,6)
 
         # sys.exit()
```

### Comparing `siman-1.3.6/siman/calculators/vasp_old.py` & `siman-1.3.7/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/chg/chg_func.py` & `siman-1.3.7/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/chg/vasputil_chgarith_module.py` & `siman-1.3.7/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/classes.py` & `siman-1.3.7/siman/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,19 +33,18 @@
 if header.pymatgen_flag:
     from pymatgen.io.cif import CifWriter
     from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
     from pymatgen.core.surface import Slab
     from pymatgen.core.composition import Composition
 
 
-# import matplotlib.pyplot as plt
 
 #siman packages
 
-from siman.header import printlog, print_and_log, runBash, plt
+from siman.header import printlog, runBash
 
 from siman import set_functions
 # from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.functions import (read_vectors, read_list, words, read_string,
      element_name_inv, invert, calculate_voronoi, 
     get_from_server, push_to_server, run_on_server, smoother, file_exists_on_server, check_output)
```

### Comparing `siman-1.3.6/siman/core/calculation.py` & `siman-1.3.7/siman/core/calculation.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,16 @@
 
 if header.pymatgen_flag:
     from pymatgen.io.cif import CifWriter
     from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
     from pymatgen.core.surface import Slab
     from pymatgen.core.composition import Composition
 
-from siman.header import printlog
 
-from siman.header import printlog, print_and_log, runBash, plt
+from siman.header import printlog
 
 from siman import set_functions
 # from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.functions import (read_vectors, read_list, words, read_string,
      element_name_inv, invert, calculate_voronoi, 
     get_from_server, push_to_server, run_on_server, smoother, file_exists_on_server, check_output)
@@ -115,15 +114,15 @@
             for line in memfile.splitlines():
                 if 'des' in line: 
                     # print line; 
                     self.des = line.split('des ')[1]+';'
                 
                 self.build = empty_struct()                
                 if 'BEGIN BUILD INFORMATION' in line:
-                    print_and_log("File contain build information! Start to read", imp = 'n')
+                    printlog("File contain build information! Start to read", imp = 'n')
                     # self.build = Structure()
                     # # self.build.rprimd = None
                     # # self.build.xred = None
                     # # self.build.xcart = None
                     # # self.build.des = None
                     # # self.build.name = None
 
@@ -140,15 +139,15 @@
                     self.build.uvw1 = read_vectors("uvw1", 1, gen_words)
                     self.build.uvw2 = read_vectors("uvw2", 1, gen_words)
                     self.build.uvw3 = read_vectors("uvw3", 1, gen_words)
                     self.build.mul  = read_vectors("mul", 1, gen_words)
                     self.build.nadded = read_list("nadded", 1, int, gen_words)[0] #total number of added atoms after building structure
                     self.build.listadded = read_list("listadded", self.build.nadded, int, gen_words) #list of added atoms corresponding to xred 
 
-                    print_and_log("Build information has been read")
+                    printlog("Build information has been read")
 
 
 
 
             self.init = Structure()
 
             #sys.exit()
@@ -159,15 +158,15 @@
 #             s1=runBash(command)
             self.natom = read_list("natom", 1, int, gen_words)[0]
             # print command
             # print s1
 #             self.natom_str = s1
 #             if s1=='':
 #                 self.natom = 0
-#                 print_and_log( """Warning! In filename """+filename+""" not found natom! set to zero.
+#                 printlog( """Warning! In filename """+filename+""" not found natom! set to zero.
 #                 It is very likely that other parameters was not 
 #                 found too, Calculation completely unusable!!!""")
 #                 raise RuntimeError
 #             else:
 #                 self.natom=int(s1.split()[1]) 
 
             self.acell = read_list("acell", 3, float, gen_words)
@@ -181,15 +180,15 @@
                       
             self.recip = calc_recip_vectors(self.rprimd) #Determine reciprocal vectors
 
 
             self.ntypat = read_list("ntypat", 1, int, gen_words)[0]
             self.typat = read_list("typat", self.natom, int, gen_words)
             if 0 in self.typat:
-                print_and_log('Error; 0 in typat is not allowed')
+                printlog('Error; 0 in typat is not allowed')
                 raise RuntimeError
 
             self.nznucl = []
 
             for typ in range(1,self.ntypat+1):
                 self.nznucl.append(  self.typat.count(typ) )
 
@@ -197,19 +196,19 @@
             self.znucl = read_list("znucl", self.ntypat, float, gen_words)
             self.xcart = read_vectors("xcart", self.natom, gen_words)
             
             self.xred = read_vectors("xred", self.natom, gen_words)
             #print self.xred
             # print(self.xcart)
             if self.xred is [None]:
-                print_and_log("Convert xcart to xred")
+                printlog("Convert xcart to xred")
                 self.xred = xcart2xred(self.xcart, self.rprimd)
             
             if self.xcart is [None]:
-                print_and_log("Convert xred to xcart")
+                printlog("Convert xred to xcart")
                 self.xcart = xred2xcart(self.xred, self.rprimd)
 
             self.hex_a = read_list("hex_a", 1, float, gen_words)[0]
             self.hex_c = read_list("hex_c", 1, float, gen_words)[0]
             self.len_units = read_list("len_units", 1, str, gen_words)[0]
 
             self.version = read_list("version", 1, int, gen_words)[0]
@@ -264,15 +263,15 @@
 
             self.state = "1.Geometry has been read"
 
 
 
         #file.close();
 
-        print_and_log( "If no warnings, geometry has been succesfully read from file "+filename+" \n")
+        printlog( "If no warnings, geometry has been succesfully read from file "+filename+" \n")
 
         return
 
 
 
 
 
@@ -295,17 +294,17 @@
             en = 1
             le = 1            
 
 
 
         if geo_exists:
             if override:
-                print_and_log("Warning! File "+geofile+" was replaced"); 
+                printlog("Warning! File "+geofile+" was replaced"); 
             else: 
-                print_and_log("Error! File "+geofile+" exists. To replace it set parameter override"); 
+                printlog("Error! File "+geofile+" exists. To replace it set parameter override"); 
                 return False
                 #raise RuntimeError
         # print "geofile name, classes:",  geofile
         # print "folder :",  os.path.dirname(geofile)
         if not os.path.exists(os.path.dirname(geofile)):
             os.makedirs(os.path.dirname(geofile))
 
@@ -313,18 +312,18 @@
             st = self.init
         elif geotype == "end":
             st = self.end
             # if not hasattr(st, 'natom'):  st.natom = self.init.natom
             # if not hasattr(st, 'ntypat'): st.ntypat = self.init.ntypat
             # if not hasattr(st, 'typat'): st.typat = self.init.typat
             # if not hasattr(st, 'znucl'): st.znucl = self.init.znucl 
-        else: print_and_log("Error! Unknown geotype \n"); raise RuntimeError                                  
+        else: printlog("Error! Unknown geotype \n"); raise RuntimeError                                  
 
         if st.natom != len(st.xred) != len(st.xcart) != len(st.typat) or len(st.znucl) != max(st.typat): 
-            print_and_log("Error! write_geometry: check your arrays.", imp = 'Y')
+            printlog("Error! write_geometry: check your arrays.", imp = 'Y')
             raise RuntimeError
 
         # print (st.magmom)
         # sys.exit()
         with open(self.path["input_geo"],"w", newline = '') as f:
             f.write("des "+description+"\n")
             f.write("len_units "+self.len_units+"\n")
@@ -379,21 +378,21 @@
 
             f.write("\nrprim  ")
             for v in st.rprimd:
                 f.write("%.12f %.12f %.12f \n"%(v[0]*le, v[1]*le, v[2]*le)  )
 
             f.write("xred  ")
             #print st.xred
-            if len(st.xred) != st.natom: print_and_log("Warning! write_geometry(): xred is empty or overfull\n");raise RuntimeError 
+            if len(st.xred) != st.natom: printlog("Warning! write_geometry(): xred is empty or overfull\n");raise RuntimeError 
             for v in st.xred:
                 f.write("%.12f %.12f %.12f \n"%(v[0], v[1], v[2])  )
 
             f.write("xcart  ")
             if len(st.xcart) != st.natom: 
-                print_and_log("Warning! write_geometry(): xcart is empty or overfull, I make it from xred\n");#raise RuntimeError
+                printlog("Warning! write_geometry(): xcart is empty or overfull, I make it from xred\n");#raise RuntimeError
                 st.xcart = xred2xcart(st.xred, st.rprimd) 
             for v in st.xcart:
                 f.write("%.12f %.12f %.12f \n"%(v[0]*le, v[1]*le, v[2]*le)  )
 
             if hasattr(st, 'select') and len(st.select) > 0 and not None in st.select:
                 f.write("\nselect  ")
                 for v in st.select:
@@ -719,14 +718,15 @@
             fit_and_plot arguments can be used
 
         RETURN:
 
         """
         from siman.header import db
         from siman.dos_functions import plot_dos
+        from siman.picture_functions import plt
         # print(self.children)
 
 
         pm = kwargs
         x_nbins = pm.get('x_nbins')
         ylim = pm.get('ylim') or (-6,7)
         xlim = pm.get('xlim') or (-8,6)
@@ -1024,15 +1024,15 @@
         to_ang_local = 1
         
         # try:
         #     if "Ang" in self.len_units:
         #         to_ang_local = 1
         #         #print "units angs"
         # except AttributeError:
-        #     print_and_log("Warning! no len_units for "+self.name+" calculation, I use Bohr \n") 
+        #     printlog("Warning! no len_units for "+self.name+" calculation, I use Bohr \n") 
         
         N_from_kspacing = []
 
         it = self.id[0]
 
 
         if not hasattr(struct_des[it], 'ngkpt_dict_for_kspacings'): #compatibiliy issues
@@ -1054,15 +1054,15 @@
         # print (self.set.kpoints_file)
         # sys.exit()
         # printlog("Warning! If you use *update_set_dic* in add(), check_kpoints() works for set before update. Please fix.") #done
         if ngkpt:
             N = ngkpt
 
         elif is_string_like(self.set.kpoints_file):
-            print_and_log("External K-points file was provided", self.set.kpoints_file)
+            printlog("External K-points file was provided", self.set.kpoints_file)
             N = None
 
         elif kspacing in ngkpt_dict:
             N = ngkpt_dict[kspacing]
             printlog('check_kpoints(): k-points will be used from *ngkpt_dict* of',it, N)
         
         elif self.set.ngkpt:
@@ -1080,54 +1080,54 @@
         elif band_structure:
             printlog('check_kpoints(): the following path is used for band structure ',band_structure)
             N = None
         else:
             # print(self.dir)
             N = None
             if self.set.periodic:
-                print_and_log("Error! check_kpoints(): no information about k-points for periodic calculation\n")
+                printlog("Error! check_kpoints(): no information about k-points for periodic calculation\n")
 
 
 
         self.init.ngkpt = N
 
         if kspacing != None and kspacing not in ngkpt_dict:
             ngkpt_dict[kspacing] = N
             printlog('check_kpoints(): I added ',N,'as a k-grid for',kspacing,'in struct_des of', it)
 
 
-        print_and_log("check_kpoints(): Kpoint   mesh is: ", N, imp = 'Y')
+        printlog("check_kpoints(): Kpoint   mesh is: ", N, imp = 'Y')
 
 
         if not hasattr(struct_des[it], 'ngkpt_dict_for_kspacings') or  kspacing not in struct_des[it].ngkpt_dict_for_kspacings:
-            print_and_log('Several other options instead of automatically determined ngkpt = ',N,np.array(self.calc_kspacings(N) ).round(2), ':', end = '\n', imp = 'y')
-            print_and_log('ngkpt              |    actual kspacings       ', end = '\n', imp = 'y' )
+            printlog('Several other options instead of automatically determined ngkpt = ',N,np.array(self.calc_kspacings(N) ).round(2), ':', end = '\n', imp = 'y')
+            printlog('ngkpt              |    actual kspacings       ', end = '\n', imp = 'y' )
             
             if N:
                 for ngkpt in itertools.product([N[0]-1, N[0], N[0]+1], [N[1]-1, N[1], N[1]+1], [N[2]-1, N[2], N[2]+1]):
-                    print_and_log(ngkpt, np.array(self.calc_kspacings(ngkpt) ).round(2), end = '\n', imp = 'y' )
+                    printlog(ngkpt, np.array(self.calc_kspacings(ngkpt) ).round(2), end = '\n', imp = 'y' )
 
             # user_ngkpt = input('Provide ngkpt:')
             # print(user_ngkpt)
             # sys.exit()
 
         else:
-            print_and_log("check_kpoints(): The actual k-spacings are ", np.array(self.calc_kspacings(N) ).round(2), imp = 'Y')
+            printlog("check_kpoints(): The actual k-spacings are ", np.array(self.calc_kspacings(N) ).round(2), imp = 'Y')
         return N
 
 
     def calc_kspacings(self, ngkpt = None, sttype = 'init'):
         """Calculates reciprocal vectors and kspacing from ngkpt"""
         # to_ang_local = header.to_ang
         # try:
         #     if "Ang" in self.len_units:
         #         to_ang_local = 1
         #         #print "units angs"
         # except AttributeError:
-        #     print_and_log("Warning! no len_units for "+self.name+" calculation, I use Bohr \n")
+        #     printlog("Warning! no len_units for "+self.name+" calculation, I use Bohr \n")
         
 
         if sttype == 'init':
             st = self.init
         if sttype == 'end':
             st = self.end 
 
@@ -1178,23 +1178,23 @@
                 elif 'SGE' in cl.schedule_system:
                     job_in_queue = check_string in run_on_server("qstat -xml ", cl.cluster['address'])
                 
                 elif 'none' in cl.schedule_system:
                     job_in_queue = ''
 
                 elif 'simple' in cl.schedule_system:
-                    print_and_log('For SCHEDULE_SYSTEM='+cl.schedule_system+' please manually run on server! ', imp = 'y')                    
+                    printlog('For SCHEDULE_SYSTEM='+cl.schedule_system+' please manually run on server! ', imp = 'y')                    
 
 
                 else:
-                    print_and_log('Attention! unknown SCHEDULE_SYSTEM='+cl.schedule_system+'; Please teach me here! ', imp = 'y')
+                    printlog('Attention! unknown SCHEDULE_SYSTEM='+cl.schedule_system+'; Please teach me here! ', imp = 'y')
                     job_in_queue = ''
 
 
-            if file_exists_on_server(os.path.join(cl.dir, 'RUNNING'), addr = cl.cluster['address']) and job_in_queue: 
+            if file_exists_on_server(os.path.join(cl.project_path_cluster +'/'+cl.dir, 'RUNNING'), addr = cl.cluster['address']) and job_in_queue: 
                 
                 cl.state = '3. Running'
 
             elif job_in_queue:
                 
                 cl.state = '3. In queue'
```

### Comparing `siman-1.3.6/siman/core/calculation_old.py` & `siman-1.3.7/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/core/cluster_batch_script.py` & `siman-1.3.7/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/core/cluster_run_script.py` & `siman-1.3.7/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/core/molecule.py` & `siman-1.3.7/siman/core/molecule.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Distributed under the terms of the GNU License.
 import os
 
 from pymatgen.core.structure import Molecule as Molecule_pymatgen
 from siman import header
 from siman.inout import read_structure
 from siman.small_functions import makedir
-from siman.header import printlog, runBash, plt
+from siman.header import printlog, runBash
 
 class Molecule(Molecule_pymatgen):
     """Class for molecule structure representation based on pymatgen Molecule """
     
     @classmethod
     def cast(cls, some_a: Molecule_pymatgen, filename = None):
         """Cast  Molecule_pymatgen into MyA."""
```

### Comparing `siman-1.3.6/siman/core/structure.py` & `siman-1.3.7/siman/core/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,20 +35,17 @@
 if header.pymatgen_flag:
     from pymatgen.io.cif import CifWriter
     from pymatgen.symmetry.analyzer import SpacegroupAnalyzer
     from pymatgen.core.surface import Slab
     from pymatgen.core.composition import Composition
 
 
-# import matplotlib.pyplot as plt
 
 #siman packages
-
-from siman.header import printlog, print_and_log, runBash, plt
-
+from siman.header import printlog, runBash
 from siman import set_functions
 # from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.small_functions import return_xred, makedir, angle, is_string_like, cat_files, grep_file, red_prec, list2string, is_list_like, b2s, calc_ngkpt, setting_sshpass
 from siman.functions import (read_vectors, read_list, words, read_string,
      element_name_inv, invert, calculate_voronoi, 
     get_from_server, push_to_server, run_on_server, smoother, file_exists_on_server, check_output)
 from siman.geo import (image_distance, replic, calc_recip_vectors, calc_kspacings, xred2xcart, xcart2xred, 
@@ -1807,15 +1804,15 @@
         """
         Now can delete only one atom with number iat (int), starting from 0. 
         Takes care of magmom, ntypat, typat, znucl, nznucl, xred and natom
         Returns Structure()
         """
 
 
-        # print_and_log('Warning! Method del_atoms() was not carefully tested ')
+        # printlog('Warning! Method del_atoms() was not carefully tested ')
         st = copy.deepcopy(self)
         # print(st.nznucl)
 
         i = iat
 
         typ = st.typat[i]
 
@@ -1904,19 +1901,19 @@
         
         return st
 
 
     def leave_only(self, atom_type = None):
         #Remove all atoms except *atom_type*(str, mendeleev element name)
         
-        print_and_log('Starting leave_only()', imp = 'n')
+        printlog('Starting leave_only()', imp = 'n')
 
         st = copy.deepcopy(self)
         
-        print_and_log('    N of atoms before = ',st.natom, imp = 'n')
+        printlog('    N of atoms before = ',st.natom, imp = 'n')
 
 
         z = element_name_inv(atom_type)
 
         new_xred = []
         new_magmom = []
         
@@ -1945,15 +1942,15 @@
 
         st.nznucl = [st.natom,]
 
         st.xcart = xred2xcart(st.xred, st.rprimd)
 
         # print st.xred
 
-        print_and_log('    N of atoms after  = ',st.natom, imp = 'n')
+        printlog('    N of atoms after  = ',st.natom, imp = 'n')
 
 
         return st
 
 
     def get_numbers(self, element):
         "return numbers of specific element "
@@ -2252,15 +2249,15 @@
         #     for xr in st.xred:
         #         xr[2] = xr[2]-zmin
 
 
 
         st.xcart = xred2xcart(st.xred, st.rprimd)
 
-        # print_and_log(str(n)+" atoms were returned to cell.\n")
+        # printlog(str(n)+" atoms were returned to cell.\n")
         #print st.xred
         return st
 
 
 
 
 
@@ -3697,15 +3694,15 @@
 
             if selective_dynamics:
                 f.write("Selective dynamics\n")
 
 
 
             if "car" in coord_type:
-                print_and_log("Warning! Cartesian regime of coordination may be obsolete and incorrect !!!", imp = 'Y')
+                printlog("Warning! Cartesian regime of coordination may be obsolete and incorrect !!!", imp = 'Y')
                 f.write("Cartesian\n")
                 for xcart in zxcart:
                     for x in xcart:
                         f.write(str(x[0]*to_ang)+" "+str(x[1]*to_ang)+" "+str(x[2]*to_ang))
                         f.write("\n")
 
                 
@@ -3730,15 +3727,15 @@
             
 
 
             elif 'None' in coord_type:
                 pass
 
             else:
-                print_and_log("Error! The type of coordinates should be 'car' or 'dir' ")
+                printlog("Error! The type of coordinates should be 'car' or 'dir' ")
                 raise NameError
 
 
 
             # print('write_poscar(): predictor:\n', st.predictor)
             if hasattr(st, 'vel') and len(st.vel)>0:
                 printlog("Writing velocity to POSCAR ", imp = 'y')
@@ -3757,15 +3754,15 @@
 
         f.close()
         # if os.getcwd() not in filename:
         #     print('rep', str(os.getcwd()), filename)
         #     path = os.getcwd()+'/'+filename
         # else:
         path = filename
-        print_and_log("POSCAR was written to", path, imp = 'y')
+        printlog("POSCAR was written to", path, imp = 'y')
         return path
 
 
 
     def write_cif(self, filename = None, mcif = False, symprec = 0.1, write_prim = 0):
         """
         Find primitive cell and write it in cif format
```

### Comparing `siman-1.3.6/siman/database.py` & `siman-1.3.7/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/default_project_conf.py` & `siman-1.3.7/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/dev_functions.py` & `siman-1.3.7/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/dos_functions.py` & `siman-1.3.7/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/fit_hex.py` & `siman-1.3.7/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/functions.py` & `siman-1.3.7/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/geo.py` & `siman-1.3.7/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/header.py` & `siman-1.3.7/siman/header.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,16 @@
 # Copyright (c) Siman Development Team.
 # Distributed under the terms of the GNU License.
 
+
+# Warning! Do not add new global variables in this file. 
+# Instead create several dictionaries, which will contain all requied information!
+# Then gradually move all variables and constants to these dictionaries.
 import os, subprocess, sys, shelve
-try:
-    import matplotlib as mpl
-    """Global matplotlib control"""
-    # size = 22 #for one coloumn figures
-    size = 26 #for DOS
-    # size = 16 #for two coloumn figures
-    mpl.rc('font',family='Serif')
-    # mpl.rc('xtick', labelsize= size) 
-    # mpl.rc('ytick', labelsize= size) 
-    # mpl.rc('axes', labelsize = size) 
-    # mpl.rc('legend', fontsize= size) 
-    # mpl.rc('Axes.annotate', fontsize= size) #does not work
-    mpl.rcParams.update({'font.size': size})
-    mpl.rcParams.update({'mathtext.fontset': "stix"})
-    # plt.rcParams['mathtext.fontset'] = "stix"
-
-    #paths to libraries needed by siman
-    # sys.path.append('/home/dim/Simulation_wrapper/ase') #
-    # plt = None
-except:
-    mpl = None
-    plt = None
-    print('Warning! matplotlib is not installed! Some functions will not work!')
-
-try:
-    import matplotlib.pyplot as plt
-except:
-    plt = None
+
 
 
 
 history = []
 
 #Defaults to some project_conf values
 PBS_PROCS = False # if true than #PBS -l procs="+str(number_cores) is used
@@ -44,14 +21,17 @@
 # warnings = 'neyY'
 warnings = 'yY' # level of warnings to show: n - all, e - normal, y - important, Y - very important
 
 #Global constants, can be overriden in project_conf.py and simanrc.py
 FROM_ONE = None # atom numbering convention; allows to override the default behaviour of functions where atomic numbers are provided as arguments
 PATH2ARCHIVE_LOCAL  = None
 SAVE_CONTCAR = 1 # adds 's' to savefile argument alowing to move CONTCAR to 1.CONTCAR
+EXCLUDE_NODES = False
+MEM_CPU = None
+
 
 #Global variables
 final_vasp_clean     = True 
 clean_vasp_files     = []
 clean_vasp_files_ignore = []
 default_savefile = 'oc'
 copy_to_cluster_flag = True
@@ -63,62 +43,112 @@
 corenum = 1
 check_job = 1 # check job by additional ssh requests
 reorganize = 0 # use this from time to time to optimize database file size
 verbose_log = 0 # in addition to normal log write verbose log in any case by openning the log_verbose each time
 cluster_address = ''
 override_cluster_address = 0 # 1 or 0, override read calculations to header.CLUSTERS[cluster]['address'], usefull when switching between proxy and back of the same cluster
 pymatgen_flag = None
-
-
+open_terminal = False #used in runBash
+siman_run = False #
+calc_database = 'only_calc.gdbm3' # name for calculation database, db dict
 
 
 
 
 
 
 
 #1. Read default global settings for siman package
 from siman.default_project_conf import *
 
-#2. Read user-related settings for siman
-simanrc = os.path.expanduser("~/simanrc.py")
-if os.path.exists(simanrc):
-    # if 'n' in war
-    print(simanrc, 'was read')
-    sys.path.insert(0, os.path.dirname(simanrc))
-    from simanrc import *
+if 0:
+    #outdated code used before version 1.3.7
+    #2. Read user-related settings for siman
+    simanrc = os.path.expanduser("~/simanrc.py")
+    if os.path.exists(simanrc):
+        # if 'n' in war
+        print(simanrc, 'was read')
+        sys.path.insert(0, os.path.dirname(simanrc))
+        from simanrc import *
+
+    #3. Read project specific
+    if os.path.exists('./project_conf.py'):
+        print('Reading project_conf.py from', os.getcwd())
+
+        from project_conf import *
+        siman_run = True
+        log = open('log','a')
+    else:
+        print('Some module is used separately; default_project_conf.py is used')
+        if mpl and not os.path.exists(simanrc):
+            mpl.use('agg') #switch matplotlib on or off; for running script using ssh
+        siman_run = False
+        history.append('separate run')
+
 
-#3. Read project specific
-if os.path.exists('./project_conf.py'):
-    print('Reading project_conf.py from', os.getcwd())
 
-    from project_conf import *
-    siman_run = True
-    log = open('log','a')
-else:
-    print('Some module is used separately; default_project_conf.py is used')
-    if mpl and not os.path.exists(simanrc):
-        mpl.use('agg') #switch matplotlib on or off; for running script using ssh
-    siman_run = False
-    history.append('separate run')
 
+def _update_configuration(filename, pfolder = None):
+    """
+    A service function to update header parameters for specific user/project, such as provided in project_conf.py
+    or global parameters, such as provided in simanrc.py
 
 
+    INPUT:
+        - filename (str) - full path to the file with configuration parameters, such as simanrc.py or project_conf.py
+        - pfolder (str) - full path to a folder with specific project. 
+            Taken automatically from the *filename* if config file has a project_conf.py name
+            if simanrc.py is read, then not needed
+    """
+    from siman import header
+    global siman_run, project_folder
 
+    if pfolder:
+        project_folder = pfolder
+    elif 'project_conf.py' in filename:
+        project_folder = os.path.dirname(filename)
+    else:
+        pass
 
+    if project_folder:
+        siman_run = 1 # means that siman is used as an application to run tasks, not just a library
 
 
 
+    import importlib.util, sys
+    spec = importlib.util.spec_from_file_location('project_conf', filename)
+    project_conf = importlib.util.module_from_spec(spec)
+    spec.loader.exec_module(project_conf)
+    # print(dir(project_conf))
+    config_vars = ['CIF2CELL', 'DEFAULT_CLUSTER', 'EXCLUDE_NODES', 
+    'NEW_BATCH', 'PATH2ARCHIVE', 'PATH2DATABASE', 'PATH2JMOL', 'PATH2NEBMAKE', 
+    'PATH2PHONOPY', 'PATH2POTENTIALS', 'PATH2PROJECT', 'PBS_PROCS', 
+    'RAMDISK', 'SIMAN_WEB', 'WALLTIME_LIMIT', 
+    'geo_folder', 'path_to_images', 'path_to_paper', 
+    'path_to_wrapper', 'pmgkey', 'reorganize', 'CLUSTERS',]
+
+    for var in config_vars:
+        try: 
+            value = getattr(project_conf, var)
+            # print(type(value))
+            setattr(header, var, value)
+            # exec(var + " = " + str(value))
+        except AttributeError:
+            print('Warning! Your project_conf.py doesnot contain', var)
+            pass
+        # print(var, value)
+    # CLUSTERS = getattr(project_conf, 'CLUSTERS')
 
+    # print(CLUSTERS)
 
+    return
 
 
 
 
-calc_database = 'only_calc.gdbm3'
 
 class CalcDict(dict):
     def __getitem__(self, key):
         # print(self)
         if type(key) == str:
             # print('String key detected', key)
             key_str = key
@@ -180,15 +210,14 @@
 
 db = CalcDict()
 # global db
 calc = db
 conv = {};
 varset = {};
 struct_des = {};
-
 sets = varset
 
 
 
 
 
 #Constants
@@ -251,16 +280,14 @@
                     }
 
 el_dict = {'void':300, 'octa':200, 'n':0, 'H':1, 'He':2, 'Li':3, 'Be':4, 'B':5, 'C':6, 'N':7, 'O':8, 'F':9, 'Ne':10, 'Na':11, 'Mg':12, 'Al':13, 'Si':14, 'P':15, 'S':16, 'Cl':17, 'Ar':18, 'K':19, 'Ca':20, 'Sc':21, 'Ti':22, 'V':23, 'Cr':24, 'Mn':25, 'Fe':26, 'Co':27, 'Ni':28, 'Cu':29, 'Zn':30, 'Ga':31, 'Ge':32, 'As':33, 'Se':34, 'Br':35, 'Kr':36, 'Rb':37, 'Sr':38, 'Y':39, 'Zr':40, 'Nb':41, 'Mo':42, 'Tc':43, 'Ru':44, 'Rh':45, 'Pd':46, 'Ag':47, 'Cd':48, 'In':49, 'Sn':50, 'Sb':51, 'Te':52, 'I':53, 'Xe':54, 'Cs':55, 'Ba':56, 'La':57, 'Ce':58, 'Pr':59, 'Nd':60, 'Pm':61, 'Sm':62, 'Eu':63, 'Gd':64, 'Tb':65, 'Dy':66, 'Ho':67, 'Er':68, 'Tm':69, 'Yb':70, 'Lu':71, 'Hf':72, 'Ta':73, 'W':74, 'Re':75, 'Os':76, 'Ir':77, 'Pt':78, 'Au':79, 'Hg':80, 'Tl':81, 'Pb':82, 'Bi':83, 'Po':84, 'At':85, 'Rn':86, 'Fr':87, 'Ra':88, 'Ac':89, 'Th':90, 'Pa':91, 'U':92, 'Np':93, 'Pu':94, 'Am':95, 'Cm':96, 'Bk':97, 'Cf':98, 'Es':99, 'Fm':100, 'Md':101, 'No':102, 'Lr':103, 'Rf':104, 'Db':105, 'Sg':106, 'Bh':107, 'Hs':108, 'Mt':109, 'Ds':110, 'Rg':111, 'Cn':112, 'Uuq':114, 'Uuh':116, }
 nu_dict = {300:'void', 200:'octa', 0:'n', 1:'H', 2:'He', 3:'Li', 4:'Be', 5:'B', 6:'C', 7:'N', 8:'O', 9:'F', 10:'Ne', 11:'Na', 12:'Mg', 13:'Al', 14:'Si', 15:'P', 16:'S', 17:'Cl', 18:'Ar', 19:'K', 20:'Ca', 21:'Sc', 22:'Ti', 23:'V', 24:'Cr', 25:'Mn', 26:'Fe', 27:'Co', 28:'Ni', 29:'Cu', 30:'Zn', 31:'Ga', 32:'Ge', 33:'As', 34:'Se', 35:'Br', 36:'Kr', 37:'Rb', 38:'Sr', 39:'Y', 40:'Zr', 41:'Nb', 42:'Mo', 43:'Tc', 44:'Ru', 45:'Rh', 46:'Pd', 47:'Ag', 48:'Cd', 49:'In', 50:'Sn', 51:'Sb', 52:'Te', 53:'I', 54:'Xe', 55:'Cs', 56:'Ba', 57:'La', 58:'Ce', 59:'Pr', 60:'Nd', 61:'Pm', 62:'Sm', 63:'Eu', 64:'Gd', 65:'Tb', 66:'Dy', 67:'Ho', 68:'Er', 69:'Tm', 70:'Yb', 71:'Lu', 72:'Hf', 73:'Ta', 74:'W', 75:'Re', 76:'Os', 77:'Ir', 78:'Pt', 79:'Au', 80:'Hg', 81:'Tl', 82:'Pb', 83:'Bi', 84:'Po', 85:'At', 86:'Rn', 87:'Fr', 88:'Ra', 89:'Ac', 90:'Th', 91:'Pa', 92:'U', 93:'Np', 94:'Pu', 95:'Am', 96:'Cm', 97:'Bk', 98:'Cf', 99:'Es', 100:'Fm', 101:'Md', 102:'No', 103:'Lr', 104:'Rf', 105:'Db', 106:'Sg', 107:'Bh', 108:'Hs', 109:'Mt', 110:'Ds', 111:'Rg', 112:'Cn', 114:'Uuq', 116:'Uuh', }
 #void 300 is not written to poscar
 nme_list = ['H', 'He', 'B', 'C', 'N', 'O', 'F', 'Ne', 'Si', 'P', 'S', 'Cl', 'Ar', 'As', 'Se', 'Br', 'Kr', 'Te', 'I', 'Xe', 'At', 'Rn', 'Ts', 'Og']
 
-EXCLUDE_NODES = False
-MEM_CPU = None
 
 
 def printlog(*logstrings, **argdic):
     """
     '' - silent
     e - errors and warnings
     a - attentions
@@ -268,14 +295,16 @@
     M - maximalistic output of scientific procedures  
     debug_level importance:
         'n' - not important at all - for debugging
         ''  - almost all actions, no flag is needed
         'y' - important - major actions
         'Y' - super important, or output asked by user
     """
+    
+    global siman_run
     end = '\n\n'# no argument for end, make one separate line
     
     debug_level  = 'e' #empty
     for key in argdic:
         if 'imp' in key:
             debug_level = argdic[key]
         
@@ -313,31 +342,32 @@
     #     # print(debug_level)
     #     if 'n' in debug_level and 'n' not in warnings:
     #         pass
     #     else:
     #         print (mystring,  end = "")
 
     if siman_run:
-        log.write(mystring)
+        with open(project_folder+'/log','a') as log:
+            log.write(mystring)
     
     if verbose_log:
-        with open('verbose_log','a') as f:
+        with open(project_folder+'/verbose_log','a') as f:
             f.write(mystring)
 
 
     if 'Error!' in mystring:
         print (mystring)
         print ('Error! keyword was detected in message; invoking RuntimeError ')
         sys.exit()
         # raise RuntimeError
 
     return
 
 print_and_log = printlog
-open_terminal = False
+
 
 
 def runBash(cmd, env = None, detached = False, cwd = None):
     """Input - string; Executes Bash commands and returns stdout
 Need: import subprocess
     """
     global open_terminal
```

### Comparing `siman-1.3.6/siman/impurity.py` & `siman-1.3.7/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/inout.py` & `siman-1.3.7/siman/inout.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     from tabulate import tabulate 
 except:
     print('inout.py: Cant import tabulate')
 
 
 
 from siman import header
-from siman.header import printlog,printlog, runBash, plt
+from siman.header import printlog, runBash
 # from siman.calc_manage import cif2poscar
 from siman.functions import element_name_inv, unique_elements, smoother
 from siman.small_functions import makedir, is_list_like, list2string, red_prec
 from siman.small_classes import empty_struct
 from siman.geo import local_surrounding, replic
 try:
     # pmg config --add VASP_PSP_DIR $VASP_PSP_DIR MAPI_KEY $MAPI_KEY
@@ -1250,14 +1250,16 @@
                 f.write('initial_moment '+str(mag)+'\n') 
 
 
 
 def read_vasp_out(cl, load = '', out_type = '', show = '', voronoi = '', path_to_outcar = '', path_to_contcar = '', ):
     """Try to read xred from CONCAR and calculate xcart"""
 
+    from siman.picture_functions import plt
+
     self = cl
 
     printlog('Path to CONTCAR', path_to_contcar)
     if os.path.exists(path_to_contcar):
         contcar_exist   = True
     else:
         contcar_exist   = False
```

### Comparing `siman-1.3.6/siman/kpoints_functions.py` & `siman-1.3.7/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/mat_prop/mat_prop.py` & `siman-1.3.7/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/matproj_functions.py` & `siman-1.3.7/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/monte.py` & `siman-1.3.7/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/monte_functions.py` & `siman-1.3.7/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/neb.py` & `siman-1.3.7/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/pairs.py` & `siman-1.3.7/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/picture_functions.py` & `siman-1.3.7/siman/picture_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,61 @@
     print('picture_functions.py: scipy is not avail')
 # from scipy.interpolate import spline 
 try:
     ''
     from scipy.interpolate import  CubicSpline
 except:
     print('scipy.interpolate.CubicSpline is not avail')
+
+
+
+
+try:
+    import matplotlib as mpl
+    """Global matplotlib control"""
+    # size = 22 #for one coloumn figures
+    size = 26 #for DOS
+    # size = 16 #for two coloumn figures
+    mpl.rc('font',family='Serif')
+    # mpl.rc('xtick', labelsize= size) 
+    # mpl.rc('ytick', labelsize= size) 
+    # mpl.rc('axes', labelsize = size) 
+    # mpl.rc('legend', fontsize= size) 
+    # mpl.rc('Axes.annotate', fontsize= size) #does not work
+    mpl.rcParams.update({'font.size': size})
+    mpl.rcParams.update({'mathtext.fontset': "stix"})
+    # plt.rcParams['mathtext.fontset'] = "stix"
+
+    #paths to libraries needed by siman
+    # sys.path.append('/home/dim/Simulation_wrapper/ase') #
+    # plt = None
+except:
+    mpl = None
+    plt = None
+    print('Warning! matplotlib is not installed! Some functions will not work!')
+
+try:
+    import matplotlib.pyplot as plt
+except:
+    plt = None
+
+
+
+
+
+
 try:
     from mpl_toolkits.mplot3d import Axes3D
     import matplotlib.pyplot as plt
     import matplotlib
     # matplotlib.use('tkagg')
+    from matplotlib import gridspec 
 except:
     print('mpl_toolkits or matplotlib are not avail')
 
-from matplotlib import gridspec 
 try:
     from adjustText import adjust_text
     adjustText_installed = True
 except:
     adjustText_installed = False
```

### Comparing `siman-1.3.6/siman/plot_functions.py` & `siman-1.3.7/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/polaron.py` & `siman-1.3.7/siman/polaron.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/polaron_hop.py` & `siman-1.3.7/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/polaron_mod.py` & `siman-1.3.7/siman/polaron_mod.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/project_funcs.py` & `siman-1.3.7/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/properties_2d.py` & `siman-1.3.7/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/properties_energy.py` & `siman-1.3.7/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/properties_lattice.py` & `siman-1.3.7/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/set_functions.py` & `siman-1.3.7/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/simanrc.py` & `siman-1.3.7/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/small_functions.py` & `siman-1.3.7/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/structure_functions.py` & `siman-1.3.7/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/table_functions.py` & `siman-1.3.7/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/thermo.py` & `siman-1.3.7/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman/workflow_utilities.py` & `siman-1.3.7/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.3.6/siman.egg-info/PKG-INFO` & `siman-1.3.7/siman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.3.6
+Version: 1.3.7
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.3.6/siman.egg-info/SOURCES.txt` & `siman-1.3.7/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

