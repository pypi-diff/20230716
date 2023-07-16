# Comparing `tmp/bge-python-sdk-0.5.1.tar.gz` & `tmp/bge-python-sdk-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bge-python-sdk-0.5.1.tar", last modified: Mon Oct 17 09:55:56 2022, max compression
+gzip compressed data, was "bge-python-sdk-0.5.2.tar", last modified: Wed Jul 12 03:19:45 2023, max compression
```

## Comparing `bge-python-sdk-0.5.1.tar` & `bge-python-sdk-0.5.2.tar`

### file list

```diff
@@ -1,70 +1,85 @@
-drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2022-10-17 09:55:56.712659 bge-python-sdk-0.5.1/
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1063 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/LICENSE
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       43 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/MANIFEST.in
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     7140 2022-10-17 09:55:56.732659 bge-python-sdk-0.5.1/PKG-INFO
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     5814 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/README.md
-drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2022-10-17 09:55:56.524656 bge-python-sdk-0.5.1/bge_python_sdk.egg-info/
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     7140 2022-10-17 09:55:55.000000 bge-python-sdk-0.5.1/bge_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1975 2022-10-17 09:55:56.000000 bge-python-sdk-0.5.1/bge_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)        1 2022-10-17 09:55:55.000000 bge-python-sdk-0.5.1/bge_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       45 2022-10-17 09:55:55.000000 bge-python-sdk-0.5.1/bge_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      145 2022-10-17 09:55:55.000000 bge-python-sdk-0.5.1/bge_python_sdk.egg-info/requires.txt
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       13 2022-10-17 09:55:55.000000 bge-python-sdk-0.5.1/bge_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2022-10-17 09:55:56.584657 bge-python-sdk-0.5.1/bgesdk/
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      124 2021-09-22 03:06:41.000000 bge-python-sdk-0.5.1/bgesdk/__init__.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2196 2022-06-08 01:56:26.000000 bge-python-sdk-0.5.1/bgesdk/__main__.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    48877 2022-10-17 09:55:03.000000 bge-python-sdk-0.5.1/bgesdk/client.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      636 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/bgesdk/constants.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      462 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/error.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      154 2022-04-20 13:38:14.000000 bge-python-sdk-0.5.1/bgesdk/fs.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     4503 2022-07-11 08:38:46.000000 bge-python-sdk-0.5.1/bgesdk/http.py
-drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2022-10-17 09:55:56.588657 bge-python-sdk-0.5.1/bgesdk/management/
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)        0 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/bgesdk/management/__init__.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      701 2022-03-02 01:55:58.000000 bge-python-sdk-0.5.1/bgesdk/management/command.py
-drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2022-10-17 09:55:56.596657 bge-python-sdk-0.5.1/bgesdk/management/commands/
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)        0 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/__init__.py
-drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2022-10-17 09:55:56.608657 bge-python-sdk-0.5.1/bgesdk/management/commands/api/
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1975 2022-06-08 01:56:26.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/__init__.py
-drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2022-10-17 09:55:56.672658 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)        0 2021-08-18 03:47:15.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/__init__.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3213 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/aggregate_omics_data.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3508 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/download.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2584 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_data_items.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1935 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_externals.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2713 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_func_abundance.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2933 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_gene_abundance.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2955 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_range_stream.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3514 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_samples.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2385 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_taxon_abundance.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1573 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_user.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1944 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_variants.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1696 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/task.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3405 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/upload.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3802 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/upload_dir.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     7118 2022-06-08 01:56:26.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/config.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3919 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/login.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    55420 2022-07-11 08:38:46.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/model.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    13811 2022-06-08 01:56:26.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/model_doc.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2515 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/token.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1183 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/bgesdk/management/commands/workon.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1508 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/bgesdk/management/constants.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     4774 2022-07-11 08:38:46.000000 bge-python-sdk-0.5.1/bgesdk/management/utils.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2044 2021-09-03 08:44:34.000000 bge-python-sdk-0.5.1/bgesdk/management/validate.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3865 2021-08-18 03:47:15.000000 bge-python-sdk-0.5.1/bgesdk/models.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      884 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/bgesdk/utils.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       46 2022-10-17 09:55:03.000000 bge-python-sdk-0.5.1/bgesdk/version.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      223 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/pytest.ini
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      144 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/requirements.txt
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1406 2022-10-17 09:55:56.736659 bge-python-sdk-0.5.1/setup.cfg
--rwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)      333 2022-03-02 01:55:58.000000 bge-python-sdk-0.5.1/setup.py
-drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2022-10-17 09:55:56.708659 bge-python-sdk-0.5.1/tests/
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       35 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/tests/__init__.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2171 2022-10-17 06:35:27.000000 bge-python-sdk-0.5.1/tests/conftest.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3687 2022-10-17 06:35:46.000000 bge-python-sdk-0.5.1/tests/test_abundance.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      210 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/tests/test_fs.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      401 2022-04-20 13:37:38.000000 bge-python-sdk-0.5.1/tests/test_model.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      783 2022-06-07 08:52:47.000000 bge-python-sdk-0.5.1/tests/test_models.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      955 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.1/tests/test_oauth2.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3004 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.1/tests/test_samples.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      389 2021-09-03 07:50:13.000000 bge-python-sdk-0.5.1/tests/test_user.py
--rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2780 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.1/tests/test_variants.py
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.501208 bge-python-sdk-0.5.2/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    77824 2023-07-12 03:17:59.000000 bge-python-sdk-0.5.2/.coverage
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       71 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/.coveragerc
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.469208 bge-python-sdk-0.5.2/.github/
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.481208 bge-python-sdk-0.5.2/.github/workflows/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      627 2022-02-28 07:59:30.000000 bge-python-sdk-0.5.2/.github/workflows/release.yml
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      221 2023-07-12 01:47:56.000000 bge-python-sdk-0.5.2/.gitignore
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    14012 2023-07-12 03:01:47.000000 bge-python-sdk-0.5.2/CHANGELOG.md
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      810 2023-01-16 06:35:31.000000 bge-python-sdk-0.5.2/Jenkinsfile
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1063 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.2/LICENSE
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       43 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.2/MANIFEST.in
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1364 2023-07-12 03:16:41.000000 bge-python-sdk-0.5.2/Makefile
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     7140 2023-07-12 03:19:45.501208 bge-python-sdk-0.5.2/PKG-INFO
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     5814 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.2/README.md
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.481208 bge-python-sdk-0.5.2/bge_python_sdk.egg-info/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     7140 2023-07-12 03:19:45.000000 bge-python-sdk-0.5.2/bge_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2175 2023-07-12 03:19:45.000000 bge-python-sdk-0.5.2/bge_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)        1 2023-07-12 03:19:45.000000 bge-python-sdk-0.5.2/bge_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       45 2023-07-12 03:19:45.000000 bge-python-sdk-0.5.2/bge_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      145 2023-07-12 03:19:45.000000 bge-python-sdk-0.5.2/bge_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       13 2023-07-12 03:19:45.000000 bge-python-sdk-0.5.2/bge_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.485208 bge-python-sdk-0.5.2/bgesdk/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      124 2021-09-22 03:06:41.000000 bge-python-sdk-0.5.2/bgesdk/__init__.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2196 2022-06-08 01:56:26.000000 bge-python-sdk-0.5.2/bgesdk/__main__.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    51777 2023-07-12 02:06:44.000000 bge-python-sdk-0.5.2/bgesdk/client.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      636 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.2/bgesdk/constants.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      462 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/error.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      154 2022-04-20 13:38:14.000000 bge-python-sdk-0.5.2/bgesdk/fs.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     4503 2022-07-11 08:38:46.000000 bge-python-sdk-0.5.2/bgesdk/http.py
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.489208 bge-python-sdk-0.5.2/bgesdk/management/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)        0 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.2/bgesdk/management/__init__.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      701 2022-03-02 01:55:58.000000 bge-python-sdk-0.5.2/bgesdk/management/command.py
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.489208 bge-python-sdk-0.5.2/bgesdk/management/commands/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)        0 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/__init__.py
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.489208 bge-python-sdk-0.5.2/bgesdk/management/commands/api/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1975 2022-06-08 01:56:26.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/__init__.py
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.497208 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)        0 2021-08-18 03:47:15.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/__init__.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3213 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/aggregate_omics_data.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3508 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/download.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2584 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_data_items.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1935 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_externals.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2713 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_func_abundance.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2933 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_gene_abundance.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2955 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_range_stream.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3514 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_samples.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2385 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_taxon_abundance.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1573 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_user.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1944 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_variants.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1696 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/task.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3405 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/upload.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3802 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/upload_dir.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     7118 2022-06-08 01:56:26.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/config.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3919 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/login.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    55420 2022-07-11 08:38:46.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/model.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    13811 2022-06-08 01:56:26.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/model_doc.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2515 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/token.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1183 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/bgesdk/management/commands/workon.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1508 2022-10-17 08:19:10.000000 bge-python-sdk-0.5.2/bgesdk/management/constants.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     4774 2022-07-11 08:38:46.000000 bge-python-sdk-0.5.2/bgesdk/management/utils.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2044 2021-09-03 08:44:34.000000 bge-python-sdk-0.5.2/bgesdk/management/validate.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3865 2021-08-18 03:47:15.000000 bge-python-sdk-0.5.2/bgesdk/models.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      884 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.2/bgesdk/utils.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       46 2023-07-12 01:57:24.000000 bge-python-sdk-0.5.2/bgesdk/version.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)    33622 2023-07-12 03:17:59.000000 bge-python-sdk-0.5.2/coverage.xml
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      243 2023-07-11 09:36:42.000000 bge-python-sdk-0.5.2/package.json
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      223 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.2/pytest.ini
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      144 2023-07-12 02:43:09.000000 bge-python-sdk-0.5.2/requirements.txt
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1407 2023-07-12 03:19:45.501208 bge-python-sdk-0.5.2/setup.cfg
+-rwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)      333 2023-07-11 09:07:48.000000 bge-python-sdk-0.5.2/setup.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      478 2023-07-11 09:24:37.000000 bge-python-sdk-0.5.2/sonar-project.properties
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      348 2022-03-02 01:55:58.000000 bge-python-sdk-0.5.2/test_env.sh.example
+drwxr-xr-x   0 zhanglei3  (1000) zhanglei3  (1000)        0 2023-07-12 03:19:45.501208 bge-python-sdk-0.5.2/tests/
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)       35 2021-05-17 07:33:01.000000 bge-python-sdk-0.5.2/tests/__init__.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3208 2023-07-12 01:24:53.000000 bge-python-sdk-0.5.2/tests/conftest.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     4013 2023-07-12 01:20:14.000000 bge-python-sdk-0.5.2/tests/test_abundance.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      210 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/tests/test_fs.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      429 2023-07-12 01:20:29.000000 bge-python-sdk-0.5.2/tests/test_model.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      768 2023-07-12 01:21:26.000000 bge-python-sdk-0.5.2/tests/test_models.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     1097 2023-07-12 01:49:04.000000 bge-python-sdk-0.5.2/tests/test_oauth2.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     2264 2023-07-12 01:49:42.000000 bge-python-sdk-0.5.2/tests/test_phenotype.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3341 2023-07-12 01:23:24.000000 bge-python-sdk-0.5.2/tests/test_samples.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      417 2023-07-12 01:23:36.000000 bge-python-sdk-0.5.2/tests/test_user.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)     3056 2023-07-12 01:24:18.000000 bge-python-sdk-0.5.2/tests/test_variants.py
+-rw-r--r--   0 zhanglei3  (1000) zhanglei3  (1000)      678 2022-04-22 03:31:36.000000 bge-python-sdk-0.5.2/tox.ini
```

### Comparing `bge-python-sdk-0.5.1/LICENSE` & `bge-python-sdk-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/PKG-INFO` & `bge-python-sdk-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bge-python-sdk
-Version: 0.5.1
+Version: 0.5.2
 Summary: 可用于调用 BGE 开放平台的相关接口。
 Home-page: https://github.com/teambge/bge-python-sdk
 Author: leafcoder,xiangji1204
 Author-email: leafcoder@gmail.com,xiangji1204@genomics.cn
 Maintainer: leafcoder
 Maintainer-email: leafcoder@gmail.com
 License: MIT
```

### Comparing `bge-python-sdk-0.5.1/README.md` & `bge-python-sdk-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bge_python_sdk.egg-info/PKG-INFO` & `bge-python-sdk-0.5.2/bge_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bge-python-sdk
-Version: 0.5.1
+Version: 0.5.2
 Summary: 可用于调用 BGE 开放平台的相关接口。
 Home-page: https://github.com/teambge/bge-python-sdk
 Author: leafcoder,xiangji1204
 Author-email: leafcoder@gmail.com,xiangji1204@genomics.cn
 Maintainer: leafcoder
 Maintainer-email: leafcoder@gmail.com
 License: MIT
```

### Comparing `bge-python-sdk-0.5.1/bge_python_sdk.egg-info/SOURCES.txt` & `bge-python-sdk-0.5.2/bge_python_sdk.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,26 @@
+.coverage
+.coveragerc
+.gitignore
+CHANGELOG.md
+Jenkinsfile
 LICENSE
 MANIFEST.in
+Makefile
 README.md
+coverage.xml
+package.json
 pytest.ini
 requirements.txt
 setup.cfg
 setup.py
+sonar-project.properties
+test_env.sh.example
+tox.ini
+.github/workflows/release.yml
 bge_python_sdk.egg-info/PKG-INFO
 bge_python_sdk.egg-info/SOURCES.txt
 bge_python_sdk.egg-info/dependency_links.txt
 bge_python_sdk.egg-info/entry_points.txt
 bge_python_sdk.egg-info/requires.txt
 bge_python_sdk.egg-info/top_level.txt
 bgesdk/__init__.py
@@ -52,10 +64,11 @@
 tests/__init__.py
 tests/conftest.py
 tests/test_abundance.py
 tests/test_fs.py
 tests/test_model.py
 tests/test_models.py
 tests/test_oauth2.py
+tests/test_phenotype.py
 tests/test_samples.py
 tests/test_user.py
 tests/test_variants.py
```

### Comparing `bge-python-sdk-0.5.1/bgesdk/__main__.py` & `bge-python-sdk-0.5.2/bgesdk/__main__.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/client.py` & `bge-python-sdk-0.5.2/bgesdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -365,14 +365,15 @@
             biosample_ids (str, 非必填): 生物样品 id,逗号分割多个;
             biosample_sites (str, 非必填): 采样部位,取值范围: 1-15;
             omics (str, 非必填): 所属组学,取值范围: 1-2;
             project_ids (str, 非必填): 所属项目,逗号分割多个;
             organisms (str, 非必填): 样品生物体,取值范围: 1-3;
             data_availability (boolean, 非必填): 数据可用性;
             statuses (str, 非必填): 数据状态,详情见 BGE 开放平台文档;
+            require_files(boolean, 非必填）: 要求返回关联文件列表
             next_page (int, 非必填): 要获取的页码,默认值为 None;
             limit (int, 非必填): 每页返回数量,默认值为 50;
 
         Returns:
             list: 样品列表;
         """
         params = {}
@@ -968,14 +969,51 @@
         request = HTTPRequest(
             self.endpoint, max_retries=max_retries, verbose=verbose)
         request.set_authorization(self.token_type, self.access_token)
         result = request.get(
             '/stream/range', params=params, timeout=timeout)
         return models.Model(result)
 
+    def write_phenotype(self, biosample_id, data_element_id,
+                        stream_generate_time, stream_data,
+                        duplicate_enabled=None, **kwargs):
+        """根据生物套件编号写入表型数据
+
+        Args:
+            biosample_id (str): 生物样品编号;
+            data_element_id (str): 数据元编号;
+            stream_generate_time (datetime): 数据流生成时间，
+                                             如：2021-03-02T10:00:00Z;
+            stream_data(dict): 数据流数据；
+            duplicate_enabled(boolean, 非必填): 允许重复写入；
+
+        Returns:
+            Model: 返回的表型数据流编号数据;
+        """
+        biosample_id = biosample_id.upper()
+        stream_data = json.dumps(stream_data)
+        data = dict()
+        data.update(kwargs)
+        data.update({
+            'biosample_id': biosample_id,
+            'data_element_id': data_element_id,
+            'stream_generate_time': stream_generate_time,
+            'stream_data': stream_data,
+            'duplicate_enabled': duplicate_enabled,
+        })
+        timeout = self.timeout
+        verbose = self.verbose
+        max_retries = self.max_retries
+        request = HTTPRequest(
+            self.endpoint, max_retries=max_retries, verbose=verbose)
+        request.set_authorization(self.token_type, self.access_token)
+        result = request.post(
+            '/datamall/phenotype/write', data=data, timeout=timeout)
+        return models.Model(result)
+
     def get_data_items(self, namespace, biosample_id,
                        collection_id=None, data_element_ids=None,
                        next_page=None, **kwargs):
         """根据数据元编号或数据集编号获取数据项
 
         Args:
             namespace(str): 命名空间
@@ -1285,7 +1323,43 @@
         max_retries = self.max_retries
         request = HTTPRequest(
             self.endpoint, max_retries=max_retries, verbose=verbose)
         request.set_authorization(self.token_type, self.access_token)
         result = request.post(
             '/model/doc_upload', data=doc, timeout=timeout)
         return models.Model(result)
+
+    def send_sms(self, template, mobiles, **kwargs):
+        """发送短信
+
+        Args:
+            template (str): 短信模板;
+            mobiles (str): 手机号，多个手机号用逗号分割;
+
+        template：pay_code（积分消费通知短信）
+            pay_code(str): 消费验证码；
+
+        template: research_download_notice（科研数据下载提示短信）
+            org_name(str): 机构名称；
+            project_name(str): 科研调查标题名称；
+            applied_date(str): 申请数据日期；
+            expiry_date(str): 数据有效期日期；
+
+        template: microarray_delivery（芯片版发报告提示短信）
+            user_nick_name(str): 用户昵称；
+
+        Returns:
+            Model: 返回的表型数据流编号数据;
+        """
+        data = dict()
+        data.update(kwargs)
+        data.update({
+            'template': template,
+            'mobiles': mobiles,
+        })
+        timeout = self.timeout
+        verbose = self.verbose
+        max_retries = self.max_retries
+        request = HTTPRequest(
+            self.endpoint, max_retries=max_retries, verbose=verbose)
+        request.set_authorization(self.token_type, self.access_token)
+        request.post('/sms/send', data=data, timeout=timeout)
```

### Comparing `bge-python-sdk-0.5.1/bgesdk/constants.py` & `bge-python-sdk-0.5.2/bgesdk/constants.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/http.py` & `bge-python-sdk-0.5.2/bgesdk/http.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/command.py` & `bge-python-sdk-0.5.2/bgesdk/management/command.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/__init__.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/__init__.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/aggregate_omics_data.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/aggregate_omics_data.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/download.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/download.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_data_items.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_data_items.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_externals.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_externals.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_func_abundance.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_func_abundance.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_gene_abundance.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_gene_abundance.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_range_stream.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_range_stream.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_samples.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_samples.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_taxon_abundance.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_taxon_abundance.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_user.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_user.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/get_variants.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/get_variants.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/task.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/task.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/upload.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/upload.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/api/commands/upload_dir.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/api/commands/upload_dir.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/config.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/config.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/login.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/login.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/model.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/model.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/model_doc.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/model_doc.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/token.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/token.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/commands/workon.py` & `bge-python-sdk-0.5.2/bgesdk/management/commands/workon.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/constants.py` & `bge-python-sdk-0.5.2/bgesdk/management/constants.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/utils.py` & `bge-python-sdk-0.5.2/bgesdk/management/utils.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/management/validate.py` & `bge-python-sdk-0.5.2/bgesdk/management/validate.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/models.py` & `bge-python-sdk-0.5.2/bgesdk/models.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/bgesdk/utils.py` & `bge-python-sdk-0.5.2/bgesdk/utils.py`

 * *Files identical despite different names*

### Comparing `bge-python-sdk-0.5.1/setup.cfg` & `bge-python-sdk-0.5.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [metadata]
 name = bge-python-sdk
-version = 0.5.1
+version = 0.5.2
 description = 可用于调用 BGE 开放平台的相关接口。
 long_description = file: README.md
 long_description_content_type = text/markdown
 maintainer = leafcoder
 maintainer_email = leafcoder@gmail.com
 url = https://github.com/teambge/bge-python-sdk
 author = leafcoder,xiangji1204
 author_email = leafcoder@gmail.com,xiangji1204@genomics.cn
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 keywords = bge-python-sdk bge bgesdk sdk
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: Chinese (Simplified)
 	Operating System :: OS Independent
```

### Comparing `bge-python-sdk-0.5.1/tests/conftest.py` & `bge-python-sdk-0.5.2/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,31 +7,39 @@
 import os
 import pytest
 import requests
 import six
 
 
 ENDPOINT = os.environ.get('ENDPOINT')
-CLIENT_ID = os.environ.get('CLIENT_ID')
-CLIENT_SECRET = os.environ.get('CLIENT_SECRET')
+
+# Authorizaion Code
+AUTHORIZATION_CLIENT_ID = os.environ.get('AUTHORIZATION_CLIENT_ID')
+AUTHORIZATION_CLIENT_SECRET = os.environ.get('AUTHORIZATION_CLIENT_SECRET')
 REDIRECT_URI = os.environ.get('REDIRECT_URI')
 AUTHORIZATION_EXTRA_QUERY = os.environ.get('AUTHORIZATION_EXTRA_QUERY')
 SELF_BIOSAMPLE_ID = os.environ.get('SELF_BIOSAMPLE_ID')
 SELF_META_BIOSAMPLE_ID = os.environ.get('SELF_META_BIOSAMPLE_ID')
 OTHER_BIOSAMPLE_ID = os.environ.get('OTHER_BIOSAMPLE_ID')
 
+# Client Credentials
+CREDENTIALS_CLIENT_ID = os.environ.get('CREDENTIALS_CLIENT_ID')
+CREDENTIALS_CLIENT_SECRET = os.environ.get('CREDENTIALS_CLIENT_SECRET')
+
 
 @pytest.fixture(scope='session')
 def redirect_uri():
     return REDIRECT_URI
 
 
 @pytest.fixture(scope='session')
-def authorization_url(oauth2, redirect_uri):
-    authorization_url = oauth2.get_authorization_url(redirect_uri)
+def authorization_url(authorization_oauth2, redirect_uri):
+    authorization_url = authorization_oauth2.get_authorization_url(
+        redirect_uri
+    )
     return '&'.join((authorization_url, AUTHORIZATION_EXTRA_QUERY))
 
 
 @pytest.fixture(scope='session')
 def authorization_code(authorization_url):
     r = requests.get(authorization_url)
     assert r.status_code == 200
@@ -45,30 +53,57 @@
 def logger():
     logger = logging.getLogger()
     logger.setLevel(logging.DEBUG)
     return logger
 
 
 @pytest.fixture(scope='session')
-def oauth2():
-    return OAuth2(CLIENT_ID, CLIENT_SECRET, endpoint=ENDPOINT, max_retries=3)
+def authorization_oauth2():
+    return OAuth2(
+        AUTHORIZATION_CLIENT_ID,
+        AUTHORIZATION_CLIENT_SECRET,
+        endpoint=ENDPOINT,
+        max_retries=3
+    )
 
 
 @pytest.fixture(scope='session')
-def access_token(oauth2, authorization_code, redirect_uri):
-    token = oauth2.exchange_authorization_code(
+def authorization_access_token(authorization_oauth2, authorization_code,
+                               redirect_uri):
+    token = authorization_oauth2.exchange_authorization_code(
         authorization_code,
         redirect_uri
     )
     return token.access_token
 
 
 @pytest.fixture(scope='session')
-def api(oauth2, access_token):
-    return oauth2.get_api(access_token)
+def authorization_api(authorization_oauth2, authorization_access_token):
+    return authorization_oauth2.get_api(authorization_access_token)
+
+
+@pytest.fixture(scope='session')
+def credentials_oauth2():
+    return OAuth2(
+        CREDENTIALS_CLIENT_ID,
+        CREDENTIALS_CLIENT_SECRET,
+        endpoint=ENDPOINT,
+        max_retries=3
+    )
+
+
+@pytest.fixture(scope='session')
+def credentials_access_token(credentials_oauth2):
+    token = credentials_oauth2.get_credentials_token()
+    return token.access_token
+
+
+@pytest.fixture(scope='session')
+def credentials_api(credentials_oauth2, credentials_access_token):
+    return credentials_oauth2.get_api(credentials_access_token)
 
 
 @pytest.fixture(scope='session')
 def self_biosample_id():
     """本人的样品编号"""
     return SELF_BIOSAMPLE_ID
```

### Comparing `bge-python-sdk-0.5.1/tests/test_abundance.py` & `bge-python-sdk-0.5.2/tests/test_abundance.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,60 +15,70 @@
     assert isinstance(result['count'], int)
     assert isinstance(next_page, int) or next_page is None
 
 
 class TestTaxonAbundance:
 
     @pytest.mark.parametrize('taxon_ids', [None, 'tx1', 'tx2'])
-    def test_result(self, api, logger, self_meta_biosample_id, taxon_ids):
+    def test_result(self, authorization_api, logger, self_meta_biosample_id,
+                    taxon_ids):
         """正常返回的数据"""
-        ret = api.get_taxon_abundance(self_meta_biosample_id)
+        ret = authorization_api.get_taxon_abundance(self_meta_biosample_id)
         logger.debug(ret)
         check_result(ret)
 
     @pytest.mark.parametrize('taxon_ids', ['txdemo', 'tx', 'test'])
-    def test_invalid_txid(self, api, logger, self_meta_biosample_id, taxon_ids):
+    def test_invalid_txid(self, authorization_api, logger,
+                          self_meta_biosample_id, taxon_ids):
         """格式错误的 taxon 编号"""
-        ret = api.get_taxon_abundance(self_meta_biosample_id, taxon_ids)
+        ret = authorization_api.get_taxon_abundance(
+            self_meta_biosample_id,
+            taxon_ids
+        )
         logger.debug(ret)
         check_result(ret)
         assert ret['count'] == 0
 
     @pytest.mark.parametrize('taxon_ids', ['txid815'])
-    def test_valid_txid(self, api, logger, self_meta_biosample_id, taxon_ids):
+    def test_valid_txid(self, authorization_api, logger,
+                        self_meta_biosample_id, taxon_ids):
         """在平台类群丰度 taxon_id 集合内的编号"""
-        ret = api.get_taxon_abundance(self_meta_biosample_id, taxon_ids)
+        ret = authorization_api.get_taxon_abundance(
+            self_meta_biosample_id,
+            taxon_ids
+        )
         logger.debug(ret)
         check_result(ret)
         assert ret['count'] == 1
 
     @pytest.mark.parametrize('taxon_ids', ['txid1323'])
-    def test_outter_txid(self, api, logger, self_meta_biosample_id, taxon_ids):
+    def test_outter_txid(self, authorization_api, logger,
+                         self_meta_biosample_id, taxon_ids):
         """不在平台类群丰度 taxon_id 集合内的编号"""
-        ret = api.get_taxon_abundance(self_meta_biosample_id, taxon_ids)
+        ret = authorization_api.get_taxon_abundance(
+            self_meta_biosample_id,
+            taxon_ids
+        )
         logger.debug(ret)
         check_result(ret)
         assert ret['count'] == 0
 
 
 class TestFuncAbundance:
 
     @pytest.mark.parametrize('catalog', ['go', 'ko', 'eggnog', 'pfam',
                                          'kegg-pwy', 'kegg-mdl', 'level4ec',
                                          'metacyc-rxn', 'metacyc-pwy'])
-    def test_result(self, api, logger, self_meta_biosample_id, catalog):
+    def test_result(self, authorization_api, logger, self_meta_biosample_id,
+                    catalog):
         """正常返回的数据"""
-        try:
-            ret = api.get_func_abundance(self_meta_biosample_id, catalog)
-        except APIError as error:
-            with pytest.raises(APIError) as e:
-                raise error
-            e.value.code == 41202
-            e.value.msg == u'BGE 私有接口错误: 样品数据未入仓'
-            return
+        ret = authorization_api.get_func_abundance(
+            self_meta_biosample_id,
+            catalog
+        )
         logger.debug(ret)
         check_result(ret)
 
 
 class TestGeneAbundance:
 
     def check_result(self, result):
@@ -78,22 +88,31 @@
         next_page = result['next_page']
         assert isinstance(result['result'], list)
         assert isinstance(result['count'], int)
         assert next_page is None or isinstance(next_page, six.text_type)
 
     @pytest.mark.parametrize('catalog, data_type', [
         ('UniRef90_HUMAnN2_0.11', 'file')])
-    def test_result(self, api, logger, self_meta_biosample_id, catalog,
-                    data_type):
+    def test_result(self, authorization_api, logger, self_meta_biosample_id,
+                    catalog, data_type):
         """正常返回的数据"""
-        ret = api.get_gene_abundance(self_meta_biosample_id, catalog, data_type)
+        ret = authorization_api.get_gene_abundance(
+            self_meta_biosample_id,
+            catalog,
+            data_type
+        )
         logger.debug(ret)
         self.check_result(ret)
 
     @pytest.mark.parametrize('catalog, data_type', [
         ('UniRef90_HUMAnN2_0.11', 'list')])
-    def test_invalid_args(self, api, self_meta_biosample_id, catalog, data_type):
+    def test_invalid_args(self, authorization_api, self_meta_biosample_id,
+                          catalog, data_type):
         """正常返回的数据"""
         with pytest.raises(APIError) as e:
-            api.get_gene_abundance(self_meta_biosample_id, catalog, data_type)
+            authorization_api.get_gene_abundance(
+                self_meta_biosample_id,
+                catalog,
+                data_type
+            )
         assert e.value.code == 41001
         assert e.value.msg == u'参数错误'
```

### Comparing `bge-python-sdk-0.5.1/tests/test_models.py` & `bge-python-sdk-0.5.2/tests/test_models.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 import json
 import pytest
 
 
 class TestModels:
 
     @pytest.mark.parametrize('attr', ['x'])
-    def test_unknown_attribute(self, api, logger, attr):
-        with pytest.raises(AttributeError) as e:
+    def test_unknown_attribute(self, logger, attr):
+        with pytest.raises(AttributeError):
             getattr(models.Model({}), attr)
 
-    def test_json(self, api, logger):
+    def test_json(self, logger):
         result = {
             "name": "Tom",
             "children": ["Lili", "Jay"],
             "detail": {
                 "age": 32
             }
         }
```

### Comparing `bge-python-sdk-0.5.1/tests/test_oauth2.py` & `bge-python-sdk-0.5.2/tests/test_oauth2.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,27 +3,31 @@
 from bgesdk.error import APIError
 
 import pytest
 
 
 class TestOAuth2:
 
-    def test_authorization_url_is_str(self, oauth2, redirect_uri):
+    def test_authorization_url_is_str(self, authorization_oauth2,
+                                      redirect_uri):
         """获取用户授权页面链接"""
-        url = oauth2.get_authorization_url(redirect_uri)
+        url = authorization_oauth2.get_authorization_url(redirect_uri)
         assert isinstance(url, str)
 
-    def test_invalid_code(self, oauth2, access_token):
+    def test_invalid_code(self, authorization_oauth2):
         """错误的用户授权 code 和 redirect_uri"""
         with pytest.raises(APIError) as e:
-            oauth2.exchange_authorization_code('code', 'http://test.cn')
+            authorization_oauth2.exchange_authorization_code(
+                'code',
+                'http://test.cn'
+            )
         assert e.value.code == 400
-        assert e.value.msg == u'非法请求: invalid_grant'
+        assert e.value.msg == u'错误的请求'
 
-    def test_invalid_access_token(self, oauth2):
+    def test_invalid_access_token(self, authorization_oauth2):
         """错误的 access_token"""
         access_token = 'demo'
-        api = oauth2.get_api(access_token)
+        api = authorization_oauth2.get_api(access_token)
         with pytest.raises(APIError) as e:
             api.get_user()
         assert e.value.code == 403
         assert e.value.msg == u'access_token 已失效或错误'
```

### Comparing `bge-python-sdk-0.5.1/tests/test_samples.py` & `bge-python-sdk-0.5.2/tests/test_samples.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,70 +13,73 @@
         assert 'next_page' in result
         next_page = result['next_page']
         assert isinstance(result['result'], list)
         assert isinstance(result['count'], int)
         assert isinstance(next_page, int) or next_page is None
 
     @pytest.mark.parametrize('biosample_sites', range(1, 16))
-    def test_valid_biosample_sites(self, api, biosample_sites):
+    def test_valid_biosample_sites(self, authorization_api,
+                                   biosample_sites):
         """在参数 choices 范围限制内"""
-        ret = api.get_samples(biosample_sites=biosample_sites)
+        ret = authorization_api.get_samples(biosample_sites=biosample_sites)
         self.check_samples(ret)
 
     @pytest.mark.parametrize('biosample_sites', [0, '0,3', 20, '3,20', 'x'])
-    def test_invalid_biosample_sites(self, api, biosample_sites):
+    def test_invalid_biosample_sites(self, authorization_api,
+                                     biosample_sites):
         """超出参数 choices 范围限制"""
         with pytest.raises(APIError) as e:
-            api.get_samples(biosample_sites=biosample_sites)
+            authorization_api.get_samples(biosample_sites=biosample_sites)
         assert e.value.code == 41001
         assert e.value.msg == u'参数错误'
 
     @pytest.mark.parametrize('omics', range(1, 3))
-    def test_valid_omics(self, api, omics):
+    def test_valid_omics(self, authorization_api, omics):
         """在参数 choices 范围限制内"""
-        ret = api.get_samples(omics=omics)
+        ret = authorization_api.get_samples(omics=omics)
         self.check_samples(ret)
 
     @pytest.mark.parametrize('omics', [0, '0,3', 4, '3,4', 'x'])
-    def test_invalid_omics(self, api, omics):
+    def test_invalid_omics(self, authorization_api, omics):
         """超出参数 choices 范围限制"""
         with pytest.raises(APIError) as e:
-            api.get_samples(omics=omics)
+            authorization_api.get_samples(omics=omics)
         assert e.value.code == 41001
         assert e.value.msg == u'参数错误'
 
     @pytest.mark.parametrize('organisms', range(1, 3))
-    def test_valid_organisms(self, api, organisms):
+    def test_valid_organisms(self, authorization_api, organisms):
         """在参数 choices 范围限制内"""
-        ret = api.get_samples(organisms=organisms)
+        ret = authorization_api.get_samples(organisms=organisms)
         self.check_samples(ret)
 
     @pytest.mark.parametrize('organisms', [0, '0,3', 4, '3,4', 'x'])
-    def test_invalid_organisms(self, api, organisms):
+    def test_invalid_organisms(self, authorization_api, organisms):
         """超出参数 choices 范围限制"""
         with pytest.raises(APIError) as e:
-            api.get_samples(organisms=organisms)
+            authorization_api.get_samples(organisms=organisms)
         assert e.value.code == 41001
         assert e.value.msg == u'参数错误'
 
-    def test_result(self, api, logger):
+    def test_result(self, authorization_api, logger):
         """返回值"""
-        ret = api.get_samples(limit=1)
+        ret = authorization_api.get_samples(limit=1)
         self.check_samples(ret)
         next_page = ret['next_page']
         if next_page is not None:
-            ret = api.get_samples(page=next_page)
+            ret = authorization_api.get_samples(page=next_page)
             self.check_samples(ret)
 
     @pytest.mark.parametrize('external_sample_ids', [None, ''])
-    def test_non_externals(self, api, logger, external_sample_ids):
+    def test_non_externals(self, authorization_api, logger,
+                           external_sample_ids):
         """空的外部编号"""
         project_id = 'P-M0000000000'
         biosample_site = 10
         with pytest.raises(APIError) as e:
-            api.externals(
+            authorization_api.externals(
                 external_sample_ids,
                 biosample_site,
                 project_id
             )
         assert e.value.code == 41001
         assert e.value.msg == u'参数错误'
```

### Comparing `bge-python-sdk-0.5.1/tests/test_variants.py` & `bge-python-sdk-0.5.2/tests/test_variants.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,58 +4,63 @@
 
 import pytest
 
 
 class TestVariant:
 
     @pytest.mark.parametrize('rsids', ['rs333', 'rs1,rs2'])
-    def test_valid_request(self, api, self_biosample_id, rsids):
+    def test_valid_request(self, authorization_api, self_biosample_id,
+                           rsids):
         # 获取不归属于自己的样品的变异数据
-        ret = api.get_variants(self_biosample_id, rsids)
+        ret = authorization_api.get_variants(self_biosample_id, rsids)
         assert isinstance(ret, list), u'成功返回数据的类型必须为列表'
 
     @pytest.mark.parametrize('rsids', ['rs333', 'rs1,rs2'])
-    def test_raise_errors(self, api, logger, other_biosample_id, rsids):
+    def test_raise_errors(self, authorization_api, logger,
+                          other_biosample_id, rsids):
         """获取不归属于自己的样品的变异数据"""
         with pytest.raises(APIError) as e:
-            api.get_variants(other_biosample_id, rsids)
+            authorization_api.get_variants(other_biosample_id, rsids)
         logger.debug(e.value)
         assert e.value.code == 41303
         assert e.value.msg == u'请提供本人的 biosample_id'
 
     @pytest.mark.parametrize(
         'rsids', ['rs1,rs2,rs3,rs4,rs5,rs6,rs7,rs8,rs9,rs10,rs11,rs12,rs13,'
                   'rs14,rs15,rs16,rs17,rs18,rs19,rs20,rs21,rs22,rs23,rs24,r'
                   's25,rs26,rs27,rs28,rs29,rs30,rs31,rs32,rs33,rs34,rs35,rs'
                   '36,rs37,rs38,rs39,rs40,rs41,rs42,rs43,rs44,rs45,rs46,rs4'
                   '7,rs48,rs49,rs50,rs51,rs52,rs53,rs54,rs55,rs56,rs57,rs58'
                   ',rs59,rs60,rs61,rs62,rs63,rs64,rs65,rs66,rs67,rs68,rs69,'
                   'rs70,rs71,rs72,rs73,rs74,rs75,rs76,rs77,rs78,rs79,rs80,r'
                   's81,rs82,rs83,rs84,rs85,rs86,rs87,rs88,rs89,rs90,rs91,rs'
                   '92,rs93,rs94,rs95,rs96,rs97,rs98,rs99,rs100,rs101'])
-    def test_too_many_rsids(self, api, logger, self_biosample_id, rsids):
+    def test_too_many_rsids(self, authorization_api, logger,
+                            self_biosample_id, rsids):
         """测试超出数量限制"""
         with pytest.raises(APIError) as e:
-            api.get_variants(self_biosample_id, rsids)
+            authorization_api.get_variants(self_biosample_id, rsids)
         logger.debug(e.value)
         assert e.value.code == 41001
         assert e.value.msg == u'参数错误'
 
     @pytest.mark.parametrize(
         'rsids', ['333', '55333,rs3', 'srs3', 'rs3,,rs34', 'rs3,,', ''])
-    def test_invalid_rsid(self, api, logger, self_biosample_id, rsids):
+    def test_invalid_rsid(self, authorization_api, logger,
+                          self_biosample_id, rsids):
         """测试格式错误的变异位点"""
         with pytest.raises(APIError) as e:
-            api.get_variants(self_biosample_id, rsids)
+            authorization_api.get_variants(self_biosample_id, rsids)
         logger.debug(e.value)
         assert e.value.code == 41001
         assert e.value.msg == u'参数错误'
 
     @pytest.mark.parametrize('biosample_id', ['demo', 'E-B112'])
-    def test_invalid_biosample_id(self, api, logger, biosample_id):
+    def test_invalid_biosample_id(self, authorization_api, logger,
+                                  biosample_id):
         """测试不存在或者格式异常的的样品编号"""
         rsids = 'rs333'
         with pytest.raises(APIError) as e:
-            api.get_variants(biosample_id, rsids)
+            authorization_api.get_variants(biosample_id, rsids)
         logger.debug(e.value)
-        assert e.value.code == 41302
-        assert e.value.msg == u'基因组报告不存在或未下机'
+        assert e.value.code == 41303
+        assert e.value.msg == u'请提供本人的 biosample_id'
```

