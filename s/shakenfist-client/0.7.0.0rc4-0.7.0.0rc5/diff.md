# Comparing `tmp/shakenfist-client-0.7.0.0rc4.tar.gz` & `tmp/shakenfist-client-0.7.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-client-0.7.0.0rc4.tar", last modified: Tue Dec 27 08:36:32 2022, max compression
+gzip compressed data, was "shakenfist-client-0.7.0.0rc5.tar", last modified: Sun Jul 16 08:19:27 2023, max compression
```

## Comparing `shakenfist-client-0.7.0.0rc4.tar` & `shakenfist-client-0.7.0.0rc5.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.833951 shakenfist-client-0.7.0.0rc4/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.821948 shakenfist-client-0.7.0.0rc4/.github/
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.825949 shakenfist-client-0.7.0.0rc4/.github/workflows/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1048 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/.github/workflows/configure-tests.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8762 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/.github/workflows/functional-tests-debian-10-localhost.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8771 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/.github/workflows/functional-tests-debian-11-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8777 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     9142 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/.github/workflows/functional-tests.tmpl
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1412 2022-11-06 04:44:16.000000 shakenfist-client-0.7.0.0rc4/.github/workflows/python-unit-tests.yml
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc4/.stestr.conf
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      131 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc4/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2022-12-27 08:36:32.833951 shakenfist-client-0.7.0.0rc4/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      280 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc4/README.md
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.825949 shakenfist-client-0.7.0.0rc4/ansible/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    10729 2022-11-20 01:06:18.000000 shakenfist-client-0.7.0.0rc4/ansible/sf_instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3994 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc4/ansible/sf_network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     3484 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc4/ansible/sf_snapshot.py
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      845 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc4/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      363 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      720 2022-12-27 08:36:32.833951 shakenfist-client-0.7.0.0rc4/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1372 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc4/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.825949 shakenfist-client-0.7.0.0rc4/shakenfist_client/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    30748 2022-12-27 08:36:15.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/apiclient.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.829950 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1012 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/admin.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    14546 2022-12-27 08:36:15.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/artifact.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2492 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/backup.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6168 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/blob.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    23636 2022-11-06 04:44:16.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/instance.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1935 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/interface.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      512 2022-01-08 00:34:31.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/label.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8243 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/namespace.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     8121 2022-11-06 04:44:16.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/network.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2015 2022-11-06 04:44:20.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/node.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4189 2022-08-12 10:06:43.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/main.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.829950 shakenfist-client-0.7.0.0rc4/shakenfist_client/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/tests/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    14815 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/tests/test_client_apiclient.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     2192 2022-01-08 00:34:31.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client/util.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.829950 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     1476 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       58 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/entry_points.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       47 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      109 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       18 2022-12-27 08:36:32.000000 shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc4/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2022-12-27 08:36:32.833951 shakenfist-client-0.7.0.0rc4/tools/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      402 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/tools/buffer.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     4017 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/tools/clone_with_depends.py
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc4/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      898 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc4/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.823839 shakenfist-client-0.7.0.0rc5/.github/
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.827839 shakenfist-client-0.7.0.0rc5/.github/workflows/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1048 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/configure-tests.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8937 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-debian-10-localhost.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8946 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-debian-11-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8952 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     9302 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests.tmpl
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1306 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/.github/workflows/python-unit-tests.yml
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       56 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/.stestr.conf
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      131 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      280 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/README.md
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.827839 shakenfist-client-0.7.0.0rc5/ansible/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    10729 2022-11-20 01:06:18.000000 shakenfist-client-0.7.0.0rc5/ansible/sf_instance.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3994 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc5/ansible/sf_network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3484 2021-11-04 05:09:57.000000 shakenfist-client-0.7.0.0rc5/ansible/sf_snapshot.py
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      845 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      398 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      720 2023-07-16 08:19:27.835839 shakenfist-client-0.7.0.0rc5/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1372 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.827839 shakenfist-client-0.7.0.0rc5/shakenfist_client/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    37569 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/apiclient.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1012 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/admin.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    13862 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/artifact.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     2492 2022-08-09 10:00:30.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/backup.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7843 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/blob.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    28703 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/instance.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     3249 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/interface.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      512 2022-01-08 00:34:31.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/label.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8896 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/namespace.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     8294 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/network.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     7475 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/node.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4222 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/main.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/shakenfist_client/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2021-09-25 23:09:43.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/tests/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    15322 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/tests/test_client_apiclient.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5829 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client/util.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.827839 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1006 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     1476 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       58 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/entry_points.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       47 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      129 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       18 2023-07-16 08:19:27.000000 shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      164 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-07-16 08:19:27.831839 shakenfist-client-0.7.0.0rc5/tools/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      402 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc5/tools/buffer.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     4017 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc5/tools/clone_with_depends.py
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      573 2022-12-27 01:53:29.000000 shakenfist-client-0.7.0.0rc5/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      899 2023-07-16 08:18:06.000000 shakenfist-client-0.7.0.0rc5/tox.ini
```

### Comparing `shakenfist-client-0.7.0.0rc4/.github/workflows/configure-tests.py` & `shakenfist-client-0.7.0.0rc5/.github/workflows/configure-tests.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/.github/workflows/functional-tests-debian-10-localhost.yml` & `shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-debian-10-localhost.yml`

 * *Files 8% similar despite different names*

```diff
@@ -10,25 +10,23 @@
       - develop
       - v*-releases
 
 jobs:
   debian-10-localhost:
     runs-on: self-hosted
     timeout-minutes: 120
+    concurrency:
+      group: ${{ github.workflow }}-${{ github.ref }}
+      cancel-in-progress: true
 
     # NOTE(mikal): git repos are checked out to /srv/github/_work/{repo}/{repo}
     # which is available as GITHUB_WORKSPACE. You can find other environment
     # variables at https://docs.github.com/en/actions/learn-github-actions/environment-variables
 
     steps:
-      - name: Remove previous unfinished runs
-        uses: n1hility/cancel-previous-runs@v2
-        with: 
-          token: ${{ secrets.GITHUB_TOKEN }}
-
       - name: Set environment variables
         run: |
           echo "SF_HEAD_SHA=${{ github.event.pull_request.head.sha }}" >> $GITHUB_ENV
           echo "SF_PRIMARY_REPO=$( echo ${{ github.repository }} | cut -f 2 -d '/' )" >> $GITHUB_ENV
           echo "SHAKENFIST_NAMESPACE=$(hostname)" >> $GITHUB_ENV
 
       - name: Checkout client-python
@@ -135,54 +133,56 @@
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               debian@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; stestr run --concurrency=3"
 
       - name: Check logs
         if: ${{ ! cancelled() }}
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
+          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
+                -o UserKnownHostsFile=/dev/null \
+                debian@$primary sudo chmod ugo+r /var/log/syslog
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               debian@$primary:/var/log/syslog \
               ${GITHUB_WORKSPACE}/syslog
 
-          # Ensure we don't have any tracebacks
-          if [ `grep -c "Traceback (most recent call last):" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "We have tracebacks in the logs!"
-            exit 1
-          fi
-
-          # Ensure we didn't log any errors -- note the inclusion of the start
-          # of the process name here to avoid errors from things like prometheus
-          # node exporter.
-          if [ `grep -c "ERROR sf" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "Errors were logged!"
-            exit 1
-          fi
+          failures=0
 
-          # Ensure nothing died
-          if [ `grep -c " died" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "A process died!"
-            exit 1
+          echo
+          etcd_conns=`grep -c "Building new etcd connection" ${GITHUB_WORKSPACE}/syslog || true`
+          echo "This CI run created $etcd_conns etcd connections."
+          if [ $etcd_conns -gt 5000 ]; then
+            echo "FAILURE: Too many etcd clients!"
+            failures=1
           fi
 
-          # Ensure no leaked vxlans
-          if [ `grep -c "Extra vxlan present" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "vxlans leaked!"
-            exit 1
-          fi
+          FORBIDDEN=("Traceback (most recent call last):"
+                     "ERROR sf"
+                     " died"
+                     "Extra vxlan present"
+                     "Fork support is only compatible with the epoll1 and poll polling strategies"
+                     "not using configured address"
+                     "Dumping thread traces"
+                     "because it is leased to"
+                     "not committing online upgrade"
+                     "Received a GOAWAY with error code ENHANCE_YOUR_CALM"
+                     "ConnectionFailedError")
+          IFS=""
+          for forbid in ${FORBIDDEN[*]}
+          do
+            if [ `grep -c "$forbid" ${GITHUB_WORKSPACE}/syslog || true` -gt 0 ]
+            then
+              echo "FAILURE: Forbidden string found in logs: $forbid"
+              failures=1
+            fi
+          done
 
-          # Ensure grpc isn't misconfigured, or being used after a fork
-          if [ `grep -c "Fork support is only compatible with the epoll1 and poll polling strategies" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "grpc called after a fork!"
-            exit 1
+          if [ $failures -gt 0 ]; then
+              echo "...failures detected."
+              exit 1
           fi
 
       - name: Gather logs
         if: ${{ ! cancelled() }}
         run: |
           set -x
           . ${GITHUB_WORKSPACE}/ci-environment.sh
```

### Comparing `shakenfist-client-0.7.0.0rc4/.github/workflows/functional-tests-debian-11-slim-primary.yml` & `shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-debian-11-slim-primary.yml`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,23 @@
       - develop
       - v*-releases
 
 jobs:
   debian-11-slim-primary:
     runs-on: self-hosted
     timeout-minutes: 120
+    concurrency:
+      group: ${{ github.workflow }}-${{ github.ref }}
+      cancel-in-progress: true
 
     # NOTE(mikal): git repos are checked out to /srv/github/_work/{repo}/{repo}
     # which is available as GITHUB_WORKSPACE. You can find other environment
     # variables at https://docs.github.com/en/actions/learn-github-actions/environment-variables
 
     steps:
-      - name: Remove previous unfinished runs
-        uses: n1hility/cancel-previous-runs@v2
-        with: 
-          token: ${{ secrets.GITHUB_TOKEN }}
-
       - name: Set environment variables
         run: |
           echo "SF_HEAD_SHA=${{ github.event.pull_request.head.sha }}" >> $GITHUB_ENV
           echo "SF_PRIMARY_REPO=$( echo ${{ github.repository }} | cut -f 2 -d '/' )" >> $GITHUB_ENV
           echo "SHAKENFIST_NAMESPACE=$(hostname)" >> $GITHUB_ENV
 
       - name: Checkout client-python
@@ -135,54 +133,56 @@
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               debian@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; stestr run --concurrency=5"
 
       - name: Check logs
         if: ${{ ! cancelled() }}
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
+          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
+                -o UserKnownHostsFile=/dev/null \
+                debian@$primary sudo chmod ugo+r /var/log/syslog
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               debian@$primary:/var/log/syslog \
               ${GITHUB_WORKSPACE}/syslog
 
-          # Ensure we don't have any tracebacks
-          if [ `grep -c "Traceback (most recent call last):" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "We have tracebacks in the logs!"
-            exit 1
-          fi
-
-          # Ensure we didn't log any errors -- note the inclusion of the start
-          # of the process name here to avoid errors from things like prometheus
-          # node exporter.
-          if [ `grep -c "ERROR sf" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "Errors were logged!"
-            exit 1
-          fi
+          failures=0
 
-          # Ensure nothing died
-          if [ `grep -c " died" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "A process died!"
-            exit 1
+          echo
+          etcd_conns=`grep -c "Building new etcd connection" ${GITHUB_WORKSPACE}/syslog || true`
+          echo "This CI run created $etcd_conns etcd connections."
+          if [ $etcd_conns -gt 5000 ]; then
+            echo "FAILURE: Too many etcd clients!"
+            failures=1
           fi
 
-          # Ensure no leaked vxlans
-          if [ `grep -c "Extra vxlan present" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "vxlans leaked!"
-            exit 1
-          fi
+          FORBIDDEN=("Traceback (most recent call last):"
+                     "ERROR sf"
+                     " died"
+                     "Extra vxlan present"
+                     "Fork support is only compatible with the epoll1 and poll polling strategies"
+                     "not using configured address"
+                     "Dumping thread traces"
+                     "because it is leased to"
+                     "not committing online upgrade"
+                     "Received a GOAWAY with error code ENHANCE_YOUR_CALM"
+                     "ConnectionFailedError")
+          IFS=""
+          for forbid in ${FORBIDDEN[*]}
+          do
+            if [ `grep -c "$forbid" ${GITHUB_WORKSPACE}/syslog || true` -gt 0 ]
+            then
+              echo "FAILURE: Forbidden string found in logs: $forbid"
+              failures=1
+            fi
+          done
 
-          # Ensure grpc isn't misconfigured, or being used after a fork
-          if [ `grep -c "Fork support is only compatible with the epoll1 and poll polling strategies" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "grpc called after a fork!"
-            exit 1
+          if [ $failures -gt 0 ]; then
+              echo "...failures detected."
+              exit 1
           fi
 
       - name: Gather logs
         if: ${{ ! cancelled() }}
         run: |
           set -x
           . ${GITHUB_WORKSPACE}/ci-environment.sh
```

### Comparing `shakenfist-client-0.7.0.0rc4/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml` & `shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests-ubuntu-2004-slim-primary.yml`

 * *Files 7% similar despite different names*

```diff
@@ -10,25 +10,23 @@
       - develop
       - v*-releases
 
 jobs:
   ubuntu-2004-slim-primary:
     runs-on: self-hosted
     timeout-minutes: 120
+    concurrency:
+      group: ${{ github.workflow }}-${{ github.ref }}
+      cancel-in-progress: true
 
     # NOTE(mikal): git repos are checked out to /srv/github/_work/{repo}/{repo}
     # which is available as GITHUB_WORKSPACE. You can find other environment
     # variables at https://docs.github.com/en/actions/learn-github-actions/environment-variables
 
     steps:
-      - name: Remove previous unfinished runs
-        uses: n1hility/cancel-previous-runs@v2
-        with: 
-          token: ${{ secrets.GITHUB_TOKEN }}
-
       - name: Set environment variables
         run: |
           echo "SF_HEAD_SHA=${{ github.event.pull_request.head.sha }}" >> $GITHUB_ENV
           echo "SF_PRIMARY_REPO=$( echo ${{ github.repository }} | cut -f 2 -d '/' )" >> $GITHUB_ENV
           echo "SHAKENFIST_NAMESPACE=$(hostname)" >> $GITHUB_ENV
 
       - name: Checkout client-python
@@ -135,54 +133,56 @@
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               ubuntu@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; stestr run --concurrency=5"
 
       - name: Check logs
         if: ${{ ! cancelled() }}
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
+          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
+                -o UserKnownHostsFile=/dev/null \
+                ubuntu@$primary sudo chmod ugo+r /var/log/syslog
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               ubuntu@$primary:/var/log/syslog \
               ${GITHUB_WORKSPACE}/syslog
 
-          # Ensure we don't have any tracebacks
-          if [ `grep -c "Traceback (most recent call last):" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "We have tracebacks in the logs!"
-            exit 1
-          fi
-
-          # Ensure we didn't log any errors -- note the inclusion of the start
-          # of the process name here to avoid errors from things like prometheus
-          # node exporter.
-          if [ `grep -c "ERROR sf" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "Errors were logged!"
-            exit 1
-          fi
+          failures=0
 
-          # Ensure nothing died
-          if [ `grep -c " died" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "A process died!"
-            exit 1
+          echo
+          etcd_conns=`grep -c "Building new etcd connection" ${GITHUB_WORKSPACE}/syslog || true`
+          echo "This CI run created $etcd_conns etcd connections."
+          if [ $etcd_conns -gt 5000 ]; then
+            echo "FAILURE: Too many etcd clients!"
+            failures=1
           fi
 
-          # Ensure no leaked vxlans
-          if [ `grep -c "Extra vxlan present" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "vxlans leaked!"
-            exit 1
-          fi
+          FORBIDDEN=("Traceback (most recent call last):"
+                     "ERROR sf"
+                     " died"
+                     "Extra vxlan present"
+                     "Fork support is only compatible with the epoll1 and poll polling strategies"
+                     "not using configured address"
+                     "Dumping thread traces"
+                     "because it is leased to"
+                     "not committing online upgrade"
+                     "Received a GOAWAY with error code ENHANCE_YOUR_CALM"
+                     "ConnectionFailedError")
+          IFS=""
+          for forbid in ${FORBIDDEN[*]}
+          do
+            if [ `grep -c "$forbid" ${GITHUB_WORKSPACE}/syslog || true` -gt 0 ]
+            then
+              echo "FAILURE: Forbidden string found in logs: $forbid"
+              failures=1
+            fi
+          done
 
-          # Ensure grpc isn't misconfigured, or being used after a fork
-          if [ `grep -c "Fork support is only compatible with the epoll1 and poll polling strategies" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "grpc called after a fork!"
-            exit 1
+          if [ $failures -gt 0 ]; then
+              echo "...failures detected."
+              exit 1
           fi
 
       - name: Gather logs
         if: ${{ ! cancelled() }}
         run: |
           set -x
           . ${GITHUB_WORKSPACE}/ci-environment.sh
```

### Comparing `shakenfist-client-0.7.0.0rc4/.github/workflows/functional-tests.tmpl` & `shakenfist-client-0.7.0.0rc5/.github/workflows/functional-tests.tmpl`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,23 @@
       - develop
       - v*-releases
 
 jobs:
   {{name}}:
     runs-on: self-hosted
     timeout-minutes: 120
+    concurrency:
+      group: {% raw %}${{ github.workflow }}-${{ github.ref }}{% endraw %}
+      cancel-in-progress: true
 
     # NOTE(mikal): git repos are checked out to /srv/github/_work/{repo}/{repo}
     # which is available as GITHUB_WORKSPACE. You can find other environment
     # variables at https://docs.github.com/en/actions/learn-github-actions/environment-variables
 
     steps:
-      - name: Remove previous unfinished runs
-        uses: n1hility/cancel-previous-runs@v2
-        with: 
-          token: {% raw %}${{{% endraw %} secrets.GITHUB_TOKEN {% raw %}}}{% endraw %}
-
       - name: Set environment variables
         run: |
           echo "SF_HEAD_SHA={% raw %}${{{% endraw %} github.event.pull_request.head.sha {% raw %}}}{% endraw %}" >> $GITHUB_ENV
           echo "SF_PRIMARY_REPO=$( echo {% raw %}${{{% endraw %} github.repository {% raw %}}}{% endraw %} | cut -f 2 -d '/' )" >> $GITHUB_ENV
           echo "SHAKENFIST_NAMESPACE=$(hostname)" >> $GITHUB_ENV
 
       - name: Checkout client-python
@@ -135,54 +133,56 @@
           ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no -o UserKnownHostsFile=/dev/null \
               {{baseuser}}@$primary "cd shakenfist/deploy; . /etc/sf/sfrc; sudo pip3 install -r requirements.txt; stestr run --concurrency={{concurrency}}"
 
       - name: Check logs
         if: {% raw %}${{{% endraw %} ! cancelled() {% raw %}}}{% endraw %}
         run: |
           . ${GITHUB_WORKSPACE}/ci-environment.sh
+          ssh -i /srv/github/id_ci -o StrictHostKeyChecking=no \
+                -o UserKnownHostsFile=/dev/null \
+                {{baseuser}}@$primary sudo chmod ugo+r /var/log/syslog
           scp -rp -i /srv/github/id_ci -o StrictHostKeyChecking=no \
               -o UserKnownHostsFile=/dev/null \
               {{baseuser}}@$primary:/var/log/syslog \
               ${GITHUB_WORKSPACE}/syslog
 
-          # Ensure we don't have any tracebacks
-          if [ `grep -c "Traceback (most recent call last):" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "We have tracebacks in the logs!"
-            exit 1
-          fi
-
-          # Ensure we didn't log any errors -- note the inclusion of the start
-          # of the process name here to avoid errors from things like prometheus
-          # node exporter.
-          if [ `grep -c "ERROR sf" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "Errors were logged!"
-            exit 1
-          fi
+          failures=0
 
-          # Ensure nothing died
-          if [ `grep -c " died" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "A process died!"
-            exit 1
+          echo
+          etcd_conns=`grep -c "Building new etcd connection" ${GITHUB_WORKSPACE}/syslog || true`
+          echo "This CI run created $etcd_conns etcd connections."
+          if [ $etcd_conns -gt 5000 ]; then
+            echo "FAILURE: Too many etcd clients!"
+            failures=1
           fi
 
-          # Ensure no leaked vxlans
-          if [ `grep -c "Extra vxlan present" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "vxlans leaked!"
-            exit 1
-          fi
+          FORBIDDEN=("Traceback (most recent call last):"
+                     "ERROR sf"
+                     " died"
+                     "Extra vxlan present"
+                     "Fork support is only compatible with the epoll1 and poll polling strategies"
+                     "not using configured address"
+                     "Dumping thread traces"
+                     "because it is leased to"
+                     "not committing online upgrade"
+                     "Received a GOAWAY with error code ENHANCE_YOUR_CALM"
+                     "ConnectionFailedError")
+          IFS=""
+          for forbid in ${FORBIDDEN[*]}
+          do
+            if [ `grep -c "$forbid" ${GITHUB_WORKSPACE}/syslog || true` -gt 0 ]
+            then
+              echo "FAILURE: Forbidden string found in logs: $forbid"
+              failures=1
+            fi
+          done
 
-          # Ensure grpc isn't misconfigured, or being used after a fork
-          if [ `grep -c "Fork support is only compatible with the epoll1 and poll polling strategies" ${GITHUB_WORKSPACE}/syslog` -gt 0 ]
-          then
-            echo "grpc called after a fork!"
-            exit 1
+          if [ $failures -gt 0 ]; then
+              echo "...failures detected."
+              exit 1
           fi
 
       - name: Gather logs
         if: {% raw %}${{{% endraw %} ! cancelled() {% raw %}}}{% endraw %}
         run: |
           set -x
           . ${GITHUB_WORKSPACE}/ci-environment.sh
```

### Comparing `shakenfist-client-0.7.0.0rc4/.github/workflows/python-unit-tests.yml` & `shakenfist-client-0.7.0.0rc5/.github/workflows/python-unit-tests.yml`

 * *Files 26% similar despite different names*

```diff
@@ -11,54 +11,45 @@
   pull_request:
     branches:
       - develop
       - v*-releases
 
 jobs:
   lint:
-    runs-on: ubuntu-latest
+    runs-on: self-hosted
 
     steps:
       - name: Checkout code with two commits
         uses: actions/checkout@v2
         with:
           fetch-depth: 2
 
       - name: Install dependencies
         run: |
-          python -m pip install --upgrade pip
-          sudo apt-get install -y -q tox
+          sudo apt-get update
+          sudo apt-get dist-upgrade -y
+          sudo apt-get remove -y -q python3-virtualenv
+          pip install -U -r test-requirements.txt
 
       - name: Lint with flake8
         run: |
           tox -eflake8
 
   build38:
-    runs-on: ubuntu-latest
+    runs-on: self-hosted
 
     steps:
       - name: Checkout code with two commits
         uses: actions/checkout@v2
         with:
           fetch-depth: 2
 
-      - name: Set up Python 3.8
-        uses: actions/setup-python@v2
-        with:
-          python-version: 3.8
-
       - name: Install dependencies
         run: |
-          python -m pip install --upgrade pip
-          sudo apt-get install -y -q tox
-
-      - name: Test with python 3.8
-        run: |
-          tox -epy3
-
-      - name: Test with python 3.8 again
-        run: |
-          tox -epy3
+          sudo apt-get update
+          sudo apt-get dist-upgrade -y
+          sudo apt-get remove -y -q python3-virtualenv
+          pip install -r test-requirements.txt
 
-      - name: Test with python 3.8 again again
+      - name: Run python3 unit tests
         run: |
           tox -epy3
```

### Comparing `shakenfist-client-0.7.0.0rc4/LICENSE` & `shakenfist-client-0.7.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/PKG-INFO` & `shakenfist-client-0.7.0.0rc5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-client
-Version: 0.7.0.0rc4
+Version: 0.7.0.0rc5
 Summary: Shaken Fist: an opinionated minimal cloud
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python REST API client for Shaken Fist
         ======================================
```

### Comparing `shakenfist-client-0.7.0.0rc4/ansible/sf_instance.py` & `shakenfist-client-0.7.0.0rc5/ansible/sf_instance.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/ansible/sf_network.py` & `shakenfist-client-0.7.0.0rc5/ansible/sf_network.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/ansible/sf_snapshot.py` & `shakenfist-client-0.7.0.0rc5/ansible/sf_snapshot.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/release.sh` & `shakenfist-client-0.7.0.0rc5/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/setup.cfg` & `shakenfist-client-0.7.0.0rc5/setup.cfg`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/setup.py` & `shakenfist-client-0.7.0.0rc5/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/apiclient.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/apiclient.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 ASYNC_BLOCK = 'block'
 
 
 class UnconfiguredException(Exception):
     pass
 
 
+class IncapableException(Exception):
+    pass
+
+
+class InvalidException(Exception):
+    pass
+
+
 class APIException(Exception):
     def __init__(self, message, method, url, status_code, text):
         self.message = message
         self.method = method
         self.url = url
         self.status_code = status_code
         self.text = text
@@ -163,14 +171,25 @@
         self.async_strategy = async_strategy
         LOG.debug('Client configured with apiurl of %s for namespace %s '
                   'and async strategy %s'
                   % (self.base_url, self.namespace, self.async_strategy))
 
         self.cached_auth = None
 
+        # Request capabilities information
+        self._collect_capabilities()
+
+    def _collect_capabilities(self):
+        r = requests.request('GET', self.base_url, allow_redirects=True)
+        self.root_html = r.text
+
+    def check_capability(self, capability_string):
+        # NOTE(mikal): this likely needs to be fancier
+        return capability_string in self.root_html
+
     def _actual_request_url(self, method, url, data=None,
                             request_body_is_binary=False,
                             response_body_is_binary=False,
                             allow_redirects=True, stream=False):
         url = self.base_url + url
 
         h = {'Authorization': self.cached_auth,
@@ -278,14 +297,127 @@
                 if time.time() > deadline:
                     LOG.debug('Deadline exceeded waiting for dependancies')
                     raise e
 
                 LOG.debug('Dependencies not ready, retrying')
                 time.sleep(1)
 
+    # The metadata calls are repetitive and handled here as a group
+    def _get_metadata(self, object_plural, object_reference):
+        r = self._request_url(
+            'GET', '/' + object_plural + '/' + object_reference + '/metadata')
+        return r.json()
+
+    def get_artifact_metadata(self, artifact_ref):
+        return self._get_metadata('artifacts', artifact_ref)
+
+    def get_blob_metadata(self, blob_uuid):
+        return self._get_metadata('blobs', blob_uuid)
+
+    def get_interface_metadata(self, interface_uuid):
+        return self._get_metadata('interfaces', interface_uuid)
+
+    def get_instance_metadata(self, instance_ref):
+        return self._get_metadata('instances', instance_ref)
+
+    def get_namespace_metadata(self, namespace):
+        return self._get_metadata('auth/namespaces', namespace)
+
+    def get_network_metadata(self, network_ref):
+        return self._get_metadata('networks', network_ref)
+
+    def get_node_metadata(self, node):
+        return self._get_metadata('nodes', node)
+
+    def _set_metadata(self, object_plural, object_reference, key, value):
+        r = self._request_url(
+            'PUT', '/' + object_plural + '/' + object_reference +
+            '/metadata/' + key, data={'value': value})
+        return r.json()
+
+    def set_artifact_metadata_item(self, artifact_ref, key, value):
+        return self._set_metadata('artifacts', artifact_ref, key, value)
+
+    def set_blob_metadata_item(self, blob_uuid, key, value):
+        return self._set_metadata('blobs', blob_uuid, key, value)
+
+    def set_interface_metadata_item(self, interface_uuid, key, value):
+        return self._set_metadata('interfaces', interface_uuid, key, value)
+
+    def set_instance_metadata_item(self, instance_ref, key, value):
+        return self._set_metadata('instances', instance_ref, key, value)
+
+    def set_namespace_metadata_item(self, namespace, key, value):
+        return self._set_metadata('auth/namespaces', namespace, key, value)
+
+    def set_network_metadata_item(self, network_ref, key, value):
+        return self._set_metadata('networks', network_ref, key, value)
+
+    def set_node_metadata_item(self, node, key, value):
+        return self._set_metadata('nodes', node, key, value)
+
+    def _delete_metadata(self, object_plural, object_reference, key):
+        r = self._request_url(
+            'DELETE', '/' + object_plural + '/' + object_reference +
+            '/metadata/' + key)
+        return r.json()
+
+    def delete_artifact_metadata_item(self, artifact_ref, key):
+        return self._delete_metadata('artifacts', artifact_ref, key)
+
+    def delete_blob_metadata_item(self, blob_uuid, key):
+        return self._delete_metadata('blobs', blob_uuid, key)
+
+    def delete_interface_metadata_item(self, interface_uuid, key):
+        return self._delete_metadata('interfaces', interface_uuid, key)
+
+    def delete_instance_metadata_item(self, instance_ref, key):
+        return self._delete_metadata('instances', instance_ref, key)
+
+    def delete_namespace_metadata_item(self, namespace, key):
+        return self._delete_metadata('auth/namespaces', namespace, key)
+
+    def delete_network_metadata_item(self, network_ref, key):
+        return self._delete_metadata('networks', network_ref, key)
+
+    def delete_node_metadata_item(self, node, key):
+        return self._delete_metadata('nodes', node, key)
+
+    # Similarly the event calls are repetitive and handled as a group
+    def _get_events(self, object_plural, object_reference, event_type, limit):
+        if event_type or limit:
+            if not self.check_capability('events-by-type'):
+                raise IncapableException(
+                    'The API server version you are talking to does not support '
+                    'filtering by event type or count.')
+
+        body = {}
+        if event_type:
+            body['event_type'] = event_type
+        if limit:
+            body['limit'] = limit
+
+        r = self._request_url(
+            'GET', '/' + object_plural + '/' + object_reference + '/events',
+            body)
+        return r.json()
+
+    def get_artifact_events(self, artifact_ref, event_type=None, limit=None):
+        return self._get_events('artifacts', artifact_ref, event_type, limit)
+
+    def get_instance_events(self, instance_ref, event_type=None, limit=None):
+        return self._get_events('instances', instance_ref, event_type, limit)
+
+    def get_network_events(self, network_ref, event_type=None, limit=None):
+        return self._get_events('networks', network_ref, event_type, limit)
+
+    def get_node_events(self, node, event_type=None, limit=None):
+        return self._get_events('nodes', node, event_type, limit)
+
+    # Other calls
     def get_instances(self, all=False):
         r = self._request_url('GET', '/instances', data={'all': all})
         return r.json()
 
     def delete_all_instances(self, namespace):
         r = self._request_url('DELETE', '/instances',
                               data={'confirm': True,
@@ -315,29 +447,14 @@
         return r.json()
 
     def get_instance_interfaces(self, instance_ref):
         r = self._request_url('GET', '/instances/' + instance_ref +
                               '/interfaces')
         return r.json()
 
-    def get_instance_metadata(self, instance_ref):
-        r = self._request_url('GET', '/instances/' + instance_ref +
-                              '/metadata')
-        return r.json()
-
-    def set_instance_metadata_item(self, instance_ref, key, value):
-        r = self._request_url('PUT', '/instances/' + instance_ref +
-                              '/metadata/' + key, data={'value': value})
-        return r.json()
-
-    def delete_instance_metadata_item(self, instance_ref, key):
-        r = self._request_url('DELETE', '/instances/' + instance_ref +
-                              '/metadata/' + key)
-        return r.json()
-
     def create_instance(self, name, cpus, memory, network, disk, sshkey, userdata,
                         namespace=None, force_placement=None, video=None, uefi=False,
                         configdrive=None, nvram_template=None, secure_boot=False,
                         metadata=None, side_channels=None):
         body = {
             # Values all instances care about
             'name': name,
@@ -500,45 +617,47 @@
             LOG.debug('Waiting for instance to be deleted')
             if time.time() > deadline:
                 LOG.debug('Deadline exceeded waiting for instance to delete')
                 return i
 
             time.sleep(1)
 
-    def get_instance_events(self, instance_ref):
-        r = self._request_url('GET', '/instances/' + instance_ref + '/events')
-        return r.json()
-
     def cache_artifact(self, image_url, shared=False, namespace=None):
         r = self._request_url('POST', '/artifacts',
                               data={
                                   'url': image_url,
                                   'shared': shared,
                                   'namespace': namespace
                               })
         return r.json()
 
     def upload_artifact(self, name, upload_uuid, source_url=None, shared=False,
-                        namespace=None):
+                        namespace=None, artifact_type='image'):
         if '/' in name:
-            raise RequestMalformedException('Names must not contain /')
+            raise InvalidException('Names must not contain /')
+
+        if artifact_type != 'image':
+            if not self.check_capability('artifact-upload-types'):
+                raise IncapableException(
+                    'The API server version you are talking to does not support '
+                    'specifying upload artifact types other than image.')
 
         r = self._request_url('POST', '/artifacts/upload/%s' % name,
                               data={
                                   'upload_uuid': upload_uuid,
                                   'source_url': source_url,
                                   'shared': shared,
                                   'namespace': namespace
                               })
         return r.json()
 
     def blob_artifact(self, name, blob_uuid, source_url=None, shared=False,
                       namespace=None):
         if '/' in name:
-            raise RequestMalformedException('Names must not contain /')
+            raise InvalidException('Names must not contain /')
 
         r = self._request_url('POST', '/artifacts/upload/%s' % name,
                               data={
                                   'blob_uuid': blob_uuid,
                                   'source_url': source_url,
                                   'shared': shared,
                                   'namespace': namespace
@@ -553,18 +672,14 @@
         r = self._request_url('GET', '/artifacts', data={'node': node})
 
         out = []
         for a in r.json():
             out.append(_correct_blob_indexes(a))
         return out
 
-    def get_artifact_events(self, artifact_ref):
-        r = self._request_url('GET', '/artifacts/' + artifact_ref + '/events')
-        return r.json()
-
     def get_artifact_versions(self, artifact_ref):
         r = self._request_url(
             'GET', '/artifacts/' + artifact_ref + '/versions')
         return r.json()
 
     def set_artifact_max_versions(self, artifact_ref, max_versions):
         r = self._request_url('POST',
@@ -639,18 +754,14 @@
         r = self._request_url('DELETE', '/networks',
                               data={'confirm': True,
                                     'namespace': namespace,
                                     'clean_wait': clean_wait,
                                     })
         return r.json()
 
-    def get_network_events(self, network_ref):
-        r = self._request_url('GET', '/networks/' + network_ref + '/events')
-        return r.json()
-
     def allocate_network(self, netblock, provide_dhcp, provide_nat, name, namespace=None):
         r = self._request_url('POST', '/networks',
                               data={
                                   'netblock': netblock,
                                   'provide_dhcp': provide_dhcp,
                                   'provide_nat': provide_nat,
                                   'name': name,
@@ -672,27 +783,20 @@
             n = self.get_network(n['uuid'])
 
     def get_network_interfaces(self, network_ref):
         r = self._request_url('GET', '/networks/' +
                               network_ref + '/interfaces')
         return r.json()
 
-    def get_network_metadata(self, network_ref):
-        r = self._request_url('GET', '/networks/' + network_ref +
-                              '/metadata')
-        return r.json()
-
-    def set_network_metadata_item(self, network_ref, key, value):
-        r = self._request_url('PUT', '/networks/' + network_ref +
-                              '/metadata/' + key, data={'value': value})
-        return r.json()
-
-    def delete_network_metadata_item(self, network_ref, key):
-        r = self._request_url('DELETE', '/networks/' + network_ref +
-                              '/metadata/' + key)
+    def get_node(self, node):
+        if not self.check_capability('node-get'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'showing a single node, try "node list" instead.')
+        r = self._request_url('GET', '/nodes/' + node)
         return r.json()
 
     def get_nodes(self):
         r = self._request_url('GET', '/nodes')
         return r.json()
 
     def delete_node(self, node):
@@ -729,14 +833,38 @@
                 pass
         return out
 
     def delete_console_data(self, instance_ref):
         url = '/instances/' + instance_ref + '/consoledata'
         self._request_url('DELETE', url)
 
+    def get_vdi_console_helper(self, instance_ref):
+        r = self._request_url('GET', '/instances/' + instance_ref + '/vdiconsolehelper')
+        return r.text
+
+    def put_instance_blob(self, instance_ref, blob_uuid, path, mode):
+        if not self.check_capability('instance-put-blob'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'placing a blob on an instance.')
+
+        r = self._request_url('POST', '/instances/' + instance_ref + '/agent/put',
+                              data={'blob_uuid': blob_uuid, 'path': path, 'mode': mode})
+        return r.json()
+
+    def instance_execute(self, instance_ref, command_line):
+        if not self.check_capability('instance-execute'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'executing a command within an instance.')
+
+        r = self._request_url('POST', '/instances/' + instance_ref + '/agent/execute',
+                              data={'command_line': command_line})
+        return r.json()
+
     def get_namespaces(self):
         r = self._request_url('GET', '/auth/namespaces')
         return r.json()
 
     def get_namespace(self, namespace):
         r = self._request_url('GET', '/auth/namespaces/' + namespace)
         return r.json()
@@ -756,33 +884,23 @@
         return r.json()
 
     def add_namespace_key(self, namespace, key_name, key):
         r = self._request_url('POST', '/auth/namespaces/' + namespace + '/keys',
                               data={'key_name': key_name, 'key': key})
         return r.json()
 
+    def update_namespace_key(self, namespace, key_name, key):
+        r = self._request_url('PUT', '/auth/namespaces/' + namespace + '/keys',
+                              data={'key_name': key_name, 'key': key})
+        return r.json()
+
     def delete_namespace_key(self, namespace, key_name):
         self._request_url(
             'DELETE', '/auth/namespaces/' + namespace + '/keys/' + key_name)
 
-    def get_namespace_metadata(self, namespace):
-        r = self._request_url('GET', '/auth/namespaces/' + namespace +
-                              '/metadata')
-        return r.json()
-
-    def set_namespace_metadata_item(self, namespace, key, value):
-        r = self._request_url('PUT', '/auth/namespaces/' + namespace +
-                              '/metadata/' + key, data={'value': value})
-        return r.json()
-
-    def delete_namespace_metadata_item(self, namespace, key):
-        r = self._request_url(
-            'DELETE', '/auth/namespaces/' + namespace + '/metadata/' + key)
-        return r.json()
-
     def add_namespace_trust(self, namespace, trusted_namespace):
         r = self._request_url('POST', '/auth/namespaces/' + namespace + '/trust',
                               data={'external_namespace': trusted_namespace})
         return r.json()
 
     def remove_namespace_trust(self, namespace, trusted_namespace):
         r = self._request_url(
@@ -803,16 +921,70 @@
         return r.json()
 
     def send_upload(self, upload_uuid, data):
         r = self._request_url('POST', '/upload/' + upload_uuid,
                               data=data, request_body_is_binary=True)
         return r.json()
 
+    def send_upload_file(self, upload_uuid, flo):
+        buffer_size = 4096
+        total = 0
+        retries = 0
+
+        d = flo.read(buffer_size)
+        while d:
+            start_time = time.time()
+            try:
+                self.send_upload(upload_uuid, d)
+                retries = 0
+            except APIException as e:
+                retries += 1
+
+                if retries > 5:
+                    raise e
+
+                self.truncate_upload(upload_uuid, total)
+                flo.seek(total)
+                buffer_size = 4096
+                d = flo.read(buffer_size)
+                continue
+
+            # We aim for each chunk to take three seconds to transfer. This is
+            # partially because of the API timeout on the other end, but also
+            # so that uploads don't appear to stall over very slow networks.
+            # However, the buffer size must also always be between 4kb and 4mb.
+            elapsed = time.time() - start_time
+            buffer_size = int(buffer_size * 3.0 / elapsed)
+            buffer_size = max(4 * 1024, buffer_size)
+            buffer_size = min(2 * 1024 * 1024, buffer_size)
+
+            sent = len(d)
+            total += sent
+
+            d = flo.read(buffer_size)
+
     def truncate_upload(self, upload_uuid, offset):
         r = self._request_url(
             'POST', '/upload/' + upload_uuid + '/truncate/' + str(offset))
         return r.json()
 
+    def get_agent_operation(self, operation_uuid):
+        if not self.check_capability('agentoperations-crud'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'agent operations.')
+
+        r = self._request_url('GET', '/agentoperations/' + operation_uuid)
+        return r.json()
+
+    def delete_agent_operation(self, operation_uuid):
+        if not self.check_capability('agentoperations-crud'):
+            raise IncapableException(
+                'The API server version you are talking to does not support '
+                'agent operations.')
+
+        self._request_url('DELETE', '/agentoperations/' + operation_uuid)
+
 
 def get_user_agent():
     sf_version = VersionInfo('shakenfist_client').version_string()
     return 'Mozilla/5.0 (Ubuntu; Linux x86_64) Shaken Fist/%s' % sf_version
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/admin.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/admin.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/artifact.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/artifact.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import click
 import datetime
-import hashlib
 import http
 import json
-import os
 from prettytable import PrettyTable
 from tqdm import tqdm
 import requests
 import sys
-import time
 import urllib3
 
-from shakenfist_client import apiclient
 from shakenfist_client import util
 
 
 @click.group(help='Artifact commands')
 def artifact():
     pass
 
@@ -53,96 +49,32 @@
                     'artifact with others.'))
 @click.option('--namespace', type=click.STRING,
               help=('If you are an admin, you can create this object in a '
                     'different namespace.'))
 @click.pass_context
 def artifact_upload(ctx, name=None, source=None, source_url=None, not_shared=True,
                     namespace=None):
-    # We can cheat here -- if we already have a blob in the cluster with the
-    # checksum of the file we're uploading, we can skip the upload entirely and
-    # just reuse that blob.
-    st = os.stat(source)
-
-    sha512_hash = hashlib.sha512()
-    total = 0
-    with open(source, 'rb') as f:
-        with tqdm(total=st.st_size, unit='B', unit_scale=True,
-                  desc='Calculate checksum') as pbar:
-            d = f.read(4096)
-            while d:
-                total += len(d)
-                sha512_hash.update(d)
-                pbar.update(total)
-                d = f.read(4096)
+    if not ctx.obj['CLIENT'].check_capability('blob-search-by-hash'):
+        blob = None
+    else:
+        # We can cheat here -- if we already have a blob in the cluster with the
+        # checksum of the file we're uploading, we can skip the upload entirely and
+        # just reuse that blob.
+        blob = util.checksum_with_progress(ctx.obj['CLIENT'], source)
 
-    print('Searching for a pre-existing blob with this hash...')
-    blob = ctx.obj['CLIENT'].get_blob_by_sha512(sha512_hash.hexdigest())
     if not blob:
-        print('None found, uploading')
-        buffer_size = 4096
-
-        upload = ctx.obj['CLIENT'].create_upload()
-        total = 0
-        retries = 0
-        with tqdm(total=st.st_size, unit='B', unit_scale=True,
-                  desc='Uploading %s to %s' % (upload['uuid'], upload['node'])) as pbar:
-            with open(source, 'rb') as f:
-                d = f.read(buffer_size)
-                while d:
-                    start_time = time.time()
-                    try:
-                        remote_total = ctx.obj['CLIENT'].send_upload(
-                            upload['uuid'], d)
-                        retries = 0
-                    except apiclient.APIException as e:
-                        retries += 1
-
-                        if retries > 5:
-                            print('Repeated failures, aborting')
-                            raise e
-
-                        print('Upload error, retrying...')
-                        ctx.obj['CLIENT'].truncate_upload(
-                            upload['uuid'], total)
-                        f.seek(total)
-                        buffer_size = 4096
-                        d = f.read(buffer_size)
-                        continue
-
-                    # We aim for each chunk to take three seconds to transfer. This is
-                    # partially because of the API timeout on the other end, but also
-                    # so that uploads don't appear to stall over very slow networks.
-                    # However, the buffer size must also always be between 4kb and 4mb.
-                    elapsed = time.time() - start_time
-                    buffer_size = int(buffer_size * 3.0 / elapsed)
-                    buffer_size = max(4 * 1024, buffer_size)
-                    buffer_size = min(2 * 1024 * 1024, buffer_size)
-
-                    sent = len(d)
-                    total += sent
-                    pbar.update(sent)
-
-                    if total != remote_total:
-                        print('Remote side has %d, we have sent %d!'
-                              % (remote_total, total))
-                        sys.exit(1)
-
-                    d = f.read(buffer_size)
-
-        s = not not_shared
-        artifact = ctx.obj['CLIENT'].upload_artifact(
-            name, upload['uuid'], source_url=source_url, shared=s, namespace=namespace)
-        print('Created artifact %s' % artifact['uuid'])
-
+        artifact = util.upload_artifact_with_progress(
+            ctx.obj['CLIENT'], name, source, source_url,
+            namespace=namespace, shared=(not not_shared))
     else:
         print('Recycling existing blob')
         s = not not_shared
         artifact = ctx.obj['CLIENT'].blob_artifact(
             name, blob['uuid'], source_url=source_url, shared=s, namespace=namespace)
-        print('Created artifact %s' % artifact['uuid'])
+    print('Created artifact %s' % artifact['uuid'])
 
 
 @artifact.command(name='download', help='Download an artifact.')
 @click.argument('artifact_ref', type=click.STRING, shell_complete=_get_artifacts)
 @click.argument('destination', type=click.Path(exists=False))
 @click.pass_context
 def artifact_download(ctx, artifact_ref=None, destination=None):
@@ -236,42 +168,57 @@
 
 
 @artifact.command(name='show', help='Show an artifact')
 @click.argument('artifact_ref', type=click.STRING, shell_complete=_get_artifacts)
 @click.pass_context
 def artifact_show(ctx, artifact_ref=None):
     a = ctx.obj['CLIENT'].get_artifact(artifact_ref)
-
     if not a:
         print('Artifact not found')
         sys.exit(1)
 
+    if not ctx.obj['CLIENT'].check_capability('artifact-metadata'):
+        metadata = {}
+    else:
+        metadata = ctx.obj['CLIENT'].get_artifact_metadata(a['uuid'])
+
     if ctx.obj['OUTPUT'] == 'json':
         out = util.filter_dict(a, ['uuid', 'namespace', 'artifact_type', 'state',
                                    'source_url', 'blob_uuid', 'index', 'blobs',
                                    'max_versions', 'shared'])
+        out['metadata'] = metadata
         print(json.dumps(out, indent=4, sort_keys=True))
         return
 
     if ctx.obj['OUTPUT'] == 'simple':
         format_string = '%s:%s'
     else:
         format_string = '%-25s: %s'
 
     print(format_string % ('uuid', a['uuid']))
     print(format_string % ('namespace', a.get('namespace', '')))
     print(format_string % ('type', a['artifact_type']))
     print(format_string % ('state', a['state']))
     print(format_string % ('source url', a['source_url']))
-    print(format_string
-          % ('current version blob uuid', a.get('blob_uuid', 'None')))
+    print(format_string % ('current version blob uuid', a.get('blob_uuid', 'None')))
     print(format_string % ('number of versions', len(a.get('blobs'))))
     print(format_string % ('maximum versions', a['max_versions']))
     print(format_string % ('shared', a.get('shared', False)))
 
+    print()
+    if ctx.obj['OUTPUT'] == 'pretty':
+        format_string = '    %-8s: %s'
+        print('Metadata:')
+        for key in metadata:
+            print(format_string % (key, metadata[key]))
+    else:
+        print('metadata,key,value')
+        for key in metadata:
+            print('metadata,%s,%s' % (key, metadata[key]))
+
     if ctx.obj['OUTPUT'] == 'simple':
         print('version,size,instance')
         format_string = '%s:%0.1fMB,%s'
         for ver, info in a.get('blobs', {}).items():
             print(format_string % (ver,
                                    int(info['size'])/1024/1024,
                                    ','.join(info['instances'])))
@@ -336,17 +283,19 @@
 @click.pass_context
 def artifact_unshare(ctx, artifact_ref=None):
     ctx.obj['CLIENT'].unshare_artifact(artifact_ref)
 
 
 @artifact.command(name='events', help='Display events for an artifact')
 @click.argument('artifact_ref', type=click.STRING, shell_complete=_get_artifacts)
+@click.option('-t', '--type', help='The event type to return')
+@click.option('-l', '--limit', help='The maximum number of events to return')
 @click.pass_context
-def artifact_events(ctx, artifact_ref=None):
-    events = ctx.obj['CLIENT'].get_artifact_events(artifact_ref)
+def artifact_events(ctx, artifact_ref=None, type=None, limit=None):
+    events = ctx.obj['CLIENT'].get_artifact_events(artifact_ref, event_type=type, limit=limit)
     if ctx.obj['OUTPUT'] == 'pretty':
         x = PrettyTable()
         x.field_names = ['timestamp', 'node', 'duration', 'message', 'extra']
         for e in events:
             e['timestamp'] = datetime.datetime.fromtimestamp(e['timestamp'])
             x.add_row([e['timestamp'], e['fqdn'], e['duration'], e['message'],
                        e.get('extra', '')])
@@ -358,7 +307,36 @@
             e['timestamp'] = datetime.datetime.fromtimestamp(e['timestamp'])
             print('%s,%s,%s,%s,%s'
                   % (e['timestamp'], e['fqdn'], e['duration'], e['message'],
                      e.get('extra', '')))
 
     elif ctx.obj['OUTPUT'] == 'json':
         print(json.dumps(events, indent=4, sort_keys=True))
+
+
+@artifact.command(name='set-metadata', help='Set a metadata item')
+@click.argument('artifact_ref', type=click.STRING, shell_complete=_get_artifacts)
+@click.argument('key', type=click.STRING)
+@click.argument('value', type=click.STRING)
+@click.pass_context
+def instance_set_metadata(ctx, artifact_ref=None, key=None, value=None):
+    if not ctx.obj['CLIENT'].check_capability('artifact-metadata'):
+        sys.stderr.write(
+            'Unfortunately this server does not implement artifact metadata.\n')
+        sys.exit(1)
+    ctx.obj['CLIENT'].set_instance_metadata_item(artifact_ref, key, value)
+    if ctx.obj['OUTPUT'] == 'json':
+        print('{}')
+
+
+@artifact.command(name='delete-metadata', help='Delete a metadata item')
+@click.argument('artifact_ref', type=click.STRING, shell_complete=_get_artifacts)
+@click.argument('key', type=click.STRING)
+@click.pass_context
+def instance_delete_metadata(ctx, artifact_ref=None, key=None):
+    if not ctx.obj['CLIENT'].check_capability('artifact-metadata'):
+        sys.stderr.write(
+            'Unfortunately this server does not implement artifact metadata.\n')
+        sys.exit(1)
+    ctx.obj['CLIENT'].delete_instance_metadata_item(artifact_ref, key)
+    if ctx.obj['OUTPUT'] == 'json':
+        print('{}')
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/backup.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/backup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/blob.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/blob.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 from collections import defaultdict
 import json
 from prettytable import PrettyTable
+import sys
 
 
 GiB = 1024 * 1024 * 1024
 
 
 @click.group(help='Blob commands')
 def blob():
@@ -25,17 +26,17 @@
     if audit:
         for instance in ctx.obj['CLIENT'].get_instances():
             for d in instance['disk_spec']:
                 blob_uuid = d.get('blob_uuid')
                 if blob_uuid:
                     discovered_blob_references[blob_uuid] += 1
 
-        for artifact in ctx.obj['CLIENT'].get_artifacts():
-            for index in artifact['blobs']:
-                discovered_blob_references[artifact['blobs']
+        for blob in ctx.obj['CLIENT'].get_blobs():
+            for index in blob['blobs']:
+                discovered_blob_references[blob['blobs']
                                            [index]['uuid']] += 1
 
         for b in ctx.obj['CLIENT'].get_blobs():
             if b['depends_on']:
                 discovered_blob_references[b['depends_on']] += 1
 
             for t in b.get('transcodes'):
@@ -114,26 +115,42 @@
 
 def _blob_show(ctx, b):
     if ctx.obj['OUTPUT'] == 'simple':
         format_string = '%s:%s'
     else:
         format_string = '%-16s: %s'
 
+    if not ctx.obj['CLIENT'].check_capability('blob-metadata'):
+        metadata = {}
+    else:
+        metadata = ctx.obj['CLIENT'].get_blob_metadata(b['uuid'])
+
     print(format_string % ('uuid', b['uuid']))
     print(format_string % ('state', b['state']))
     print(format_string % ('actual size', b['size']))
     print(format_string % ('virtual size', b.get('virtual size', '0')))
     print(format_string % ('sha512', b.get('sha512')))
     print(format_string % ('format', b.get('file format')))
     print(format_string % ('fetched at', b['fetched_at']))
     print(format_string % ('last used', b['last_used']))
     print(format_string % ('reference count', b['reference_count']))
     print(format_string % ('locations', ' '.join(b['locations'])))
 
     print()
+    if ctx.obj['OUTPUT'] == 'pretty':
+        format_string = '    %-8s: %s'
+        print('Metadata:')
+        for key in metadata:
+            print(format_string % (key, metadata[key]))
+    else:
+        print('metadata,key,value')
+        for key in metadata:
+            print('metadata,%s,%s' % (key, metadata[key]))
+
+    print()
     for t in b.get('transcodes'):
         print('Transcoded as %s at %s' % (t, b['transcodes'][t]))
 
     print()
     for i in b.get('instances'):
         print('Used by instance %s' % i)
 
@@ -166,7 +183,36 @@
         return
 
     if not blob:
         print('No blob found')
         return
 
     _blob_show(ctx, blob)
+
+
+@blob.command(name='set-metadata', help='Set a metadata item')
+@click.argument('uuid', type=click.STRING, shell_complete=_get_blobs)
+@click.argument('key', type=click.STRING)
+@click.argument('value', type=click.STRING)
+@click.pass_context
+def instance_set_metadata(ctx, uuid=None, key=None, value=None):
+    if not ctx.obj['CLIENT'].check_capability('blob-metadata'):
+        sys.stderr.write(
+            'Unfortunately this server does not implement blob metadata.\n')
+        sys.exit(1)
+    ctx.obj['CLIENT'].set_instance_metadata_item(uuid, key, value)
+    if ctx.obj['OUTPUT'] == 'json':
+        print('{}')
+
+
+@blob.command(name='delete-metadata', help='Delete a metadata item')
+@click.argument('uuid', type=click.STRING, shell_complete=_get_blobs)
+@click.argument('key', type=click.STRING)
+@click.pass_context
+def instance_delete_metadata(ctx, uuid=None, key=None):
+    if not ctx.obj['CLIENT'].check_capability('blob-metadata'):
+        sys.stderr.write(
+            'Unfortunately this server does not implement blob metadata.\n')
+        sys.exit(1)
+    ctx.obj['CLIENT'].delete_instance_metadata_item(uuid, key)
+    if ctx.obj['OUTPUT'] == 'json':
+        print('{}')
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/instance.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/instance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import base64
 import click
 import datetime
 import json
+import os
 from prettytable import PrettyTable
+import subprocess
 import sys
+import tempfile
+import time
 
 from shakenfist_client import apiclient, util
 
 
 @click.group(help='Instance commands')
 def instance():
     pass
@@ -123,15 +127,15 @@
     interfaces = ctx.obj['CLIENT'].get_instance_interfaces(i['uuid'])
     if include_snapshots:
         snapshots = ctx.obj['CLIENT'].get_instance_snapshots(i['uuid'])
 
     if ctx.obj['OUTPUT'] == 'json':
         out = util.filter_dict(i, ['uuid', 'name', 'namespace', 'cpus', 'memory',
                                    'disk_spec', 'video', 'node', 'console_port',
-                                   'vdi_port', 'ssh_key', 'user_data',
+                                   'vdi_port', 'vdi_tls_port', 'ssh_key', 'user_data',
                                    'power_state', 'state', 'uefi', 'secure_boot',
                                    'nvram_template', 'side_channels'])
         out['network_interfaces'] = []
         for interface in interfaces:
             util.show_interface(ctx, interface, out)
 
         out['metadata'] = metadata
@@ -171,15 +175,19 @@
     print(format_string % ('power state', i.get('power_state', '')))
     print(format_string % ('state', i.get('state', '')))
     print(format_string % ('error message', i.get('error_message', '')))
 
     # NOTE(mikal): I am not sure we should expose this, but it will do
     # for now until a proxy is written.
     print(format_string % ('console port', i.get('console_port', '')))
+
     print(format_string % ('vdi port', i.get('vdi_port', '')))
+    if i.get('vdi_tls_port'):
+        print(format_string % ('vdi tls port', i.get('vdi_tls_port', '')))
+
     print(format_string % ('side channels', ' '.join(i.get('side_channels', []))))
 
     print()
     print(format_string % ('ssh key', i['ssh_key']))
     print(format_string % ('user data', i['user_data']))
 
     if ctx.obj['OUTPUT'] == 'simple':
@@ -234,20 +242,20 @@
             for snap in snapshots:
                 print('snapshot,%s,%s,%s'
                       % (snap['uuid'], snap['device'],
                          datetime.datetime.fromtimestamp(snap['created'])))
 
 
 @instance.command(name='show', help='Show an instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.argument('snapshots', type=click.BOOL, default=False)
 @click.pass_context
-def instance_show(ctx, instance_uuid=None, snapshots=False):
+def instance_show(ctx, instance_ref=None, snapshots=False):
     _show_instance(ctx, ctx.obj['CLIENT'].get_instance(
-        instance_uuid), snapshots)
+        instance_ref), snapshots)
 
 
 def _parse_spec(spec):
     if '@' not in spec:
         return spec, None
     return spec.split('@')
 
@@ -433,31 +441,37 @@
             return
         try:
             val = _convert_metadata(key, val)
         except json.decoder.JSONDecodeError:
             return
         metadata_def[key] = val
 
-    _show_instance(
-        ctx,
-        ctx.obj['CLIENT'].create_instance(
+    kwargs = {
+        'force_placement': placement,
+        'namespace': namespace,
+        'video': video,
+        'uefi': uefi,
+        'configdrive': configdrive,
+        'secure_boot': secure_boot,
+        'nvram_template': nvram_template,
+        'metadata': metadata_def,
+        'side_channels': side_channel
+    }
+
+    _show_instance(ctx, ctx.obj['CLIENT'].create_instance(
             name, cpus, memory, netdefs, diskdefs, sshkey_content,
-            userdata_content, force_placement=placement,
-            namespace=namespace, video=video, uefi=uefi,
-            configdrive=configdrive, secure_boot=secure_boot,
-            nvram_template=nvram_template, metadata=metadata_def,
-            side_channels=side_channel))
+            userdata_content, **kwargs))
 
 
 @instance.command(name='delete', help='Delete an instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.option('--namespace', type=click.STRING)
 @click.pass_context
-def instance_delete(ctx, instance_uuid=None, namespace=None):
-    out = ctx.obj['CLIENT'].delete_instance(instance_uuid, namespace=namespace)
+def instance_delete(ctx, instance_ref=None, namespace=None):
+    out = ctx.obj['CLIENT'].delete_instance(instance_ref, namespace=namespace)
     if ctx.obj['OUTPUT'] == 'json':
         print(json.dumps(out, indent=4, sort_keys=True))
 
 
 @instance.command(name='delete-all', help='Delete ALL instances')
 @click.option('--confirm',  is_flag=True)
 @click.option('--namespace', type=click.STRING)
@@ -467,18 +481,20 @@
         print('You must be sure. Use option --confirm.')
         return
 
     ctx.obj['CLIENT'].delete_all_instances(namespace)
 
 
 @instance.command(name='events', help='Display events for an instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
+@click.option('-t', '--type', help='The event type to return')
+@click.option('-l', '--limit', help='The maximum number of events to return')
 @click.pass_context
-def instance_events(ctx, instance_uuid=None):
-    events = ctx.obj['CLIENT'].get_instance_events(instance_uuid)
+def instance_events(ctx, instance_ref=None, type=None, limit=None):
+    events = ctx.obj['CLIENT'].get_instance_events(instance_ref, event_type=type, limit=limit)
     if ctx.obj['OUTPUT'] == 'pretty':
         x = PrettyTable()
         x.field_names = ['timestamp', 'node', 'duration', 'message', 'extra']
         for e in events:
             e['timestamp'] = datetime.datetime.fromtimestamp(e['timestamp'])
             x.add_row([e['timestamp'], e['fqdn'], e['duration'], e['message'],
                        e.get('extra', '')])
@@ -493,114 +509,238 @@
                      e.get('extra', '')))
 
     elif ctx.obj['OUTPUT'] == 'json':
         print(json.dumps(events, indent=4, sort_keys=True))
 
 
 @instance.command(name='set-metadata', help='Set a metadata item')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.argument('key', type=click.STRING)
 @click.argument('value', type=click.STRING)
 @click.pass_context
-def instance_set_metadata(ctx, instance_uuid=None, key=None, value=None):
+def instance_set_metadata(ctx, instance_ref=None, key=None, value=None):
     try:
         value = _convert_metadata(key, value)
     except json.decoder.JSONDecodeError:
         return
-    ctx.obj['CLIENT'].set_instance_metadata_item(instance_uuid, key, value)
+    ctx.obj['CLIENT'].set_instance_metadata_item(instance_ref, key, value)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @instance.command(name='delete-metadata', help='Delete a metadata item')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.argument('key', type=click.STRING)
 @click.pass_context
-def instance_delete_metadata(ctx, instance_uuid=None, key=None):
-    ctx.obj['CLIENT'].delete_instance_metadata_item(instance_uuid, key)
+def instance_delete_metadata(ctx, instance_ref=None, key=None):
+    ctx.obj['CLIENT'].delete_instance_metadata_item(instance_ref, key)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @instance.command(name='reboot', help='Reboot instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.option('--hard/--soft', default=False)
 @click.pass_context
-def instance_reboot(ctx, instance_uuid=None, hard=False):
-    ctx.obj['CLIENT'].reboot_instance(instance_uuid, hard=hard)
+def instance_reboot(ctx, instance_ref=None, hard=False):
+    ctx.obj['CLIENT'].reboot_instance(instance_ref, hard=hard)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @instance.command(name='poweron', help='Power on an instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.pass_context
-def instance_power_on(ctx, instance_uuid=None):
-    ctx.obj['CLIENT'].power_on_instance(instance_uuid)
+def instance_power_on(ctx, instance_ref=None):
+    ctx.obj['CLIENT'].power_on_instance(instance_ref)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @instance.command(name='poweroff', help='Power off an instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.pass_context
-def instance_power_off(ctx, instance_uuid=None):
-    ctx.obj['CLIENT'].power_off_instance(instance_uuid)
+def instance_power_off(ctx, instance_ref=None):
+    ctx.obj['CLIENT'].power_off_instance(instance_ref)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @instance.command(name='pause', help='Pause an instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.pass_context
-def instance_pause(ctx, instance_uuid=None):
-    ctx.obj['CLIENT'].pause_instance(instance_uuid)
+def instance_pause(ctx, instance_ref=None):
+    ctx.obj['CLIENT'].pause_instance(instance_ref)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @instance.command(name='unpause', help='Unpause an instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.pass_context
-def instance_unpause(ctx, instance_uuid=None):
-    ctx.obj['CLIENT'].unpause_instance(instance_uuid)
+def instance_unpause(ctx, instance_ref=None):
+    ctx.obj['CLIENT'].unpause_instance(instance_ref)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @instance.command(name='consoledata', help='Get console data for an instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.argument('length', type=click.INT, default=10240)
 @click.pass_context
-def instance_consoledata(ctx, instance_uuid=None, length=None):
-    print(ctx.obj['CLIENT'].get_console_data(instance_uuid, length=length))
+def instance_consoledata(ctx, instance_ref=None, length=None):
+    print(ctx.obj['CLIENT'].get_console_data(instance_ref, length=length))
 
 
 @instance.command(name='consoledelete', help='Clear the console log for this instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
+@click.pass_context
+def instance_consoledelete(ctx, instance_ref=None):
+    ctx.obj['CLIENT'].delete_console_data(instance_ref)
+
+
+@instance.command(name='vdiconsole', help='Launch a VDI console for the instance')
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.pass_context
-def instance_consoledelete(ctx, instance_uuid=None):
-    ctx.obj['CLIENT'].delete_console_data(instance_uuid)
+def instance_vdiconsole(ctx, instance_ref=None):
+    if not ctx.obj['CLIENT'].check_capability('vdi-console-helper'):
+        sys.stderr.write(
+            'Unfortunately this server does not implement VDI console helpers.\n')
+        sys.exit(1)
+
+    debug = ''
+    if ctx.obj['VERBOSE']:
+        debug = '--debug'
+
+    # We don't use NamedTemporaryFile as a context manager as the .vv file
+    # will also attempt to clean up the file.
+    (temp_handle, temp_name) = tempfile.mkstemp()
+    os.close(temp_handle)
+    try:
+        with open(temp_name, 'w') as f:
+            f.write(ctx.obj['CLIENT'].get_vdi_console_helper(instance_ref))
+
+        p = subprocess.run('remote-viewer %s %s' % (debug, temp_name), shell=True)
+        if ctx.obj['VERBOSE']:
+            print('Remote viewer process exited with %d return code'
+                  % p.returncode)
+    finally:
+        if os.path.exists(temp_name):
+            os.unlink(temp_name)
+
+
+@instance.command(name='vdiconsolefile', help='Download a .vv file for the VDI console')
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
+@click.pass_context
+def instance_vdiconsolefile(ctx, instance_ref=None):
+    if not ctx.obj['CLIENT'].check_capability('vdi-console-helper'):
+        sys.stderr.write(
+            'Unfortunately this server does not implement VDI console helpers.\n')
+        sys.exit(1)
+
+    print(ctx.obj['CLIENT'].get_vdi_console_helper(instance_ref))
 
 
 @instance.command(name='snapshot', help='Snapshot instance')
-@click.argument('instance_uuid', type=click.STRING, shell_complete=_get_instances)
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
 @click.option('-a', '--all', is_flag=True,
               help='Snapshot all disks, not just disk 0.')
 @click.option('-d', '--device', default=None,
               help='Snapshot this specific device, instead of disk 0.')
 @click.option('-l', '--label_name', default=None,
               help='Label this snapshot with the specified name.')
 @click.option('--delete-snapshot-after-label/--retain-snapshot-after-label',
               is_flag=True, default=False)
 @click.option('--thin/--flatten', is_flag=True, default=False)
 @click.pass_context
-def instance_snapshot(ctx, instance_uuid=None, all=False, device=None, label_name=None,
+def instance_snapshot(ctx, instance_ref=None, all=False, device=None, label_name=None,
                       delete_snapshot_after_label=None, thin=None):
     snapshot = ctx.obj['CLIENT'].snapshot_instance(
-        instance_uuid, all, device=device, label_name=label_name,
+        instance_ref, all, device=device, label_name=label_name,
         delete_snapshot_after_label=delete_snapshot_after_label,
         thin=thin)
     if ctx.obj['OUTPUT'] == 'json':
         print(json.dumps(snapshot, indent=4, sort_keys=True))
     else:
         print('Created snapshot %s' % snapshot)
+
+
+@instance.command(name='upload', help='Upload a file to an instance')
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
+@click.argument('source', type=click.Path(exists=True))
+@click.argument('destination', type=click.Path())
+@click.pass_context
+def instance_upload(ctx, instance_ref=None, source=None, destination=None):
+    if not ctx.obj['CLIENT'].check_capability('instance-put-blob'):
+        sys.stderr.write(
+            'Unfortunately this server does not implement copying files into instances.\n')
+        sys.exit(1)
+
+    if not ctx.obj['CLIENT'].check_capability('blob-search-by-hash'):
+        blob = None
+    else:
+        # We can cheat here -- if we already have a blob in the cluster with the
+        # checksum of the file we're uploading, we can skip the upload entirely and
+        # just reuse that blob.
+        blob = util.checksum_with_progress(ctx.obj['CLIENT'], source)
+
+    if not blob:
+        artifact = util.upload_artifact_with_progress(
+            ctx.obj['CLIENT'], 'upload-to-%s' % instance_ref, source, None)
+    else:
+        print('Recycling existing blob')
+        artifact = ctx.obj['CLIENT'].blob_artifact(
+            'upload-to-%s' % instance_ref, blob['uuid'], source_url=None)
+    print('Created artifact %s' % artifact['uuid'])
+
+    st = os.stat(source)
+    op = ctx.obj['CLIENT'].put_instance_blob(
+            instance_ref, artifact['blob_uuid'], destination, st.st_mode)
+
+    # Wait for the copy to complete
+    while True:
+        if op['state'] == 'complete':
+            break
+        time.sleep(5)
+        op = ctx.obj['CLIENT'].get_agent_operation(op['uuid'])
+
+    print('Done')
+
+
+@instance.command(name='execute', help='Execute a command on an instance')
+@click.argument('instance_ref', type=click.STRING, shell_complete=_get_instances)
+@click.argument('commandline', type=click.STRING)
+@click.pass_context
+def instance_execute(ctx, instance_ref=None, commandline=None):
+    if not ctx.obj['CLIENT'].check_capability('instance-execute'):
+        sys.stderr.write(
+            'Unfortunately this server does not implement executing commands on instances.\n')
+        sys.exit(1)
+
+    op = ctx.obj['CLIENT'].instance_execute(instance_ref, commandline)
+
+    # Wait for the operation to be complete
+    while True:
+        if op['state'] == 'complete':
+            break
+        time.sleep(5)
+        op = ctx.obj['CLIENT'].get_agent_operation(op['uuid'])
+
+    # Wait for the operation to have results
+    while True:
+        if op['results'] != {}:
+            break
+        time.sleep(5)
+        op = ctx.obj['CLIENT'].get_agent_operation(op['uuid'])
+
+    if ctx.obj['OUTPUT'] == 'json':
+        print(json.dumps(op, indent=4, sort_keys=True))
+        return
+
+    if ctx.obj['OUTPUT'] == 'simple':
+        format_string = '%s:%s'
+    else:
+        format_string = '%-14s: %s'
+
+    print(format_string % ('exit code', op['return-code']))
+    print(format_string % ('stdout', op['stdout']))
+    print(format_string % ('stderr', op['stderr']))
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/label.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/label.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/namespace.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/namespace.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,14 +146,27 @@
 @click.argument('keyname', type=click.STRING)
 @click.argument('key', type=click.STRING)
 @click.pass_context
 def namespace_add_key(ctx, namespace=None, keyname=None, key=None):
     ctx.obj['CLIENT'].add_namespace_key(namespace, keyname, key)
 
 
+@namespace.command(name='update-key',
+                   help=('update a key already present in the namespace.\n\n'
+                         'NAMESPACE: The name of the namespace\n'
+                         'KEY_NAME:  The unique name of the key\n'
+                         'KEY:       The new password for the namespace'))
+@click.argument('namespace', type=click.STRING, shell_complete=_get_namespaces)
+@click.argument('keyname', type=click.STRING)
+@click.argument('key', type=click.STRING)
+@click.pass_context
+def namespace_update_key(ctx, namespace=None, keyname=None, key=None):
+    ctx.obj['CLIENT'].update_namespace_key(namespace, keyname, key)
+
+
 @namespace.command(name='delete-key',
                    help=('delete a specific key from a namespace.\n\n'
                          'NAMESPACE: The name of the namespace\n'
                          'KEYNAME:   The name of the key'))
 @click.argument('namespace', type=click.STRING, shell_complete=_get_namespaces)
 @click.argument('keyname', type=click.STRING)
 @click.pass_context
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/commandline/network.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/commandline/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,18 +75,18 @@
     else:
         print('metadata,key,value')
         for key in metadata:
             print('metadata,%s,%s' % (key, metadata[key]))
 
 
 @network.command(name='show', help='Show a network')
-@click.argument('network_uuid', type=click.STRING, shell_complete=util.get_networks)
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
 @click.pass_context
-def network_show(ctx, network_uuid=None):
-    _show_network(ctx, ctx.obj['CLIENT'].get_network(network_uuid))
+def network_show(ctx, network_ref=None):
+    _show_network(ctx, ctx.obj['CLIENT'].get_network(network_ref))
 
 
 @network.command(name='create',
                  help=('Create a network.\n\n'
                        'NAME:             The name of the network\n'
                        'NETBLOCK:         The IP address block to use, as a CIDR\n'
                        '                  range -- for example 192.168.200.1/24\n'
@@ -116,18 +116,20 @@
         print('You must be sure. Use option --confirm.')
         return
 
     ctx.obj['CLIENT'].delete_all_networks(namespace)
 
 
 @network.command(name='events', help='Display events for a network')
-@click.argument('network_uuid', type=click.STRING, shell_complete=util.get_networks)
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
+@click.option('-t', '--type', help='The event type to return')
+@click.option('-l', '--limit', help='The maximum number of events to return')
 @click.pass_context
-def network_events(ctx, network_uuid=None):
-    events = ctx.obj['CLIENT'].get_network_events(network_uuid)
+def network_events(ctx, network_ref=None, type=None, limit=None):
+    events = ctx.obj['CLIENT'].get_network_events(network_ref, event_type=type, limit=limit)
     if ctx.obj['OUTPUT'] == 'pretty':
         x = PrettyTable()
         x.field_names = ['timestamp', 'node', 'duration', 'message', 'extra']
         for e in events:
             e['timestamp'] = datetime.datetime.fromtimestamp(e['timestamp'])
             x.add_row([e['timestamp'], e['fqdn'], e['duration'],
                        e['message'], e.get('extra', '')])
@@ -142,29 +144,29 @@
                      e.get('extra', '')))
 
     elif ctx.obj['OUTPUT'] == 'json':
         print(json.dumps(events, indent=4, sort_keys=True))
 
 
 @network.command(name='delete', help='Delete a network')
-@click.argument('network_uuid', type=click.STRING, shell_complete=util.get_networks)
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
 @click.option('--namespace', type=click.STRING)
 @click.pass_context
-def network_delete(ctx, network_uuid=None, namespace=None):
-    out = ctx.obj['CLIENT'].delete_network(network_uuid, namespace=None)
+def network_delete(ctx, network_ref=None, namespace=None):
+    out = ctx.obj['CLIENT'].delete_network(network_ref, namespace=None)
     if ctx.obj['OUTPUT'] == 'json':
         print(json.dumps(out, indent=4, sort_keys=True))
 
 
 @network.command(name='instances', help='List instances on a network')
-@click.argument('network_uuid',
+@click.argument('network_ref',
                 type=click.STRING, shell_complete=util.get_networks)
 @click.pass_context
-def network_list_instances(ctx, network_uuid=None):
-    interfaces = ctx.obj['CLIENT'].get_network_interfaces(network_uuid)
+def network_list_instances(ctx, network_ref=None):
+    interfaces = ctx.obj['CLIENT'].get_network_interfaces(network_ref)
 
     if ctx.obj['OUTPUT'] == 'pretty':
         x = PrettyTable()
         x.field_names = ['instance_uuid', 'ipv4', 'floating']
         for ni in interfaces:
             x.add_row([ni['instance_uuid'], ni['ipv4'], ni['floating']])
         print(x)
@@ -176,40 +178,40 @@
                   (ni['instance_uuid'], ni['ipv4'], ni['floating']))
 
     elif ctx.obj['OUTPUT'] == 'json':
         print(json.dumps(interfaces, indent=4, sort_keys=True))
 
 
 @network.command(name='set-metadata', help='Set a metadata item')
-@click.argument('network_uuid', type=click.STRING, shell_complete=util.get_networks)
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
 @click.argument('key', type=click.STRING)
 @click.argument('value', type=click.STRING)
 @click.pass_context
-def network_set_metadata(ctx, network_uuid=None, key=None, value=None):
-    ctx.obj['CLIENT'].set_network_metadata_item(network_uuid, key, value)
+def network_set_metadata(ctx, network_ref=None, key=None, value=None):
+    ctx.obj['CLIENT'].set_network_metadata_item(network_ref, key, value)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @network.command(name='delete-metadata', help='Delete a metadata item')
-@click.argument('network_uuid', type=click.STRING, shell_complete=util.get_networks)
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
 @click.argument('key', type=click.STRING)
 @click.pass_context
-def network_delete_metadata(ctx, network_uuid=None, key=None, value=None):
-    ctx.obj['CLIENT'].delete_network_metadata_item(network_uuid, key)
+def network_delete_metadata(ctx, network_ref=None, key=None, value=None):
+    ctx.obj['CLIENT'].delete_network_metadata_item(network_ref, key)
     if ctx.obj['OUTPUT'] == 'json':
         print('{}')
 
 
 @network.command(name='ping', help='Ping on this network')
-@click.argument('network_uuid', type=click.STRING, shell_complete=util.get_networks)
+@click.argument('network_ref', type=click.STRING, shell_complete=util.get_networks)
 @click.argument('address', type=click.STRING)
 @click.pass_context
-def network_ping(ctx, network_uuid=None, address=None):
-    output = ctx.obj['CLIENT'].ping(network_uuid, address)
+def network_ping(ctx, network_ref=None, address=None):
+    output = ctx.obj['CLIENT'].ping(network_ref, address)
     if ctx.obj['OUTPUT'] in ['pretty', 'simple']:
         for line in output.get('stdout', '').split('\n'):
             print('stdout: %s' % line)
         for line in output.get('stderr', '').split('\n'):
             print('stderr: %s' % line)
 
     elif ctx.obj['OUTPUT'] == 'json':
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/main.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 @click.option('--async-strategy', '--async', envvar='SHAKENFIST_ASYNC', default='pause',
               type=click.Choice(['continue', 'pause', 'block'], case_sensitive=False))
 @click.pass_context
 def cli(ctx, output, verbose, namespace, key, apiurl, async_strategy):
     if not ctx.obj:
         ctx.obj = {}
     ctx.obj['OUTPUT'] = output
+    ctx.obj['VERBOSE'] = verbose
 
     if verbose:
         LOG.setLevel(logging.DEBUG)
         LOG.debug('Set log level to DEBUG')
     else:
         LOG.setLevel(logging.INFO)
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client/tests/test_client_apiclient.py` & `shakenfist-client-0.7.0.0rc5/shakenfist_client/tests/test_client_apiclient.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,19 @@
         super(ApiClientTestCase, self).setUp()
 
         self.request_url = mock.patch(
             'shakenfist_client.apiclient.Client._request_url')
         self.mock_request = self.request_url.start()
         self.addCleanup(self.request_url.stop)
 
+        self.capabilities = mock.patch(
+            'shakenfist_client.apiclient.Client._collect_capabilities')
+        self.capabilities = self.capabilities.start()
+        self.addCleanup(self.capabilities.stop)
+
         self.sleep = mock.patch('time.sleep')
         self.mock_sleep = self.sleep.start()
         self.addCleanup(self.sleep.stop)
 
     def test_get_instances(self):
         client = apiclient.Client(suppress_configuration_lookup=True,
                                   base_url='http://localhost:13000')
@@ -358,14 +363,22 @@
     "lastseen": "Mon, 13 Apr 2020 03:04:17 -0000"
 }
 ]
 """)
 
 
 class ApiClientGetNodesTestCase(testtools.TestCase):
+    def setUp(self):
+        super(ApiClientGetNodesTestCase, self).setUp()
+
+        self.capabilities = mock.patch(
+            'shakenfist_client.apiclient.Client._collect_capabilities')
+        self.capabilities = self.capabilities.start()
+        self.addCleanup(self.capabilities.stop)
+
     @mock.patch('shakenfist_client.apiclient.Client._request_url',
                 return_value=GetNodesMock())
     def test_get_nodes(self, mock_request):
         client = apiclient.Client(suppress_configuration_lookup=True,
                                   base_url='http://localhost:13000')
         list(client.get_nodes())
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/PKG-INFO` & `shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-client
-Version: 0.7.0.0rc4
+Version: 0.7.0.0rc5
 Summary: Shaken Fist: an opinionated minimal cloud
 Home-page: https://madebymikal.com/shakenfist
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: Python REST API client for Shaken Fist
         ======================================
```

### Comparing `shakenfist-client-0.7.0.0rc4/shakenfist_client.egg-info/SOURCES.txt` & `shakenfist-client-0.7.0.0rc5/shakenfist_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/tools/clone_with_depends.py` & `shakenfist-client-0.7.0.0rc5/tools/clone_with_depends.py`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/tools/flake8wrap.sh` & `shakenfist-client-0.7.0.0rc5/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-client-0.7.0.0rc4/tox.ini` & `shakenfist-client-0.7.0.0rc5/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [testenv]
 deps =
   -r{toxinidir}/requirements.txt
   -r{toxinidir}/test-requirements.txt
 commands =
     # NOTE: you can run any command line tool here - not just tests
     stestr run {posargs}
-whitelist_externals =
+allowlist_externals =
   bash
   find
   rm
   env
 setenv =
   VIRTUAL_ENV={envdir}
   LANGUAGE=en_US
@@ -39,8 +39,8 @@
 setenv =
   PYTHON=coverage run --source client --parallel-mode
 commands =
   coverage erase
   stestr run {posargs}
   coverage combine
   coverage html -d cover
-  coverage report
+  coverage report
```

