# Comparing `tmp/MisER-0.0.2.tar.gz` & `tmp/MisER-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MisER-0.0.2.tar", last modified: Sat Jul 15 14:58:54 2023, max compression
+gzip compressed data, was "MisER-0.0.3.tar", last modified: Sun Jul 16 03:22:31 2023, max compression
```

## Comparing `MisER-0.0.2.tar` & `MisER-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-15 14:58:54.892251 MisER-0.0.2/
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)     1065 2023-01-08 14:32:54.000000 MisER-0.0.2/LICENSE
-drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-15 14:58:54.892251 MisER-0.0.2/MisER/
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-01-08 14:32:54.000000 MisER-0.0.2/MisER/__init__.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)    12220 2023-01-08 14:32:54.000000 MisER-0.0.2/MisER/block_class.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)     7902 2023-01-08 14:32:54.000000 MisER-0.0.2/MisER/find_small_exon.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)    35631 2023-07-15 14:41:38.000000 MisER-0.0.2/MisER/fix_small_exon_multiproc.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)     4403 2023-01-08 14:51:55.000000 MisER-0.0.2/MisER/run_miser.py
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)       18 2023-07-15 14:54:02.000000 MisER-0.0.2/MisER/version.py
-drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-15 14:58:54.892251 MisER-0.0.2/MisER.egg-info/
--rw-rw-r--   0 zhen      (1000) zhen      (1000)     6895 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/PKG-INFO
--rw-rw-r--   0 zhen      (1000) zhen      (1000)      336 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/SOURCES.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)        1 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/dependency_links.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)       47 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/entry_points.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)       42 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/requires.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)        6 2023-07-15 14:58:54.000000 MisER-0.0.2/MisER.egg-info/top_level.txt
--rw-rw-r--   0 zhen      (1000) zhen      (1000)     6895 2023-07-15 14:58:54.892251 MisER-0.0.2/PKG-INFO
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)     6460 2023-01-08 14:49:13.000000 MisER-0.0.2/README.md
--rw-rw-r--   0 zhen      (1000) zhen      (1000)       38 2023-07-15 14:58:54.892251 MisER-0.0.2/setup.cfg
--rwxrwxr-x   0 zhen      (1000) zhen      (1000)      980 2023-07-15 07:39:37.000000 MisER-0.0.2/setup.py
+drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-16 03:22:31.586908 MisER-0.0.3/
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)     1065 2023-01-08 14:32:54.000000 MisER-0.0.3/LICENSE
+drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-16 03:22:31.582908 MisER-0.0.3/MisER/
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-01-08 14:32:54.000000 MisER-0.0.3/MisER/__init__.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)    12220 2023-01-08 14:32:54.000000 MisER-0.0.3/MisER/block_class.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)     7902 2023-01-08 14:32:54.000000 MisER-0.0.3/MisER/find_small_exon.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)    35968 2023-07-16 03:20:43.000000 MisER-0.0.3/MisER/fix_small_exon_multiproc.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)     4403 2023-01-08 14:51:55.000000 MisER-0.0.3/MisER/run_miser.py
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)       18 2023-07-16 03:22:10.000000 MisER-0.0.3/MisER/version.py
+drwxrwxr-x   0 zhen      (1000) zhen      (1000)        0 2023-07-16 03:22:31.586908 MisER-0.0.3/MisER.egg-info/
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)     6895 2023-07-16 03:22:31.000000 MisER-0.0.3/MisER.egg-info/PKG-INFO
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)      336 2023-07-16 03:22:31.000000 MisER-0.0.3/MisER.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)        1 2023-07-16 03:22:31.000000 MisER-0.0.3/MisER.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)       47 2023-07-16 03:22:31.000000 MisER-0.0.3/MisER.egg-info/entry_points.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)       42 2023-07-16 03:22:31.000000 MisER-0.0.3/MisER.egg-info/requires.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)        6 2023-07-16 03:22:31.000000 MisER-0.0.3/MisER.egg-info/top_level.txt
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)     6895 2023-07-16 03:22:31.586908 MisER-0.0.3/PKG-INFO
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)     6460 2023-01-08 14:49:13.000000 MisER-0.0.3/README.md
+-rw-rw-r--   0 zhen      (1000) zhen      (1000)       38 2023-07-16 03:22:31.586908 MisER-0.0.3/setup.cfg
+-rwxrwxr-x   0 zhen      (1000) zhen      (1000)      980 2023-07-15 07:39:37.000000 MisER-0.0.3/setup.py
```

### Comparing `MisER-0.0.2/LICENSE` & `MisER-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MisER-0.0.2/MisER/block_class.py` & `MisER-0.0.3/MisER/block_class.py`

 * *Files identical despite different names*

### Comparing `MisER-0.0.2/MisER/find_small_exon.py` & `MisER-0.0.3/MisER/find_small_exon.py`

 * *Files identical despite different names*

### Comparing `MisER-0.0.2/MisER/fix_small_exon_multiproc.py` & `MisER-0.0.3/MisER/fix_small_exon_multiproc.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import csv
 import re
 import sys
 import time
 import warnings
 import os
 import logging
+import random
+import string
 
 import numpy as np
 import pandas as pd
 import multiprocessing as mp
 import pysam
 import parasail
 import collections
@@ -33,14 +35,17 @@
     """
     indexs_dict = collections.defaultdict(list)
     for i, elem in enumerate(seq):
         indexs_dict[key_fun(elem)].append(i)
     for key, idxs in indexs_dict.items():
         yield key, [seq[i] for i in idxs]
 
+def generate_random_string(length=8):
+    c = string.ascii_letters + string.digits
+    return ''.join(random.choice(c) for i in range(length))
 
 def parse_bed(bed_path):
     """
     The function parse an annotation BED file to a dataframe contain list.
     We used to use list of dict as the result.
     [{'tx_i':146, 'chrom':'chrIS', 'strand':'+', 'start':6955486, 'end':6962816, 'name':'R1_101_1', 'block_count':3, 'block_sizes':[243, 116, 360], 'block_starts':[0, 4897, 6970]},
      {...},
@@ -389,14 +394,15 @@
         start_ci=realign_ss["realign_end_ci"]))
     new_cigar = Cigar_fromlist(new_cigar_list)
     # check new cigar:
     # check_cigar_seq(new_cigar, read.query_sequence, ref_fa.fetch(realign_ss["chrom"], start=read.reference_start, end=read.reference_end))
     return new_cigar, increase_score
 
 
+
 def find_fix(proc_region, ori_bam_path, out_bam_path, ref_fa_path, annot_bed, annot_exon,
              small_exon_size=80, flank_len=20, ignore_strand=True, set_tag=True,
              delta_ratio_thd=0.5, simplify=True, float_flank_len=False, only_region=False):
     """
     The function is used to find and fix small exon in one process.
     The proc_region is a three elements dict. {proc_id, start_read_id, end_read_id}
     Return a dict {"filter_list":[a list of realign_ss], "stat_dict":{a dict with statistics of misaligned reads}}
@@ -408,15 +414,16 @@
         print("Build reference index...")
         pysam.faidx(ref_fa_path)
     ref_fa = pysam.FastaFile(ref_fa_path)
     # 0 based, left close right open
     start_read_id = proc_region["start_read_id"]
     end_read_id = proc_region["end_read_id"]
     if not only_region:
-        out_bam_path_proc = out_bam_path + ".tmp{0}".format(proc_id)
+        random_str = generate_random_string(8)
+        out_bam_path_proc = out_bam_path + ".tmp{0}_thread{1}.bam".format(random_str, proc_id)
         realign_bam = pysam.AlignmentFile(
             out_bam_path_proc, "wb", template=ori_bam)
     filter_list = []
     read_i = 0  # 0 based
     spliced_read_num = 0
     total_intron = 0
     misaligned_read_num = 0
@@ -528,28 +535,29 @@
     The proc_region is a three elements dict. {proc_id, start_read_id, end_read_id}
     Return a dict {"filter_list":[a list of realign_ss], "stat_dict":{a dict with statistics of misaligned reads}}
     """
     proc_id = proc_region["proc_id"]
     score_matrix = parasail.matrix_create("ACGT", 1, -1)
     ori_bam = pysam.AlignmentFile(ori_bam_path, "rb")
     # define a bam to record the reads with error
-    error_bam_path = ori_bam_path+".tmp{0}".format(proc_id)+"_err"
+    random_str = generate_random_string(8)
+    error_bam_path = ori_bam_path+".tmp{0}_thread{1}_err.bam".format(random_str, proc_id)
     error_bam = pysam.AlignmentFile(
         error_bam_path, "wb", template=ori_bam)
     error_case = 0
     # Check the exist of reference fasta index
     if not os.path.exists("{0}.fai".format(ref_fa_path)):
         print("Build reference index...")
         pysam.faidx(ref_fa_path)
     ref_fa = pysam.FastaFile(ref_fa_path)
     # 0 based, left close right open
     start_read_id = proc_region["start_read_id"]
     end_read_id = proc_region["end_read_id"]
     if not only_region:
-        out_bam_path_proc = out_bam_path + ".tmp{0}".format(proc_id)
+        out_bam_path_proc = out_bam_path + ".tmp{0}_thread{1}.bam".format(random_str, proc_id)
         realign_bam = pysam.AlignmentFile(
             out_bam_path_proc, "wb", template=ori_bam)
     filter_list = []
     read_i = 0  # 0 based
     spliced_read_num = 0
     total_intron = 0
     misaligned_read_num = 0
```

### Comparing `MisER-0.0.2/MisER/run_miser.py` & `MisER-0.0.3/MisER/run_miser.py`

 * *Files identical despite different names*

### Comparing `MisER-0.0.2/MisER.egg-info/PKG-INFO` & `MisER-0.0.3/MisER.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MisER
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find and fix missed small exons.
 Home-page: https://github.com/zhenLiuXplr/MisER-project
 Author: Zhen Liu
 Author-email: liuzhen_sirius@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `MisER-0.0.2/PKG-INFO` & `MisER-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MisER
-Version: 0.0.2
+Version: 0.0.3
 Summary: Find and fix missed small exons.
 Home-page: https://github.com/zhenLiuXplr/MisER-project
 Author: Zhen Liu
 Author-email: liuzhen_sirius@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `MisER-0.0.2/README.md` & `MisER-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `MisER-0.0.2/setup.py` & `MisER-0.0.3/setup.py`

 * *Files identical despite different names*

