# Comparing `tmp/hyfi-1.2.6.tar.gz` & `tmp/hyfi-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-1.2.6.tar", max compression
+gzip compressed data, was "hyfi-1.2.7.tar", max compression
```

## Comparing `hyfi-1.2.6.tar` & `hyfi-1.2.7.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1071 2023-07-15 05:44:41.219177 hyfi-1.2.6/LICENSE
--rw-r--r--   0        0        0     1881 2023-07-15 05:44:41.219177 hyfi-1.2.6/README.md
--rw-r--r--   0        0        0     4862 2023-07-15 05:45:12.296234 hyfi-1.2.6/pyproject.toml
--rw-r--r--   0        0        0     3281 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/__cli__.py
--rw-r--r--   0        0        0     2465 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/__click__.py
--rw-r--r--   0        0        0      715 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-07-15 05:45:12.204233 hyfi-1.2.6/src/hyfi/_version.py
--rw-r--r--   0        0        0     2376 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/about/__init__.py
--rw-r--r--   0        0        0     7287 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/batch/__init__.py
--rw-r--r--   0        0        0     1206 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/__init__.py
--rw-r--r--   0        0        0    14373 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/cache_file.py
--rw-r--r--   0        0        0     1100 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/common.py
--rw-r--r--   0        0        0     1921 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/file_lock.py
--rw-r--r--   0        0        0     3441 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/meta.py
--rw-r--r--   0        0        0     3247 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/progress.py
--rw-r--r--   0        0        0     1437 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2942 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1222 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/testing.py
--rw-r--r--   0        0        0     4799 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/cached_path/version.py
--rw-r--r--   0        0        0    26044 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/composer/__init__.py
--rw-r--r--   0        0        0     1933 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/composer/pydantic.py
--rw-r--r--   0        0        0        0 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-07-15 05:45:12.208233 hyfi-1.2.6/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      588 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0        0 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/cmd/__init__.yaml
--rw-r--r--   0        0        0       49 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      155 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/cmd/copy_conf.yaml
--rw-r--r--   0        0        0       83 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/cmd/run_task.yaml
--rw-r--r--   0        0        0       91 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/cmd/run_workflow.yaml
--rw-r--r--   0        0        0      328 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      569 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      709 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      322 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      137 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      198 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/mode/__debug__.yaml
--rw-r--r--   0        0        0      901 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0       61 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/module/__init__.yaml
--rw-r--r--   0        0        0       72 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      880 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      125 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/path/__task__.yaml
--rw-r--r--   0        0        0      291 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/path/dirnames/__init__.yaml
--rw-r--r--   0        0        0       76 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/__dataframe__.yaml
--rw-r--r--   0        0        0       77 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
--rw-r--r--   0        0        0       79 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
--rw-r--r--   0        0        0       70 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/__general_external_funcs__.yaml
--rw-r--r--   0        0        0       72 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/__general_instance_methods__.yaml
--rw-r--r--   0        0        0      128 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/__init__.yaml
--rw-r--r--   0        0        0      236 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/load_dataframes.yaml
--rw-r--r--   0        0        0      241 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/save_dataframes.yaml
--rw-r--r--   0        0        0       90 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipe/test_preprocessing.yaml
--rw-r--r--   0        0        0       69 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipeline/__init__.yaml
--rw-r--r--   0        0        0      388 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipeline/__test_dataframe__.yaml
--rw-r--r--   0        0        0      268 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/pipeline/__test_general__.yaml
--rw-r--r--   0        0        0      744 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0      160 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/project/__test__.yaml
--rw-r--r--   0        0        0       38 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/running/__init__.yaml
--rw-r--r--   0        0        0      142 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/task/__batch__.yaml
--rw-r--r--   0        0        0      298 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0      183 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/task/__test__.yaml
--rw-r--r--   0        0        0      124 2023-07-15 05:44:41.227177 hyfi-1.2.6/src/hyfi/conf/workflow/__init__.yaml
--rw-r--r--   0        0        0      128 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/conf/workflow/__test__.yaml
--rw-r--r--   0        0        0     6558 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/copier/__init__.py
--rw-r--r--   0        0        0      844 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/core/__init__.py
--rw-r--r--   0        0        0    10581 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/core/config.py
--rw-r--r--   0        0        0     5915 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/dotenv/__init__.py
--rw-r--r--   0        0        0     3517 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/graphics/__init__.py
--rw-r--r--   0        0        0     8470 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/graphics/collage.py
--rw-r--r--   0        0        0     4538 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/graphics/motion.py
--rw-r--r--   0        0        0     7020 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/graphics/utils.py
--rw-r--r--   0        0        0     4214 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/joblib/__init__.py
--rw-r--r--   0        0        0      111 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/joblib/batch/__init__.py
--rw-r--r--   0        0        0     6312 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/joblib/batch/apply.py
--rw-r--r--   0        0        0     4779 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/joblib/batch/apply_batch.py
--rw-r--r--   0        0        0    13823 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/joblib/batch/batcher.py
--rw-r--r--   0        0        0    13627 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/main/__init__.py
--rw-r--r--   0        0        0      280 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/module/__init__.py
--rw-r--r--   0        0        0     4909 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/path/__init__.py
--rw-r--r--   0        0        0     4183 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/path/base.py
--rw-r--r--   0        0        0      533 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/path/batch.py
--rw-r--r--   0        0        0      599 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/path/dirnames.py
--rw-r--r--   0        0        0     1603 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/path/task.py
--rw-r--r--   0        0        0     5030 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/pipe/__init__.py
--rw-r--r--   0        0        0     1455 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/pipe/test.py
--rw-r--r--   0        0        0     8169 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/pipeline/__init__.py
--rw-r--r--   0        0        0     2874 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/pipeline/configs.py
--rw-r--r--   0        0        0     5837 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/project/__init__.py
--rw-r--r--   0        0        0        0 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/py.typed
--rw-r--r--   0        0        0     4262 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/task/__init__.py
--rw-r--r--   0        0        0     7041 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/task/batch.py
--rw-r--r--   0        0        0        0 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0    12742 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/conf.py
--rw-r--r--   0        0        0     1314 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/contexts.py
--rw-r--r--   0        0        0    30089 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/datasets.py
--rw-r--r--   0        0        0     8871 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/envs.py
--rw-r--r--   0        0        0    10857 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/funcs.py
--rw-r--r--   0        0        0     4930 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/gpumon.py
--rw-r--r--   0        0        0    20881 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/iolibs.py
--rw-r--r--   0        0        0     2259 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    12820 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/notebooks.py
--rw-r--r--   0        0        0     6955 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/packages.py
--rw-r--r--   0        0        0      382 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/utils/types.py
--rw-r--r--   0        0        0      753 2023-07-15 05:44:41.231178 hyfi-1.2.6/src/hyfi/workflow/__init__.py
--rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-15 23:50:05.093052 hyfi-1.2.7/LICENSE
+-rw-r--r--   0        0        0     1881 2023-07-15 23:50:05.093052 hyfi-1.2.7/README.md
+-rw-r--r--   0        0        0     4862 2023-07-15 23:50:31.609465 hyfi-1.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3281 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0     2465 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/__click__.py
+-rw-r--r--   0        0        0      715 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-15 23:50:31.533464 hyfi-1.2.7/src/hyfi/_version.py
+-rw-r--r--   0        0        0     2376 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/about/__init__.py
+-rw-r--r--   0        0        0     7287 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/batch/__init__.py
+-rw-r--r--   0        0        0     1206 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/__init__.py
+-rw-r--r--   0        0        0    14373 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1100 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/common.py
+-rw-r--r--   0        0        0     1921 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3441 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/meta.py
+-rw-r--r--   0        0        0     3247 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/progress.py
+-rw-r--r--   0        0        0     1437 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-07-15 23:50:05.097052 hyfi-1.2.7/src/hyfi/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2942 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1222 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/cached_path/testing.py
+-rw-r--r--   0        0        0     4799 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/cached_path/version.py
+-rw-r--r--   0        0        0    26044 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/composer/__init__.py
+-rw-r--r--   0        0        0     1933 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/composer/pydantic.py
+-rw-r--r--   0        0        0        0 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-07-15 23:50:31.533464 hyfi-1.2.7/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      588 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/cmd/__init__.yaml
+-rw-r--r--   0        0        0       49 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      155 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/cmd/copy_conf.yaml
+-rw-r--r--   0        0        0       83 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/cmd/run_task.yaml
+-rw-r--r--   0        0        0       91 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/cmd/run_workflow.yaml
+-rw-r--r--   0        0        0      328 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      569 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      709 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      322 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      137 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      198 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/mode/__debug__.yaml
+-rw-r--r--   0        0        0      969 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0       61 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/module/__init__.yaml
+-rw-r--r--   0        0        0       72 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      880 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      125 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/path/__task__.yaml
+-rw-r--r--   0        0        0      291 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/path/dirnames/__init__.yaml
+-rw-r--r--   0        0        0       76 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/__dataframe__.yaml
+-rw-r--r--   0        0        0       77 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/__dataframe_external_funcs__.yaml
+-rw-r--r--   0        0        0       79 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/__dataframe_instance_methods__.yaml
+-rw-r--r--   0        0        0       70 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/__general_external_funcs__.yaml
+-rw-r--r--   0        0        0       72 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/__general_instance_methods__.yaml
+-rw-r--r--   0        0        0      128 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/__init__.yaml
+-rw-r--r--   0        0        0      236 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/load_dataframes.yaml
+-rw-r--r--   0        0        0      241 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/save_dataframes.yaml
+-rw-r--r--   0        0        0       90 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipe/test_preprocessing.yaml
+-rw-r--r--   0        0        0       69 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipeline/__init__.yaml
+-rw-r--r--   0        0        0      388 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipeline/__test_dataframe__.yaml
+-rw-r--r--   0        0        0      268 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/pipeline/__test_general__.yaml
+-rw-r--r--   0        0        0      744 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0      160 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/project/__test__.yaml
+-rw-r--r--   0        0        0       38 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/running/__init__.yaml
+-rw-r--r--   0        0        0      142 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/task/__batch__.yaml
+-rw-r--r--   0        0        0      298 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/task/__init__.yaml
+-rw-r--r--   0        0        0      183 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/task/__test__.yaml
+-rw-r--r--   0        0        0      124 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/workflow/__init__.yaml
+-rw-r--r--   0        0        0      128 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/conf/workflow/__test__.yaml
+-rw-r--r--   0        0        0     6558 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/copier/__init__.py
+-rw-r--r--   0        0        0      844 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/core/__init__.py
+-rw-r--r--   0        0        0    10581 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/core/config.py
+-rw-r--r--   0        0        0     5915 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/dotenv/__init__.py
+-rw-r--r--   0        0        0     3517 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/graphics/__init__.py
+-rw-r--r--   0        0        0     8470 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/graphics/collage.py
+-rw-r--r--   0        0        0     4538 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/graphics/motion.py
+-rw-r--r--   0        0        0     7020 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/graphics/utils.py
+-rw-r--r--   0        0        0     4214 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/joblib/__init__.py
+-rw-r--r--   0        0        0      111 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/joblib/batch/__init__.py
+-rw-r--r--   0        0        0     6312 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/joblib/batch/apply.py
+-rw-r--r--   0        0        0     4779 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/joblib/batch/apply_batch.py
+-rw-r--r--   0        0        0    13823 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/joblib/batch/batcher.py
+-rw-r--r--   0        0        0    13627 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/main/__init__.py
+-rw-r--r--   0        0        0      280 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/module/__init__.py
+-rw-r--r--   0        0        0     4909 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/path/__init__.py
+-rw-r--r--   0        0        0     4183 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/path/base.py
+-rw-r--r--   0        0        0      533 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/path/batch.py
+-rw-r--r--   0        0        0      599 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/path/dirnames.py
+-rw-r--r--   0        0        0     1603 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/path/task.py
+-rw-r--r--   0        0        0     5030 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/pipe/__init__.py
+-rw-r--r--   0        0        0     1455 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/pipe/test.py
+-rw-r--r--   0        0        0     8169 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/pipeline/__init__.py
+-rw-r--r--   0        0        0     3094 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/pipeline/configs.py
+-rw-r--r--   0        0        0     5837 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/project/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/py.typed
+-rw-r--r--   0        0        0     4262 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/task/__init__.py
+-rw-r--r--   0        0        0     7041 2023-07-15 23:50:05.101052 hyfi-1.2.7/src/hyfi/task/batch.py
+-rw-r--r--   0        0        0        0 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0    12742 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/conf.py
+-rw-r--r--   0        0        0     1314 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/contexts.py
+-rw-r--r--   0        0        0    30089 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/datasets.py
+-rw-r--r--   0        0        0     8871 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/envs.py
+-rw-r--r--   0        0        0    10857 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/funcs.py
+-rw-r--r--   0        0        0     4930 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/gpumon.py
+-rw-r--r--   0        0        0    20881 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/iolibs.py
+-rw-r--r--   0        0        0     2259 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    12820 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/notebooks.py
+-rw-r--r--   0        0        0     6955 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/packages.py
+-rw-r--r--   0        0        0      382 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0      753 2023-07-15 23:50:05.105052 hyfi-1.2.7/src/hyfi/workflow/__init__.py
+-rw-r--r--   0        0        0     3386 1970-01-01 00:00:00.000000 hyfi-1.2.7/PKG-INFO
```

### Comparing `hyfi-1.2.6/LICENSE` & `hyfi-1.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/README.md` & `hyfi-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/pyproject.toml` & `hyfi-1.2.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "1.2.6"
+version = "1.2.7"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-1.2.6/src/hyfi/__cli__.py` & `hyfi-1.2.7/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/__click__.py` & `hyfi-1.2.7/src/hyfi/__click__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/__init__.py` & `hyfi-1.2.7/src/hyfi/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/about/__init__.py` & `hyfi-1.2.7/src/hyfi/about/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/batch/__init__.py` & `hyfi-1.2.7/src/hyfi/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/__init__.py` & `hyfi-1.2.7/src/hyfi/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/_cached_path.py` & `hyfi-1.2.7/src/hyfi/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/cache_file.py` & `hyfi-1.2.7/src/hyfi/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/common.py` & `hyfi-1.2.7/src/hyfi/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/file_lock.py` & `hyfi-1.2.7/src/hyfi/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/meta.py` & `hyfi-1.2.7/src/hyfi/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/progress.py` & `hyfi-1.2.7/src/hyfi/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/schemes/__init__.py` & `hyfi-1.2.7/src/hyfi/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/schemes/beaker.py` & `hyfi-1.2.7/src/hyfi/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/schemes/hf.py` & `hyfi-1.2.7/src/hyfi/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/schemes/http.py` & `hyfi-1.2.7/src/hyfi/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/schemes/scheme_client.py` & `hyfi-1.2.7/src/hyfi/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/testing.py` & `hyfi-1.2.7/src/hyfi/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/cached_path/util.py` & `hyfi-1.2.7/src/hyfi/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/composer/__init__.py` & `hyfi-1.2.7/src/hyfi/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/composer/pydantic.py` & `hyfi-1.2.7/src/hyfi/composer/pydantic.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/conf/batch/__init__.yaml` & `hyfi-1.2.7/src/hyfi/conf/batch/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/conf/copier/conf.yaml` & `hyfi-1.2.7/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-1.2.7/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-1.2.7/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/conf/mode/__init__.yaml` & `hyfi-1.2.7/src/hyfi/conf/mode/__init__.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # @package _global_
 debug_mode: false
 resolve: true
 verbose: false
 ignore_warnings: true
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
-hydra_log_dir: ${oc.select:project.path.project_logs, ${oc.select:task.path.task_logs, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}/logs}}/hydra
+hydra_log_dir: ${oc.select:project.global_hyfi_root, ${alt:${oc.env:HYFI_GLOBAL_ROOT,null},${__home_path__:}/.hyfi}}/${oc.select:project.global_workspace_name, ${alt:${oc.env:HYFI_GLOBAL_WORKSPACE_NAME,null},workspace}}/logs/hydra
 
 hydra:
   job:
     name: ${oc.select:project.project_name, ${oc.select:task.project.project_name, ${alt:${oc.env:HYFI_PROJECT_NAME,null},hyfi-project}}}
     chdir: true
   run:
     dir: ${hydra_log_dir}/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
```

### Comparing `hyfi-1.2.6/src/hyfi/conf/path/__init__.yaml` & `hyfi-1.2.7/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/conf/project/__init__.yaml` & `hyfi-1.2.7/src/hyfi/conf/project/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/copier/__init__.py` & `hyfi-1.2.7/src/hyfi/copier/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/core/__init__.py` & `hyfi-1.2.7/src/hyfi/core/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/core/config.py` & `hyfi-1.2.7/src/hyfi/core/config.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/dotenv/__init__.py` & `hyfi-1.2.7/src/hyfi/dotenv/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/graphics/__init__.py` & `hyfi-1.2.7/src/hyfi/graphics/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/graphics/collage.py` & `hyfi-1.2.7/src/hyfi/graphics/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/graphics/motion.py` & `hyfi-1.2.7/src/hyfi/graphics/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/graphics/utils.py` & `hyfi-1.2.7/src/hyfi/graphics/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/joblib/__init__.py` & `hyfi-1.2.7/src/hyfi/joblib/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/joblib/batch/apply.py` & `hyfi-1.2.7/src/hyfi/joblib/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/joblib/batch/apply_batch.py` & `hyfi-1.2.7/src/hyfi/joblib/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/joblib/batch/batcher.py` & `hyfi-1.2.7/src/hyfi/joblib/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/main/__init__.py` & `hyfi-1.2.7/src/hyfi/main/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/path/__init__.py` & `hyfi-1.2.7/src/hyfi/path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/path/base.py` & `hyfi-1.2.7/src/hyfi/path/base.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/path/batch.py` & `hyfi-1.2.7/src/hyfi/path/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/path/dirnames.py` & `hyfi-1.2.7/src/hyfi/path/dirnames.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/path/task.py` & `hyfi-1.2.7/src/hyfi/path/task.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/pipe/__init__.py` & `hyfi-1.2.7/src/hyfi/pipe/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/pipe/test.py` & `hyfi-1.2.7/src/hyfi/pipe/test.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/pipeline/__init__.py` & `hyfi-1.2.7/src/hyfi/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/pipeline/configs.py` & `hyfi-1.2.7/src/hyfi/pipeline/configs.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,21 +71,24 @@
         elif self.pipe_target:
             return Composer.partial(self.pipe_target)
         else:
             return None
 
     def get_run_func(self) -> Optional[Callable]:
         if self.run.startswith("lambda"):
+            logger.info("Returning lambda function: %s", self.run)
             return eval(self.run)
         elif self.run:
             kwargs = self.run_with or {}
             if self.pipe_obj_arg_name:
                 kwargs.pop(self.pipe_obj_arg_name)
+            logger.info("Returning partial function: %s with kwargs: %s", self.run, kwargs)
             return Composer.partial(self.run, **kwargs)
         else:
+            logger.warning("No function found for %s", self)
             return None
 
 
 class DataframePipeConfig(PipeConfig):
     columns_to_apply: Optional[Union[str, List[str]]] = []
     use_batcher: bool = True
     num_workers: int = 1
```

### Comparing `hyfi-1.2.6/src/hyfi/project/__init__.py` & `hyfi-1.2.7/src/hyfi/project/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/task/__init__.py` & `hyfi-1.2.7/src/hyfi/task/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/task/batch.py` & `hyfi-1.2.7/src/hyfi/task/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/conf.py` & `hyfi-1.2.7/src/hyfi/utils/conf.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/contexts.py` & `hyfi-1.2.7/src/hyfi/utils/contexts.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/datasets.py` & `hyfi-1.2.7/src/hyfi/utils/datasets.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/envs.py` & `hyfi-1.2.7/src/hyfi/utils/envs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/funcs.py` & `hyfi-1.2.7/src/hyfi/utils/funcs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/gpumon.py` & `hyfi-1.2.7/src/hyfi/utils/gpumon.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/iolibs.py` & `hyfi-1.2.7/src/hyfi/utils/iolibs.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/logging.py` & `hyfi-1.2.7/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/notebooks.py` & `hyfi-1.2.7/src/hyfi/utils/notebooks.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/utils/packages.py` & `hyfi-1.2.7/src/hyfi/utils/packages.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/src/hyfi/workflow/__init__.py` & `hyfi-1.2.7/src/hyfi/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-1.2.6/PKG-INFO` & `hyfi-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 1.2.6
+Version: 1.2.7
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

