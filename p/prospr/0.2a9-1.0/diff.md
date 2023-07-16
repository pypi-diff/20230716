# Comparing `tmp/prospr-0.2a9.tar.gz` & `tmp/prospr-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prospr-0.2a9.tar", last modified: Mon Nov 14 17:29:55 2022, max compression
+gzip compressed data, was "prospr-1.0.tar", last modified: Sun Jul 16 09:52:19 2023, max compression
```

## Comparing `prospr-0.2a9.tar` & `prospr-1.0.tar`

### file list

```diff
@@ -1,63 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.483569 prospr-0.2a9/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-14 17:29:39.000000 prospr-0.2a9/COPYING.LESSER
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-11-14 17:29:39.000000 prospr-0.2a9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-11-14 17:29:55.479569 prospr-0.2a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3093 2022-11-14 17:29:39.000000 prospr-0.2a9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.471568 prospr-0.2a9/prospr/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.471568 prospr-0.2a9/prospr/core/
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/core/core_module.cpp
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.467568 prospr-0.2a9/prospr/data/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.475568 prospr-0.2a9/prospr/data/vanEck1000/
--rw-r--r--   0 runner    (1001) docker     (121)    14902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP10.csv
--rw-r--r--   0 runner    (1001) docker     (121)   104902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP100.csv
--rw-r--r--   0 runner    (1001) docker     (121)    19902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP15.csv
--rw-r--r--   0 runner    (1001) docker     (121)    24902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP20.csv
--rw-r--r--   0 runner    (1001) docker     (121)    29902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP25.csv
--rw-r--r--   0 runner    (1001) docker     (121)    34902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP30.csv
--rw-r--r--   0 runner    (1001) docker     (121)    39902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP35.csv
--rw-r--r--   0 runner    (1001) docker     (121)    44902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP40.csv
--rw-r--r--   0 runner    (1001) docker     (121)    49902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP45.csv
--rw-r--r--   0 runner    (1001) docker     (121)    54902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP50.csv
--rw-r--r--   0 runner    (1001) docker     (121)    59902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP55.csv
--rw-r--r--   0 runner    (1001) docker     (121)    64902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP60.csv
--rw-r--r--   0 runner    (1001) docker     (121)    69902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP65.csv
--rw-r--r--   0 runner    (1001) docker     (121)    74902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP70.csv
--rw-r--r--   0 runner    (1001) docker     (121)    79902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP75.csv
--rw-r--r--   0 runner    (1001) docker     (121)    84902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP80.csv
--rw-r--r--   0 runner    (1001) docker     (121)    89902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP85.csv
--rw-r--r--   0 runner    (1001) docker     (121)    94902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP90.csv
--rw-r--r--   0 runner    (1001) docker     (121)    99902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck1000/HP95.csv
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.479569 prospr-0.2a9/prospr/data/vanEck250/
--rw-r--r--   0 runner    (1001) docker     (121)     3652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP10.csv
--rw-r--r--   0 runner    (1001) docker     (121)    26152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP100.csv
--rw-r--r--   0 runner    (1001) docker     (121)     4902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP15.csv
--rw-r--r--   0 runner    (1001) docker     (121)     6152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP20.csv
--rw-r--r--   0 runner    (1001) docker     (121)     7402 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP25.csv
--rw-r--r--   0 runner    (1001) docker     (121)     8652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP30.csv
--rw-r--r--   0 runner    (1001) docker     (121)     9902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP35.csv
--rw-r--r--   0 runner    (1001) docker     (121)    11152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP40.csv
--rw-r--r--   0 runner    (1001) docker     (121)    12402 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP45.csv
--rw-r--r--   0 runner    (1001) docker     (121)    13652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP50.csv
--rw-r--r--   0 runner    (1001) docker     (121)    14902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP55.csv
--rw-r--r--   0 runner    (1001) docker     (121)    16152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP60.csv
--rw-r--r--   0 runner    (1001) docker     (121)    17402 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP65.csv
--rw-r--r--   0 runner    (1001) docker     (121)    18652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP70.csv
--rw-r--r--   0 runner    (1001) docker     (121)    19902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP75.csv
--rw-r--r--   0 runner    (1001) docker     (121)    21152 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP80.csv
--rw-r--r--   0 runner    (1001) docker     (121)    22402 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP85.csv
--rw-r--r--   0 runner    (1001) docker     (121)    23652 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP90.csv
--rw-r--r--   0 runner    (1001) docker     (121)    24902 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/data/vanEck250/HP95.csv
--rw-r--r--   0 runner    (1001) docker     (121)      861 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3274 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)    10318 2022-11-14 17:29:39.000000 prospr-0.2a9/prospr/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 17:29:55.471568 prospr-0.2a9/prospr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-14 17:29:55.000000 prospr-0.2a9/prospr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-14 17:29:39.000000 prospr-0.2a9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 17:29:55.483569 prospr-0.2a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2015 2022-11-14 17:29:39.000000 prospr-0.2a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.140101 prospr-1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-16 09:52:05.000000 prospr-1.0/COPYING.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-16 09:52:05.000000 prospr-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-07-16 09:52:19.140101 prospr-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-07-16 09:52:05.000000 prospr-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.124100 prospr-1.0/prospr/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-16 09:52:05.000000 prospr-1.0/prospr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-16 09:52:05.000000 prospr-1.0/prospr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.124100 prospr-1.0/prospr/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/core_module.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.128100 prospr-1.0/prospr/core/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/amino_acid.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/amino_acid.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/beam_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/beam_search.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/depth_first.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/depth_first.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/depth_first_bnb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/depth_first_bnb.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15007 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/protein.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3786 2023-07-16 09:52:05.000000 prospr-1.0/prospr/core/src/protein.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.124100 prospr-1.0/prospr/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.128100 prospr-1.0/prospr/data/vanEck1000/
+-rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   104902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP15.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    29902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    34902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP30.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    39902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP35.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP40.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    49902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP45.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    54902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP50.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    59902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP55.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    64902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP60.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    69902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP65.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    74902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP70.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    79902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP75.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    84902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP80.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    89902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP85.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    94902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP90.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    99902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck1000/HP95.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.132100 prospr-1.0/prospr/data/vanEck250/
+-rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP10.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26152 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP100.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP15.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP20.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP25.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP30.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP35.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP40.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    12402 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP45.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13652 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP50.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP55.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    16152 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP60.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    17402 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP65.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    18652 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP70.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    19902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP75.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21152 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP80.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22402 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP85.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    23652 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP90.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24902 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck250/HP95.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.140101 prospr-1.0/prospr/data/vanEck_hratio/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r0.9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP10_r1.0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21078 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21561 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21309 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21477 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    22317 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     9862 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r0.9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP15_r1.0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26514 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    24928 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    25864 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26176 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    26384 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    28802 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r0.9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP20_r1.0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     8932 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30429 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38427 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38179 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35389 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    40287 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35110 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    43852 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    38861 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r0.9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP25_r1.0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    35586 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.1.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    51786 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.2.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44262 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.3.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41742 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.4.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41814 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.5.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    41202 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.6.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    44046 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.7.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    47070 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    36054 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r0.9.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-16 09:52:05.000000 prospr-1.0/prospr/data/vanEck_hratio/HP30_r1.0.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-16 09:52:05.000000 prospr-1.0/prospr/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-07-16 09:52:05.000000 prospr-1.0/prospr/gen_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-07-16 09:52:05.000000 prospr-1.0/prospr/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-07-16 09:52:05.000000 prospr-1.0/prospr/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 09:52:19.124100 prospr-1.0/prospr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-07-16 09:52:19.000000 prospr-1.0/prospr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-07-16 09:52:19.000000 prospr-1.0/prospr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:52:19.000000 prospr-1.0/prospr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 09:52:18.000000 prospr-1.0/prospr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 09:52:19.000000 prospr-1.0/prospr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-16 09:52:05.000000 prospr-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 09:52:19.140101 prospr-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-16 09:52:05.000000 prospr-1.0/setup.py
```

### Comparing `prospr-0.2a9/COPYING.LESSER` & `prospr-1.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/LICENSE` & `prospr-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/PKG-INFO` & `prospr-1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,21 @@
-Metadata-Version: 2.1
-Name: prospr
-Version: 0.2a9
-Summary: A toolbox for protein folding with Python.
-Home-page: https://github.com/okkevaneck/prospr
-Author: okkevaneck
-License: LGPLv3
-Keywords: prospr protein structure prediction toolbox python c++ swig cmake extension heuristics pypi package
-Platform: any
-Classifier: Programming Language :: Python :: 3
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: COPYING.LESSER
-
 ## Prospr: The Protein Structure Prediction Toolbox
 <p align="center">
     <img src="docs/source/_static/prospr_logo.png" alt="Prospr's logo" width="496" height="308">  
 </p>
+<div align="center">
 
 ![GitHub](https://img.shields.io/github/license/OkkeVanEck/prospr)
 ![GitHub release (latest by date including pre-releases)](https://img.shields.io/github/v/release/OkkeVanEck/prospr?include_prereleases)
-![GitHub Workflow Status (branch)](https://img.shields.io/github/workflow/status/OkkeVanEck/prospr/CI-CD/master)
+![GitHub Workflow Status (branch)](https://img.shields.io/github/actions/workflow/status/OkkeVanEck/prospr/.github/workflows/build_deploy.yml?branch=master)
 [![Documentation Status](https://readthedocs.org/projects/prospr/badge/?version=latest)](https://prospr.readthedocs.io/en/latest/?badge=latest)
-[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)  
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+
+</div>
+
 **Creator:** Okke van Eck
 
 Prospr is a universal toolbox for protein structure prediction within the
 HP-model.
 At the core, Prospr offers an easy-to-use Protein data structure, which can be
 used to simulate protein folding.
 It also offers algorithms, datasets and visualization functions.
```

### Comparing `prospr-0.2a9/prospr/core/core_module.cpp` & `prospr-1.0/prospr/core/core_module.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,93 @@
 /* File:            core_module.cpp
  * Description:     Source file defining the pybind11 interfaces for exporting
  *                  the c++ core to a Python interface.
  * License:         This file is licensed under the GNU LGPL V3 license by
- *                  Okke van Eck (2020 - 2022). See the LICENSE file for the
+ *                  Okke van Eck (2020 - 2023). See the LICENSE file for the
  *                  specifics.
  */
 
 #include <pybind11/pybind11.h>
 #include <pybind11/stl.h>
 namespace py = pybind11;
 
 #include "src/amino_acid.cpp"
-#include "src/protein.cpp"
+#include "src/beam_search.cpp"
 #include "src/depth_first.cpp"
 #include "src/depth_first_bnb.cpp"
-
+#include "src/protein.cpp"
 
 PYBIND11_MODULE(prospr_core, m) {
-    m.doc() = "Prospr core written in C++.";
+  m.doc() = "Prospr core written in C++.";
 
-    /* AminoAcid class definition. */
-    py::class_<AminoAcid>(m, "AminoAcid")
-        .def(py::init<char, int , int, int &>(),
-                "AminoAcid constructor", py::arg("type"), py::arg("index"),
-                py::arg("prev_move")=0, py::arg("next_move")=0)
-        .def_property_readonly("type", &AminoAcid::get_type)
-        .def_property_readonly("index", &AminoAcid::get_index)
-        .def_property_readonly("prev_move", &AminoAcid::get_prev_move)
-        .def_property_readonly("next_move", &AminoAcid::get_next_move)
-    ;
-
-    /* Definition for bond_values as default parameter value. */
-    std::map<std::string, int> bond_values_cpp = {};
-    py::object bond_values = py::cast(bond_values_cpp);
-
-    /* Protein class definition. */
-    py::class_<Protein>(m, "Protein")
-        .def(py::init<const std::string, int, const std::string,
-                std::map<std::string, int>, bool &>(),
-                "Protein constructor", py::arg("sequence"), py::arg("dim")=2,
-                py::arg("model")="HP", py::arg("bond_values")=bond_values,
-                py::arg("bond_symmetry")=true)
-        .def_property_readonly("solutions_checked",
-            &Protein::get_solutions_checked)
-        .def_property_readonly("aminos_placed",
-            &Protein::get_aminos_placed)
-        .def_property_readonly("cur_len", &Protein::get_cur_len)
-        .def_property_readonly("dim", &Protein::get_dim)
-        .def_property_readonly("bond_values", &Protein::get_bond_values)
-        .def_property_readonly("last_move", &Protein::get_last_move)
-        .def_property_readonly("last_pos", &Protein::get_last_pos)
-        .def_property_readonly("score", &Protein::get_score)
-        .def_property_readonly("sequence", &Protein::get_sequence)
-        .def_property_readonly("max_weights", &Protein::get_max_weights)
-
-        .def("get_amino", &Protein::get_amino,
-            "Get amino index and next direction from amino at given position",
-            py::arg("position"))
-        .def("is_weighted", &Protein::is_weighted,
-            "Check if the amino acid at index is weighted", py::arg("index"))
-        .def("reset", &Protein::reset, "Reset the whole protein")
-        .def("reset_conformation", &Protein::reset_conformation,
-            "Reset only the conformation of the protein, not the statistics")
-        .def("is_valid", &Protein::is_valid, "Check if a given move is valid",
-            py::arg("move"))
-        .def("place_amino", &Protein::place_amino,
-            "Place a protein in a given direction", py::arg("move"),
-            py::arg("track")=true)
-        .def("remove_amino", &Protein::remove_amino,
-            "Remove the last placed amino")
-        .def("hash_fold", &Protein::hash_fold,
-            "Process the current conformation into a sequence of moves")
-        .def("set_hash", &Protein::set_hash,
-            "Set the conformation to the given sequence of moves",
-            py::arg("fold_hash"), py::arg("track")=false)
-    ;
+  /* AminoAcid class definition. */
+  py::class_<AminoAcid>(m, "AminoAcid")
+      .def(py::init<char, int, int, int &>(), "AminoAcid constructor",
+           py::arg("type"), py::arg("index"), py::arg("prev_move") = 0,
+           py::arg("next_move") = 0)
+      .def_property_readonly("type", &AminoAcid::get_type)
+      .def_property_readonly("index", &AminoAcid::get_index)
+      .def_property_readonly("prev_move", &AminoAcid::get_prev_move)
+      .def_property_readonly("next_move", &AminoAcid::get_next_move);
+
+  /* Definition for bond_values as default parameter value. */
+  std::map<std::string, int> bond_values_cpp = {};
+  py::object bond_values = py::cast(bond_values_cpp);
+
+  /* Protein class definition. */
+  py::class_<Protein>(m, "Protein")
+      .def(py::init<const std::string, int, const std::string,
+                    std::map<std::string, int>, bool &>(),
+           "Protein constructor", py::arg("sequence"), py::arg("dim") = 2,
+           py::arg("model") = "HP", py::arg("bond_values") = bond_values,
+           py::arg("bond_symmetry") = true)
+      .def_property_readonly("solutions_checked",
+                             &Protein::get_solutions_checked)
+      .def_property_readonly("aminos_placed", &Protein::get_aminos_placed)
+      .def_property_readonly("cur_len", &Protein::get_cur_len)
+      .def_property_readonly("dim", &Protein::get_dim)
+      .def_property_readonly("bond_values", &Protein::get_bond_values)
+      .def_property_readonly("last_move", &Protein::get_last_move)
+      .def_property_readonly("last_pos", &Protein::get_last_pos)
+      .def_property_readonly("score", &Protein::get_score)
+      .def_property_readonly("sequence", &Protein::get_sequence)
+      .def_property_readonly("max_weights", &Protein::get_max_weights)
+
+      .def("get_amino", &Protein::get_amino,
+           "Get amino index and next direction from amino at given position",
+           py::arg("position"), py::return_value_policy::reference_internal)
+      .def("is_weighted", &Protein::is_weighted,
+           "Check if the amino acid at index is weighted", py::arg("index"))
+      .def("reset", &Protein::reset, "Reset the whole protein")
+      .def("reset_conformation", &Protein::reset_conformation,
+           "Reset only the conformation of the protein, not the statistics")
+      .def("is_valid", &Protein::is_valid, "Check if a given move is valid",
+           py::arg("move"))
+      .def("place_amino", &Protein::place_amino,
+           "Place a protein in a given direction", py::arg("move"),
+           py::arg("track") = true)
+      .def("remove_amino", &Protein::remove_amino,
+           "Remove the last placed amino")
+      .def("hash_fold", &Protein::hash_fold,
+           "Process the current conformation into a sequence of moves")
+      .def("set_hash", &Protein::set_hash,
+           "Set the conformation to the given sequence of moves",
+           py::arg("fold_hash"), py::arg("track") = false)
+      .def("get_bonds", &Protein::get_bonds, py::return_value_policy::copy,
+           "Return list of amino acid indexes forming bonds");
 
-    /* Depth-first search function definition. */
-    m.def("depth_first", depth_first,
+  /* Depth-first search function definition. */
+  m.def("depth_first", depth_first,
         "Finds the optimal conformation via depth-first search",
         py::arg("protein"));
 
-    /* Depth-first branch-and-bound search function definition. */
-    m.def("depth_first_bnb", depth_first_bnb,
-        "Finds the optimal conformation via depth-first branch-and-bound search",
-        py::arg("protein"));
+  /* Depth-first branch-and-bound search function definition. */
+  m.def("depth_first_bnb", depth_first_bnb,
+        "Finds the optimal conformation via depth-first branch-and-bound "
+        "search",
+        py::arg("protein"), py::arg("prune_func") = "");
+
+  /* Beam search function definition. */
+  m.def("beam_search", beam_search,
+        "Finds a best-effort conformation via beam search", py::arg("protein"),
+        py::arg("beam_width") = -1);
 }
```

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP10.csv` & `prospr-1.0/prospr/data/vanEck1000/HP10.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP100.csv` & `prospr-1.0/prospr/data/vanEck1000/HP100.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP15.csv` & `prospr-1.0/prospr/data/vanEck1000/HP15.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP20.csv` & `prospr-1.0/prospr/data/vanEck1000/HP20.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP25.csv` & `prospr-1.0/prospr/data/vanEck1000/HP25.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP30.csv` & `prospr-1.0/prospr/data/vanEck1000/HP30.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP35.csv` & `prospr-1.0/prospr/data/vanEck1000/HP35.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP40.csv` & `prospr-1.0/prospr/data/vanEck1000/HP40.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP45.csv` & `prospr-1.0/prospr/data/vanEck1000/HP45.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP50.csv` & `prospr-1.0/prospr/data/vanEck1000/HP50.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP55.csv` & `prospr-1.0/prospr/data/vanEck1000/HP55.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP60.csv` & `prospr-1.0/prospr/data/vanEck1000/HP60.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP65.csv` & `prospr-1.0/prospr/data/vanEck1000/HP65.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP70.csv` & `prospr-1.0/prospr/data/vanEck1000/HP70.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP75.csv` & `prospr-1.0/prospr/data/vanEck1000/HP75.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP80.csv` & `prospr-1.0/prospr/data/vanEck1000/HP80.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP85.csv` & `prospr-1.0/prospr/data/vanEck1000/HP85.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP90.csv` & `prospr-1.0/prospr/data/vanEck1000/HP90.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck1000/HP95.csv` & `prospr-1.0/prospr/data/vanEck1000/HP95.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP10.csv` & `prospr-1.0/prospr/data/vanEck250/HP10.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP100.csv` & `prospr-1.0/prospr/data/vanEck250/HP100.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP15.csv` & `prospr-1.0/prospr/data/vanEck250/HP15.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP20.csv` & `prospr-1.0/prospr/data/vanEck250/HP20.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP25.csv` & `prospr-1.0/prospr/data/vanEck250/HP25.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP30.csv` & `prospr-1.0/prospr/data/vanEck250/HP30.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP35.csv` & `prospr-1.0/prospr/data/vanEck250/HP35.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP40.csv` & `prospr-1.0/prospr/data/vanEck250/HP40.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP45.csv` & `prospr-1.0/prospr/data/vanEck250/HP45.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP50.csv` & `prospr-1.0/prospr/data/vanEck250/HP50.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP55.csv` & `prospr-1.0/prospr/data/vanEck250/HP55.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP60.csv` & `prospr-1.0/prospr/data/vanEck250/HP60.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP65.csv` & `prospr-1.0/prospr/data/vanEck250/HP65.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP70.csv` & `prospr-1.0/prospr/data/vanEck250/HP70.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP75.csv` & `prospr-1.0/prospr/data/vanEck250/HP75.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP80.csv` & `prospr-1.0/prospr/data/vanEck250/HP80.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP85.csv` & `prospr-1.0/prospr/data/vanEck250/HP85.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP90.csv` & `prospr-1.0/prospr/data/vanEck250/HP90.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/data/vanEck250/HP95.csv` & `prospr-1.0/prospr/data/vanEck250/HP95.csv`

 * *Files identical despite different names*

### Comparing `prospr-0.2a9/prospr/datasets.py` & `prospr-1.0/prospr/datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 #!/usr/bin/env python3
 """
-File:           vanEck.py
+File:           datasets.py
 Description:    This file contains functions for loading datasets.
 License:        This file is licensed under the GNU LGPL V3 license by
-                Okke van Eck (2020 - 2022). See the LICENSE file for the
+                Okke van Eck (2020 - 2023). See the LICENSE file for the
                 specifics.
 """
 
-import pkg_resources
 import pandas as pd
 
 
 def _load_dataset(folder, filename):
     """Returns a specified dataset as a dataframe."""
-    stream = pkg_resources.resource_stream(
-        "prospr", f"data/{folder}/{filename}"
-    )
-    return pd.read_csv(stream)
+    return pd.read_csv(f"prospr/data/{folder}/{filename}")
 
 
 def load_vanEck250(length=10):
     """Returns a vanEck250 dataset as a pandas dataframe."""
     return _load_dataset("vanEck250", f"HP{length}.csv")
 
 
 def load_vanEck1000(length=10):
-    """Returns a vanEck250 dataset as a pandas dataframe."""
+    """Returns a vanEck1000 dataset as a pandas dataframe."""
     return _load_dataset("vanEck1000", f"HP{length}.csv")
+
+
+def load_vanEck_hratio(length=25, hratio=0.1):
+    """Returns a vanEck_hratio dataset as a pandas dataframe."""
+    return _load_dataset("vanEck_hratio", f"HP{length}_r{hratio}.csv")
```

### Comparing `prospr-0.2a9/prospr/helpers.py` & `prospr-1.0/prospr/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 """
 File:           helpers.py
 Description:    This file contains helper functions for a Protein instance.
 License:        This file is licensed under the GNU LGPL V3 license by
-                Okke van Eck (2020 - 2022). See the LICENSE file for the
+                Okke van Eck (2020 - 2023). See the LICENSE file for the
                 specifics.
 """
 
 import numpy as np
 
 
 def get_scoring_aminos(protein):
```

### Comparing `prospr-0.2a9/prospr/visualize.py` & `prospr-1.0/prospr/visualize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 """
 File:           visualize.py
 Description:    This file contains functions for visualizing a Protein
                 instance.
 License:        This file is licensed under the GNU LGPL V3 license by
-                Okke van Eck (2020 - 2022). See the LICENSE file for the
+                Okke van Eck (2020 - 2023). See the LICENSE file for the
                 specifics.
 """
 
 from .helpers import get_ordered_positions, get_scoring_pairs
 
 from matplotlib import pyplot as plt
 from matplotlib.ticker import MaxNLocator
@@ -50,87 +50,100 @@
             color="indianred",
             alpha=0.9,
             zorder=1,
             lw=2,
         )
 
 
-def _plot_aminos_2d_paper(protein, df, ax):
+def _plot_aminos_2d_paper(
+    protein, df, ax, linewidth, markersize, annotate_first=False
+):
     """
     Plot amino acids in paper style in a 2D figure.
     :param Protein      protein:    Protein object to plot the hash of.
     :param DataFrame    df:         DataFrame with all ordered positions.
     :param Axes         ax:         Axis to plot on.
+    :param float        linewidth:      Width of the lines.
+    :param float        markersize:     Size of the markers.
     """
     # Split dataframe on amino acid type.
     df_H = df.loc[df["Type"] == "H"]
     df_P = df.loc[df["Type"] == "P"]
 
-    ax.plot(df["x"], df["y"], color="black", alpha=0.65, zorder=1)
+    ax.plot(
+        df["x"],
+        df["y"],
+        color="black",
+        alpha=0.65,
+        linewidth=linewidth,
+        zorder=1,
+    )
     sns.scatterplot(
         x="x",
         y="y",
         data=df_H,
         marker="o",
         edgecolor="royalblue",
-        s=80,
+        s=markersize,
         zorder=2,
         ax=ax,
         label="H",
     )
     sns.scatterplot(
         x="x",
         y="y",
         data=df_P,
         marker="o",
         facecolor="white",
         edgecolor="orange",
-        linewidth=2,
-        s=80,
+        linewidth=2.5,
+        s=markersize,
         zorder=2,
         ax=ax,
         label="P",
     )
 
-    # Plot first point with a different color.
-    if df.iloc[0]["Type"] == "H":
-        ax.scatter(
-            df.iloc[0]["x"],
-            df.iloc[0]["y"],
-            marker="o",
-            fc="royalblue",
-            ec="#00ce00",
-            lw=2.5,
-            s=80,
-            zorder=2,
-        )
-    else:
-        ax.scatter(
-            df.iloc[0]["x"],
-            df.iloc[0]["y"],
-            marker="o",
-            fc="white",
-            ec="#00ce00",
-            lw=2.5,
-            s=80,
-            zorder=2,
-        )
+    # Plot first point with a green edge color.
+    if annotate_first:
+        # Plot first point with a different color.
+        if df.iloc[0]["Type"] == "H":
+            ax.scatter(
+                df.iloc[0]["x"],
+                df.iloc[0]["y"],
+                marker="o",
+                fc="royalblue",
+                ec="#00ce00",
+                lw=2.5,
+                s=markersize,
+                zorder=2,
+            )
+        else:
+            ax.scatter(
+                df.iloc[0]["x"],
+                df.iloc[0]["y"],
+                marker="o",
+                fc="white",
+                ec="#00ce00",
+                lw=2.5,
+                s=markersize,
+                zorder=2,
+            )
 
     # Plot dotted lines between the aminos that increase the stability.
     pairs = get_scoring_pairs(protein)
 
     for pos1, pos2 in pairs:
         ax.plot(
             [pos1[0], pos2[0]],
             [pos1[1], pos2[1]],
             linestyle=":",
             color="indianred",
             alpha=0.9,
+            linewidth=linewidth,
             zorder=1,
-            lw=2,
         )
 
     # Remove axis, and position legend in the upper right with created space.
     ax.axis("off")
 
 
 def _plot_aminos_3d_basic(protein, df, ax):
@@ -180,133 +193,150 @@
             color="indianred",
             alpha=0.9,
             zorder=1,
             lw=2,
         )
 
 
-def _plot_aminos_3d_paper(protein, df, ax):
+def _plot_aminos_3d_paper(
+    protein, df, ax, linewidth, markersize, annotate_first=False
+):
     """
     Plot amino acids in paper style in a 3D figure.
     :param Protein      protein:    Protein object to plot the hash of.
     :param DataFrame    df:         DataFrame with all ordered positions.
     :param Axes         ax:         Axis to plot on.
     """
     # Split dataframe on amino acid type.
     df_H = df.loc[df["Type"] == "H"]
     df_P = df.loc[df["Type"] == "P"]
 
-    ax.plot(df["x"], df["y"], df["z"], color="black", alpha=0.65, zorder=1)
+    ax.plot(
+        df["x"],
+        df["y"],
+        df["z"],
+        color="black",
+        alpha=0.65,
+        linewidth=linewidth,
+        zorder=1,
+    )
 
-    sns.scatterplot(
+    ax.scatter(
         df_H["x"],
         df_H["y"],
         df_H["z"],
-        data=df_H,
         marker="o",
         edgecolor="royalblue",
-        s=60,
+        s=markersize,
         zorder=2,
-        ax=ax,
         label="H",
+        depthshade=False,
     )
-    sns.scatterplot(
+    ax.scatter(
         df_P["x"],
         df_P["y"],
         df_P["z"],
-        data=df_P,
         marker="o",
         facecolor="white",
         edgecolor="orange",
-        linewidth=2,
-        s=60,
+        lw=1.3,
+        s=markersize,
         zorder=2,
-        ax=ax,
         label="P",
+        depthshade=False,
     )
 
-    # Plot first point with a different color.
-    if df.iloc[0]["Type"] == "H":
-        ax.scatter(
-            df.iloc[0]["x"],
-            df.iloc[0]["y"],
-            marker="o",
-            fc="royalblue",
-            ec="#00ce00",
-            lw=2.5,
-            s=80,
-            zorder=2,
-        )
-    else:
-        ax.scatter(
-            df.iloc[0]["x"],
-            df.iloc[0]["y"],
-            marker="o",
-            fc="white",
-            ec="#00ce00",
-            lw=2.5,
-            s=80,
-            zorder=2,
-        )
+    # Plot first point with a green edge color.
+    if annotate_first:
+        if df.iloc[0]["Type"] == "H":
+            ax.scatter(
+                df.iloc[0]["x"],
+                df.iloc[0]["y"],
+                df.iloc[0]["z"],
+                marker="o",
+                fc="royalblue",
+                ec="#00ce00",
+                lw=1.3,
+                s=markersize,
+                zorder=2,
+            )
+        else:
+            ax.scatter(
+                df.iloc[0]["x"],
+                df.iloc[0]["y"],
+                df.iloc[0]["z"],
+                marker="o",
+                fc="white",
+                ec="#00ce00",
+                lw=1.3,
+                s=markersize,
+                zorder=2,
+            )
 
     # Plot dotted lines between the aminos that increase the stability.
     pairs = get_scoring_pairs(protein)
 
     for pos1, pos2 in pairs:
         ax.plot(
             [pos1[0], pos2[0]],
             [pos1[1], pos2[1]],
             [pos1[2], pos2[2]],
             linestyle=":",
             color="indianred",
             alpha=0.9,
             zorder=1,
-            lw=2,
+            lw=linewidth,
         )
 
     # Remove axis, and position legend in the upper right with created space.
     ax.axis("off")
 
 
 def plot_protein(
     protein,
     style="basic",
     ax=None,
     legend=True,
     legend_style="inner",
     show=True,
+    linewidth=2.5,
+    markersize=210,
+    annotate_first=False,
 ):
     """
     Plot conformation of a protein.
     :param Protein  protein:        Protein object to plot the hash of.
     :param [str]    style:          What style to plot the proteins in.
     :param Axes     ax:             Axis to plot Protein on.
     :param bool     legend:         True if a legend needs to be added.
     :param str      legend_style:   Either 'inner' or 'outer'.
     :param bool     show:           True if plot.show() needs to be called.
+    :param float    linewidth:      Width of the lines.
+    :param float    markersize:     Size of the markers.
+    :param bool     annotate_first: True if first amino acids needs annotation.
     """
     # Catch unplottable dimensions.
     if protein.dim != 2 and protein.dim != 3:
         raise RuntimeError(
             f"Cannot plot the structure of a protein with "
             f"dimension '{protein.dim}'"
         )
 
     # Create axis to plot onto if not given.
     if ax is None:
         if style == "paper":
-            fig = plt.figure(figsize=(4, 2.5))
+            fig = plt.figure(figsize=(5, 3.125))
         else:
             fig = plt.figure(figsize=(5, 6))
             sns.set_style("whitegrid")
 
         if protein.dim == 2:
             ax = fig.gca()
         else:
-            ax = fig.gca(projection="3d")
+            ax = fig.add_subplot(projection="3d")
 
     # Fetch data in right dimension.
     if protein.dim == 2:
         df = pd.DataFrame(
             get_ordered_positions(protein), columns=["x", "y", "Type"]
         )
         df = df.astype({"x": "int32", "y": "int32"})
@@ -315,17 +345,21 @@
             get_ordered_positions(protein), columns=["x", "y", "z", "Type"]
         )
         df = df.astype({"x": "int32", "y": "int32", "z": "int32"})
 
     # Plot the selected style.
     if style == "paper":
         if protein.dim == 2:
-            _plot_aminos_2d_paper(protein, df, ax)
+            _plot_aminos_2d_paper(
+                protein, df, ax, linewidth, markersize, annotate_first
+            )
         else:
-            _plot_aminos_3d_paper(protein, df, ax)
+            _plot_aminos_3d_paper(
+                protein, df, ax, linewidth, markersize, annotate_first
+            )
     elif style == "basic":
         ax.set_xlabel("x-axis", fontsize=13)
         ax.set_ylabel("y-axis", fontsize=13)
         ax.xaxis.set_major_locator(MaxNLocator(integer=True))
         ax.yaxis.set_major_locator(MaxNLocator(integer=True))
 
         # Plot dimension specific.
@@ -337,39 +371,42 @@
             ax.set_zlabel("z-axis", fontsize=13)
             ax.zaxis.set_major_locator(MaxNLocator(integer=True))
             _plot_aminos_3d_basic(protein, df, ax)
 
     # If adding legend, remove title from legend and add item for bonds.
     if legend:
         handles, labels = ax.get_legend_handles_labels()
-        score_patch = Line2D(
-            [],
-            [],
-            color="indianred",
-            linestyle=":",
-            alpha=0.9,
-            label="Bond",
-            lw=2,
-        )
-        handles.append(score_patch)
-        labels.append(score_patch.get_label())
+
+        # Only add bond label if actually in plot.
+        if protein.score != 0:
+            score_patch = Line2D(
+                [],
+                [],
+                color="indianred",
+                linestyle=":",
+                linewidth=linewidth,
+                alpha=0.9,
+                label="Bond",
+            )
+            handles.append(score_patch)
+            labels.append(score_patch.get_label())
 
         # Style legend according to plotting style.
         if (
             style == "paper" and legend_style == "outer"
         ) or legend_style == "outer":
             box = ax.get_position()
             ax.set_position([box.x0, box.y0, box.width * 0.7, box.height])
             ax.legend(
                 handles=handles,
                 labels=labels,
                 loc="upper left",
                 bbox_to_anchor=(1, 1),
             )
         else:
-            ax.legend(handles=handles, labels=labels)
-    else:
+            ax.legend(handles=handles, labels=labels, prop={"size": 12})
+    elif protein.dim == 2:
         ax.get_legend().remove()
 
     # Show plot if specified.
     if show:
         plt.show()
```

### Comparing `prospr-0.2a9/setup.py` & `prospr-1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-#!/usr/bin/env python3
-"""
-File:           setup.py
-Description:    This file contains the setup required for distributing the
-                package on PyPi.org.
-License:        This file is licensed under the GNU LGPL V3 license by
-                Okke van Eck (2020 - 2022). See the LICENSE file for the
-                specifics.
-"""
-
-import os
-from setuptools import setup
-from pybind11.setup_helpers import Pybind11Extension, build_ext
-
-__version__ = "0.2a9"
-
-# Define core module extension.
-ext_modules = [
-    Pybind11Extension(
-        "prospr_core",
-        ["prospr/core/core_module.cpp"],
-        define_macros=[("VERSION_INFO", __version__)],
-        optional=os.environ.get("CIBUILDWHEEL", "0") != "1",
-        language="c++",
-    ),
+[build-system]
+requires = [
+    "setuptools>=42",
+    "wheel",
+    "pybind11~=2.11.0",
 ]
+build-backend = "setuptools.build_meta"
 
-# Load README for PyPI description.
-with open("README.md", "r") as f:
-    long_description = f.read()
-
-setup(
-    name="prospr",
-    version=__version__,
-    author="okkevaneck",
-    description="A toolbox for protein folding with Python.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/okkevaneck/prospr",
-    license="LGPLv3",
-    ext_modules=ext_modules,
-    cmdclass={"build_ext": build_ext},
-    packages=["prospr"],
-    package_data={"prospr": ["data/*/*.csv"]},
-    platforms=["any"],
-    python_requires=">=3.9",
-    zip_safe=False,
-    install_requires=[
-        "matplotlib",
-        "seaborn",
-        "numpy",
-        "pandas",
-    ],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Development Status :: 2 - Pre-Alpha",
-        "License :: OSI Approved :: GNU Lesser General Public License v3 "
-        + "(LGPLv3)",
-        "Operating System :: OS Independent",
-        "Topic :: Education",
-        "Topic :: Scientific/Engineering",
-        "Topic :: Scientific/Engineering :: Bio-Informatics",
-    ],
-    keywords=[
-        "prospr protein structure prediction toolbox python c++ swig cmake "
-        + "extension heuristics pypi package"
-    ],
-)
+[project]
+name = "prospr"
+authors = [
+    {name = "okkevaneck", email = "okke.van.eck@gmail.com"},
+]
+dynamic = ["version"]
+description = "A toolbox for protein folding with Python."
+readme = "README.md"
+requires-python = ">=3.9"
+license = {file = "LICENSE"}
+keywords = [
+    "prospr",
+    "protein",
+    "structure",
+    "prediction",
+    "toolbox",
+    "python",
+    "c++",
+    "extension",
+    "pypi",
+    "package",
+]
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "Development Status :: 2 - Pre-Alpha",
+    "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
+    "Operating System :: OS Independent",
+    "Topic :: Education",
+    "Topic :: Scientific/Engineering",
+    "Topic :: Scientific/Engineering :: Bio-Informatics",
+]
+
+[project.urls]
+homepage = "https://github.com/okkevaneck/prospr"
+documentation = "https://prospr.readthedocs.io"
+repository = "https://github.com/okkevaneck/prospr"
+
+[tool.setuptools]
+packages = ["prospr"]
+package-dir = {"prospr" = "prospr"}
+zip-safe = false
+platforms = ["Linux", "macOS", "Windows"]
+
+[tool.setuptools.package-data]
+prospr = ["data/*/*.csv", "core/src/*"]
+
+[tool.setuptools.dynamic]
+version = {attr = "prospr._version.__version__"}
+
+[tool.black]
+line-length = 79
+
+[tool.pytest]
+minversion = 7.1
+
+[tool.pytest.ini_options]
+pythonpath = [
+  ".",
+]
```

