# Comparing `tmp/muutils-0.4.3.tar.gz` & `tmp/muutils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muutils-0.4.3.tar", max compression
+gzip compressed data, was "muutils-0.4.4.tar", max compression
```

## Comparing `muutils-0.4.3.tar` & `muutils-0.4.4.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.4.3/LICENSE
--rw-r--r--   0        0        0       22 2023-06-14 07:25:08.958584 muutils-0.4.3/muutils/__init__.py
--rw-r--r--   0        0        0     4014 2023-06-14 07:24:44.650510 muutils-0.4.3/muutils/_wip/dataclass_validator.py
--rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.4.3/muutils/_wip/experiments.ipynb
--rw-r--r--   0        0        0     5834 2023-06-14 07:24:44.650510 muutils-0.4.3/muutils/_wip/gptdataset.py
--rw-r--r--   0        0        0    23255 2023-06-14 07:24:44.650510 muutils-0.4.3/muutils/_wip/json_serialize_old.py
--rw-r--r--   0        0        0     3281 2023-06-14 07:24:44.656519 muutils-0.4.3/muutils/_wip/lazy_externals.py
--rw-r--r--   0        0        0    10195 2023-06-14 07:24:44.656731 muutils-0.4.3/muutils/_wip/newargparser.py
--rw-r--r--   0        0        0     7415 2023-06-14 07:24:44.657732 muutils-0.4.3/muutils/_wip/torch_util_old.py
--rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.4.3/muutils/dictmagic.py
--rw-r--r--   0        0        0     1950 2023-06-14 07:24:44.658733 muutils-0.4.3/muutils/group_equiv.py
--rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.4.3/muutils/json_serialize/__init__.py
--rw-r--r--   0        0        0     6272 2023-05-20 23:35:42.047282 muutils-0.4.3/muutils/json_serialize/array.py
--rw-r--r--   0        0        0    11124 2023-06-14 07:24:44.659732 muutils-0.4.3/muutils/json_serialize/dataclass_factories.py
--rw-r--r--   0        0        0     9048 2023-05-20 23:35:42.048268 muutils-0.4.3/muutils/json_serialize/json_serialize.py
--rw-r--r--   0        0        0    16919 2023-05-28 05:49:08.535171 muutils-0.4.3/muutils/json_serialize/serializable_dataclass.py
--rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.4.3/muutils/json_serialize/util.py
--rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.4.3/muutils/jsonlines.py
--rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.4.3/muutils/logger/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.4.3/muutils/logger/exception_context.py
--rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.4.3/muutils/logger/headerfuncs.py
--rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.4.3/muutils/logger/log_util.py
--rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.4.3/muutils/logger/logger.py
--rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.4.3/muutils/logger/loggingstream.py
--rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.4.3/muutils/logger/simplelogger.py
--rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.4.3/muutils/logger/timing.py
--rw-r--r--   0        0        0     2607 2023-05-17 07:31:29.361724 muutils-0.4.3/muutils/misc.py
--rw-r--r--   0        0        0     3356 2023-06-13 21:17:26.051156 muutils-0.4.3/muutils/mlutils.py
--rw-r--r--   0        0        0        0 2023-06-13 21:17:26.051156 muutils-0.4.3/muutils/nbutils/__init__.py
--rw-r--r--   0        0        0     1452 2023-06-13 21:17:26.052156 muutils-0.4.3/muutils/nbutils/configure_notebook.py
--rw-r--r--   0        0        0    12383 2023-06-14 07:24:44.660732 muutils-0.4.3/muutils/nbutils/convert_ipynb_to_script.py
--rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.4.3/muutils/nbutils/print_tex.py
--rw-r--r--   0        0        0     3860 2023-06-14 07:24:44.661730 muutils-0.4.3/muutils/nbutils/run_notebook_tests.py
--rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.4.3/muutils/py.typed
--rw-r--r--   0        0        0     7753 2023-05-28 05:49:08.539161 muutils-0.4.3/muutils/statcounter.py
--rw-r--r--   0        0        0     6376 2023-06-14 07:24:44.661730 muutils-0.4.3/muutils/sysinfo.py
--rw-r--r--   0        0        0    10235 2023-05-28 05:49:08.540162 muutils-0.4.3/muutils/tensor_utils.py
--rw-r--r--   0        0        0     1344 2023-06-14 07:25:17.339614 muutils-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     3041 2023-06-14 02:35:51.207754 muutils-0.4.3/README.md
--rw-r--r--   0        0        0     3975 1970-01-01 00:00:00.000000 muutils-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    35823 2021-01-10 20:54:08.928022 muutils-0.4.4/LICENSE
+-rw-r--r--   0        0        0       22 2023-07-15 22:26:31.993759 muutils-0.4.4/muutils/__init__.py
+-rw-r--r--   0        0        0     4014 2023-06-14 07:24:44.650510 muutils-0.4.4/muutils/_wip/dataclass_validator.py
+-rw-r--r--   0        0        0     4652 2023-02-16 09:10:54.613167 muutils-0.4.4/muutils/_wip/experiments.ipynb
+-rw-r--r--   0        0        0     5834 2023-06-14 07:24:44.650510 muutils-0.4.4/muutils/_wip/gptdataset.py
+-rw-r--r--   0        0        0    23255 2023-06-14 07:24:44.650510 muutils-0.4.4/muutils/_wip/json_serialize_old.py
+-rw-r--r--   0        0        0     3281 2023-06-14 07:24:44.656519 muutils-0.4.4/muutils/_wip/lazy_externals.py
+-rw-r--r--   0        0        0    10195 2023-06-14 07:24:44.656731 muutils-0.4.4/muutils/_wip/newargparser.py
+-rw-r--r--   0        0        0     7415 2023-06-14 07:24:44.657732 muutils-0.4.4/muutils/_wip/torch_util_old.py
+-rw-r--r--   0        0        0     3751 2023-04-10 21:51:10.344133 muutils-0.4.4/muutils/dictmagic.py
+-rw-r--r--   0        0        0     1950 2023-06-14 07:24:44.658733 muutils-0.4.4/muutils/group_equiv.py
+-rw-r--r--   0        0        0      897 2023-03-24 22:25:29.761326 muutils-0.4.4/muutils/json_serialize/__init__.py
+-rw-r--r--   0        0        0     6272 2023-05-20 23:35:42.047282 muutils-0.4.4/muutils/json_serialize/array.py
+-rw-r--r--   0        0        0    11124 2023-06-14 07:24:44.659732 muutils-0.4.4/muutils/json_serialize/dataclass_factories.py
+-rw-r--r--   0        0        0     9048 2023-05-20 23:35:42.048268 muutils-0.4.4/muutils/json_serialize/json_serialize.py
+-rw-r--r--   0        0        0    16919 2023-05-28 05:49:08.535171 muutils-0.4.4/muutils/json_serialize/serializable_dataclass.py
+-rw-r--r--   0        0        0     3764 2023-03-28 07:47:43.743882 muutils-0.4.4/muutils/json_serialize/util.py
+-rw-r--r--   0        0        0     1878 2023-03-24 22:25:29.764321 muutils-0.4.4/muutils/jsonlines.py
+-rw-r--r--   0        0        0     1225 2023-07-15 22:26:31.994739 muutils-0.4.4/muutils/kappa.py
+-rw-r--r--   0        0        0      267 2023-03-06 19:25:21.021547 muutils-0.4.4/muutils/logger/__init__.py
+-rw-r--r--   0        0        0     1183 2023-03-06 19:25:21.021547 muutils-0.4.4/muutils/logger/exception_context.py
+-rw-r--r--   0        0        0     1667 2023-03-24 22:25:29.765321 muutils-0.4.4/muutils/logger/headerfuncs.py
+-rw-r--r--   0        0        0     2072 2023-03-24 22:25:29.765321 muutils-0.4.4/muutils/logger/log_util.py
+-rw-r--r--   0        0        0    10676 2023-05-28 05:49:08.536167 muutils-0.4.4/muutils/logger/logger.py
+-rw-r--r--   0        0        0     3820 2023-05-28 05:49:08.537161 muutils-0.4.4/muutils/logger/loggingstream.py
+-rw-r--r--   0        0        0     2124 2023-03-24 22:25:29.768323 muutils-0.4.4/muutils/logger/simplelogger.py
+-rw-r--r--   0        0        0     2538 2023-05-28 05:49:08.537161 muutils-0.4.4/muutils/logger/timing.py
+-rw-r--r--   0        0        0     2607 2023-05-17 07:31:29.361724 muutils-0.4.4/muutils/misc.py
+-rw-r--r--   0        0        0     3356 2023-06-13 21:17:26.051156 muutils-0.4.4/muutils/mlutils.py
+-rw-r--r--   0        0        0        0 2023-06-13 21:17:26.051156 muutils-0.4.4/muutils/nbutils/__init__.py
+-rw-r--r--   0        0        0     1452 2023-06-13 21:17:26.052156 muutils-0.4.4/muutils/nbutils/configure_notebook.py
+-rw-r--r--   0        0        0    12383 2023-06-14 07:24:44.660732 muutils-0.4.4/muutils/nbutils/convert_ipynb_to_script.py
+-rw-r--r--   0        0        0      446 2023-05-28 05:49:08.538163 muutils-0.4.4/muutils/nbutils/print_tex.py
+-rw-r--r--   0        0        0     3860 2023-06-14 07:24:44.661730 muutils-0.4.4/muutils/nbutils/run_notebook_tests.py
+-rw-r--r--   0        0        0        0 2023-03-28 07:47:43.743882 muutils-0.4.4/muutils/py.typed
+-rw-r--r--   0        0        0     7753 2023-05-28 05:49:08.539161 muutils-0.4.4/muutils/statcounter.py
+-rw-r--r--   0        0        0     6376 2023-06-14 07:24:44.661730 muutils-0.4.4/muutils/sysinfo.py
+-rw-r--r--   0        0        0    10235 2023-05-28 05:49:08.540162 muutils-0.4.4/muutils/tensor_utils.py
+-rw-r--r--   0        0        0     1344 2023-07-15 22:26:31.996740 muutils-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     3123 2023-06-14 19:35:15.200488 muutils-0.4.4/README.md
+-rw-r--r--   0        0        0     3955 1970-01-01 00:00:00.000000 muutils-0.4.4/PKG-INFO
```

### Comparing `muutils-0.4.3/LICENSE` & `muutils-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/_wip/dataclass_validator.py` & `muutils-0.4.4/muutils/_wip/dataclass_validator.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/_wip/experiments.ipynb` & `muutils-0.4.4/muutils/_wip/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/_wip/gptdataset.py` & `muutils-0.4.4/muutils/_wip/gptdataset.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/_wip/json_serialize_old.py` & `muutils-0.4.4/muutils/_wip/json_serialize_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/_wip/lazy_externals.py` & `muutils-0.4.4/muutils/_wip/lazy_externals.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/_wip/newargparser.py` & `muutils-0.4.4/muutils/_wip/newargparser.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/_wip/torch_util_old.py` & `muutils-0.4.4/muutils/_wip/torch_util_old.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/dictmagic.py` & `muutils-0.4.4/muutils/dictmagic.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/group_equiv.py` & `muutils-0.4.4/muutils/group_equiv.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/json_serialize/__init__.py` & `muutils-0.4.4/muutils/json_serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/json_serialize/array.py` & `muutils-0.4.4/muutils/json_serialize/array.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/json_serialize/dataclass_factories.py` & `muutils-0.4.4/muutils/json_serialize/dataclass_factories.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/json_serialize/json_serialize.py` & `muutils-0.4.4/muutils/json_serialize/json_serialize.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/json_serialize/serializable_dataclass.py` & `muutils-0.4.4/muutils/json_serialize/serializable_dataclass.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/json_serialize/util.py` & `muutils-0.4.4/muutils/json_serialize/util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/jsonlines.py` & `muutils-0.4.4/muutils/jsonlines.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/logger/exception_context.py` & `muutils-0.4.4/muutils/logger/exception_context.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/logger/headerfuncs.py` & `muutils-0.4.4/muutils/logger/headerfuncs.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/logger/log_util.py` & `muutils-0.4.4/muutils/logger/log_util.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/logger/logger.py` & `muutils-0.4.4/muutils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/logger/loggingstream.py` & `muutils-0.4.4/muutils/logger/loggingstream.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/logger/simplelogger.py` & `muutils-0.4.4/muutils/logger/simplelogger.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/logger/timing.py` & `muutils-0.4.4/muutils/logger/timing.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/misc.py` & `muutils-0.4.4/muutils/misc.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/mlutils.py` & `muutils-0.4.4/muutils/mlutils.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/nbutils/configure_notebook.py` & `muutils-0.4.4/muutils/nbutils/configure_notebook.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/nbutils/convert_ipynb_to_script.py` & `muutils-0.4.4/muutils/nbutils/convert_ipynb_to_script.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/nbutils/run_notebook_tests.py` & `muutils-0.4.4/muutils/nbutils/run_notebook_tests.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/statcounter.py` & `muutils-0.4.4/muutils/statcounter.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/sysinfo.py` & `muutils-0.4.4/muutils/sysinfo.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/muutils/tensor_utils.py` & `muutils-0.4.4/muutils/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `muutils-0.4.3/pyproject.toml` & `muutils-0.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muutils"
-version = "0.4.3"
+version = "0.4.4"
 description = "A collection of miscellaneous python utilities"
 license = "GPL-3.0-only"
 authors = ["mivanit <mivanits@umich.edu>"]
 readme = "README.md"
 classifiers=[
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
```

### Comparing `muutils-0.4.3/README.md` & `muutils-0.4.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,7 +32,11 @@
 # installation
 
 PyPi: [muutils](https://pypi.org/project/muutils/)
 
 ```
 pip install muutils
 ```
+
+# todos:
+
+- [ ] option to have notebook conversion create pytest-compatible tests
```

### Comparing `muutils-0.4.3/PKG-INFO` & `muutils-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 Metadata-Version: 2.1
 Name: muutils
-Version: 0.4.3
+Version: 0.4.4
 Summary: A collection of miscellaneous python utilities
 Home-page: https://github.com/mivanit/muutils
 License: GPL-3.0-only
 Author: mivanit
 Author-email: mivanits@umich.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jaxtyping (>=0.2.12,<0.3.0)
 Requires-Dist: numpy (>=1.22.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: torch (>=1.13.1,<2.0.0)
 Project-URL: Repository, https://github.com/mivanit/muutils
 Description-Content-Type: text/markdown
 
@@ -57,7 +55,10 @@
 
 PyPi: [muutils](https://pypi.org/project/muutils/)
 
 ```
 pip install muutils
 ```
 
+# todos:
+
+- [ ] option to have notebook conversion create pytest-compatible tests
```

