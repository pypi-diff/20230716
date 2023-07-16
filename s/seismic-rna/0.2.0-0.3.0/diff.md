# Comparing `tmp/seismic-rna-0.2.0.tar.gz` & `tmp/seismic-rna-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seismic-rna-0.2.0.tar", last modified: Sat Jul 15 03:49:40 2023, max compression
+gzip compressed data, was "seismic-rna-0.3.0.tar", last modified: Sun Jul 16 01:36:08 2023, max compression
```

## Comparing `seismic-rna-0.2.0.tar` & `seismic-rna-0.3.0.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.506955 seismic-rna-0.2.0/
--rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.2.0/LICENSE
--rw-r--r--   0 mfa        (503) staff       (20)     1930 2023-07-15 03:49:40.506597 seismic-rna-0.2.0/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     1367 2023-07-09 21:54:37.000000 seismic-rna-0.2.0/README.md
--rw-r--r--   0 mfa        (503) staff       (20)     1034 2023-07-14 03:05:41.000000 seismic-rna-0.2.0/pyproject.toml
--rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-15 03:49:40.507065 seismic-rna-0.2.0/setup.cfg
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:39.880285 seismic-rna-0.2.0/src/
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:39.893599 seismic-rna-0.2.0/src/seismic_rna.egg-info/
--rw-r--r--   0 mfa        (503) staff       (20)     1930 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/PKG-INFO
--rw-r--r--   0 mfa        (503) staff       (20)     3014 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/SOURCES.txt
--rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/dependency_links.txt
--rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/entry_points.txt
--rw-r--r--   0 mfa        (503) staff       (20)      176 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/requires.txt
--rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-15 03:49:39.000000 seismic-rna-0.2.0/src/seismic_rna.egg-info/top_level.txt
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:39.909350 seismic-rna-0.2.0/src/seismicrna/
--rw-r--r--   0 mfa        (503) staff       (20)      171 2023-07-07 22:10:20.000000 seismic-rna-0.2.0/src/seismicrna/__init__.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:39.947381 seismic-rna-0.2.0/src/seismicrna/align/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/align/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.2.0/src/seismicrna/align/fq2bam.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-07-09 17:46:17.000000 seismic-rna-0.2.0/src/seismicrna/align/fqutil.py
--rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-07-09 17:46:17.000000 seismic-rna-0.2.0/src/seismicrna/align/main.py
--rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/align/strandedness.py
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/align/test.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.011993 seismic-rna-0.2.0/src/seismicrna/cluster/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    12885 2023-07-11 14:25:48.000000 seismic-rna-0.2.0/src/seismicrna/cluster/compare.py
--rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/em.py
--rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/krun.py
--rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2464 2023-07-12 20:23:19.000000 seismic-rna-0.2.0/src/seismicrna/cluster/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1264 2023-07-15 00:22:05.000000 seismic-rna-0.2.0/src/seismicrna/cluster/names.py
--rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/cluster/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.206074 seismic-rna-0.2.0/src/seismicrna/core/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.2.0/src/seismicrna/core/bitcall.py
--rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.2.0/src/seismicrna/core/bitvect.py
--rw-r--r--   0 mfa        (503) staff       (20)    18246 2023-07-15 03:16:29.000000 seismic-rna-0.2.0/src/seismicrna/core/cli.py
--rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.2.0/src/seismicrna/core/depend.py
--rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/docdef.py
--rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/docstring.py
--rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/dump.py
--rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/files.py
--rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.2.0/src/seismicrna/core/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.2.0/src/seismicrna/core/logs.py
--rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/mu.py
--rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.2.0/src/seismicrna/core/mu_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-07-12 20:28:15.000000 seismic-rna-0.2.0/src/seismicrna/core/parallel.py
--rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.2.0/src/seismicrna/core/path.py
--rw-r--r--   0 mfa        (503) staff       (20)    29387 2023-07-14 20:09:45.000000 seismic-rna-0.2.0/src/seismicrna/core/rel.py
--rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.2.0/src/seismicrna/core/rel_test.py
--rw-r--r--   0 mfa        (503) staff       (20)    29740 2023-07-12 04:26:52.000000 seismic-rna-0.2.0/src/seismicrna/core/report.py
--rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/rna.py
--rw-r--r--   0 mfa        (503) staff       (20)    27329 2023-07-09 16:52:06.000000 seismic-rna-0.2.0/src/seismicrna/core/sect.py
--rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.2.0/src/seismicrna/core/sect_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.2.0/src/seismicrna/core/seq.py
--rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.2.0/src/seismicrna/core/seq_test.py
--rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.2.0/src/seismicrna/core/shell.py
--rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.2.0/src/seismicrna/core/sim.py
--rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.2.0/src/seismicrna/core/sim_test.py
--rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/core/types.py
--rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.2.0/src/seismicrna/core/xam.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.226177 seismic-rna-0.2.0/src/seismicrna/demult/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/demult/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)    42624 2023-07-09 17:46:17.000000 seismic-rna-0.2.0/src/seismicrna/demult/demultiplex.py
--rw-r--r--   0 mfa        (503) staff       (20)     2103 2023-07-09 17:46:17.000000 seismic-rna-0.2.0/src/seismicrna/demult/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.276729 seismic-rna-0.2.0/src/seismicrna/draw/
--rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.2.0/src/seismicrna/draw/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/load_dataset.py
--rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/manipulator.py
--rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.2.0/src/seismicrna/draw/plotter.py
--rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/study.py
--rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/draw/util.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.319723 seismic-rna-0.2.0/src/seismicrna/graph/
--rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/graph/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     8731 2023-07-14 21:02:58.000000 seismic-rna-0.2.0/src/seismicrna/graph/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     3539 2023-07-15 02:04:52.000000 seismic-rna-0.2.0/src/seismicrna/graph/color.py
--rw-r--r--   0 mfa        (503) staff       (20)     2701 2023-07-12 18:10:50.000000 seismic-rna-0.2.0/src/seismicrna/graph/default.py
--rw-r--r--   0 mfa        (503) staff       (20)     7483 2023-07-14 03:47:40.000000 seismic-rna-0.2.0/src/seismicrna/graph/hist.py
--rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/graph/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    13371 2023-07-15 03:18:18.000000 seismic-rna-0.2.0/src/seismicrna/graph/seq.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.326149 seismic-rna-0.2.0/src/seismicrna/logo/
--rw-r--r--   0 mfa        (503) staff       (20)        0 2023-07-09 20:01:37.000000 seismic-rna-0.2.0/src/seismicrna/logo/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3492 2023-07-12 02:42:12.000000 seismic-rna-0.2.0/src/seismicrna/logo/logo.py
--rw-r--r--   0 mfa        (503) staff       (20)     9517 2023-07-12 20:26:39.000000 seismic-rna-0.2.0/src/seismicrna/main.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.361295 seismic-rna-0.2.0/src/seismicrna/mask/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/mask/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     4074 2023-07-08 00:07:16.000000 seismic-rna-0.2.0/src/seismicrna/mask/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     4447 2023-07-09 18:20:20.000000 seismic-rna-0.2.0/src/seismicrna/mask/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/mask/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    14001 2023-07-06 23:57:39.000000 seismic-rna-0.2.0/src/seismicrna/mask/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.430951 seismic-rna-0.2.0/src/seismicrna/relate/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/export.py
--rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     3203 2023-07-09 18:21:57.000000 seismic-rna-0.2.0/src/seismicrna/relate/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/relate.py
--rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/report.py
--rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.2.0/src/seismicrna/relate/sam.py
--rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/seqpos.py
--rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/relate/test.py
--rw-r--r--   0 mfa        (503) staff       (20)    15085 2023-07-10 03:02:51.000000 seismic-rna-0.2.0/src/seismicrna/relate/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.450355 seismic-rna-0.2.0/src/seismicrna/struct/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/struct/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     3937 2023-07-09 20:18:58.000000 seismic-rna-0.2.0/src/seismicrna/struct/main.py
--rw-r--r--   0 mfa        (503) staff       (20)     1850 2023-07-09 19:43:33.000000 seismic-rna-0.2.0/src/seismicrna/struct/rnastructure.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.492896 seismic-rna-0.2.0/src/seismicrna/table/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/table/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)     9414 2023-07-15 00:14:41.000000 seismic-rna-0.2.0/src/seismicrna/table/base.py
--rw-r--r--   0 mfa        (503) staff       (20)     7236 2023-07-15 00:22:19.000000 seismic-rna-0.2.0/src/seismicrna/table/load.py
--rw-r--r--   0 mfa        (503) staff       (20)     1724 2023-07-12 20:21:49.000000 seismic-rna-0.2.0/src/seismicrna/table/main.py
--rw-r--r--   0 mfa        (503) staff       (20)    16181 2023-07-15 00:02:34.000000 seismic-rna-0.2.0/src/seismicrna/table/tabulate.py
--rw-r--r--   0 mfa        (503) staff       (20)     4684 2023-07-15 00:02:34.000000 seismic-rna-0.2.0/src/seismicrna/table/write.py
-drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-15 03:49:40.506089 seismic-rna-0.2.0/src/seismicrna/test/
--rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.2.0/src/seismicrna/test/__init__.py
--rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.2.0/src/seismicrna/test/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.601873 seismic-rna-0.3.0/
+-rw-r--r--   0 mfa        (503) staff       (20)    35150 2023-06-29 02:33:57.000000 seismic-rna-0.3.0/LICENSE
+-rw-r--r--   0 mfa        (503) staff       (20)     1930 2023-07-16 01:36:08.601517 seismic-rna-0.3.0/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     1367 2023-07-09 21:54:37.000000 seismic-rna-0.3.0/README.md
+-rw-r--r--   0 mfa        (503) staff       (20)     1034 2023-07-16 00:38:22.000000 seismic-rna-0.3.0/pyproject.toml
+-rw-r--r--   0 mfa        (503) staff       (20)       38 2023-07-16 01:36:08.601966 seismic-rna-0.3.0/setup.cfg
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.494389 seismic-rna-0.3.0/src/
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.506234 seismic-rna-0.3.0/src/seismic_rna.egg-info/
+-rw-r--r--   0 mfa        (503) staff       (20)     1930 2023-07-16 01:36:08.000000 seismic-rna-0.3.0/src/seismic_rna.egg-info/PKG-INFO
+-rw-r--r--   0 mfa        (503) staff       (20)     3037 2023-07-16 01:36:08.000000 seismic-rna-0.3.0/src/seismic_rna.egg-info/SOURCES.txt
+-rw-r--r--   0 mfa        (503) staff       (20)        1 2023-07-16 01:36:08.000000 seismic-rna-0.3.0/src/seismic_rna.egg-info/dependency_links.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       50 2023-07-16 01:36:08.000000 seismic-rna-0.3.0/src/seismic_rna.egg-info/entry_points.txt
+-rw-r--r--   0 mfa        (503) staff       (20)      176 2023-07-16 01:36:08.000000 seismic-rna-0.3.0/src/seismic_rna.egg-info/requires.txt
+-rw-r--r--   0 mfa        (503) staff       (20)       11 2023-07-16 01:36:08.000000 seismic-rna-0.3.0/src/seismic_rna.egg-info/top_level.txt
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.508908 seismic-rna-0.3.0/src/seismicrna/
+-rw-r--r--   0 mfa        (503) staff       (20)      201 2023-07-16 01:27:23.000000 seismic-rna-0.3.0/src/seismicrna/__init__.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.515519 seismic-rna-0.3.0/src/seismicrna/align/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/align/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    22758 2023-07-05 00:01:54.000000 seismic-rna-0.3.0/src/seismicrna/align/fq2bam.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    20020 2023-07-09 17:46:17.000000 seismic-rna-0.3.0/src/seismicrna/align/fqutil.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7709 2023-07-09 17:46:17.000000 seismic-rna-0.3.0/src/seismicrna/align/main.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)     9115 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/align/strandedness.py
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/align/test.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.523554 seismic-rna-0.3.0/src/seismicrna/cluster/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/cluster/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    13197 2023-07-15 21:12:26.000000 seismic-rna-0.3.0/src/seismicrna/cluster/compare.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18681 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/cluster/em.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6262 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/cluster/krun.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4209 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/cluster/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2464 2023-07-16 00:26:28.000000 seismic-rna-0.3.0/src/seismicrna/cluster/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1264 2023-07-15 00:22:05.000000 seismic-rna-0.3.0/src/seismicrna/cluster/names.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2862 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/cluster/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4981 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/cluster/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.555282 seismic-rna-0.3.0/src/seismicrna/core/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/core/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15704 2023-06-29 18:01:10.000000 seismic-rna-0.3.0/src/seismicrna/core/bitcall.py
+-rw-r--r--   0 mfa        (503) staff       (20)    19264 2023-07-07 22:07:51.000000 seismic-rna-0.3.0/src/seismicrna/core/bitvect.py
+-rw-r--r--   0 mfa        (503) staff       (20)    18191 2023-07-16 00:30:24.000000 seismic-rna-0.3.0/src/seismicrna/core/cli.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1120 2023-06-29 21:48:51.000000 seismic-rna-0.3.0/src/seismicrna/core/depend.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6844 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/core/docdef.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2201 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/core/docstring.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1972 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/core/dump.py
+-rw-r--r--   0 mfa        (503) staff       (20)      628 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/core/files.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7933 2023-07-07 22:47:51.000000 seismic-rna-0.3.0/src/seismicrna/core/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2837 2023-07-07 02:37:13.000000 seismic-rna-0.3.0/src/seismicrna/core/logs.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14124 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/core/mu.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10537 2023-06-30 18:53:43.000000 seismic-rna-0.3.0/src/seismicrna/core/mu_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14509 2023-07-12 20:28:15.000000 seismic-rna-0.3.0/src/seismicrna/core/parallel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    23511 2023-07-07 00:11:58.000000 seismic-rna-0.3.0/src/seismicrna/core/path.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29387 2023-07-14 20:09:45.000000 seismic-rna-0.3.0/src/seismicrna/core/rel.py
+-rw-r--r--   0 mfa        (503) staff       (20)    45953 2023-06-30 18:58:01.000000 seismic-rna-0.3.0/src/seismicrna/core/rel_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    29740 2023-07-12 04:26:52.000000 seismic-rna-0.3.0/src/seismicrna/core/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9169 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/core/rna.py
+-rw-r--r--   0 mfa        (503) staff       (20)    27329 2023-07-09 16:52:06.000000 seismic-rna-0.3.0/src/seismicrna/core/sect.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7101 2023-07-06 00:49:26.000000 seismic-rna-0.3.0/src/seismicrna/core/sect_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9798 2023-06-30 03:50:29.000000 seismic-rna-0.3.0/src/seismicrna/core/seq.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6634 2023-06-30 14:56:23.000000 seismic-rna-0.3.0/src/seismicrna/core/seq_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2799 2023-06-29 21:49:14.000000 seismic-rna-0.3.0/src/seismicrna/core/shell.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1054 2023-06-29 19:54:35.000000 seismic-rna-0.3.0/src/seismicrna/core/sim.py
+-rw-r--r--   0 mfa        (503) staff       (20)      769 2023-07-06 00:49:45.000000 seismic-rna-0.3.0/src/seismicrna/core/sim_test.py
+-rw-r--r--   0 mfa        (503) staff       (20)      758 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/core/types.py
+-rwxr-xr-x   0 mfa        (503) staff       (20)    14291 2023-06-30 03:36:23.000000 seismic-rna-0.3.0/src/seismicrna/core/xam.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.558154 seismic-rna-0.3.0/src/seismicrna/demult/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/demult/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)    42624 2023-07-09 17:46:17.000000 seismic-rna-0.3.0/src/seismicrna/demult/demultiplex.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2103 2023-07-09 17:46:17.000000 seismic-rna-0.3.0/src/seismicrna/demult/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.565189 seismic-rna-0.3.0/src/seismicrna/draw/
+-rw-r--r--   0 mfa        (503) staff       (20)      256 2023-06-29 19:38:33.000000 seismic-rna-0.3.0/src/seismicrna/draw/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      225 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/draw/load_dataset.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6013 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/draw/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     6656 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/draw/manipulator.py
+-rw-r--r--   0 mfa        (503) staff       (20)    17447 2023-06-29 19:43:29.000000 seismic-rna-0.3.0/src/seismicrna/draw/plotter.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15931 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/draw/study.py
+-rw-r--r--   0 mfa        (503) staff       (20)    11285 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/draw/util.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.571697 seismic-rna-0.3.0/src/seismicrna/graph/
+-rw-r--r--   0 mfa        (503) staff       (20)       22 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/graph/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     8731 2023-07-14 21:02:58.000000 seismic-rna-0.3.0/src/seismicrna/graph/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3539 2023-07-15 02:04:52.000000 seismic-rna-0.3.0/src/seismicrna/graph/color.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2701 2023-07-12 18:10:50.000000 seismic-rna-0.3.0/src/seismicrna/graph/default.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7493 2023-07-16 00:28:27.000000 seismic-rna-0.3.0/src/seismicrna/graph/hist.py
+-rw-r--r--   0 mfa        (503) staff       (20)      337 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/graph/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    13371 2023-07-16 00:27:55.000000 seismic-rna-0.3.0/src/seismicrna/graph/seq.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.573767 seismic-rna-0.3.0/src/seismicrna/logo/
+-rw-r--r--   0 mfa        (503) staff       (20)        0 2023-07-09 20:01:37.000000 seismic-rna-0.3.0/src/seismicrna/logo/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3492 2023-07-12 02:42:12.000000 seismic-rna-0.3.0/src/seismicrna/logo/logo.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9616 2023-07-16 01:27:58.000000 seismic-rna-0.3.0/src/seismicrna/main.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.580061 seismic-rna-0.3.0/src/seismicrna/mask/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/mask/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4074 2023-07-08 00:07:16.000000 seismic-rna-0.3.0/src/seismicrna/mask/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4447 2023-07-16 00:26:07.000000 seismic-rna-0.3.0/src/seismicrna/mask/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1315 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/mask/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    14222 2023-07-15 22:36:16.000000 seismic-rna-0.3.0/src/seismicrna/mask/write.py
+-rw-r--r--   0 mfa        (503) staff       (20)      164 2023-07-16 01:29:14.000000 seismic-rna-0.3.0/src/seismicrna/meta.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.589424 seismic-rna-0.3.0/src/seismicrna/relate/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/relate/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1413 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/relate/export.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3241 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/relate/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3203 2023-07-16 00:25:12.000000 seismic-rna-0.3.0/src/seismicrna/relate/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    28055 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/relate/relate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1509 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/relate/report.py
+-rw-r--r--   0 mfa        (503) staff       (20)    10170 2023-06-30 02:27:38.000000 seismic-rna-0.3.0/src/seismicrna/relate/sam.py
+-rw-r--r--   0 mfa        (503) staff       (20)     2984 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/relate/seqpos.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3066 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/relate/test.py
+-rw-r--r--   0 mfa        (503) staff       (20)    15085 2023-07-10 03:02:51.000000 seismic-rna-0.3.0/src/seismicrna/relate/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.592441 seismic-rna-0.3.0/src/seismicrna/struct/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/struct/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     3937 2023-07-16 00:27:31.000000 seismic-rna-0.3.0/src/seismicrna/struct/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1850 2023-07-09 19:43:33.000000 seismic-rna-0.3.0/src/seismicrna/struct/rnastructure.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.598863 seismic-rna-0.3.0/src/seismicrna/table/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/table/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)     9414 2023-07-15 00:14:41.000000 seismic-rna-0.3.0/src/seismicrna/table/base.py
+-rw-r--r--   0 mfa        (503) staff       (20)     7236 2023-07-15 00:22:19.000000 seismic-rna-0.3.0/src/seismicrna/table/load.py
+-rw-r--r--   0 mfa        (503) staff       (20)     1724 2023-07-16 00:27:03.000000 seismic-rna-0.3.0/src/seismicrna/table/main.py
+-rw-r--r--   0 mfa        (503) staff       (20)    16181 2023-07-15 00:02:34.000000 seismic-rna-0.3.0/src/seismicrna/table/tabulate.py
+-rw-r--r--   0 mfa        (503) staff       (20)     4684 2023-07-15 00:02:34.000000 seismic-rna-0.3.0/src/seismicrna/table/write.py
+drwxr-xr-x   0 mfa        (503) staff       (20)        0 2023-07-16 01:36:08.600729 seismic-rna-0.3.0/src/seismicrna/test/
+-rw-r--r--   0 mfa        (503) staff       (20)       35 2023-06-29 02:17:49.000000 seismic-rna-0.3.0/src/seismicrna/test/__init__.py
+-rw-r--r--   0 mfa        (503) staff       (20)      971 2023-07-06 00:56:02.000000 seismic-rna-0.3.0/src/seismicrna/test/main.py
```

### Comparing `seismic-rna-0.2.0/LICENSE` & `seismic-rna-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/PKG-INFO` & `seismic-rna-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.2.0
+Version: 0.3.0
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `seismic-rna-0.2.0/README.md` & `seismic-rna-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/pyproject.toml` & `seismic-rna-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "seismic-rna"
-version = "0.2.0"
+version = "0.3.0"
 authors = [
     {name="Matty Allan"},
     {name="Yves Martin"},
     {name="Scott Grote"},
     {name="Alberic de Lajarte"},
 ]
 description = "RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering"
```

### Comparing `seismic-rna-0.2.0/src/seismic_rna.egg-info/PKG-INFO` & `seismic-rna-0.3.0/src/seismic_rna.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seismic-rna
-Version: 0.2.0
+Version: 0.3.0
 Summary: RNA Structure Ensemble Inference via Sequencing, Mutation Identification, and Clustering
 Author: Matty Allan, Yves Martin, Scott Grote, Alberic de Lajarte
 License: GPL-3.0-only
 Project-URL: Homepage, https://github.com/rouskinlab/seismic-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/seismic-rna/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `seismic-rna-0.2.0/src/seismic_rna.egg-info/SOURCES.txt` & `seismic-rna-0.3.0/src/seismic_rna.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/seismic_rna.egg-info/SOURCES.txt
 src/seismic_rna.egg-info/dependency_links.txt
 src/seismic_rna.egg-info/entry_points.txt
 src/seismic_rna.egg-info/requires.txt
 src/seismic_rna.egg-info/top_level.txt
 src/seismicrna/__init__.py
 src/seismicrna/main.py
+src/seismicrna/meta.py
 src/seismicrna/align/__init__.py
 src/seismicrna/align/fq2bam.py
 src/seismicrna/align/fqutil.py
 src/seismicrna/align/main.py
 src/seismicrna/align/strandedness.py
 src/seismicrna/align/test.py
 src/seismicrna/cluster/__init__.py
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/align/fq2bam.py` & `seismic-rna-0.3.0/src/seismicrna/align/fq2bam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/align/fqutil.py` & `seismic-rna-0.3.0/src/seismicrna/align/fqutil.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/align/main.py` & `seismic-rna-0.3.0/src/seismicrna/align/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/align/strandedness.py` & `seismic-rna-0.3.0/src/seismicrna/align/strandedness.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/cluster/compare.py` & `seismic-rna-0.3.0/src/seismicrna/cluster/compare.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Auth: Matty
 
 Collect and compare the results from independent runs of EM clustering.
 """
 
 from __future__ import annotations
 
-from itertools import combinations
+from itertools import combinations, islice
 from typing import Callable, Iterable
 
 import numpy as np
 import pandas as pd
 
 from .em import EmClustering
 from .names import EXP_NAME, OBS_NAME, ORD_NAME
@@ -86,15 +86,15 @@
 
 
 def format_exp_count_col(order: int):
     return f"{EXP_NAME}, {ORD_NAME} {order}"
 
 
 def get_log_exp_obs_counts(ord_runs: dict[int, RunOrderResults]):
-    """ Compute the expected and observed log counts. """
+    """ Get the expected and observed log counts of each bit vector. """
     # Retrieve the unique bit vectors from the clusters.
     uniq_muts = get_common_best_run_attr(ord_runs, "muts")
     # Compute the observed log counts of the bit vectors.
     log_obs = pd.Series(np.log(uniq_muts.counts),
                         index=uniq_muts.get_uniq_names())
     # For each order of clustering, compute the expected log counts.
     log_exp = ((format_exp_count_col(order),
@@ -263,15 +263,15 @@
                 # weighted series.
                 inner = iter(self._inner())
                 weighted = iter(ival - self._weight for ival in self._inner())
                 # Get the first element from each iterator. Both should
                 # have > 0 items and should not raise StopIteration.
                 ival = next(inner)
                 wval = next(weighted)
-                # Yield elements until the both iterators are exhausted.
+                # Yield elements until both iterators are exhausted.
                 while True:
                     # Yield the larger value and advance its iterator.
                     if ival is not None and ival >= wval:
                         # Yield the inner value.
                         yield self._cache(ival)
                         # Get the next inner value, or None if empty.
                         ival = next(inner, None)
@@ -297,7 +297,17 @@
     # Make series of log likelihoods.
     series = LikelihoodSeries(log_diffs[0], lambda: [0.])
     for log_diff in log_diffs[1:]:
         series = LikelihoodSeries(log_diff, series.iter)
 
     # Return an iterator of log likelihood values adjusted by the base.
     return iter(value + log_base for value in series.iter())
+
+
+def max_n_likelihoods(p: np.ndarray, n: int | None = None):
+    """ Return the top n bit vector likelihoods. """
+    return np.array(list(islice(iter_all_likelihoods(p), n)))
+
+
+def cum_log_exp_obs_counts():
+    """ Get the cumulative expected and observed log counts per bit
+    vector. """
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/cluster/em.py` & `seismic-rna-0.3.0/src/seismicrna/cluster/em.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/cluster/krun.py` & `seismic-rna-0.3.0/src/seismicrna/cluster/krun.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/cluster/load.py` & `seismic-rna-0.3.0/src/seismicrna/cluster/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/cluster/main.py` & `seismic-rna-0.3.0/src/seismicrna/cluster/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from logging import getLogger
 from pathlib import Path
 
 from click import command
 
 from .krun import cluster
 from ..core import docdef, path
-from ..core.cli import (opt_input_file, opt_max_clusters, opt_em_runs,
+from ..core.cli import (arg_input_file, opt_max_clusters, opt_em_runs,
                         opt_min_em_iter, opt_max_em_iter, opt_em_thresh,
                         opt_parallel, opt_max_procs, opt_rerun)
 from ..core.parallel import as_list_of_tuples, dispatch
 
 logger = getLogger(__name__)
 
 DEFAULT_ORDER = 2
 
 params = [
     # Input files
-    opt_input_file,
+    arg_input_file,
     # Clustering options
     opt_max_clusters,
     opt_em_runs,
     opt_min_em_iter,
     opt_max_em_iter,
     opt_em_thresh,
     # Parallelization
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/cluster/names.py` & `seismic-rna-0.3.0/src/seismicrna/cluster/names.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/cluster/report.py` & `seismic-rna-0.3.0/src/seismicrna/cluster/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/cluster/write.py` & `seismic-rna-0.3.0/src/seismicrna/cluster/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/bitcall.py` & `seismic-rna-0.3.0/src/seismicrna/core/bitcall.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/bitvect.py` & `seismic-rna-0.3.0/src/seismicrna/core/bitvect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/cli.py` & `seismic-rna-0.3.0/src/seismicrna/core/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Define all command line interface (CLI) options and their defaults.
 """
 
 from datetime import datetime
 import logging
 import os
 
-from click import Choice, Option, Parameter, Path
+from click import Argument, Choice, Option, Parameter, Path
 
 # System information
 CWD = os.getcwd()
 if (NUM_CPUS := os.cpu_count()) is None:
     logging.warning("Failed to determine CPU count: defaulting to 1")
     NUM_CPUS = 1
 
@@ -38,20 +38,18 @@
 opt_config = Option(
     ("--config", "-g"),
     type=Path(exists=True, dir_okay=False),
     help="Configuration file for parameters")
 
 # Input/output options
 
-opt_input_file = Option(
-    ("--input-file", "-i"),
+arg_input_file = Argument(
+    ("input-file",),
     type=Path(exists=True),
-    multiple=True,
-    default=(),
-    help="File containing input data")
+    nargs=-1)
 
 opt_out_dir = Option(
     ("--out-dir", "-o"),
     type=Path(file_okay=False),
     default=os.path.join(".", "out"),
     help="Where to output all finished files")
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/depend.py` & `seismic-rna-0.3.0/src/seismicrna/core/depend.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/docdef.py` & `seismic-rna-0.3.0/src/seismicrna/core/docdef.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/docstring.py` & `seismic-rna-0.3.0/src/seismicrna/core/docstring.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/dump.py` & `seismic-rna-0.3.0/src/seismicrna/core/dump.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/files.py` & `seismic-rna-0.3.0/src/seismicrna/core/files.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/load.py` & `seismic-rna-0.3.0/src/seismicrna/core/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/logs.py` & `seismic-rna-0.3.0/src/seismicrna/core/logs.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/mu.py` & `seismic-rna-0.3.0/src/seismicrna/core/mu.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/mu_test.py` & `seismic-rna-0.3.0/src/seismicrna/core/mu_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/parallel.py` & `seismic-rna-0.3.0/src/seismicrna/core/parallel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/path.py` & `seismic-rna-0.3.0/src/seismicrna/core/path.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/rel.py` & `seismic-rna-0.3.0/src/seismicrna/core/rel.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/rel_test.py` & `seismic-rna-0.3.0/src/seismicrna/core/rel_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/report.py` & `seismic-rna-0.3.0/src/seismicrna/core/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/rna.py` & `seismic-rna-0.3.0/src/seismicrna/core/rna.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/sect.py` & `seismic-rna-0.3.0/src/seismicrna/core/sect.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/sect_test.py` & `seismic-rna-0.3.0/src/seismicrna/core/sect_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/seq.py` & `seismic-rna-0.3.0/src/seismicrna/core/seq.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/seq_test.py` & `seismic-rna-0.3.0/src/seismicrna/core/seq_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/shell.py` & `seismic-rna-0.3.0/src/seismicrna/core/shell.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/sim.py` & `seismic-rna-0.3.0/src/seismicrna/core/sim.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/sim_test.py` & `seismic-rna-0.3.0/src/seismicrna/core/sim_test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/types.py` & `seismic-rna-0.3.0/src/seismicrna/core/types.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/core/xam.py` & `seismic-rna-0.3.0/src/seismicrna/core/xam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/demult/demultiplex.py` & `seismic-rna-0.3.0/src/seismicrna/demult/demultiplex.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/demult/main.py` & `seismic-rna-0.3.0/src/seismicrna/demult/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/draw/main.py` & `seismic-rna-0.3.0/src/seismicrna/draw/main.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/draw/manipulator.py` & `seismic-rna-0.3.0/src/seismicrna/draw/manipulator.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/draw/plotter.py` & `seismic-rna-0.3.0/src/seismicrna/draw/plotter.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/draw/study.py` & `seismic-rna-0.3.0/src/seismicrna/draw/study.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/draw/util.py` & `seismic-rna-0.3.0/src/seismicrna/draw/util.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/graph/base.py` & `seismic-rna-0.3.0/src/seismicrna/graph/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/graph/color.py` & `seismic-rna-0.3.0/src/seismicrna/graph/color.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/graph/default.py` & `seismic-rna-0.3.0/src/seismicrna/graph/default.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/graph/hist.py` & `seismic-rna-0.3.0/src/seismicrna/graph/hist.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 from click import command
 from plotly import graph_objects as go
 
 from .base import (find_tables, GraphWriter, CartesianGraph, OneTableGraph,
                    OneSampGraph)
 from .color import RelColorMap
 from ..core import docdef
-from ..core.cli import (opt_table, opt_rels,
+from ..core.cli import (arg_input_file, opt_rels,
                         opt_y_ratio, opt_hist_bins,
                         opt_csv, opt_html, opt_pdf,
                         opt_max_procs, opt_parallel)
 from ..core.parallel import dispatch
 from ..table.base import Table
 from ..table.load import (RelReadTableLoader,
                           MaskReadTableLoader, ClustReadTableLoader)
 
 # Number of digits to which to round decimals.
 PRECISION = 6
 
 params = [
-    opt_table,
+    arg_input_file,
     opt_rels,
     opt_hist_bins,
     opt_y_ratio,
     opt_csv,
     opt_html,
     opt_pdf,
     opt_max_procs,
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/graph/seq.py` & `seismic-rna-0.3.0/src/seismicrna/graph/seq.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .base import (PRECISION, find_tables, GraphWriter, CartesianGraph,
                    OneTableSeqGraph, OneSampGraph)
 from .color import ColorMap, RelColorMap, SeqColorMap
 from ..cluster.names import (ENSEMBLE_NAME, CLS_NAME, ORD_NAME, ORD_CLS_NAME,
                              fmt_clust_name, validate_order_cluster)
 from ..core import docdef
-from ..core.cli import (opt_input_file, opt_rels,
+from ..core.cli import (arg_input_file, opt_rels,
                         opt_stack, opt_arrange, opt_y_ratio,
                         opt_csv, opt_html, opt_pdf, opt_max_procs, opt_parallel,
                         CLUST_INDIV, CLUST_UNITE, CLUST_ORDER)
 from ..core.parallel import dispatch
 from ..core.sect import BASE_NAME, POS_NAME
 from ..core.seq import BASES
 from ..table.base import REL_CODES, REL_NAME
@@ -27,15 +27,15 @@
                           MaskPosTableLoader, ClustPosTableLoader)
 
 logger = getLogger(__name__)
 
 # Number of digits to which to round decimals.
 
 params = [
-    opt_input_file,
+    arg_input_file,
     opt_rels,
     opt_stack,
     opt_arrange,
     opt_y_ratio,
     opt_csv,
     opt_html,
     opt_pdf,
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/logo/logo.py` & `seismic-rna-0.3.0/src/seismicrna/logo/logo.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/main.py` & `seismic-rna-0.3.0/src/seismicrna/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
                table as table_mod,
                struct as fold_mod,
                graph as graph_mod,
                test as test_mod)
 from .core import docdef, logs
 from .core.cli import (merge_params, opt_demultiplex,
                        opt_verbose, opt_quiet, opt_log, opt_profile, opt_fold)
+from .meta import __version__
 
 all_params = merge_params([opt_demultiplex],
                           demultiplex_mod.params,
                           align_mod.params,
                           relate_mod.params,
                           mask_mod.params,
                           cluster_mod.params,
@@ -32,38 +33,39 @@
     """ Run 'align', 'relate', 'mask', (optionally) 'cluster', 'table',
     (optionally) 'fold', and (optionally) 'graph', in that order. """
     return run(*args, **kwargs)
 
 
 @docdef.auto()
 def run(*,
+        # Arguments
+        input_file: tuple[str, ...],
         # General options
         out_dir: str,
         temp_dir: str,
         save_temp: bool,
         rerun: bool,
         max_procs: int,
         parallel: bool,
-        # Input files
-        input_file: tuple[str, ...],
+        # FASTQ options
         fasta: str,
         fastqs: tuple[str, ...],
         fastqi: tuple[str, ...],
         fastqp: tuple[str, ...],
         phred_enc: int,
-        # Demultiplexing
+        # Demultiplexing options
         demulti_overwrite: bool,
         demult_on: bool,
         parallel_demultiplexing: bool,
         clipped: int,
         mismatch_tolerence: int,
         index_tolerance: int,
         barcode_start: int,
         barcode_length: int,
-        # Alignment
+        # Align options
         dmfastqs: tuple[str, ...],
         dmfastqi: tuple[str, ...],
         dmfastqp: tuple[str, ...],
         fastqc: bool,
         qc_extract: bool,
         cut: bool,
         cut_q1: int,
@@ -92,20 +94,20 @@
         bt2_gbar: int,
         bt2_l: int,
         bt2_s: str,
         bt2_d: int,
         bt2_r: int,
         bt2_dpad: int,
         bt2_orient: str,
-        # Relating
+        # Relate options
         min_phred: int,
         min_reads: int,
         ambrel: bool,
         batch_size: float,
-        # Masking
+        # Mask options
         coords: tuple[tuple[str, int, int], ...],
         primers: tuple[tuple[str, str, str], ...],
         primer_gap: int,
         sections_file: str,
         count_del: bool,
         count_ins: bool,
         discount_mut: tuple[str, ...],
@@ -113,23 +115,23 @@
         exclude_gu: bool,
         exclude_pos: tuple[tuple[str, int], ...],
         min_finfo_read: float,
         max_fmut_read: int,
         min_mut_gap: int,
         min_ninfo_pos: int,
         max_fmut_pos: float,
-        # Clustering
+        # Cluster options
         max_clusters: int,
         em_runs: int,
         min_em_iter: int,
         max_em_iter: int,
         em_thresh: float,
-        # Tabulation
+        # Table options
         rels: str,
-        # Folding
+        # Fold options
         fold: bool,
         quantile: float):
     """ Run entire pipeline. """
     # Demultiplexing
     if demult_on:
         for dms, dmi, dmm in demultiplex_mod.run(
                 fasta=fasta,
@@ -281,15 +283,15 @@
     opt_log,
     opt_profile,
 ]
 
 
 # Group for main commands
 @group(params=main_params, context_settings={"show_default": True})
-@version_option()
+@version_option(__version__)
 @pass_context
 def main_cli(ctx: Context, verbose: int, quiet: int, log: str, profile: str,
              **kwargs):
     """ SEISMIC-RNA command line interface """
     # Configure logging.
     os.makedirs(os.path.dirname(log), exist_ok=True)
     logs.config(verbose, quiet, log_file=log)
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/mask/load.py` & `seismic-rna-0.3.0/src/seismicrna/mask/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/mask/main.py` & `seismic-rna-0.3.0/src/seismicrna/mask/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 from typing import Iterable
 
 from click import command
 
 from .write import mask_section
 from ..relate.load import open_reports
 from ..core import docdef, path
-from ..core.cli import (opt_input_file,
+from ..core.cli import (arg_input_file,
                         opt_coords, opt_primers, opt_primer_gap, opt_sections_file,
                         opt_count_del, opt_count_ins, opt_discount_mut,
                         opt_exclude_polya, opt_exclude_gu, opt_exclude_pos,
                         opt_min_finfo_read, opt_max_fmut_read, opt_min_mut_gap,
                         opt_min_ninfo_pos, opt_max_fmut_pos,
                         opt_max_procs, opt_parallel, opt_rerun)
 from ..core.parallel import dispatch
 from ..core.sect import encode_primers, RefSections
 from ..core.seq import DNA
 
 logger = getLogger(__name__)
 
 params = [
     # Input/output paths
-    opt_input_file,
+    arg_input_file,
     # Sections
     opt_coords, opt_primers, opt_primer_gap, opt_sections_file,
     # Mutation counting
     opt_count_del, opt_count_ins, opt_discount_mut,
     # Filtering
     opt_exclude_polya, opt_exclude_gu, opt_exclude_pos,
     opt_min_finfo_read, opt_max_fmut_read, opt_min_mut_gap,
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/mask/report.py` & `seismic-rna-0.3.0/src/seismicrna/mask/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/mask/write.py` & `seismic-rna-0.3.0/src/seismicrna/mask/write.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
     def __init__(self,
                  loader: RelateLoader,
                  section: Section,
                  bit_caller: BitCaller, *,
                  exclude_polya: int = 0,
                  exclude_gu: bool = False,
-                 exclude_pos: Iterable[int] = (),
+                 exclude_pos: Iterable[tuple[str, int]] = (),
                  min_mut_gap: int = 0,
                  min_finfo_read: float = 0.,
                  max_fmut_read: float = 1.,
                  min_ninfo_pos: int = 0,
                  max_fmut_pos: float = 1.):
         """
         Parameters
@@ -67,16 +67,17 @@
         bit_caller: BitCaller
             Bit caller
         exclude_polya: int = 0
             Exclude stretches of consecutive A bases at least this long.
             If 0, exclude no bases. Must be ≥ 0.
         exclude_gu: bool = False
             Whether to exclude G and U bases.
-        exclude_pos: Iterable[int] = ()
-            Additional, arbitrary positions to exclude.
+        exclude_pos: Iterable[tuple[str, int]] = ()
+            Additional, arbitrary positions to exclude. Each position
+            must be a tuple of (reference name, 1-indexed position).
         min_mut_gap: int = 0
             Filter out reads with any two mutations separated by fewer
             than `min_mut_gap` positions. Adjacent mutations have a
             gap of 0. If 0, keep all. Must be in [0, length_of_section).
         min_finfo_read: float = 0.0
             Filter out reads with less than this fraction of informative
             bases (i.e. match or mutation). If 0.0, keep all. Must be in
@@ -98,15 +99,17 @@
         # Create a new section to compute the masked positions.
         self.section = Section(loader.ref, loader.get_refseq(),
                                end5=section.end5, end3=section.end3,
                                name=section.name)
         # Set the parameters for excluding positions from the section.
         self.exclude_polya = exclude_polya
         self.exclude_gu = exclude_gu
-        self.exclude_pos = np.array(exclude_pos, dtype=int)
+        self.exclude_pos = np.array([pos for ref, pos in exclude_pos
+                                     if ref == self.ref],
+                                    dtype=int)
         # Set the parameters for filtering reads.
         self.min_mut_gap = min_mut_gap
         self.min_finfo_read = min_finfo_read
         self.max_fmut_read = max_fmut_read
         # Set the parameters for filtering positions.
         if not min_ninfo_pos >= 0:
             raise ValueError(
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/export.py` & `seismic-rna-0.3.0/src/seismicrna/relate/export.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/load.py` & `seismic-rna-0.3.0/src/seismicrna/relate/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/main.py` & `seismic-rna-0.3.0/src/seismicrna/relate/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,29 +10,29 @@
 from logging import getLogger
 from pathlib import Path
 
 from click import command
 
 from .write import relate_all, get_relaters
 from ..core import docdef, path
-from ..core.cli import (opt_fasta, opt_input_file,
+from ..core.cli import (arg_input_file, opt_fasta,
                         opt_out_dir, opt_temp_dir,
                         opt_phred_enc, opt_min_phred,
                         opt_min_reads, opt_batch_size, opt_ambrel,
                         opt_parallel, opt_max_procs,
                         opt_rerun, opt_save_temp)
 from ..core.parallel import lock_temp_dir
 
 logger = getLogger(__name__)
 
 # Parameters for command line interface
 params = [
     # Input files
+    arg_input_file,
     opt_fasta,
-    opt_input_file,
     # Output directories
     opt_out_dir,
     opt_temp_dir,
     # SAM options
     opt_phred_enc,
     opt_min_phred,
     # Vectoring options
@@ -53,16 +53,16 @@
     """ For every read, find the relationship between each read base and
     the reference base to which it aligned. """
     return run(**kwargs)
 
 
 @lock_temp_dir
 @docdef.auto()
-def run(fasta: str,
-        input_file: tuple[str, ...],
+def run(input_file: tuple[str, ...],
+        fasta: str,
         *,
         out_dir: str,
         temp_dir: str,
         phred_enc: int,
         min_phred: int,
         min_reads: int,
         batch_size: float,
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/relate.py` & `seismic-rna-0.3.0/src/seismicrna/relate/relate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/report.py` & `seismic-rna-0.3.0/src/seismicrna/relate/report.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/sam.py` & `seismic-rna-0.3.0/src/seismicrna/relate/sam.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/seqpos.py` & `seismic-rna-0.3.0/src/seismicrna/relate/seqpos.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/test.py` & `seismic-rna-0.3.0/src/seismicrna/relate/test.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/relate/write.py` & `seismic-rna-0.3.0/src/seismicrna/relate/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/struct/main.py` & `seismic-rna-0.3.0/src/seismicrna/struct/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from logging import getLogger
 from pathlib import Path
 
 from click import command
 
 from .rnastructure import fold, ct2dot
 from ..core import docdef, path
-from ..core.cli import (opt_temp_dir, opt_save_temp, opt_input_file,
+from ..core.cli import (arg_input_file, opt_temp_dir, opt_save_temp,
                         opt_fasta, opt_sections_file,
                         opt_coords, opt_primers, opt_primer_gap,
                         opt_quantile,
                         opt_max_procs, opt_parallel, opt_rerun)
 from ..core.depend import confirm_dependency
 from ..core.parallel import as_list_of_tuples, dispatch, lock_temp_dir
 from ..core.rna import RnaProfile
@@ -17,15 +17,15 @@
 from ..core.seq import parse_fasta
 from ..core.shell import RNASTRUCTURE_FOLD_CMD
 from ..table.load import load, MaskPosTableLoader, ClustPosTableLoader
 
 logger = getLogger(__name__)
 
 params = [
-    opt_input_file,
+    arg_input_file,
     opt_fasta,
     opt_sections_file,
     opt_coords,
     opt_primers,
     opt_primer_gap,
     opt_quantile,
     opt_temp_dir,
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/struct/rnastructure.py` & `seismic-rna-0.3.0/src/seismicrna/struct/rnastructure.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/table/base.py` & `seismic-rna-0.3.0/src/seismicrna/table/base.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/table/load.py` & `seismic-rna-0.3.0/src/seismicrna/table/load.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/table/main.py` & `seismic-rna-0.3.0/src/seismicrna/table/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 from logging import getLogger
 from pathlib import Path
 
 from click import command
 
 from .write import write
 from ..core import docdef, path
-from ..core.cli import (opt_input_file, opt_rels,
+from ..core.cli import (arg_input_file, opt_rels,
                         opt_max_procs, opt_parallel, opt_rerun)
 from ..core.parallel import dispatch
 
 logger = getLogger(__name__)
 
-params = [opt_input_file, opt_rels, opt_max_procs, opt_parallel, opt_rerun]
+params = [arg_input_file, opt_rels, opt_max_procs, opt_parallel, opt_rerun]
 
 
 @command(path.MOD_TABLE, params=params)
 def cli(*args, **kwargs):
     """ Tabulate per-base and per-read mutation counts from 'relate' and
     'mask', and mutation rates and read memberships from 'cluster'. """
     return run(*args, **kwargs)
```

### Comparing `seismic-rna-0.2.0/src/seismicrna/table/tabulate.py` & `seismic-rna-0.3.0/src/seismicrna/table/tabulate.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/table/write.py` & `seismic-rna-0.3.0/src/seismicrna/table/write.py`

 * *Files identical despite different names*

### Comparing `seismic-rna-0.2.0/src/seismicrna/test/main.py` & `seismic-rna-0.3.0/src/seismicrna/test/main.py`

 * *Files identical despite different names*

