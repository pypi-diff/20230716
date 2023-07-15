# Comparing `tmp/ribs-0.5.1.tar.gz` & `tmp/ribs-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ribs-0.5.1.tar", last modified: Thu Mar  2 07:55:15 2023, max compression
+gzip compressed data, was "dist/ribs-0.5.2.tar", last modified: Sat Jul 15 22:06:03 2023, max compression
```

## Comparing `ribs-0.5.1.tar` & `ribs-0.5.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:55:15.000000 ribs-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-03-02 07:54:24.000000 ribs-0.5.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-03-02 07:54:24.000000 ribs-0.5.1/HISTORY.md
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-02 07:54:24.000000 ribs-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-02 07:54:24.000000 ribs-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    32315 2023-03-02 07:55:15.000000 ribs-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16437 2023-03-02 07:54:24.000000 ribs-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs/archives/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_add_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_archive_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_archive_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_archive_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_cqd_score_result.py
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_cvt_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_elite.py
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_grid_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    19477 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/archives/_sliding_boundaries_archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs/emitters/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/_emitter_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/_evolution_strategy_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/_gaussian_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19787 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/_gradient_arborescence_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/_iso_line_emitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs/emitters/opt/
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/_adam_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/_cma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/_evolution_strategy_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/_gradient_ascent_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/_gradient_opt_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/_lm_ma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/_openai_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/opt/_sep_cma_es.py
--rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/emitters/rankers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17303 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/schedulers/_bandit_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16302 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/schedulers/_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    34379 2023-03-02 07:54:24.000000 ribs-0.5.1/ribs/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    32315 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-02 07:55:15.000000 ribs-0.5.1/ribs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-02 07:55:15.000000 ribs-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-03-02 07:54:24.000000 ribs-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:06:03.000000 ribs-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     9394 2023-07-15 22:04:56.000000 ribs-0.5.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-07-15 22:04:56.000000 ribs-0.5.2/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 22:04:56.000000 ribs-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-15 22:04:56.000000 ribs-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    34821 2023-07-15 22:06:03.000000 ribs-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17909 2023-07-15 22:04:56.000000 ribs-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs/archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_add_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54074 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_archive_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_archive_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_archive_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_cqd_score_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_cvt_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_elite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_grid_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19477 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/archives/_sliding_boundaries_archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs/emitters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/_emitter_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/_evolution_strategy_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/_gaussian_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20239 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/_gradient_arborescence_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7078 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/_iso_line_emitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs/emitters/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/_adam_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12970 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/_cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/_evolution_strategy_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/_gradient_ascent_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/_gradient_opt_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/_lm_ma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/_openai_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/opt/_sep_cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14143 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/emitters/rankers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17758 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/schedulers/_bandit_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16748 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/schedulers/_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34686 2023-07-15 22:04:56.000000 ribs-0.5.2/ribs/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34821 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-15 22:06:03.000000 ribs-0.5.2/ribs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-15 22:06:03.000000 ribs-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-15 22:04:56.000000 ribs-0.5.2/setup.py
```

### Comparing `ribs-0.5.1/CONTRIBUTING.md` & `ribs-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/HISTORY.md` & `ribs-0.5.2/HISTORY.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,35 @@
 # History
 
+## 0.5.2
+
+This release contains miscellaneous edits to our documentation from v0.5.1.
+Furthermore, the library is updated to support Python 3.11, removed deprecated
+options, and strengthened with more robust checks and error messages in the
+schedulers.
+
+### Changelog
+
+#### API
+
+- Support Python 3.11 (#342)
+- Check that emitters passed in are lists/iterables in scheduler (#341)
+- Fix Matplotlib `get_cmap` deprecation (#340)
+- **Backwards-incompatible:** Default `plot_centroids` to False when plotting
+  (#339)
+- Raise error messages when `ask` is called without `ask_dqd` (#338)
+
+#### Documentation
+
+- Add BibTex citation for GECCO 2023 (#337)
+
+#### Improvements
+
+- Update distribution dependencies (#344)
+
 ## 0.5.1
 
 This release contains miscellaneous edits to our documentation from v0.5.0.
 There were no changes to library functionality in this release.
 
 ## 0.5.0
```

### Comparing `ribs-0.5.1/LICENSE` & `ribs-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/PKG-INFO` & `ribs-0.5.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ribs
-Version: 0.5.1
+Version: 0.5.2
 Summary: A bare-bones Python library for quality diversity optimization.
 Home-page: https://github.com/icaros-usc/pyribs
 Author: ICAROS Lab pyribs Team
 Author-email: team@pyribs.org
 License: MIT license
 Description: # pyribs
         
@@ -90,28 +90,36 @@
         
         Two years after the initial release of pyribs, we released a paper which
         elaborates on the RIBS framework and the design decisions behind pyribs! For
         more information on this paper, see [here](https://pyribs.org/paper).
         
         ## Citation
         
-        If you use pyribs in your research, please cite it as follows. Note that you
-        will need to include the
-        [hyperref](https://www.overleaf.com/learn/latex/Hyperlinks#Linking_web_addresses)
-        package in order to use the `\url` command. Also consider citing any algorithms
-        you use as shown [below](#citing-algorithms-in-pyribs).
+        If you use pyribs in your research, please consider citing our
+        [GECCO 2023 paper](https://dl.acm.org/doi/10.1145/3583131.3590374) as follows.
+        Also consider citing any algorithms you use as shown
+        [below](#citing-algorithms-in-pyribs).
         
         ```
-        @misc{pyribs,
-          title={pyribs: A Bare-Bones Python Library for Quality Diversity Optimization},
-          author={Bryon Tjanaka and Matthew C. Fontaine and David H. Lee and Yulun Zhang and Nivedit Reddy Balam and Nathaniel Dennler and Sujay S. Garlanka and Nikitas Dimitri Klapsis and Stefanos Nikolaidis},
-          year={2023},
-          eprint={2303.00191},
-          archivePrefix={arXiv},
-          primaryClass={cs.NE}
+        @inproceedings{10.1145/3583131.3590374,
+          author = {Tjanaka, Bryon and Fontaine, Matthew C and Lee, David H and Zhang, Yulun and Balam, Nivedit Reddy and Dennler, Nathaniel and Garlanka, Sujay S and Klapsis, Nikitas Dimitri and Nikolaidis, Stefanos},
+          title = {Pyribs: A Bare-Bones Python Library for Quality Diversity Optimization},
+          year = {2023},
+          isbn = {9798400701191},
+          publisher = {Association for Computing Machinery},
+          address = {New York, NY, USA},
+          url = {https://doi.org/10.1145/3583131.3590374},
+          doi = {10.1145/3583131.3590374},
+          abstract = {Recent years have seen a rise in the popularity of quality diversity (QD) optimization, a branch of optimization that seeks to find a collection of diverse, high-performing solutions to a given problem. To grow further, we believe the QD community faces two challenges: developing a framework to represent the field's growing array of algorithms, and implementing that framework in software that supports a range of researchers and practitioners. To address these challenges, we have developed pyribs, a library built on a highly modular conceptual QD framework. By replacing components in the conceptual framework, and hence in pyribs, users can compose algorithms from across the QD literature; equally important, they can identify unexplored algorithm variations. Furthermore, pyribs makes this framework simple, flexible, and accessible, with a user-friendly API supported by extensive documentation and tutorials. This paper overviews the creation of pyribs, focusing on the conceptual framework that it implements and the design principles that have guided the library's development. Pyribs is available at https://pyribs.org},
+          booktitle = {Proceedings of the Genetic and Evolutionary Computation Conference},
+          pages = {220–229},
+          numpages = {10},
+          keywords = {framework, quality diversity, software library},
+          location = {Lisbon, Portugal},
+          series = {GECCO '23}
         }
         ```
         
         ## Usage
         
         Here we show an example application of CMA-ME in pyribs. To initialize the
         algorithm, we first create:
@@ -356,14 +364,40 @@
         [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
         [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
         project template.
         
         
         # History
         
+        ## 0.5.2
+        
+        This release contains miscellaneous edits to our documentation from v0.5.1.
+        Furthermore, the library is updated to support Python 3.11, removed deprecated
+        options, and strengthened with more robust checks and error messages in the
+        schedulers.
+        
+        ### Changelog
+        
+        #### API
+        
+        - Support Python 3.11 (#342)
+        - Check that emitters passed in are lists/iterables in scheduler (#341)
+        - Fix Matplotlib `get_cmap` deprecation (#340)
+        - **Backwards-incompatible:** Default `plot_centroids` to False when plotting
+          (#339)
+        - Raise error messages when `ask` is called without `ask_dqd` (#338)
+        
+        #### Documentation
+        
+        - Add BibTex citation for GECCO 2023 (#337)
+        
+        #### Improvements
+        
+        - Update distribution dependencies (#344)
+        
         ## 0.5.1
         
         This release contains miscellaneous edits to our documentation from v0.5.0.
         There were no changes to library functionality in this release.
         
         ## 0.5.0
         
@@ -610,14 +644,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: visualize
 Provides-Extra: all
```

### Comparing `ribs-0.5.1/README.md` & `ribs-0.5.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,28 +82,36 @@
 
 Two years after the initial release of pyribs, we released a paper which
 elaborates on the RIBS framework and the design decisions behind pyribs! For
 more information on this paper, see [here](https://pyribs.org/paper).
 
 ## Citation
 
-If you use pyribs in your research, please cite it as follows. Note that you
-will need to include the
-[hyperref](https://www.overleaf.com/learn/latex/Hyperlinks#Linking_web_addresses)
-package in order to use the `\url` command. Also consider citing any algorithms
-you use as shown [below](#citing-algorithms-in-pyribs).
+If you use pyribs in your research, please consider citing our
+[GECCO 2023 paper](https://dl.acm.org/doi/10.1145/3583131.3590374) as follows.
+Also consider citing any algorithms you use as shown
+[below](#citing-algorithms-in-pyribs).
 
 ```
-@misc{pyribs,
-  title={pyribs: A Bare-Bones Python Library for Quality Diversity Optimization},
-  author={Bryon Tjanaka and Matthew C. Fontaine and David H. Lee and Yulun Zhang and Nivedit Reddy Balam and Nathaniel Dennler and Sujay S. Garlanka and Nikitas Dimitri Klapsis and Stefanos Nikolaidis},
-  year={2023},
-  eprint={2303.00191},
-  archivePrefix={arXiv},
-  primaryClass={cs.NE}
+@inproceedings{10.1145/3583131.3590374,
+  author = {Tjanaka, Bryon and Fontaine, Matthew C and Lee, David H and Zhang, Yulun and Balam, Nivedit Reddy and Dennler, Nathaniel and Garlanka, Sujay S and Klapsis, Nikitas Dimitri and Nikolaidis, Stefanos},
+  title = {Pyribs: A Bare-Bones Python Library for Quality Diversity Optimization},
+  year = {2023},
+  isbn = {9798400701191},
+  publisher = {Association for Computing Machinery},
+  address = {New York, NY, USA},
+  url = {https://doi.org/10.1145/3583131.3590374},
+  doi = {10.1145/3583131.3590374},
+  abstract = {Recent years have seen a rise in the popularity of quality diversity (QD) optimization, a branch of optimization that seeks to find a collection of diverse, high-performing solutions to a given problem. To grow further, we believe the QD community faces two challenges: developing a framework to represent the field's growing array of algorithms, and implementing that framework in software that supports a range of researchers and practitioners. To address these challenges, we have developed pyribs, a library built on a highly modular conceptual QD framework. By replacing components in the conceptual framework, and hence in pyribs, users can compose algorithms from across the QD literature; equally important, they can identify unexplored algorithm variations. Furthermore, pyribs makes this framework simple, flexible, and accessible, with a user-friendly API supported by extensive documentation and tutorials. This paper overviews the creation of pyribs, focusing on the conceptual framework that it implements and the design principles that have guided the library's development. Pyribs is available at https://pyribs.org},
+  booktitle = {Proceedings of the Genetic and Evolutionary Computation Conference},
+  pages = {220–229},
+  numpages = {10},
+  keywords = {framework, quality diversity, software library},
+  location = {Lisbon, Portugal},
+  series = {GECCO '23}
 }
 ```
 
 ## Usage
 
 Here we show an example application of CMA-ME in pyribs. To initialize the
 algorithm, we first create:
```

### Comparing `ribs-0.5.1/ribs/_docstrings.py` & `ribs-0.5.2/ribs/_docstrings.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/_utils.py` & `ribs-0.5.2/ribs/_utils.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/archives/_add_status.py` & `ribs-0.5.2/ribs/archives/_add_status.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/archives/_archive_base.py` & `ribs-0.5.2/ribs/archives/_archive_base.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/archives/_archive_data_frame.py` & `ribs-0.5.2/ribs/archives/_archive_data_frame.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/archives/_archive_stats.py` & `ribs-0.5.2/ribs/archives/_archive_stats.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/archives/_cqd_score_result.py` & `ribs-0.5.2/ribs/archives/_cqd_score_result.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/archives/_cvt_archive.py` & `ribs-0.5.2/ribs/archives/_cvt_archive.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     point, as recommended in the docs for :meth:`timeit.Timer.repeat`.  Note the
     logarithmic scales. This plot was generated on a reasonably modern laptop.
 
     .. image:: ../_static/imgs/cvt_add_plot.png
         :alt: Runtime to insert 100k entries into CVTArchive
 
     Across almost all numbers of cells, using the k-D tree is faster than using
-    brute force. Thus, **we recommend always using he k-D tree.** See
+    brute force. Thus, **we recommend always using the k-D tree.** See
     `benchmarks/cvt_add.py
     <https://github.com/icaros-usc/pyribs/tree/master/benchmarks/cvt_add.py>`_
     in the project repo for more information about how this plot was generated.
 
     Finally, if running multiple experiments, it may be beneficial to use the
     same centroids across each experiment. Doing so can keep experiments
     consistent and reduce execution time. To do this, either (1) construct
@@ -51,14 +51,17 @@
     subsequent experiments.
 
     .. note:: The idea of archive thresholds was introduced in `Fontaine 2022
         <https://arxiv.org/abs/2205.10752>`_. Refer to our `CMA-MAE tutorial
         <../../tutorials/cma_mae.html>`_ for more info on thresholds, including
         the ``learning_rate`` and ``threshold_min`` parameters.
 
+    .. note:: For more information on our choice of k-D tree implementation, see
+        `#38 <https://github.com/icaros-usc/pyribs/issues/38>`_.
+
     Args:
         solution_dim (int): Dimension of the solution space.
         cells (int): The number of cells to use in the archive, equivalent to
             the number of centroids/areas in the CVT.
         ranges (array-like of (float, float)): Upper and lower bound of each
             dimension of the measure space, e.g. ``[(-1, 1), (-2, 2)]``
             indicates the first dimension should have bounds :math:`[-1,1]`
@@ -181,14 +184,15 @@
             if custom_centroids.shape != (cells, self._measure_dim):
                 raise ValueError(
                     f"custom_centroids has shape {custom_centroids.shape} but "
                     f"must be of shape (cells={cells}, len(ranges)="
                     f"{self._measure_dim})")
             self._centroids = custom_centroids
             self._samples = None
+
         if self._centroids is None:
             self._samples = self._rng.uniform(
                 self._lower_bounds,
                 self._upper_bounds,
                 size=(self._samples, self._measure_dim),
             ).astype(self.dtype) if isinstance(self._samples,
                                                int) else self._samples
@@ -260,17 +264,16 @@
         """
         measures_batch = np.asarray(measures_batch)
         check_batch_shape(measures_batch, "measures_batch", self.measure_dim,
                           "measure_dim")
         check_finite(measures_batch, "measures_batch")
 
         if self._use_kd_tree:
-            return np.asarray(
-                self._centroid_kd_tree.query(measures_batch))[1].astype(
-                    np.int32)
+            _, indices = self._centroid_kd_tree.query(measures_batch)
+            return indices.astype(np.int32)
 
         # Brute force distance calculation -- start by taking the difference
         # between each measure i and all the centroids.
         distances = np.expand_dims(measures_batch, axis=1) - self.centroids
 
         # Compute the total squared distance -- no need to compute actual
         # distance with a sqrt.
```

### Comparing `ribs-0.5.1/ribs/archives/_elite.py` & `ribs-0.5.2/ribs/archives/_elite.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/archives/_grid_archive.py` & `ribs-0.5.2/ribs/archives/_grid_archive.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/archives/_sliding_boundaries_archive.py` & `ribs-0.5.2/ribs/archives/_sliding_boundaries_archive.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/_emitter_base.py` & `ribs-0.5.2/ribs/emitters/_emitter_base.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/_evolution_strategy_emitter.py` & `ribs-0.5.2/ribs/emitters/_evolution_strategy_emitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     the mean and covariance of the distribution.
 
     Args:
         archive (ribs.archives.ArchiveBase): An archive to use when creating
             and inserting solutions. For instance, this can be
             :class:`ribs.archives.GridArchive`.
         x0 (np.ndarray): Initial solution. Must be 1-dimensional.
-        sigma0 (float): Initial step size / standard deviation.
+        sigma0 (float): Initial step size / standard deviation of the
+            distribution from which solutions are sampled.
         ranker (Callable or str): The ranker is a :class:`RankerBase` object
             that orders the solutions after they have been evaluated in the
             environment. This parameter may be a callable (e.g. a class or
             a lambda function) that takes in no parameters and returns an
             instance of :class:`RankerBase`, or it may be a full or abbreviated
             ranker name as described in
             :meth:`ribs.emitters.rankers.get_ranker`.
@@ -215,17 +216,16 @@
         # Preprocessing arguments.
         solution_batch = np.asarray(solution_batch)
         objective_batch = np.asarray(objective_batch)
         measures_batch = np.asarray(measures_batch)
         status_batch = np.asarray(status_batch)
         value_batch = np.asarray(value_batch)
         batch_size = solution_batch.shape[0]
-        metadata_batch = (np.empty(batch_size, dtype=object) if
-                          metadata_batch is None else np.asarray(metadata_batch,
-                                                                 dtype=object))
+        metadata_batch = (np.empty(batch_size, dtype=object) if metadata_batch
+                          is None else np.asarray(metadata_batch, dtype=object))
 
         # Validate arguments.
         validate_batch_args(archive=self.archive,
                             solution_batch=solution_batch,
                             objective_batch=objective_batch,
                             measures_batch=measures_batch,
                             status_batch=status_batch,
```

### Comparing `ribs-0.5.1/ribs/emitters/_gaussian_emitter.py` & `ribs-0.5.2/ribs/emitters/_gaussian_emitter.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/_gradient_arborescence_emitter.py` & `ribs-0.5.2/ribs/emitters/_gradient_arborescence_emitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ribs.emitters._emitter_base import EmitterBase
 from ribs.emitters.opt import _get_es, _get_grad_opt
 from ribs.emitters.rankers import _get_ranker
 
 
 class GradientArborescenceEmitter(EmitterBase):
     """Generates solutions with a gradient arborescence, with coefficients
-    parameterized by an ES.
+    parameterized by an evolution strategy.
 
     This emitter originates in `Fontaine 2021
     <https://arxiv.org/abs/2106.03894>`_. It leverages the gradient information
     of the objective and measure functions, generating new solutions around a
     *solution point* :math:`\\boldsymbol{\\theta}` using *gradient
     arborescence*, with coefficients drawn from a Gaussian distribution.
     Essentially, this means that the emitter samples coefficients
@@ -47,15 +47,16 @@
         information to the emitter.
 
     Args:
         archive (ribs.archives.ArchiveBase): An archive to use when creating and
             inserting solutions. For instance, this can be
             :class:`ribs.archives.GridArchive`.
         x0 (np.ndarray): Initial solution.
-        sigma0 (float): Initial step size / standard deviation.
+        sigma0 (float): Initial step size / standard deviation of the
+            distribution of gradient coefficients.
         lr (float): Learning rate for the gradient optimizer.
         ranker (Callable or str): The ranker is a :class:`RankerBase` object
             that orders the solutions after they have been evaluated in the
             environment. This parameter may be a callable (e.g. a class or a
             lambda function) that takes in no parameters and returns an instance
             of :class:`RankerBase`, or it may be a full or abbreviated ranker
             name as described in :mod:`ribs.emitters.rankers`.
@@ -68,18 +69,18 @@
             restart after this many iterations, where each iteration is a call
             to :meth:`tell`. With "basic", only the default CMA-ES convergence
             rules will be used, while with "no_improvement", the emitter will
             restart when none of the proposed solutions were added to the
             archive.
         grad_opt (Callable or str): Gradient optimizer to use for the gradient
             ascent step of the algorithm. The optimizer is a
-            :class:`GradientOptBase` object. This parameter may be a callable
-            (e.g. a class or a lambda function) which takes in the ``theta0``
-            and ``lr`` arguments, or it may be a full or abbreviated name as
-            described in :mod:`ribs.emitters.opt`.
+            :class:`~ribs.emitters.opt.GradientOptBase` object. This parameter
+            may be a callable (e.g. a class or a lambda function) which takes in
+            the ``theta0`` and ``lr`` arguments, or it may be a full or
+            abbreviated name as described in :mod:`ribs.emitters.opt`.
         grad_opt_kwargs (dict): Additional arguments to pass to the gradient
             optimizer. See the gradient-based optimizers in
             :mod:`ribs.emitters.opt` for the arguments allowed by each
             optimizer. Note that we already pass in ``theta0`` and ``lr``.
         es (Callable or str): The evolution strategy is an
             :class:`EvolutionStrategyBase` object that is used to adapt the
             distribution from which new gradient coefficients are sampled. This
@@ -96,18 +97,17 @@
             be normalized. Otherwise, it will not be normalized.
         bounds: This argument may be used for providing solution space bounds in
             the future. This emitter does not currently support solution space
             bounds, as bounding solutions for DQD algorithms such as CMA-MEGA is
             an open problem. Hence, this argument must be set to None.
         batch_size (int): Number of solutions to return in :meth:`ask`. If not
             passed in, a batch size will be automatically calculated using the
-            default CMA-ES rules. Note that `batch_size` **does not** include
-            the number of solutions returned by :meth:`ask_dqd`, but also note
-            that :meth:`ask_dqd` always returns one solution, i.e. the solution
-            point.
+            default CMA-ES rules. This **does not** account for the **one**
+            solution returned by :meth:`ask_dqd`, which is the solution point
+            maintained by the gradient optimizer.
         epsilon (float): For numerical stability, we add a small epsilon when
             normalizing gradients in :meth:`tell_dqd` -- refer to the
             implementation `here
             <../_modules/ribs/emitters/_gradient_arborescence_emitter.html#GradientArborescenceEmitter.tell_dqd>`_.
             Pass this parameter to configure that epsilon.
         seed (int): Value to seed the random number generator. Set to None to
             avoid a fixed seed.
@@ -248,21 +248,28 @@
     def ask(self):
         """Samples new solutions from a gradient arborescence parameterized by a
         multivariate Gaussian distribution.
 
         The multivariate Gaussian is parameterized by the evolution strategy
         optimizer ``self._opt``.
 
-        Note that this method returns `batch_size - 1` solution as one solution
-        is returned via ask_dqd.
+        This method returns ``batch_size`` solutions, even though one solution
+        is returned via ``ask_dqd``.
 
         Returns:
-            (batch_size, :attr:`solution_dim`) array -- a batch of new solutions
-            to evaluate.
+            (:attr:`batch_size`, :attr:`solution_dim`) array -- a batch of new
+            solutions to evaluate.
+        Raises:
+            RuntimeError: This method was called without first passing gradients
+                with calls to ask_dqd() and tell_dqd().
         """
+        if self._jacobian_batch is None:
+            raise RuntimeError("Please call ask_dqd() and tell_dqd() "
+                               "before calling ask().")
+
         coeff_lower_bounds = np.full(
             self._num_coefficients,
             -np.inf,
             dtype=self._archive.dtype,
         )
         coeff_upper_bounds = np.full(
             self._num_coefficients,
@@ -331,17 +338,16 @@
         # Preprocessing arguments.
         solution_batch = np.asarray(solution_batch)
         objective_batch = np.asarray(objective_batch)
         measures_batch = np.asarray(measures_batch)
         status_batch = np.asarray(status_batch)
         value_batch = np.asarray(value_batch)
         batch_size = solution_batch.shape[0]
-        metadata_batch = (np.empty(batch_size, dtype=object) if
-                          metadata_batch is None else np.asarray(metadata_batch,
-                                                                 dtype=object))
+        metadata_batch = (np.empty(batch_size, dtype=object) if metadata_batch
+                          is None else np.asarray(metadata_batch, dtype=object))
 
         # Validate arguments.
         validate_batch_args(archive=self.archive,
                             solution_batch=solution_batch,
                             objective_batch=objective_batch,
                             measures_batch=measures_batch,
                             status_batch=status_batch,
@@ -379,37 +385,40 @@
                 :class:`ribs.archive.addstatus` returned by a series of calls
                 to archive's :meth:`add()` method.
             value_batch (array-like): 1d array of floats returned by a series
                 of calls to archive's :meth:`add()` method. for what these
                 floats represent, refer to :meth:`ribs.archives.add()`.
             metadata_batch (array-like): 1d object array containing a metadata
                 object for each solution.
+        Raises:
+            RuntimeError: This method was called without first passing gradients
+                with calls to ask_dqd() and tell_dqd().
         """
         # Preprocessing arguments.
         solution_batch = np.asarray(solution_batch)
         objective_batch = np.asarray(objective_batch)
         measures_batch = np.asarray(measures_batch)
         status_batch = np.asarray(status_batch)
         value_batch = np.asarray(value_batch)
         batch_size = solution_batch.shape[0]
-        metadata_batch = (np.empty(batch_size, dtype=object) if
-                          metadata_batch is None else np.asarray(metadata_batch,
-                                                                 dtype=object))
+        metadata_batch = (np.empty(batch_size, dtype=object) if metadata_batch
+                          is None else np.asarray(metadata_batch, dtype=object))
 
         # Validate arguments.
         validate_batch_args(archive=self.archive,
                             solution_batch=solution_batch,
                             objective_batch=objective_batch,
                             measures_batch=measures_batch,
                             status_batch=status_batch,
                             value_batch=value_batch,
                             metadata_batch=metadata_batch)
 
         if self._jacobian_batch is None:
-            raise RuntimeError("tell() was called without calling tell_dqd().")
+            raise RuntimeError("Please call ask_dqd(), tell_dqd(), and ask() "
+                               "before calling tell().")
 
         # Increase iteration counter.
         self._itrs += 1
 
         # Count number of new solutions.
         new_sols = status_batch.astype(bool).sum()
```

### Comparing `ribs-0.5.1/ribs/emitters/_iso_line_emitter.py` & `ribs-0.5.2/ribs/emitters/_iso_line_emitter.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/__init__.py` & `ribs-0.5.2/ribs/emitters/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/_adam_opt.py` & `ribs-0.5.2/ribs/emitters/opt/_adam_opt.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/_cma_es.py` & `ribs-0.5.2/ribs/emitters/opt/_cma_es.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/_evolution_strategy_base.py` & `ribs-0.5.2/ribs/emitters/opt/_evolution_strategy_base.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/_gradient_ascent_opt.py` & `ribs-0.5.2/ribs/emitters/opt/_gradient_ascent_opt.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/_gradient_opt_base.py` & `ribs-0.5.2/ribs/emitters/opt/_gradient_opt_base.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/_lm_ma_es.py` & `ribs-0.5.2/ribs/emitters/opt/_lm_ma_es.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/_openai_es.py` & `ribs-0.5.2/ribs/emitters/opt/_openai_es.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/opt/_sep_cma_es.py` & `ribs-0.5.2/ribs/emitters/opt/_sep_cma_es.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/emitters/rankers.py` & `ribs-0.5.2/ribs/emitters/rankers.py`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs/schedulers/_bandit_scheduler.py` & `ribs-0.5.2/ribs/schedulers/_bandit_scheduler.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,15 +56,16 @@
             in pyribs 0.4.0 and before. We highly recommend using "batch" mode
             since it is significantly faster.
         result_archive (ribs.archives.ArchiveBase): In some algorithms, such as
             CMA-MAE, the archive does not store all the best-performing
             solutions. The `result_archive` is a secondary archive where we can
             store all the best-performing solutions.
     Raises:
-        ValueError: Number of active emitter is less than one.
+        TypeError: The `emitter_pool` argument was not a list of emitters.
+        ValueError: Number of active emitters is less than one.
         ValueError: Less emitters in the pool than the number of active
             emitters.
         ValueError: The emitters passed in do not have the same solution
             dimensions.
         ValueError: The same emitter instance was passed in multiple times.
             Each emitter should be a unique instance (see the warning above).
         ValueError: Invalid value for `add_mode`.
@@ -78,18 +79,25 @@
                  reselect="terminated",
                  zeta=0.05,
                  result_archive=None,
                  add_mode="batch"):
         if num_active < 1:
             raise ValueError("num_active cannot be less than 1.")
 
-        if len(emitter_pool) < num_active:
-            raise ValueError(f"The emitter pool must contain at least"
-                             f"num_active emitters, but only"
-                             f"{len(emitter_pool)} are given.")
+        try:
+            if len(emitter_pool) < num_active:
+                raise ValueError(f"The emitter pool must contain at least"
+                                 f"num_active emitters, but only"
+                                 f"{len(emitter_pool)} are given.")
+        except TypeError as exception:
+            # TypeError will be raised by len(). We avoid directly checking if
+            # `emitter_pool` is an instance of list since we do not want to be
+            # too restrictive.
+            raise TypeError("`emitter_pool` must be a list of emitter objects."
+                           ) from exception
 
         emitter_ids = set(id(e) for e in emitter_pool)
         if len(emitter_ids) != len(emitter_pool):
             raise ValueError(
                 "Not all emitters passed in were unique (i.e. some emitters "
                 "had the same id). If emitters were created with something "
                 "like [EmitterClass(...)] * n, instead use "
@@ -234,15 +242,15 @@
         # The ranking of emitters also follows these rules:
         # - Emitters that have never been selected are prioritized.
         # - If reselect is "terminated", then only active emitters that have
         #   terminated/restarted will be reselected. Otherwise, if reselect is
         #   "all", then all emitters are reselected.
         if reselect.any():
             ucb1 = np.full_like(self._emitter_pool, np.inf)
-            update_ucb = (self._selection != 0)
+            update_ucb = self._selection != 0
             if update_ucb.any():
                 ucb1[update_ucb] = (
                     self._success[update_ucb] / self._selection[update_ucb] +
                     self._zeta * np.sqrt(
                         np.log(self._success.sum()) /
                         self._selection[update_ucb]))
             # Activate top emitters based on UCB1.
```

### Comparing `ribs-0.5.1/ribs/schedulers/_scheduler.py` & `ribs-0.5.2/ribs/schedulers/_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,30 +37,39 @@
             pyribs 0.4.0 and before. We highly recommend using "batch" mode
             since it is significantly faster.
         result_archive (ribs.archives.ArchiveBase): In some algorithms, such as
             CMA-MAE, the archive does not store all the best-performing
             solutions. The `result_archive` is a secondary archive where we can
             store all the best-performing solutions.
     Raises:
+        TypeError: The `emitters` argument was not a list of emitters.
         ValueError: The emitters passed in do not have the same solution
             dimensions.
         ValueError: There is no emitter passed in.
         ValueError: The same emitter instance was passed in multiple times. Each
             emitter should be a unique instance (see the warning above).
         ValueError: Invalid value for `add_mode`.
     """
 
     def __init__(self,
                  archive,
                  emitters,
                  *,
                  result_archive=None,
                  add_mode="batch"):
-        if len(emitters) == 0:
-            raise ValueError("Pass in at least one emitter to the scheduler.")
+        try:
+            if len(emitters) == 0:
+                raise ValueError(
+                    "Pass in at least one emitter to the scheduler.")
+        except TypeError as exception:
+            # TypeError will be raised by len(). We avoid directly checking if
+            # `emitters` is an instance of list since we do not want to be too
+            # restrictive.
+            raise TypeError(
+                "`emitters` must be a list of emitter objects.") from exception
 
         emitter_ids = set(id(e) for e in emitters)
         if len(emitter_ids) != len(emitters):
             raise ValueError(
                 "Not all emitters passed in were unique (i.e. some emitters "
                 "had the same id). If emitters were created with something "
                 "like [EmitterClass(...)] * n, instead use "
```

### Comparing `ribs-0.5.1/ribs/visualize.py` & `ribs-0.5.2/ribs/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     "parallel_axes_plot",
 ]
 
 
 def _retrieve_cmap(cmap):
     """Retrieves colormap from matplotlib."""
     if isinstance(cmap, str):
-        return matplotlib.cm.get_cmap(cmap)
+        return plt.get_cmap(cmap)
     if isinstance(cmap, list):
         return matplotlib.colors.ListedColormap(cmap)
     return cmap
 
 
 def _validate_heatmap_visual_args(aspect, cbar, measure_dim, valid_dims,
                                   error_msg_measure_dim):
@@ -255,15 +255,15 @@
     # Create color bar.
     _set_cbar(t, ax, cbar, cbar_kwargs)
 
 
 def cvt_archive_heatmap(archive,
                         ax=None,
                         *,
-                        plot_centroids=True,
+                        plot_centroids=False,
                         plot_samples=False,
                         transpose_measures=False,
                         cmap="magma",
                         aspect="auto",
                         ms=1,
                         lw=0.5,
                         vmin=None,
@@ -399,14 +399,19 @@
             region_obj[region_idx] = obj
 
     # Override objective value range.
     min_obj = min_obj if vmin is None else vmin
     max_obj = max_obj if vmax is None else vmax
 
     # Shade the regions.
+    #
+    # Note: by default, the first region will be an empty list -- see:
+    # https://docs.scipy.org/doc/scipy/reference/generated/scipy.spatial.Voronoi.html
+    # However, this empty region is ignored by ax.fill since `polygon` is also
+    # an empty list in this case.
     for region, objective in zip(vor.regions, region_obj):
         # This check is O(n), but n is typically small, and creating
         # `polygon` is also O(n) anyway.
         if -1 not in region:
             if objective is None:
                 color = "white"
             else:
@@ -770,9 +775,10 @@
                      alpha=alpha,
                      linewidth=linewidth)
 
     # Create a colorbar.
     mappable = ScalarMappable(cmap=cmap)
     mappable.set_clim(vmin, vmax)
     host_ax.figure.colorbar(mappable,
+                            ax=host_ax,
                             pad=cbar_pad,
                             orientation=cbar_orientation)
```

### Comparing `ribs-0.5.1/ribs.egg-info/PKG-INFO` & `ribs-0.5.2/ribs.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ribs
-Version: 0.5.1
+Version: 0.5.2
 Summary: A bare-bones Python library for quality diversity optimization.
 Home-page: https://github.com/icaros-usc/pyribs
 Author: ICAROS Lab pyribs Team
 Author-email: team@pyribs.org
 License: MIT license
 Description: # pyribs
         
@@ -90,28 +90,36 @@
         
         Two years after the initial release of pyribs, we released a paper which
         elaborates on the RIBS framework and the design decisions behind pyribs! For
         more information on this paper, see [here](https://pyribs.org/paper).
         
         ## Citation
         
-        If you use pyribs in your research, please cite it as follows. Note that you
-        will need to include the
-        [hyperref](https://www.overleaf.com/learn/latex/Hyperlinks#Linking_web_addresses)
-        package in order to use the `\url` command. Also consider citing any algorithms
-        you use as shown [below](#citing-algorithms-in-pyribs).
+        If you use pyribs in your research, please consider citing our
+        [GECCO 2023 paper](https://dl.acm.org/doi/10.1145/3583131.3590374) as follows.
+        Also consider citing any algorithms you use as shown
+        [below](#citing-algorithms-in-pyribs).
         
         ```
-        @misc{pyribs,
-          title={pyribs: A Bare-Bones Python Library for Quality Diversity Optimization},
-          author={Bryon Tjanaka and Matthew C. Fontaine and David H. Lee and Yulun Zhang and Nivedit Reddy Balam and Nathaniel Dennler and Sujay S. Garlanka and Nikitas Dimitri Klapsis and Stefanos Nikolaidis},
-          year={2023},
-          eprint={2303.00191},
-          archivePrefix={arXiv},
-          primaryClass={cs.NE}
+        @inproceedings{10.1145/3583131.3590374,
+          author = {Tjanaka, Bryon and Fontaine, Matthew C and Lee, David H and Zhang, Yulun and Balam, Nivedit Reddy and Dennler, Nathaniel and Garlanka, Sujay S and Klapsis, Nikitas Dimitri and Nikolaidis, Stefanos},
+          title = {Pyribs: A Bare-Bones Python Library for Quality Diversity Optimization},
+          year = {2023},
+          isbn = {9798400701191},
+          publisher = {Association for Computing Machinery},
+          address = {New York, NY, USA},
+          url = {https://doi.org/10.1145/3583131.3590374},
+          doi = {10.1145/3583131.3590374},
+          abstract = {Recent years have seen a rise in the popularity of quality diversity (QD) optimization, a branch of optimization that seeks to find a collection of diverse, high-performing solutions to a given problem. To grow further, we believe the QD community faces two challenges: developing a framework to represent the field's growing array of algorithms, and implementing that framework in software that supports a range of researchers and practitioners. To address these challenges, we have developed pyribs, a library built on a highly modular conceptual QD framework. By replacing components in the conceptual framework, and hence in pyribs, users can compose algorithms from across the QD literature; equally important, they can identify unexplored algorithm variations. Furthermore, pyribs makes this framework simple, flexible, and accessible, with a user-friendly API supported by extensive documentation and tutorials. This paper overviews the creation of pyribs, focusing on the conceptual framework that it implements and the design principles that have guided the library's development. Pyribs is available at https://pyribs.org},
+          booktitle = {Proceedings of the Genetic and Evolutionary Computation Conference},
+          pages = {220–229},
+          numpages = {10},
+          keywords = {framework, quality diversity, software library},
+          location = {Lisbon, Portugal},
+          series = {GECCO '23}
         }
         ```
         
         ## Usage
         
         Here we show an example application of CMA-ME in pyribs. To initialize the
         algorithm, we first create:
@@ -356,14 +364,40 @@
         [Cookiecutter](https://github.com/audreyr/cookiecutter) and the
         [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage)
         project template.
         
         
         # History
         
+        ## 0.5.2
+        
+        This release contains miscellaneous edits to our documentation from v0.5.1.
+        Furthermore, the library is updated to support Python 3.11, removed deprecated
+        options, and strengthened with more robust checks and error messages in the
+        schedulers.
+        
+        ### Changelog
+        
+        #### API
+        
+        - Support Python 3.11 (#342)
+        - Check that emitters passed in are lists/iterables in scheduler (#341)
+        - Fix Matplotlib `get_cmap` deprecation (#340)
+        - **Backwards-incompatible:** Default `plot_centroids` to False when plotting
+          (#339)
+        - Raise error messages when `ask` is called without `ask_dqd` (#338)
+        
+        #### Documentation
+        
+        - Add BibTex citation for GECCO 2023 (#337)
+        
+        #### Improvements
+        
+        - Update distribution dependencies (#344)
+        
         ## 0.5.1
         
         This release contains miscellaneous edits to our documentation from v0.5.0.
         There were no changes to library functionality in this release.
         
         ## 0.5.0
         
@@ -610,14 +644,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: visualize
 Provides-Extra: all
```

### Comparing `ribs-0.5.1/ribs.egg-info/SOURCES.txt` & `ribs-0.5.2/ribs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ribs-0.5.1/ribs.egg-info/requires.txt` & `ribs-0.5.2/ribs.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,14 @@
 sphinx-material==0.0.32
 sphinx-autobuild==2021.3.14
 sphinx-copybutton==0.3.1
 myst-nb==0.17.1
 sphinx-toolbox==3.1.0
 sphinx-autodoc-typehints==1.18.2
 sphinx-codeautolink==0.12.1
-bump2version==0.5.11
-wheel==0.36.2
-twine==1.14.0
-check-wheel-contents==0.2.0
+bump2version==1.0.1
+wheel==0.40.0
+twine==4.0.2
+check-wheel-contents==0.4.0
 
 [visualize]
 matplotlib>=3.0.0
```

### Comparing `ribs-0.5.1/setup.cfg` & `ribs-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.5.1
+current_version = 0.5.2
 commit = True
 tag = False
 
 [bumpversion:file:setup.py]
 search = version="{current_version}"
 replace = version="{new_version}"
```

### Comparing `ribs-0.5.1/setup.py` & `ribs-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,18 +48,18 @@
         "sphinx-copybutton==0.3.1",
         "myst-nb==0.17.1",
         "sphinx-toolbox==3.1.0",
         "sphinx-autodoc-typehints==1.18.2",
         "sphinx-codeautolink==0.12.1",
 
         # Distribution
-        "bump2version==0.5.11",
-        "wheel==0.36.2",
-        "twine==1.14.0",
-        "check-wheel-contents==0.2.0",
+        "bump2version==1.0.1",
+        "wheel==0.40.0",
+        "twine==4.0.2",
+        "check-wheel-contents==0.4.0",
     ],
 }
 
 setup(
     author="ICAROS Lab pyribs Team",
     author_email="team@pyribs.org",
     classifiers=[
@@ -70,14 +70,15 @@
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     description=
     "A bare-bones Python library for quality diversity optimization.",
     install_requires=install_requires,
@@ -88,10 +89,10 @@
     include_package_data=True,
     keywords="ribs",
     name="ribs",
     packages=find_packages(include=["ribs", "ribs.*"]),
     python_requires=">=3.7.0",
     test_suite="tests",
     url="https://github.com/icaros-usc/pyribs",
-    version="0.5.1",
+    version="0.5.2",
     zip_safe=False,
 )
```

