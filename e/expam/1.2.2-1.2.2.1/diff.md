# Comparing `tmp/expam-1.2.2.tar.gz` & `tmp/expam-1.2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expam-1.2.2.tar", last modified: Thu Dec 15 04:19:58 2022, max compression
+gzip compressed data, was "expam-1.2.2.1.tar", last modified: Sun Jul 16 01:14:54 2023, max compression
```

## Comparing `expam-1.2.2.tar` & `expam-1.2.2.1.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.957675 expam-1.2.2/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     1534 2021-11-29 01:19:26.000000 expam-1.2.2/LICENSE
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      152 2022-04-26 01:28:57.000000 expam-1.2.2/MANIFEST.in
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     8166 2022-12-15 04:19:58.957853 expam-1.2.2/PKG-INFO
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     7374 2022-08-15 22:48:48.000000 expam-1.2.2/README.md
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      118 2022-05-18 04:56:39.000000 expam-1.2.2/pyproject.toml
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)       74 2022-12-15 04:19:58.958510 expam-1.2.2/setup.cfg
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     4386 2022-08-15 00:08:04.000000 expam-1.2.2/setup.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.902126 expam-1.2.2/src/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.911666 expam-1.2.2/src/expam/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)       24 2022-12-15 03:23:08.000000 expam-1.2.2/src/expam/__init__.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.918830 expam-1.2.2/src/expam/classify/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      920 2022-08-17 01:38:45.000000 expam-1.2.2/src/expam/classify/__init__.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    26028 2022-10-24 04:37:14.000000 expam-1.2.2/src/expam/classify/classify.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     2610 2022-10-10 11:16:42.000000 expam-1.2.2/src/expam/classify/config.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     1226 2022-04-24 03:04:23.000000 expam-1.2.2/src/expam/classify/process.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    11058 2022-08-17 05:48:04.000000 expam-1.2.2/src/expam/classify/taxonomy.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.923644 expam-1.2.2/src/expam/cli/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-04-26 02:24:46.000000 expam-1.2.2/src/expam/cli/__init__.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     5806 2022-12-15 03:11:54.000000 expam-1.2.2/src/expam/cli/build.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     6675 2022-08-23 04:43:22.000000 expam-1.2.2/src/expam/cli/classify.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    13885 2022-12-15 03:27:04.000000 expam-1.2.2/src/expam/cli/main.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    21510 2022-12-15 04:18:05.000000 expam-1.2.2/src/expam/cli/tree.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     9807 2022-04-26 02:35:04.000000 expam-1.2.2/src/expam/cli/utils.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.928065 expam-1.2.2/src/expam/database/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     1620 2022-04-25 12:25:25.000000 expam-1.2.2/src/expam/database/__init__.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     9903 2022-08-12 06:20:03.000000 expam-1.2.2/src/expam/database/build.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    10674 2022-05-19 22:27:58.000000 expam-1.2.2/src/expam/database/config.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     4075 2022-10-12 23:34:51.000000 expam-1.2.2/src/expam/database/db.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      898 2022-04-24 02:11:01.000000 expam-1.2.2/src/expam/database/shm.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.929228 expam-1.2.2/src/expam/ext/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-04-26 02:25:00.000000 expam-1.2.2/src/expam/ext/__init__.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.931987 expam-1.2.2/src/expam/ext/kmers/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      255 2022-04-25 11:38:02.000000 expam-1.2.2/src/expam/ext/kmers/__init__.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.903205 expam-1.2.2/src/expam/ext/kmers/_build/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.903318 expam-1.2.2/src/expam/ext/kmers/_build/src/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.903430 expam-1.2.2/src/expam/ext/kmers/_build/src/expam/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.903544 expam-1.2.2/src/expam/ext/kmers/_build/src/expam/ext/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.932953 expam-1.2.2/src/expam/ext/kmers/_build/src/expam/ext/kmers/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)  1020865 2022-12-15 04:19:54.000000 expam-1.2.2/src/expam/ext/kmers/_build/src/expam/ext/kmers/extract.c
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     7650 2022-03-03 20:52:46.000000 expam-1.2.2/src/expam/ext/kmers/extract.pyx
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      845 2022-03-03 20:52:46.000000 expam-1.2.2/src/expam/ext/kmers/jellyfish.c
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     4571 2022-03-03 20:52:46.000000 expam-1.2.2/src/expam/ext/kmers/kmers.c
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.936236 expam-1.2.2/src/expam/ext/map/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      139 2022-04-25 11:38:00.000000 expam-1.2.2/src/expam/ext/map/__init__.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.904230 expam-1.2.2/src/expam/ext/map/_build/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.904422 expam-1.2.2/src/expam/ext/map/_build/src/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.904603 expam-1.2.2/src/expam/ext/map/_build/src/expam/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.904739 expam-1.2.2/src/expam/ext/map/_build/src/expam/ext/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.936876 expam-1.2.2/src/expam/ext/map/_build/src/expam/ext/map/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)  1092297 2022-12-15 04:19:56.000000 expam-1.2.2/src/expam/ext/map/_build/src/expam/ext/map/map.c
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     9202 2022-04-24 02:59:08.000000 expam-1.2.2/src/expam/ext/map/map.pyx
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.942629 expam-1.2.2/src/expam/ext/sets/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)       58 2022-04-25 12:16:15.000000 expam-1.2.2/src/expam/ext/sets/__init__.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.905325 expam-1.2.2/src/expam/ext/sets/_build/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.905474 expam-1.2.2/src/expam/ext/sets/_build/src/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.905623 expam-1.2.2/src/expam/ext/sets/_build/src/expam/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.905768 expam-1.2.2/src/expam/ext/sets/_build/src/expam/ext/
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.943171 expam-1.2.2/src/expam/ext/sets/_build/src/expam/ext/sets/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)   916827 2022-12-15 04:19:58.000000 expam-1.2.2/src/expam/ext/sets/_build/src/expam/ext/sets/sets.c
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     9819 2022-03-03 20:52:46.000000 expam-1.2.2/src/expam/ext/sets/mfil.c
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     3336 2022-04-24 02:59:47.000000 expam-1.2.2/src/expam/ext/sets/sets.pyx
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     2272 2022-04-23 07:30:03.000000 expam-1.2.2/src/expam/logger.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      885 2022-12-15 03:27:07.000000 expam-1.2.2/src/expam/main.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.951610 expam-1.2.2/src/expam/process/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      106 2022-04-23 10:00:12.000000 expam-1.2.2/src/expam/process/__init__.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     5343 2022-04-24 03:21:53.000000 expam-1.2.2/src/expam/process/classify.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     9483 2022-04-24 03:21:48.000000 expam-1.2.2/src/expam/process/genome.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    16337 2022-04-24 03:06:58.000000 expam-1.2.2/src/expam/process/jobworker.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    21995 2022-04-25 22:02:42.000000 expam-1.2.2/src/expam/process/manager.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    14640 2022-04-24 03:20:02.000000 expam-1.2.2/src/expam/process/piler.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     5111 2022-05-23 06:35:01.000000 expam-1.2.2/src/expam/process/reads.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.952801 expam-1.2.2/src/expam/sandbox/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-04-26 02:25:15.000000 expam-1.2.2/src/expam/sandbox/__init__.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     4751 2022-05-11 03:00:29.000000 expam-1.2.2/src/expam/sandbox/main.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    10447 2022-04-25 12:17:36.000000 expam-1.2.2/src/expam/sequences.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.957206 expam-1.2.2/src/expam/tree/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)      801 2022-04-26 00:49:10.000000 expam-1.2.2/src/expam/tree/__init__.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     4250 2022-09-28 05:45:31.000000 expam-1.2.2/src/expam/tree/location.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     1741 2022-04-25 09:54:26.000000 expam-1.2.2/src/expam/tree/simulate.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     2956 2022-12-15 04:18:08.000000 expam-1.2.2/src/expam/tree/sourmash.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)    33051 2022-10-14 02:26:08.000000 expam-1.2.2/src/expam/tree/tree.py
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     2669 2022-05-19 08:15:12.000000 expam-1.2.2/src/expam/utils.py
-drwxr-xr-x   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        0 2022-12-15 04:19:58.915371 expam-1.2.2/src/expam.egg-info/
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     8166 2022-12-15 04:19:58.000000 expam-1.2.2/src/expam.egg-info/PKG-INFO
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)     1636 2022-12-15 04:19:58.000000 expam-1.2.2/src/expam.egg-info/SOURCES.txt
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)        1 2022-12-15 04:19:58.000000 expam-1.2.2/src/expam.egg-info/dependency_links.txt
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)       80 2022-12-15 04:19:58.000000 expam-1.2.2/src/expam.egg-info/entry_points.txt
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)       93 2022-12-15 04:19:58.000000 expam-1.2.2/src/expam.egg-info/requires.txt
--rw-r--r--   0 ssol0002 (1359105870) MONASH\Domain Users (907548567)       21 2022-12-15 04:19:58.000000 expam-1.2.2/src/expam.egg-info/top_level.txt
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.470057 expam-1.2.2.1/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     1534 2021-11-29 01:19:26.000000 expam-1.2.2.1/LICENSE
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      152 2022-04-26 01:28:57.000000 expam-1.2.2.1/MANIFEST.in
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     8168 2023-07-16 01:14:54.470696 expam-1.2.2.1/PKG-INFO
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     7374 2022-08-15 22:48:48.000000 expam-1.2.2.1/README.md
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      118 2022-05-18 04:56:39.000000 expam-1.2.2.1/pyproject.toml
+-rw-r--r--   0 ssol0002 (1359105870) 907548567       74 2023-07-16 01:14:54.472499 expam-1.2.2.1/setup.cfg
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     4389 2023-07-16 01:10:37.000000 expam-1.2.2.1/setup.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.392183 expam-1.2.2.1/src/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.406901 expam-1.2.2.1/src/expam/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567       27 2023-07-16 01:10:20.000000 expam-1.2.2.1/src/expam/__init__.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.416920 expam-1.2.2.1/src/expam/classify/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      920 2022-08-17 01:38:45.000000 expam-1.2.2.1/src/expam/classify/__init__.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    26028 2022-10-24 04:37:14.000000 expam-1.2.2.1/src/expam/classify/classify.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     2610 2022-10-10 11:16:42.000000 expam-1.2.2.1/src/expam/classify/config.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     1226 2022-04-24 03:04:23.000000 expam-1.2.2.1/src/expam/classify/process.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    11058 2022-08-17 05:48:04.000000 expam-1.2.2.1/src/expam/classify/taxonomy.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.424573 expam-1.2.2.1/src/expam/cli/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567        0 2022-04-26 02:24:46.000000 expam-1.2.2.1/src/expam/cli/__init__.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     5806 2022-12-15 03:11:54.000000 expam-1.2.2.1/src/expam/cli/build.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     6675 2022-08-23 04:43:22.000000 expam-1.2.2.1/src/expam/cli/classify.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    13885 2022-12-15 03:27:04.000000 expam-1.2.2.1/src/expam/cli/main.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    21766 2023-07-16 01:13:29.000000 expam-1.2.2.1/src/expam/cli/tree.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     9807 2022-04-26 02:35:04.000000 expam-1.2.2.1/src/expam/cli/utils.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.429944 expam-1.2.2.1/src/expam/database/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     1620 2022-04-25 12:25:25.000000 expam-1.2.2.1/src/expam/database/__init__.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     9903 2022-08-12 06:20:03.000000 expam-1.2.2.1/src/expam/database/build.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    10674 2022-05-19 22:27:58.000000 expam-1.2.2.1/src/expam/database/config.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     4075 2022-10-12 23:34:51.000000 expam-1.2.2.1/src/expam/database/db.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      898 2022-04-24 02:11:01.000000 expam-1.2.2.1/src/expam/database/shm.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.431365 expam-1.2.2.1/src/expam/ext/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567        0 2022-04-26 02:25:00.000000 expam-1.2.2.1/src/expam/ext/__init__.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.434603 expam-1.2.2.1/src/expam/ext/kmers/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      255 2022-04-25 11:38:02.000000 expam-1.2.2.1/src/expam/ext/kmers/__init__.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.393583 expam-1.2.2.1/src/expam/ext/kmers/_build/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.393708 expam-1.2.2.1/src/expam/ext/kmers/_build/src/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.393859 expam-1.2.2.1/src/expam/ext/kmers/_build/src/expam/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.394018 expam-1.2.2.1/src/expam/ext/kmers/_build/src/expam/ext/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.435768 expam-1.2.2.1/src/expam/ext/kmers/_build/src/expam/ext/kmers/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567  1024108 2023-07-16 01:14:50.000000 expam-1.2.2.1/src/expam/ext/kmers/_build/src/expam/ext/kmers/extract.c
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     7650 2022-03-03 20:52:46.000000 expam-1.2.2.1/src/expam/ext/kmers/extract.pyx
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      845 2022-03-03 20:52:46.000000 expam-1.2.2.1/src/expam/ext/kmers/jellyfish.c
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     4571 2022-03-03 20:52:46.000000 expam-1.2.2.1/src/expam/ext/kmers/kmers.c
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.439492 expam-1.2.2.1/src/expam/ext/map/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      139 2022-04-25 11:38:00.000000 expam-1.2.2.1/src/expam/ext/map/__init__.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.394814 expam-1.2.2.1/src/expam/ext/map/_build/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.395025 expam-1.2.2.1/src/expam/ext/map/_build/src/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.395209 expam-1.2.2.1/src/expam/ext/map/_build/src/expam/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.395376 expam-1.2.2.1/src/expam/ext/map/_build/src/expam/ext/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.440372 expam-1.2.2.1/src/expam/ext/map/_build/src/expam/ext/map/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567  1097078 2023-07-16 01:14:52.000000 expam-1.2.2.1/src/expam/ext/map/_build/src/expam/ext/map/map.c
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     9202 2022-04-24 02:59:08.000000 expam-1.2.2.1/src/expam/ext/map/map.pyx
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.446873 expam-1.2.2.1/src/expam/ext/sets/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567       58 2022-04-25 12:16:15.000000 expam-1.2.2.1/src/expam/ext/sets/__init__.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.396251 expam-1.2.2.1/src/expam/ext/sets/_build/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.396518 expam-1.2.2.1/src/expam/ext/sets/_build/src/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.396778 expam-1.2.2.1/src/expam/ext/sets/_build/src/expam/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.397019 expam-1.2.2.1/src/expam/ext/sets/_build/src/expam/ext/
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.447430 expam-1.2.2.1/src/expam/ext/sets/_build/src/expam/ext/sets/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567   921493 2023-07-16 01:14:53.000000 expam-1.2.2.1/src/expam/ext/sets/_build/src/expam/ext/sets/sets.c
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     9819 2022-03-03 20:52:46.000000 expam-1.2.2.1/src/expam/ext/sets/mfil.c
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     3336 2022-04-24 02:59:47.000000 expam-1.2.2.1/src/expam/ext/sets/sets.pyx
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     2272 2022-04-23 07:30:03.000000 expam-1.2.2.1/src/expam/logger.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      885 2022-12-15 03:27:07.000000 expam-1.2.2.1/src/expam/main.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.457988 expam-1.2.2.1/src/expam/process/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      106 2022-04-23 10:00:12.000000 expam-1.2.2.1/src/expam/process/__init__.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     5343 2022-04-24 03:21:53.000000 expam-1.2.2.1/src/expam/process/classify.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     9483 2022-04-24 03:21:48.000000 expam-1.2.2.1/src/expam/process/genome.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    16337 2022-04-24 03:06:58.000000 expam-1.2.2.1/src/expam/process/jobworker.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    21995 2022-04-25 22:02:42.000000 expam-1.2.2.1/src/expam/process/manager.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    14640 2022-04-24 03:20:02.000000 expam-1.2.2.1/src/expam/process/piler.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     5111 2022-05-23 06:35:01.000000 expam-1.2.2.1/src/expam/process/reads.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.460556 expam-1.2.2.1/src/expam/sandbox/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567        0 2022-04-26 02:25:15.000000 expam-1.2.2.1/src/expam/sandbox/__init__.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     4751 2022-05-11 03:00:29.000000 expam-1.2.2.1/src/expam/sandbox/main.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    10447 2022-04-25 12:17:36.000000 expam-1.2.2.1/src/expam/sequences.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.468020 expam-1.2.2.1/src/expam/tree/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567      801 2022-04-26 00:49:10.000000 expam-1.2.2.1/src/expam/tree/__init__.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     4250 2022-09-28 05:45:31.000000 expam-1.2.2.1/src/expam/tree/location.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     1741 2022-04-25 09:54:26.000000 expam-1.2.2.1/src/expam/tree/simulate.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     2956 2022-12-15 04:18:08.000000 expam-1.2.2.1/src/expam/tree/sourmash.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567    33051 2022-10-14 02:26:08.000000 expam-1.2.2.1/src/expam/tree/tree.py
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     2669 2022-05-19 08:15:12.000000 expam-1.2.2.1/src/expam/utils.py
+drwxr-xr-x   0 ssol0002 (1359105870) 907548567        0 2023-07-16 01:14:54.411428 expam-1.2.2.1/src/expam.egg-info/
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     8168 2023-07-16 01:14:54.000000 expam-1.2.2.1/src/expam.egg-info/PKG-INFO
+-rw-r--r--   0 ssol0002 (1359105870) 907548567     1636 2023-07-16 01:14:54.000000 expam-1.2.2.1/src/expam.egg-info/SOURCES.txt
+-rw-r--r--   0 ssol0002 (1359105870) 907548567        1 2023-07-16 01:14:54.000000 expam-1.2.2.1/src/expam.egg-info/dependency_links.txt
+-rw-r--r--   0 ssol0002 (1359105870) 907548567       80 2023-07-16 01:14:54.000000 expam-1.2.2.1/src/expam.egg-info/entry_points.txt
+-rw-r--r--   0 ssol0002 (1359105870) 907548567       93 2023-07-16 01:14:54.000000 expam-1.2.2.1/src/expam.egg-info/requires.txt
+-rw-r--r--   0 ssol0002 (1359105870) 907548567       21 2023-07-16 01:14:54.000000 expam-1.2.2.1/src/expam.egg-info/top_level.txt
```

### Comparing `expam-1.2.2/LICENSE` & `expam-1.2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/PKG-INFO` & `expam-1.2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expam
-Version: 1.2.2
+Version: 1.2.2.1
 Summary: Metagenomic profiling using a reference phylogeny
 Home-page: https://github.com/seansolari/expam
 Author: Sean Solari
 Author-email: sean.solari@monash.edu
 Project-URL: Bug Reports, https://github.com/seansolari/expam/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `expam-1.2.2/README.md` & `expam-1.2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/setup.py` & `expam-1.2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 ]
 
 setup(
     #
     # Metadata.
     #
     name="expam",
-    version="%d.%d.%d" % __version__,
+    version="%d.%d.%d.%d" % __version__,
     description="Metagenomic profiling using a reference phylogeny",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/seansolari/expam",
     author="Sean Solari",
     author_email="sean.solari@monash.edu",
     classifiers=[
```

### Comparing `expam-1.2.2/src/expam/classify/__init__.py` & `expam-1.2.2.1/src/expam/classify/__init__.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/classify/classify.py` & `expam-1.2.2.1/src/expam/classify/classify.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/classify/config.py` & `expam-1.2.2.1/src/expam/classify/config.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/classify/process.py` & `expam-1.2.2.1/src/expam/classify/process.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/classify/taxonomy.py` & `expam-1.2.2.1/src/expam/classify/taxonomy.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/cli/build.py` & `expam-1.2.2.1/src/expam/cli/build.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/cli/classify.py` & `expam-1.2.2.1/src/expam/cli/classify.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/cli/main.py` & `expam-1.2.2.1/src/expam/cli/main.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/cli/tree.py` & `expam-1.2.2.1/src/expam/cli/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import re
 import shutil
 import subprocess
+from tempfile import TemporaryDirectory
 from typing import List, Set, Tuple, Union
 from expam.classify import ResultsPathConfig
 from expam.classify.classify import ClassificationResults, name_to_id
 from expam.classify.config import make_results_config, validate_results_configuration
 from expam.classify.taxonomy import TaxonomyNCBI
 from expam.cli.main import CommandGroup, ExpamOptions
 from expam.database import FileLocationConfig
@@ -488,17 +489,22 @@
                 self.mash_sketch(k=k, s=s, p=n, sequences=sequences, out_dir=file_path)
 
     def sour_sketch(self, k: int, s: int, sequences: List[str], sig_dir: str):
         from expam.tree.sourmash import make_signatures
         make_signatures(self.get_n_processes(), sequences, sig_dir, k, s)
 
     def mash_sketch(self, k, s, p, sequences, out_dir):
-        cmd_fmt = "mash sketch -k %d -p %d -s %d -o %s %s"
-        cmd = cmd_fmt % (k, p, s, out_dir, ' '.join(sequences))
-        self.shell(cmd)
+        # prepare temporary directory to link files
+        with TemporaryDirectory() as tmp_dir:
+            for seq in sequences:
+                os.symlink(seq, tmp_dir)
+            # run mash on temp directory
+            cmd_fmt = "mash sketch -k %d -p %d -s %d -o %s %s/*"
+            cmd = cmd_fmt % (k, p, s, out_dir, tmp_dir)
+            self.shell(cmd)
 
     """
     Compute pairwise distances between sketched sequences
     =====================================================
     
     """
     def distance(self):
```

### Comparing `expam-1.2.2/src/expam/cli/utils.py` & `expam-1.2.2.1/src/expam/cli/utils.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/database/__init__.py` & `expam-1.2.2.1/src/expam/database/__init__.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/database/build.py` & `expam-1.2.2.1/src/expam/database/build.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/database/config.py` & `expam-1.2.2.1/src/expam/database/config.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/database/db.py` & `expam-1.2.2.1/src/expam/database/db.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/database/shm.py` & `expam-1.2.2.1/src/expam/database/shm.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/ext/kmers/_build/src/expam/ext/kmers/extract.c` & `expam-1.2.2.1/src/expam/ext/kmers/_build/src/expam/ext/kmers/extract.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "src/expam/ext/kmers/jellyfish.c",
             "src/expam/ext/kmers/kmers.c"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "src/expam/ext/kmers",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include"
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "kmers._build.kmers",
         "sources": [
             "src/expam/ext/kmers/extract.pyx",
             "src/expam/ext/kmers/kmers.c",
             "src/expam/ext/kmers/jellyfish.c"
         ]
@@ -41,16 +41,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -110,24 +110,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -235,15 +239,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -274,15 +278,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -397,17 +401,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -477,14 +478,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -584,35 +590,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1129,195 +1135,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1393,42 +1381,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1697,26 +1685,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -2040,14 +2028,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* ImportFrom.proto */
@@ -2076,22 +2081,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -5761,15 +5774,15 @@
  * 
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5778,29 +5791,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -5811,15 +5824,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5828,29 +5841,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -5861,15 +5874,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5878,29 +5891,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -5911,15 +5924,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5928,29 +5941,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -5961,15 +5974,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -5978,29 +5991,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6011,212 +6024,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":928
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":932
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":940
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6232,15 +6253,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -6248,84 +6269,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -6340,15 +6361,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":946
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6364,15 +6385,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6380,84 +6401,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6472,15 +6493,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":952
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6496,15 +6517,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -6512,84 +6533,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -6604,176 +6625,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":966
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":981
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":996
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7082,15 +7103,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -9060,15 +9081,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -11363,15 +11384,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -11436,15 +11457,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -14116,15 +14137,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(2, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -19639,15 +19660,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -19843,15 +19864,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -20006,15 +20027,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -20028,15 +20049,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -20128,15 +20149,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -20159,15 +20180,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -20392,15 +20413,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -20412,15 +20433,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -20541,15 +20562,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"reverse_complement", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_5kmers_6_build_5kmers_1reverse_complement, METH_VARARGS|METH_KEYWORDS, 0},
   {0, 0, 0, 0}
@@ -20736,15 +20757,15 @@
   {&__pyx_n_s_view, __pyx_k_view, sizeof(__pyx_k_view), 0, 0, 1, 1},
   {&__pyx_n_s_x, __pyx_k_x, sizeof(__pyx_k_x), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 31, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 249, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 941, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
   return 0;
@@ -20752,33 +20773,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -21149,15 +21170,20 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -21273,55 +21299,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -21506,15 +21516,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_kmers___build__kmers) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -22288,17 +22298,15 @@
     PyObject *old_exc, *old_val, *old_tb;
     PyObject *ctx;
     __Pyx_PyThreadState_declare
 #ifdef WITH_THREAD
     PyGILState_STATE state;
     if (nogil)
         state = PyGILState_Ensure();
-#ifdef _MSC_VER
-    else state = (PyGILState_STATE)-1;
-#endif
+    else state = (PyGILState_STATE)0;
 #endif
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
     if (full_traceback) {
         Py_XINCREF(old_exc);
         Py_XINCREF(old_val);
         Py_XINCREF(old_tb);
@@ -22665,15 +22673,15 @@
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
 #if CYTHON_FAST_PYCALL
     if (PyFunction_Check(func)) {
         return __Pyx_PyFunction_FastCall(func, NULL, 0);
     }
 #endif
-#ifdef __Pyx_CyFunction_USED
+#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
     if (likely(PyCFunction_Check(func) || __Pyx_CyFunction_Check(func)))
 #else
     if (likely(PyCFunction_Check(func)))
 #endif
     {
         if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
             return __Pyx_PyObject_CallMethO(func, NULL);
@@ -22971,28 +22979,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -23208,15 +23216,15 @@
 #endif
     return PyObject_GetAttr(o, n);
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -23864,61 +23872,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -23926,15 +23952,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -25337,15 +25363,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -25491,15 +25517,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -25643,15 +25669,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26029,15 +26055,15 @@
                         } else if (8 * sizeof(unsigned PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
                             return (unsigned PY_LONG_LONG) (((((((((unsigned PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (unsigned PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26225,15 +26251,15 @@
                         } else if (8 * sizeof(npy_uint64) >= 4 * PyLong_SHIFT) {
                             return (npy_uint64) (((((((((npy_uint64)digits[3]) << PyLong_SHIFT) | (npy_uint64)digits[2]) << PyLong_SHIFT) | (npy_uint64)digits[1]) << PyLong_SHIFT) | (npy_uint64)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26428,15 +26454,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26624,15 +26650,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `expam-1.2.2/src/expam/ext/kmers/extract.pyx` & `expam-1.2.2.1/src/expam/ext/kmers/extract.pyx`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/ext/kmers/jellyfish.c` & `expam-1.2.2.1/src/expam/ext/kmers/jellyfish.c`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/ext/kmers/kmers.c` & `expam-1.2.2.1/src/expam/ext/kmers/kmers.c`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/ext/map/_build/src/expam/ext/map/map.c` & `expam-1.2.2.1/src/expam/ext/map/_build/src/expam/ext/map/map.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include"
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "map._build.map",
         "sources": [
             "src/expam/ext/map/map.pyx"
         ]
     },
     "module_name": "map._build.map"
@@ -33,16 +33,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -102,24 +102,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -227,15 +231,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -266,15 +270,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -389,17 +393,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -469,14 +470,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -576,35 +582,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1120,195 +1126,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1377,42 +1365,42 @@
 struct __pyx_obj_3map_6_build_3map___pyx_scope_struct__compressed_to_string;
 struct __pyx_obj_3map_6_build_3map___pyx_scope_struct_1_genexpr;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1721,26 +1709,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1853,30 +1841,60 @@
 /* IncludeStringH.proto */
 #include <string.h>
 
 /* JoinPyUnicode.proto */
 static PyObject* __Pyx_PyUnicode_Join(PyObject* value_tuple, Py_ssize_t value_count, Py_ssize_t result_ulength,
                                       Py_UCS4 max_char);
 
-/* GetTopmostException.proto */
-#if CYTHON_USE_EXC_INFO_STACK
-static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
-#endif
-
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
 #define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
 #define __Pyx_PyErr_Occurred()  PyErr_Occurred()
 #endif
 
+/* PyErrFetchRestore.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
+#if CYTHON_COMPILING_IN_CPYTHON
+#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
+#else
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#endif
+#else
+#define __Pyx_PyErr_Clear() PyErr_Clear()
+#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
+#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
+#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
+#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
+#endif
+
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
+/* GetTopmostException.proto */
+#if CYTHON_USE_EXC_INFO_STACK
+static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
+#endif
+
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_ExceptionSave(type, value, tb)  __Pyx__ExceptionSave(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionSave(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
@@ -1896,39 +1914,14 @@
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_GetException(type, value, tb)  __Pyx__GetException(__pyx_tstate, type, value, tb)
 static int __Pyx__GetException(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
 #else
 static int __Pyx_GetException(PyObject **type, PyObject **value, PyObject **tb);
 #endif
 
-/* PyErrFetchRestore.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
-#else
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#endif
-#else
-#define __Pyx_PyErr_Clear() PyErr_Clear()
-#define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
-#define __Pyx_ErrRestoreWithState(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
-#define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
-#define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
-#endif
-
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* ArgTypeTest.proto */
 #define __Pyx_ArgTypeTest(obj, type, none_allowed, name, exact)\
     ((likely((Py_TYPE(obj) == type) | (none_allowed && (obj == Py_None)))) ? 1 :\
         __Pyx__ArgTypeTest(obj, type, name, exact))
@@ -2047,14 +2040,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
 }
 
 /* ImportFrom.proto */
@@ -2083,22 +2093,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -4945,15 +4963,15 @@
     __pyx_t_3 = 0;
     __pyx_t_8 = 0;
     __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_7, __pyx_t_12, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 200, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
   }
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 200, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_6))||((__pyx_t_6) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_6)->tp_name), 0))) __PYX_ERR(0, 200, __pyx_L1_error)
   __Pyx_DECREF_SET(__pyx_v_comp_string, ((PyObject*)__pyx_t_6));
   __pyx_t_6 = 0;
 
   /* "src/expam/ext/map/map.pyx":203
  * 
  *     # Classification from lineage(s), with cutoff from alpha.
  *     required_counts = <int>ceil(alpha * kmers.shape[0])             # <<<<<<<<<<<<<<
@@ -6667,15 +6685,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6684,29 +6702,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -6717,15 +6735,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6734,29 +6752,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -6767,15 +6785,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6784,29 +6802,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -6817,15 +6835,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6834,29 +6852,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -6867,15 +6885,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6884,29 +6902,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -6917,212 +6935,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":928
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":932
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":940
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7138,15 +7164,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -7154,84 +7180,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__4, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -7246,15 +7272,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":946
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7270,15 +7296,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7286,84 +7312,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7378,15 +7404,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":952
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7402,15 +7428,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -7418,84 +7444,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__5, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -7510,176 +7536,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":966
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":981
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":996
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -7988,15 +8014,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -9966,15 +9992,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -12269,15 +12295,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -12342,15 +12368,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -15022,15 +15048,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(2, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -20545,15 +20571,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -20845,15 +20871,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static struct __pyx_obj_3map_6_build_3map___pyx_scope_struct_1_genexpr *__pyx_freelist_3map_6_build_3map___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_3map_6_build_3map___pyx_scope_struct_1_genexpr = 0;
 
@@ -20958,15 +20984,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -20987,15 +21013,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -21150,15 +21176,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -21172,15 +21198,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -21272,15 +21298,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -21303,15 +21329,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -21536,15 +21562,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -21556,15 +21582,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -21685,15 +21711,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {"binarysearch", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3map_6_build_3map_1binarysearch, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3map_6_build_3map_binarysearch},
   {"binarysearch_get", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_3map_6_build_3map_5binarysearch_get, METH_VARARGS|METH_KEYWORDS, __pyx_doc_3map_6_build_3map_4binarysearch_get},
@@ -21869,15 +21895,15 @@
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_values, __pyx_k_values, sizeof(__pyx_k_values), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 43, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 941, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
@@ -21886,33 +21912,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__4);
   __Pyx_GIVEREF(__pyx_tuple__4);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__5 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__5);
   __Pyx_GIVEREF(__pyx_tuple__5);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -22199,15 +22225,20 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -22339,55 +22370,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -22572,15 +22587,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_map___build__map) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -23208,18 +23223,16 @@
 
 /* UnpackItemEndCheck */
 static int __Pyx_IternextUnpackEndCheck(PyObject *retval, Py_ssize_t expected) {
     if (unlikely(retval)) {
         Py_DECREF(retval);
         __Pyx_RaiseTooManyValuesError(expected);
         return -1;
-    } else {
-        return __Pyx_IterFinish();
     }
-    return 0;
+    return __Pyx_IterFinish();
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
     return likely(dict) ? __PYX_GET_DICT_VERSION(dict) : 0;
@@ -23592,15 +23605,15 @@
     return result;
 }
 #endif
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -23699,14 +23712,78 @@
 #else
     result_ulength++;
     value_count++;
     return PyUnicode_Join(__pyx_empty_unicode, value_tuple);
 #endif
 }
 
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
+#endif
+
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -23854,38 +23931,14 @@
     *tb = 0;
     Py_XDECREF(local_type);
     Py_XDECREF(local_value);
     Py_XDECREF(local_tb);
     return -1;
 }
 
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-}
-#endif
-
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
                         CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
     Py_XINCREF(type);
     if (!value || value == Py_None)
@@ -24015,28 +24068,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -24866,61 +24919,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -24928,15 +24999,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -26238,15 +26309,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -26392,15 +26463,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -26544,15 +26615,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -26740,15 +26811,15 @@
                         } else if (8 * sizeof(npy_uint16) >= 4 * PyLong_SHIFT) {
                             return (npy_uint16) (((((((((npy_uint16)digits[3]) << PyLong_SHIFT) | (npy_uint16)digits[2]) << PyLong_SHIFT) | (npy_uint16)digits[1]) << PyLong_SHIFT) | (npy_uint16)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27012,15 +27083,15 @@
                         } else if (8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
                             return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27284,15 +27355,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -27480,15 +27551,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -28749,15 +28820,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_Generator_init(void) {
     __pyx_GeneratorType_type.tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
     __pyx_GeneratorType_type.tp_iter = PyObject_SelfIter;
     __pyx_GeneratorType = __Pyx_FetchCommonType(&__pyx_GeneratorType_type);
```

### Comparing `expam-1.2.2/src/expam/ext/map/map.pyx` & `expam-1.2.2.1/src/expam/ext/map/map.pyx`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/ext/sets/_build/src/expam/ext/sets/sets.c` & `expam-1.2.2.1/src/expam/ext/sets/_build/src/expam/ext/sets/sets.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-/* Generated by Cython 0.29.32 */
+/* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "src/expam/ext/sets/mfil.c"
         ],
         "extra_compile_args": [
             "-std=c99"
         ],
         "include_dirs": [
             "src/expam/ext/sets",
-            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/core/include"
+            "/private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/core/include"
         ],
         "name": "sets._build.sets",
         "sources": [
             "src/expam/ext/sets/sets.pyx",
             "src/expam/ext/sets/mfil.c"
         ]
     },
@@ -39,16 +39,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_32"
-#define CYTHON_HEX_VERSION 0x001D20F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -108,24 +108,28 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC (PYPY_VERSION_HEX >= 0x07030900)
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
 #elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -233,15 +237,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -272,15 +276,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -395,17 +399,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -475,14 +476,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -582,35 +588,35 @@
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
 #define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
 #define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
 #if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if defined(PyUnicode_IS_READY)
-  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                              0 : _PyUnicode_Ready((PyObject *)(op)))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_READY(op)       (0)
   #else
-  #define __Pyx_PyUnicode_READY(op)       (0)
+    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                                0 : _PyUnicode_Ready((PyObject *)(op)))
   #endif
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
   #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
   #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
-  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
-  #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+  #if PY_VERSION_HEX >= 0x030C0000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-  #endif
-  #else
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
+    #else
+    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
+    #endif
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
@@ -1126,195 +1132,177 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":689
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":688
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":690
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":689
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":691
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":690
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":692
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":696
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":695
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":697
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":696
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":698
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":697
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":699
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":703
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":702
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":704
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":703
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":713
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":712
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
+ * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":714
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":713
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
- * ctypedef npy_longlong   longlong_t
- * 
- */
-typedef npy_longlong __pyx_t_5numpy_long_t;
-
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":715
- * ctypedef npy_long       int_t
- * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":717
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
+ * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":718
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":716
  * 
  * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
- * ctypedef npy_ulonglong  ulonglong_t
- * 
- */
-typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
-
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":719
- * ctypedef npy_ulong      uint_t
- * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":721
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":722
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":724
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":725
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":726
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":723
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1363,42 +1351,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":728
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":729
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":730
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":732
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1666,26 +1654,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  {\
+#define __Pyx_GetModuleGlobalName(var, name)  do {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
+} while(0)
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-}
+} while(0)
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1792,14 +1780,19 @@
 #define __Pyx_ExceptionReset(type, value, tb)  __Pyx__ExceptionReset(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx__ExceptionReset(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 #else
 #define __Pyx_ExceptionSave(type, value, tb)   PyErr_GetExcInfo(type, value, tb)
 #define __Pyx_ExceptionReset(type, value, tb)  PyErr_SetExcInfo(type, value, tb)
 #endif
 
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
+
 /* PyErrExceptionMatches.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
 static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
 #define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
@@ -1994,14 +1987,31 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_PyList_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
@@ -2033,22 +2043,30 @@
 /* PyObjectGetAttrStrNoError.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
 static int __Pyx_setup_reduce(PyObject* type_obj);
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto
-#define __PYX_HAVE_RT_ImportType_proto
-enum __Pyx_ImportType_CheckSize {
-   __Pyx_ImportType_CheckSize_Error = 0,
-   __Pyx_ImportType_CheckSize_Warn = 1,
-   __Pyx_ImportType_CheckSize_Ignore = 2
+#ifndef __PYX_HAVE_RT_ImportType_proto_0_29_36
+#define __PYX_HAVE_RT_ImportType_proto_0_29_36
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT_0_29_36(s) sizeof(void*)
+#endif
+enum __Pyx_ImportType_CheckSize_0_29_36 {
+   __Pyx_ImportType_CheckSize_Error_0_29_36 = 0,
+   __Pyx_ImportType_CheckSize_Warn_0_29_36 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_0_29_36 = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size);
 #endif
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
@@ -3658,15 +3676,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_sizes, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_temp_arr, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":734
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3675,29 +3693,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":732
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3708,15 +3726,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":737
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3725,29 +3743,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":734
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3758,15 +3776,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":740
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3775,29 +3793,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3808,15 +3826,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":743
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3825,29 +3843,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3858,15 +3876,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":746
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3875,29 +3893,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3908,212 +3926,220 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":749
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":748
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":750
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":753
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":750
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":749
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":928
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
+  int __pyx_t_1;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":926
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":927
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
+  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 927, __pyx_L1_error)
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":925
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
+  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":932
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":932
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":934
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":931
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":936
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":933
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":929
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":940
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4129,15 +4155,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4145,84 +4171,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":939
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 939, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":943
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":940
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 940, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":944
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 941, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 944, __pyx_L5_except_error)
+      __PYX_ERR(1, 941, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":938
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":940
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":937
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4237,15 +4263,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":946
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4261,15 +4287,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4277,84 +4303,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":945
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 945, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":949
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":946
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 946, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":950
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 947, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 950, __pyx_L5_except_error)
+      __PYX_ERR(1, 947, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":944
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":946
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":943
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4369,15 +4395,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":952
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4393,15 +4419,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4409,84 +4435,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":951
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 951, __pyx_L3_error)
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":955
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":952
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 952, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":956
+      /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":953
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 953, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 956, __pyx_L5_except_error)
+      __PYX_ERR(1, 953, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":950
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":952
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":949
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4501,176 +4527,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":966
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":978
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":975
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":966
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":963
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":981
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":993
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":990
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":981
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":978
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":996
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1003
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1000
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":996
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":993
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1010
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1007
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1006
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1003
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+/* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1017
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1014
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":1013
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":1010
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4979,15 +5005,15 @@
   /* "View.MemoryView":141
  *         if not isinstance(format, bytes):
  *             format = format.encode('ASCII')
  *         self._format = format  # keep a reference to the byte string             # <<<<<<<<<<<<<<
  *         self.format = self._format
  * 
  */
-  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
+  if (!(likely(PyBytes_CheckExact(__pyx_v_format))||((__pyx_v_format) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_v_format)->tp_name), 0))) __PYX_ERR(2, 141, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_format;
   __Pyx_INCREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_format);
   __Pyx_DECREF(__pyx_v_self->_format);
   __pyx_v_self->_format = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
@@ -6957,15 +6983,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_Enum__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 17, __pyx_L1_error)
   __pyx_t_1 = __pyx_unpickle_Enum__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
  *         return __pyx_unpickle_Enum, (type(self), 0xb068931, state)
@@ -9260,15 +9286,15 @@
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_6, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 512, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 512, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
 
     /* "View.MemoryView":511
  *         cdef Py_ssize_t i
  * 
  *         if isinstance(value, tuple):             # <<<<<<<<<<<<<<
@@ -9333,15 +9359,15 @@
       PyTuple_SET_ITEM(__pyx_t_8, 1+__pyx_t_7, __pyx_v_value);
       __pyx_t_1 = 0;
       __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_t_8, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 514, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     }
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_t_4))||((__pyx_t_4) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "bytes", Py_TYPE(__pyx_t_4)->tp_name), 0))) __PYX_ERR(2, 514, __pyx_L1_error)
     __pyx_v_bytesvalue = ((PyObject*)__pyx_t_4);
     __pyx_t_4 = 0;
   }
   __pyx_L3:;
 
   /* "View.MemoryView":516
  *             bytesvalue = struct.pack(self.view.format, value)
@@ -12013,15 +12039,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(2, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -17536,15 +17562,15 @@
     /* "(tree fragment)":9
  *     __pyx_result = Enum.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_Enum__set_state(<Enum> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_Enum__set_state(Enum __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||((void)PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(2, 9, __pyx_L1_error)
     __pyx_t_4 = __pyx_unpickle_Enum__set_state(((struct __pyx_MemviewEnum_obj *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_4)) __PYX_ERR(2, 9, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "(tree fragment)":8
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  *     __pyx_result = Enum.__new__(__pyx_type)
@@ -17740,15 +17766,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -17903,15 +17929,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -17925,15 +17951,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -18025,15 +18051,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -18056,15 +18082,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18289,15 +18315,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -18309,15 +18335,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -18438,15 +18464,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -18604,15 +18630,15 @@
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 43, __pyx_L1_error)
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 49, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 941, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
   return 0;
@@ -18620,33 +18646,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":941
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 941, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-dn99qalz/lib/python3.9/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../private/var/folders/t4/14ylkfvd68l_s9gdlgsqsl6s8h4ltf/T/build-env-5jvsuv3w/lib/python3.9/site-packages/numpy/__init__.pxd":947
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 947, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -18933,15 +18959,20 @@
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
@@ -19057,55 +19088,39 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_0_29_36(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(3, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
-   if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 823, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -19290,15 +19305,15 @@
   #endif
   __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_d);
   __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_b);
   __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
   Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Initialize various global constants etc. ---*/
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   if (__pyx_module_is_main_sets___build__sets) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name_2, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
@@ -20256,14 +20271,54 @@
     #endif
     Py_XDECREF(tmp_type);
     Py_XDECREF(tmp_value);
     Py_XDECREF(tmp_tb);
 }
 #endif
 
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+    else state = (PyGILState_STATE)0;
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
+    #if PY_MAJOR_VERSION < 3
+    ctx = PyString_FromString(name);
+    #else
+    ctx = PyUnicode_FromString(name);
+    #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
 /* PyErrExceptionMatches */
 #if CYTHON_FAST_THREAD_STATE
 static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
     for (i=0; i<n; i++) {
@@ -20418,28 +20473,28 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
@@ -20844,15 +20899,15 @@
 #endif
     return PyObject_GetAttr(o, n);
 }
 
 /* ObjectGetItem */
 #if CYTHON_USE_TYPE_SLOTS
 static PyObject *__Pyx_PyObject_GetIndex(PyObject *obj, PyObject* index) {
-    PyObject *runerr;
+    PyObject *runerr = NULL;
     Py_ssize_t key_value;
     PySequenceMethods *m = Py_TYPE(obj)->tp_as_sequence;
     if (unlikely(!(m && m->sq_item))) {
         PyErr_Format(PyExc_TypeError, "'%.200s' object is not subscriptable", Py_TYPE(obj)->tp_name);
         return NULL;
     }
     key_value = __Pyx_PyIndex_AsSsize_t(index);
@@ -21473,61 +21528,79 @@
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 
 /* TypeImport */
-#ifndef __PYX_HAVE_RT_ImportType
-#define __PYX_HAVE_RT_ImportType
-static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+#ifndef __PYX_HAVE_RT_ImportType_0_29_36
+#define __PYX_HAVE_RT_ImportType_0_29_36
+static PyTypeObject *__Pyx_ImportType_0_29_36(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_0_29_36 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
+    if (check_size == __Pyx_ImportType_CheckSize_Error_0_29_36 && (size_t)basicsize != size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_0_29_36 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -21535,15 +21608,15 @@
     Py_XDECREF(result);
     return NULL;
 }
 #endif
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
@@ -22787,15 +22860,15 @@
                         z = __Pyx_c_prod_float(a, a);
                         return __Pyx_c_prod_float(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = powf(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -22941,15 +23014,15 @@
                         z = __Pyx_c_prod_double(a, a);
                         return __Pyx_c_prod_double(z, z);
                 }
             }
             if (a.imag == 0) {
                 if (a.real == 0) {
                     return a;
-                } else if (b.imag == 0) {
+                } else if ((b.imag == 0) && (a.real >= 0)) {
                     z.real = pow(a.real, b.real);
                     z.imag = 0;
                     return z;
                 } else if (a.real > 0) {
                     r = a.real;
                     theta = 0;
                 } else {
@@ -23093,15 +23166,15 @@
                         } else if (8 * sizeof(npy_uint64) >= 4 * PyLong_SHIFT) {
                             return (npy_uint64) (((((((((npy_uint64)digits[3]) << PyLong_SHIFT) | (npy_uint64)digits[2]) << PyLong_SHIFT) | (npy_uint64)digits[1]) << PyLong_SHIFT) | (npy_uint64)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23365,15 +23438,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23599,15 +23672,15 @@
                         } else if (8 * sizeof(npy_int64) >= 4 * PyLong_SHIFT) {
                             return (npy_int64) (((((((((npy_int64)digits[3]) << PyLong_SHIFT) | (npy_int64)digits[2]) << PyLong_SHIFT) | (npy_int64)digits[1]) << PyLong_SHIFT) | (npy_int64)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -23833,15 +23906,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -24029,15 +24102,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `expam-1.2.2/src/expam/ext/sets/mfil.c` & `expam-1.2.2.1/src/expam/ext/sets/mfil.c`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/ext/sets/sets.pyx` & `expam-1.2.2.1/src/expam/ext/sets/sets.pyx`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/logger.py` & `expam-1.2.2.1/src/expam/logger.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/main.py` & `expam-1.2.2.1/src/expam/main.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/process/classify.py` & `expam-1.2.2.1/src/expam/process/classify.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/process/genome.py` & `expam-1.2.2.1/src/expam/process/genome.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/process/jobworker.py` & `expam-1.2.2.1/src/expam/process/jobworker.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/process/manager.py` & `expam-1.2.2.1/src/expam/process/manager.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/process/piler.py` & `expam-1.2.2.1/src/expam/process/piler.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/process/reads.py` & `expam-1.2.2.1/src/expam/process/reads.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/sandbox/main.py` & `expam-1.2.2.1/src/expam/sandbox/main.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/sequences.py` & `expam-1.2.2.1/src/expam/sequences.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/tree/__init__.py` & `expam-1.2.2.1/src/expam/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/tree/location.py` & `expam-1.2.2.1/src/expam/tree/location.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/tree/simulate.py` & `expam-1.2.2.1/src/expam/tree/simulate.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/tree/sourmash.py` & `expam-1.2.2.1/src/expam/tree/sourmash.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/tree/tree.py` & `expam-1.2.2.1/src/expam/tree/tree.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam/utils.py` & `expam-1.2.2.1/src/expam/utils.py`

 * *Files identical despite different names*

### Comparing `expam-1.2.2/src/expam.egg-info/PKG-INFO` & `expam-1.2.2.1/src/expam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expam
-Version: 1.2.2
+Version: 1.2.2.1
 Summary: Metagenomic profiling using a reference phylogeny
 Home-page: https://github.com/seansolari/expam
 Author: Sean Solari
 Author-email: sean.solari@monash.edu
 Project-URL: Bug Reports, https://github.com/seansolari/expam/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `expam-1.2.2/src/expam.egg-info/SOURCES.txt` & `expam-1.2.2.1/src/expam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

