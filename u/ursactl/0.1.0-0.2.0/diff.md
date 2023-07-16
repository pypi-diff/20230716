# Comparing `tmp/ursactl-0.1.0.tar.gz` & `tmp/ursactl-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-ozcx7k0k/ursactl-0.1.0.tar", last modified: Mon Jul 10 13:20:28 2023, max compression
+gzip compressed data, was "/Users/jgsmith/Code/ursactl/dist/.tmp-daz7ybe8/ursactl-0.2.0.tar", last modified: Sun Jul 16 15:00:16 2023, max compression
```

## Comparing `ursactl-0.1.0.tar` & `ursactl-0.2.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/
--rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.1.0/CHANGELOG.md
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.1.0/LICENSE.md
--rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.1.0/MANIFEST.in
--rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-10 13:20:28.000000 ursactl-0.1.0/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1072 2023-02-14 14:26:01.000000 ursactl-0.1.0/README.md
--rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.1.0/pyproject.toml
--rw-r--r--   0 jgsmith    (501) staff       (20)      144 2023-07-08 17:43:40.000000 ursactl-0.1.0/requirements-dev.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      197 2023-06-04 21:29:27.000000 ursactl-0.1.0/requirements.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)     1172 2023-07-10 13:20:28.000000 ursactl-0.1.0/setup.cfg
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/tests/
--rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.1.0/tests/test_ursactl.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.1.0/ursactl/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/airflow_provider/
--rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.1.0/ursactl/airflow_provider/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.1.0/ursactl/airflow_provider/hooks.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/controllers/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.1.0/ursactl/controllers/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.1.0/ursactl/controllers/base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8178 2023-07-05 18:27:53.000000 ursactl-0.1.0/ursactl/controllers/create.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.1.0/ursactl/controllers/delete.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.1.0/ursactl/controllers/get.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1647 2023-07-05 18:27:53.000000 ursactl-0.1.0/ursactl/controllers/init.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.1.0/ursactl/controllers/list.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.1.0/ursactl/controllers/refresh.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2293 2023-06-04 21:29:27.000000 ursactl-0.1.0/ursactl/controllers/run.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.1.0/ursactl/controllers/send.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      522 2023-03-24 15:51:14.000000 ursactl-0.1.0/ursactl/controllers/show.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.1.0/ursactl/controllers/stop.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     7488 2023-07-05 18:27:53.000000 ursactl-0.1.0/ursactl/controllers/sync.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     5680 2023-07-05 18:27:53.000000 ursactl-0.1.0/ursactl/controllers/update.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/controllers/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.1.0/ursactl/controllers/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2780 2023-07-05 14:33:27.000000 ursactl-0.1.0/ursactl/controllers/utils/transforms.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/core/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.1.0/ursactl/core/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      543 2023-06-22 13:08:38.000000 ursactl-0.1.0/ursactl/core/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2301 2023-07-05 18:27:53.000000 ursactl-0.1.0/ursactl/core/dataset.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.1.0/ursactl/core/exc.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1571 2023-02-17 18:11:59.000000 ursactl-0.1.0/ursactl/core/project.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/core/services/
--rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.1.0/ursactl/core/services/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1776 2023-07-10 12:55:55.000000 ursactl-0.1.0/ursactl/core/services/_base.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    31479 2023-07-10 12:55:55.000000 ursactl-0.1.0/ursactl/core/services/ape_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     8420 2023-04-21 15:03:51.000000 ursactl-0.1.0/ursactl/core/services/dss_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1916 2023-07-05 18:27:53.000000 ursactl-0.1.0/ursactl/core/services/iam_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)    11256 2023-05-08 17:11:56.000000 ursactl-0.1.0/ursactl/core/services/planning_client.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.1.0/ursactl/core/services/project_client.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/core/utils/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.1.0/ursactl/core/utils/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.1.0/ursactl/core/utils/magic.py
--rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-10 13:17:36.000000 ursactl-0.1.0/ursactl/core/version.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/ext/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.1.0/ursactl/ext/__init__.py
--rw-r--r--   0 jgsmith    (501) staff       (20)     4208 2023-07-05 18:27:53.000000 ursactl-0.1.0/ursactl/main.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/plugins/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.1.0/ursactl/plugins/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl/templates/
--rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.1.0/ursactl/templates/__init__.py
-drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl.egg-info/
--rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl.egg-info/PKG-INFO
--rw-r--r--   0 jgsmith    (501) staff       (20)     1466 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl.egg-info/SOURCES.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl.egg-info/dependency_links.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl.egg-info/entry_points.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)      197 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl.egg-info/requires.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-10 13:20:28.000000 ursactl-0.1.0/ursactl.egg-info/top_level.txt
--rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.1.0/ursactl.egg-info/zip-safe
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/
+-rw-r--r--   0 jgsmith    (501) staff       (20)       67 2023-01-01 19:09:45.000000 ursactl-0.2.0/CHANGELOG.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-01-01 19:09:45.000000 ursactl-0.2.0/LICENSE.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)      135 2023-01-01 19:09:45.000000 ursactl-0.2.0/MANIFEST.in
+-rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-16 15:00:16.000000 ursactl-0.2.0/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1072 2023-02-14 14:26:01.000000 ursactl-0.2.0/README.md
+-rw-r--r--   0 jgsmith    (501) staff       (20)       81 2023-01-01 19:09:45.000000 ursactl-0.2.0/pyproject.toml
+-rw-r--r--   0 jgsmith    (501) staff       (20)      144 2023-07-08 17:43:40.000000 ursactl-0.2.0/requirements-dev.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 14:14:44.000000 ursactl-0.2.0/requirements.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1172 2023-07-16 15:00:16.000000 ursactl-0.2.0/setup.cfg
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/tests/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      382 2023-01-31 15:40:54.000000 ursactl-0.2.0/tests/test_ursactl.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/airflow_provider/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      431 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/airflow_provider/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3787 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/airflow_provider/hooks.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/controllers/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/controllers/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1089 2023-01-31 15:40:54.000000 ursactl-0.2.0/ursactl/controllers/base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7879 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/create.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     3313 2023-06-04 21:29:27.000000 ursactl-0.2.0/ursactl/controllers/delete.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1150 2023-03-24 15:51:14.000000 ursactl-0.2.0/ursactl/controllers/get.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1647 2023-07-05 18:27:53.000000 ursactl-0.2.0/ursactl/controllers/init.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7280 2023-07-10 12:55:55.000000 ursactl-0.2.0/ursactl/controllers/list.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      446 2023-02-16 21:42:16.000000 ursactl-0.2.0/ursactl/controllers/refresh.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2293 2023-06-04 21:29:27.000000 ursactl-0.2.0/ursactl/controllers/run.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1944 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/controllers/send.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      762 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/show.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      764 2023-04-18 14:46:09.000000 ursactl-0.2.0/ursactl/controllers/stop.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     7698 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/sync.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     6031 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/update.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/controllers/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-06-04 21:29:27.000000 ursactl-0.2.0/ursactl/controllers/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     5403 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/controllers/utils/transforms.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/core/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/core/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      543 2023-07-12 14:08:56.000000 ursactl-0.2.0/ursactl/core/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1682 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/agent.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2301 2023-07-05 18:27:53.000000 ursactl-0.2.0/ursactl/core/dataset.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      301 2023-04-18 14:46:09.000000 ursactl-0.2.0/ursactl/core/exc.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2727 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/project.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      865 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/running_agent.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/core/services/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      871 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/core/services/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1823 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/services/_base.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    31479 2023-07-10 12:55:55.000000 ursactl-0.2.0/ursactl/core/services/ape_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     8420 2023-04-21 15:03:51.000000 ursactl-0.2.0/ursactl/core/services/dss_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1916 2023-07-05 18:27:53.000000 ursactl-0.2.0/ursactl/core/services/iam_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)    11923 2023-07-16 14:14:44.000000 ursactl-0.2.0/ursactl/core/services/planning_client.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     2910 2023-05-04 12:27:25.000000 ursactl-0.2.0/ursactl/core/services/project_client.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/core/utils/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-18 13:39:22.000000 ursactl-0.2.0/ursactl/core/utils/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1470 2023-04-18 14:46:09.000000 ursactl-0.2.0/ursactl/core/utils/magic.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)      203 2023-07-16 14:59:58.000000 ursactl-0.2.0/ursactl/core/version.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/ext/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/ext/__init__.py
+-rw-r--r--   0 jgsmith    (501) staff       (20)     4208 2023-07-05 18:27:53.000000 ursactl-0.2.0/ursactl/main.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/plugins/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/plugins/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl/templates/
+-rw-r--r--   0 jgsmith    (501) staff       (20)        0 2023-01-01 19:09:45.000000 ursactl-0.2.0/ursactl/templates/__init__.py
+drwxr-xr-x   0 jgsmith    (501) staff       (20)        0 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/
+-rw-r--r--   0 jgsmith    (501) staff       (20)      994 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/PKG-INFO
+-rw-r--r--   0 jgsmith    (501) staff       (20)     1518 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/SOURCES.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/dependency_links.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)       46 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/entry_points.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)      207 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/requires.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        8 2023-07-16 15:00:16.000000 ursactl-0.2.0/ursactl.egg-info/top_level.txt
+-rw-r--r--   0 jgsmith    (501) staff       (20)        1 2023-02-17 20:26:57.000000 ursactl-0.2.0/ursactl.egg-info/zip-safe
```

### Comparing `ursactl-0.1.0/PKG-INFO` & `ursactl-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.1.0
+Version: 0.2.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ursactl-0.1.0/README.md` & `ursactl-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/setup.cfg` & `ursactl-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/airflow_provider/hooks.py` & `ursactl-0.2.0/ursactl/airflow_provider/hooks.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/base.py` & `ursactl-0.2.0/ursactl/controllers/base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/create.py` & `ursactl-0.2.0/ursactl/controllers/create.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from cement import Controller, ex
 import json
 import yaml
 
 from ..core.services import client
 from ..core.utils.magic import magic
-import ursactl.controllers.utils.transforms
+from ursactl.controllers.utils.transforms import load_transform
 
 
 def _yaml_load(fd):
     return list(yaml.load_all(fd, Loader=yaml.Loader))
 
 
 class Create(Controller):
@@ -65,26 +65,19 @@
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
     def transform(self):
         project_uuid = self._project_scope
         ape_client = client('ape', self.app)
 
         file = self.app.pargs.file
-        if file.endswith('.yaml') or file.endswith('.yml'):
-            loader = _yaml_load
-        elif file.endswith('.json'):
-            loader = json.load
-        elif file.endswith('.md'):
-            loader = ursactl.controllers.utils.transforms.load_from_markdown
-        else:
-            print("Only YAML, JSON, and Markdown files may be uploaded.")
-            sys.exit(1)
+        documents = load_transform(file)
 
-        with open(file, 'r', encoding='utf-8') as fd:
-            documents = loader(fd)
+        if documents is None:
+            print(f"Unable to load transform from {file}")
+            sys.exit(1)
 
         if not isinstance(documents, list):
             documents = [documents]
 
         for content in documents:
             args = {
                 'path': content['path'],
```

### Comparing `ursactl-0.1.0/ursactl/controllers/delete.py` & `ursactl-0.2.0/ursactl/controllers/delete.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/get.py` & `ursactl-0.2.0/ursactl/controllers/get.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/init.py` & `ursactl-0.2.0/ursactl/controllers/init.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/list.py` & `ursactl-0.2.0/ursactl/controllers/list.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/run.py` & `ursactl-0.2.0/ursactl/controllers/run.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/send.py` & `ursactl-0.2.0/ursactl/controllers/send.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/stop.py` & `ursactl-0.2.0/ursactl/controllers/stop.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/controllers/sync.py` & `ursactl-0.2.0/ursactl/controllers/sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             for key in ['seeders', 'generators', 'description']:
                 if key in item and item[key] is not None:
                     args[key] = item[key]
 
             result = client.sync_pipeline(**args)
             self._print(result)
 
-    def _load_resources(self, root):
+    def _load_resources(self, root):  # noqa: C901
         # we want to look at each resource we can find locally and compute a hash
         # that makes sense for the data stored on the server - to see if there's a difference
         # for now, we're focused on the data side of things
         # we'll need to look at the planning side of things later
         # we look in each of the directories created by `init`, but use them only to
         # establish the default resource type. Resources can have a `kind` metadata
         # attribute that we can use to determin the kind of resource we're looking at.
@@ -149,14 +149,18 @@
                 continue
             info = None
             suffix = file.suffix
             if suffix == '.md':
                 # likely a transform
                 with open(file, "r") as fd:
                     info = ursactl.controllers.utils.transforms.load_from_markdown(fd)
+            if suffix == '.lua':
+                # likely a transform
+                with open(file, "r") as fd:
+                    info = ursactl.controllers.utils.transforms.load_from_lua(fd)
             elif suffix in ['.yaml', '.yml']:
                 with open(file, "r") as fd:
                     info = list(yaml.load_all(fd, Loader=yaml.Loader))
             elif suffix == '.json':
                 with open(file, "r") as fd:
                     info = json.load(fd)
             else:
```

### Comparing `ursactl-0.1.0/ursactl/controllers/update.py` & `ursactl-0.2.0/ursactl/controllers/update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 
 from cement import Controller, ex
 import json
 import yaml
 
 from ..core.services import client
-import ursactl.controllers.utils.transforms
+from ursactl.controllers.utils.transforms import load_transform
 
 
 def _yaml_load(fd):
     return list(yaml.load_all(fd, Loader=yaml.Loader))
 
 
 class Update(Controller):
@@ -42,26 +42,19 @@
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'})
         ])
     def transform(self):
         project_uuid = self._project_scope
         ape_client = client('ape', self.app)
 
         file = self.app.pargs.file
-        if file.endswith('.yaml') or file.endswith('.yml'):
-            loader = _yaml_load
-        elif file.endswith('.json'):
-            loader = json.load
-        elif file.endswith('.md'):
-            loader = ursactl.controllers.utils.transforms.load_from_markdown
-        else:
-            print("Only YAML, JSON, and Markdown files may be uploaded.")
-            sys.exit(1)
+        documents = load_transform(file)
 
-        with open(file, 'r', encoding='utf-8') as fd:
-            documents = loader(fd)
+        if documents is None:
+            print(f"Unable to load transform from {file}")
+            sys.exit(1)
 
         if not isinstance(documents, list):
             documents = [documents]
 
         for content in documents:
             args = {
                 'path': content['path'],
@@ -116,14 +109,31 @@
             for key in ['extract', 'description']:
                 if key in content and content[key] is not None:
                     args[key] = content[key]
 
             result = ape_client.update_generator(**args)
             self._print(result)
 
+    @ex(help='update an existing package from a file',
+        arguments=[
+            (['file'], {'help': 'package definition file', 'action': 'store'}),
+            (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
+        ])
+    def package(self):
+        project_uuid = self._project_scope
+        planning_client = client('planning', self.app)
+
+        file = self.app.pargs.file
+        with open(file) as fd:
+            # read the content of the file
+            content = fd.read()
+
+        result = planning_client.update_package(project_uuid=project_uuid, content=content)
+        self._print(result)
+
     @ex(help='update an existing pipeline from a file',
         arguments=[
             (['file'], {'help': 'pipeline definition file', 'action': 'store'}),
             (['--project'], {'help': 'project identifier', 'dest': 'project', 'action': 'store'}),
         ])
     def pipeline(self):
         ape_client = client('ape', self.app)
```

### Comparing `ursactl-0.1.0/ursactl/core/_base.py` & `ursactl-0.2.0/ursactl/core/_base.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/core/dataset.py` & `ursactl-0.2.0/ursactl/core/dataset.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/core/project.py` & `ursactl-0.2.0/ursactl/core/project.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 from ursactl.core._base import Base
 
 
 class Project(Base):
     """
     Provides access to a project and its related resources.
     """
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        if self._uuid is None:
+            self._uuid = self.app.config.get('ursactl', 'project')
+
     @property
     def client(self):
         if self._client is None:
             self._client = client('usage', self.app)
         return self._client
 
     @property
@@ -17,16 +22,43 @@
         return self._data['name']
 
     @property
     def description(self):
         return self._data['description']
 
     @property
-    def is_closed(self):
-        return self._data['isClosed']
+    def is_archived(self):
+        return self._data['isArchived']
+
+    def Agent(self, *args, **kwargs):
+        from ursactl.core.agent import Agent as AgentClass
+
+        return AgentClass(*args, project_uuid=self.uuid, **kwargs)
+
+    def agents(self):
+        """
+        Returns a generator listing all agents belonging to the project.
+        """
+        from ursactl.core.agent import Agent
+
+        if self.uuid is None:
+            return []
+        planning_client = client('planning', self.app)
+        return (
+            Agent(client=planning_client, app=self.app, project_uuid=self.uuid, **info)
+            for info in planning_client.list_agents(project_scope=self.uuid)
+        )
+
+    def agent(self, name):
+        """
+        Returns an agent with the given name.
+        """
+        planning_client = client('planning', self.app)
+        info = planning_client.get_agent(name, project_uuid=self.uuid)
+        return self.Agent(uuid=info['id'], client=planning_client, app=self.app, **info)
 
     def Dataset(self, *args, **kwargs):
         from ursactl.core.dataset import Dataset as DatasetClass
 
         return DatasetClass(*args, project_uuid=self.uuid, **kwargs)
 
     def datasets(self):
@@ -35,23 +67,23 @@
         """
         from ursactl.core.dataset import Dataset
 
         if self.uuid is None:
             return []
         dss_client = client('dss', self.app)
         return (
-            Dataset(client=dss_client, app=self.app, **info)
+            Dataset(client=dss_client, app=self.app, project_uuid=self.uuid, **info)
             for info in dss_client.list_datasets(project_scope=self.uuid)
         )
 
     @property
     def _data(self):
         if self._cached_data is None:
             if self.uuid is None:
                 self._cached_data = {
                     'name': None,
                     'description': None,
-                    'isClosed': None
+                    'isArchived': None
                 }
             else:
-                self._cached_data = self.client.get_dataset_details(self.uuid)
+                self._cached_data = self.client.get_project_details(self.uuid)
         return self._cached_data
```

### Comparing `ursactl-0.1.0/ursactl/core/services/__init__.py` & `ursactl-0.2.0/ursactl/core/services/__init__.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/core/services/_base.py` & `ursactl-0.2.0/ursactl/core/services/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,8 +48,10 @@
         return result
 
     @staticmethod
     def is_uuid(s: str) -> bool:
         """
         Test if the string looks like a UUID.
         """
+        if s is None:
+            return False
         return re.match(r'^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$', s)
```

### Comparing `ursactl-0.1.0/ursactl/core/services/ape_client.py` & `ursactl-0.2.0/ursactl/core/services/ape_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/core/services/dss_client.py` & `ursactl-0.2.0/ursactl/core/services/dss_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/core/services/iam_client.py` & `ursactl-0.2.0/ursactl/core/services/iam_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/core/services/planning_client.py` & `ursactl-0.2.0/ursactl/core/services/planning_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,30 @@
             id
             name
         }
     }
 }
 """
 
+UPDATE_PACKAGE_MUTATION = """\
+mutation update_package($input: UpdatePackageInput!) {
+    updatePackage(input: $input) {
+        errors {
+            code
+            message
+            fields
+        }
+        result {
+            id
+            name
+        }
+    }
+}
+"""
+
 GET_PACKAGE_BY_NAME = """\
 query get_package($name: String!, $project_id: String!) {
     project(handleName: $project_id) {
         packages(limit: 1, filter: { name: { eq: $name } }) {
             id
             name
         }
@@ -292,14 +308,26 @@
             'input': {
                 'source': content,
                 'project': project_uuid
             }
         })
         return mutation_response['data']['createPackage']
 
+    def update_package(self, project_uuid=None, content=None):
+        """
+        Update an existing package.
+        """
+        mutation_response = self.raw_query(query=UPDATE_PACKAGE_MUTATION, variables={
+            'input': {
+                'source': content,
+                'project': project_uuid
+            }
+        })
+        return mutation_response['data']['updatePackage']
+
     def create_agent(self, project_uuid=None, name=None, packages=None, behaviors=None):
         """
         Create a new agent.
         """
         mutation_response = self.raw_query(query=CREATE_AGENT_MUTATION, variables={
             'input': {
                 'name': name,
```

### Comparing `ursactl-0.1.0/ursactl/core/services/project_client.py` & `ursactl-0.2.0/ursactl/core/services/project_client.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/core/utils/magic.py` & `ursactl-0.2.0/ursactl/core/utils/magic.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl/main.py` & `ursactl-0.2.0/ursactl/main.py`

 * *Files identical despite different names*

### Comparing `ursactl-0.1.0/ursactl.egg-info/PKG-INFO` & `ursactl-0.2.0/ursactl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ursactl
-Version: 0.1.0
+Version: 0.2.0
 Summary: command line tool and library for intercting with ursafrontier.cloud
 Author: Ursa Frontier LLC
 Author-email: contact@ursafrontier.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `ursactl-0.1.0/ursactl.egg-info/SOURCES.txt` & `ursactl-0.2.0/ursactl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -32,17 +32,19 @@
 ursactl/controllers/stop.py
 ursactl/controllers/sync.py
 ursactl/controllers/update.py
 ursactl/controllers/utils/__init__.py
 ursactl/controllers/utils/transforms.py
 ursactl/core/__init__.py
 ursactl/core/_base.py
+ursactl/core/agent.py
 ursactl/core/dataset.py
 ursactl/core/exc.py
 ursactl/core/project.py
+ursactl/core/running_agent.py
 ursactl/core/version.py
 ursactl/core/services/__init__.py
 ursactl/core/services/_base.py
 ursactl/core/services/ape_client.py
 ursactl/core/services/dss_client.py
 ursactl/core/services/iam_client.py
 ursactl/core/services/planning_client.py
```

