# Comparing `tmp/modsys-0.4.2.tar.gz` & `tmp/modsys-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modsys-0.4.2.tar", last modified: Sat Jul 15 23:10:35 2023, max compression
+gzip compressed data, was "modsys-0.4.3.tar", last modified: Sat Jul 15 23:28:11 2023, max compression
```

## Comparing `modsys-0.4.2.tar` & `modsys-0.4.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.925051 modsys-0.4.2/
--rw-r--r--   0 abpyguru   (501) staff       (20)    10964 2023-07-11 22:52:05.000000 modsys-0.4.2/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 23:10:35.924793 modsys-0.4.2/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)    12090 2023-07-11 22:52:05.000000 modsys-0.4.2/README.md
--rwxr-xr-x   0 abpyguru   (501) staff       (20)      876 2023-07-11 22:52:05.000000 modsys-0.4.2/cli.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.891382 modsys-0.4.2/modsys/
--rw-r--r--   0 abpyguru   (501) staff       (20)     5463 2023-07-14 02:29:55.000000 modsys-0.4.2/modsys/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     8056 2023-07-15 23:08:44.000000 modsys-0.4.2/modsys/client.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.894509 modsys-0.4.2/modsys/connectors/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.895271 modsys-0.4.2/modsys/connectors/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.2/modsys/connectors/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.896845 modsys-0.4.2/modsys/connectors/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      864 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/google/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1077 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/google/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2887 2023-07-13 04:55:23.000000 modsys-0.4.2/modsys/connectors/google/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1024 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/google/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.897060 modsys-0.4.2/modsys/connectors/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.2/modsys/connectors/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.898513 modsys-0.4.2/modsys/connectors/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      851 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1073 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/openai/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2569 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/openai/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1006 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/openai/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.899364 modsys-0.4.2/modsys/connectors/sightengine/
--rw-r--r--   0 abpyguru   (501) staff       (20)      840 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/sightengine/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1071 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/sightengine/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2879 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/sightengine/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      982 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/connectors/sightengine/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.899575 modsys-0.4.2/modsys/connectors/spot/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.2/modsys/connectors/spot/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2044 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.899840 modsys-0.4.2/modsys/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.903177 modsys-0.4.2/modsys/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1538 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3544 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.903855 modsys-0.4.2/modsys/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.904178 modsys-0.4.2/modsys/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.904864 modsys-0.4.2/modsys/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.908691 modsys-0.4.2/modsys/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      789 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1603 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      860 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4247 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2492 2023-07-14 02:29:55.000000 modsys-0.4.2/modsys/manager.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.915916 modsys-0.4.2/modsys/plugins/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/plugins/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     5296 2023-07-15 23:08:44.000000 modsys-0.4.2/modsys/plugins/evaluations.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2770 2023-07-15 23:08:44.000000 modsys-0.4.2/modsys/plugins/grading.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2217 2023-07-15 22:44:53.000000 modsys-0.4.2/modsys/plugins/prompts.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4072 2023-07-15 23:08:44.000000 modsys-0.4.2/modsys/plugins/utils.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     6503 2023-07-15 22:44:53.000000 modsys-0.4.2/modsys/plugins/validation.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2114 2023-07-14 02:29:55.000000 modsys-0.4.2/modsys/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.916530 modsys-0.4.2/modsys/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.917173 modsys-0.4.2/modsys/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.922639 modsys-0.4.2/modsys/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      804 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      942 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1397 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      905 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.922975 modsys-0.4.2/modsys/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.2/modsys/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:10:35.893856 modsys-0.4.2/modsys.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 23:10:35.000000 modsys-0.4.2/modsys.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1674 2023-07-15 23:10:35.000000 modsys-0.4.2/modsys.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-07-15 23:10:35.000000 modsys-0.4.2/modsys.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       43 2023-07-15 23:10:35.000000 modsys-0.4.2/modsys.egg-info/entry_points.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      521 2023-07-15 23:10:35.000000 modsys-0.4.2/modsys.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-07-15 23:10:35.000000 modsys-0.4.2/modsys.egg-info/top_level.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-07-15 23:10:35.925451 modsys-0.4.2/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     2408 2023-07-15 23:09:09.000000 modsys-0.4.2/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.441648 modsys-0.4.3/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    10964 2023-07-11 22:52:05.000000 modsys-0.4.3/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 23:28:11.441413 modsys-0.4.3/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12090 2023-07-11 22:52:05.000000 modsys-0.4.3/README.md
+-rwxr-xr-x   0 abpyguru   (501) staff       (20)      876 2023-07-11 22:52:05.000000 modsys-0.4.3/cli.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.429941 modsys-0.4.3/modsys/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5463 2023-07-14 02:29:55.000000 modsys-0.4.3/modsys/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     8057 2023-07-15 23:26:18.000000 modsys-0.4.3/modsys/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.431571 modsys-0.4.3/modsys/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.431905 modsys-0.4.3/modsys/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.3/modsys/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.433097 modsys-0.4.3/modsys/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      864 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/google/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1077 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/google/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2887 2023-07-13 04:55:23.000000 modsys-0.4.3/modsys/connectors/google/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1024 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/google/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.433296 modsys-0.4.3/modsys/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.3/modsys/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.434166 modsys-0.4.3/modsys/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      851 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1073 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/openai/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2569 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/openai/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1006 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/openai/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.434969 modsys-0.4.3/modsys/connectors/sightengine/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      840 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/sightengine/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1071 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/sightengine/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2879 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/sightengine/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      982 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/sightengine/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.435146 modsys-0.4.3/modsys/connectors/spot/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.3/modsys/connectors/spot/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2044 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.435408 modsys-0.4.3/modsys/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.436167 modsys-0.4.3/modsys/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1538 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3544 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.436339 modsys-0.4.3/modsys/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.436528 modsys-0.4.3/modsys/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.437103 modsys-0.4.3/modsys/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.437989 modsys-0.4.3/modsys/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      789 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1603 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      860 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4247 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2492 2023-07-14 02:29:55.000000 modsys-0.4.3/modsys/manager.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.439654 modsys-0.4.3/modsys/plugins/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/plugins/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5296 2023-07-15 23:08:44.000000 modsys-0.4.3/modsys/plugins/evaluations.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3217 2023-07-15 23:27:23.000000 modsys-0.4.3/modsys/plugins/grading.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2217 2023-07-15 22:44:53.000000 modsys-0.4.3/modsys/plugins/prompts.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4072 2023-07-15 23:08:44.000000 modsys-0.4.3/modsys/plugins/utils.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     6503 2023-07-15 22:44:53.000000 modsys-0.4.3/modsys/plugins/validation.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2114 2023-07-14 02:29:55.000000 modsys-0.4.3/modsys/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.439979 modsys-0.4.3/modsys/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.440171 modsys-0.4.3/modsys/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.440930 modsys-0.4.3/modsys/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      804 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      942 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1397 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      905 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.441132 modsys-0.4.3/modsys/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.431414 modsys-0.4.3/modsys.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1674 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       43 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/entry_points.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      521 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/top_level.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-07-15 23:28:11.441700 modsys-0.4.3/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2408 2023-07-15 23:27:42.000000 modsys-0.4.3/setup.py
```

### Comparing `modsys-0.4.2/LICENSE` & `modsys-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/PKG-INFO` & `modsys-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modsys
-Version: 0.4.2
+Version: 0.4.3
 Summary: A radically simple framework for ML/AI model management
 Home-page: https://github.com/modsysML/modsys
 Author: ModsysML
 Author-email: adrbrownx@gmail.com
 License: Apache License, Version 2.0
 Platform: Any
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modsys Version: 0.4.2 Summary: A radically simple
+Metadata-Version: 2.1 Name: modsys Version: 0.4.3 Summary: A radically simple
 framework for ML/AI model management Home-page: https://github.com/modsysML/
 modsys Author: ModsysML Author-email: adrbrownx@gmail.com License: Apache
 License, Version 2.0 Platform: Any Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE # modsys: model management
 tool [![python](https://img.shields.io/pypi/pyversions/3)](https://
 www.python.org/downloads/) ![GitHub Workflow Status](https://img.shields.io/
```

### Comparing `modsys-0.4.2/README.md` & `modsys-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/cli.py` & `modsys-0.4.3/cli.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/__init__.py` & `modsys-0.4.3/modsys/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/client.py` & `modsys-0.4.3/modsys/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,18 +206,18 @@
         run the evaluation.
 
         vars (json): [
             {
                 "item": "You suck at this game.",
                 "__expected": {
                     "TOXICITY": {
-                        "value": "0.50"
+                        "value": "0.83"
                     }
                 },
-                "__trend": "lower"
+                "__trend": "higher"
             }
         ] - responsible for setting up test run
 
         provider (str): "google_perspective:analyze"
         """
         if cls.model == "Google":
             conn = cls._api_manager.load_provider(
```

### Comparing `modsys-0.4.2/modsys/connectors/__init__.py` & `modsys-0.4.3/modsys/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/aws/__init__.py` & `modsys-0.4.3/modsys/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/google/__init__.py` & `modsys-0.4.3/modsys/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/google/base.py` & `modsys-0.4.3/modsys/connectors/google/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/google/cloud.py` & `modsys-0.4.3/modsys/connectors/google/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/google/local.py` & `modsys-0.4.3/modsys/connectors/google/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/microsoft/__init__.py` & `modsys-0.4.3/modsys/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/openai/__init__.py` & `modsys-0.4.3/modsys/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/openai/base.py` & `modsys-0.4.3/modsys/connectors/openai/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/openai/cloud.py` & `modsys-0.4.3/modsys/connectors/openai/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/openai/local.py` & `modsys-0.4.3/modsys/connectors/openai/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/sightengine/__init__.py` & `modsys-0.4.3/modsys/connectors/sightengine/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/sightengine/base.py` & `modsys-0.4.3/modsys/connectors/sightengine/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/sightengine/cloud.py` & `modsys-0.4.3/modsys/connectors/sightengine/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/sightengine/local.py` & `modsys-0.4.3/modsys/connectors/sightengine/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/connectors/spot/__init__.py` & `modsys-0.4.3/modsys/connectors/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/const.py` & `modsys-0.4.3/modsys/const.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/__init__.py` & `modsys-0.4.3/modsys/database/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/firebase/__init__.py` & `modsys-0.4.3/modsys/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/firebase/base.py` & `modsys-0.4.3/modsys/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/firebase/cloud.py` & `modsys-0.4.3/modsys/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/firebase/local.py` & `modsys-0.4.3/modsys/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/mongo/__init__.py` & `modsys-0.4.3/modsys/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/mysql/__init__.py` & `modsys-0.4.3/modsys/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/postgres/__init__.py` & `modsys-0.4.3/modsys/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/supabase/__init__.py` & `modsys-0.4.3/modsys/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/supabase/base.py` & `modsys-0.4.3/modsys/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/supabase/cloud.py` & `modsys-0.4.3/modsys/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/database/supabase/local.py` & `modsys-0.4.3/modsys/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/exceptions.py` & `modsys-0.4.3/modsys/exceptions.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/manager.py` & `modsys-0.4.3/modsys/manager.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/plugins/__init__.py` & `modsys-0.4.3/modsys/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/plugins/evaluations.py` & `modsys-0.4.3/modsys/plugins/evaluations.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/plugins/grading.py` & `modsys-0.4.3/modsys/plugins/grading.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,34 +38,42 @@
     if provider_path.startswith("google_perspective:"):
         # Update expected if we're running eval: so that way we can format
         # a dict to pull its value
         if type(expected) == str:
             expected = json.loads(expected)
 
         trend = kwargs["trend"] if "trend" in kwargs else "lower"
+        output_policy = list(output.keys())
         output_dict = list(output.values())
         output_value = round(output_dict[0]["value"] * 100, 2)
+        expected_policy = list(expected.keys())
         expected_dict = list(expected.values())
         expected_value = round(float(expected_dict[0]["value"]) * 100, 2)
         accuracy = (
-            min(expected_value, output_value) / max(expected_value, output_vale)
+            min(expected_value, output_value) / max(expected_value, output_value)
         ) * 100
+        accuracy = round(accuracy, 3)
 
-        if trend == "lower":
-            boolean = bool(accuracy >= 90)
-        elif trend == "higher":
-            boolean = bool(accuracy >= 70)
+        if output_policy[0] == expected_policy[0]:
+            if trend == "lower":
+                boolean = bool(accuracy >= 90)
+            elif trend == "higher":
+                boolean = bool(accuracy >= 70)
+            else:
+                raise ValueError(
+                    "Unsupported assertion, use lower or higher to denote a wider acceptance criteria"
+                )
+            return {
+                "state": boolean,
+                "reason": f"Precision is at {accuracy}%, if trend is lower the acceptance criteria is >=90%, higher is >=70%",
+            }
         else:
-            raise ValueError(
-                "Unsupported assertion, use lower or higher to denote a wider acceptance criteria"
-            )
+            return {
+                "state": False,
+                "reason": f"Output and expected policy category didn't match. {output_policy[0]} != {expected_policy[0]}",
+            }
     elif provider_path.startswith("openai:"):
         raise NotImplementedError
     elif provider_path.startswith("sightengine:"):
         raise NotImplementedError
     else:
         raise NotImplementedError
-
-    return {
-        "state": boolean,
-        "reason": f"Output {output} for provider has a precision rate of {accuracy}% for the expected value {expected}",
-    }
```

### Comparing `modsys-0.4.2/modsys/plugins/prompts.py` & `modsys-0.4.3/modsys/plugins/prompts.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/plugins/utils.py` & `modsys-0.4.3/modsys/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/plugins/validation.py` & `modsys-0.4.3/modsys/plugins/validation.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/resource.py` & `modsys-0.4.3/modsys/resource.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/service/__init__.py` & `modsys-0.4.3/modsys/service/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/service/graphql/__init__.py` & `modsys-0.4.3/modsys/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/service/json/__init__.py` & `modsys-0.4.3/modsys/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/service/json/base.py` & `modsys-0.4.3/modsys/service/json/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/service/json/cloud.py` & `modsys-0.4.3/modsys/service/json/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/service/json/local.py` & `modsys-0.4.3/modsys/service/json/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys/tests/__init__.py` & `modsys-0.4.3/modsys/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys.egg-info/PKG-INFO` & `modsys-0.4.3/modsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modsys
-Version: 0.4.2
+Version: 0.4.3
 Summary: A radically simple framework for ML/AI model management
 Home-page: https://github.com/modsysML/modsys
 Author: ModsysML
 Author-email: adrbrownx@gmail.com
 License: Apache License, Version 2.0
 Platform: Any
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: modsys Version: 0.4.2 Summary: A radically simple
+Metadata-Version: 2.1 Name: modsys Version: 0.4.3 Summary: A radically simple
 framework for ML/AI model management Home-page: https://github.com/modsysML/
 modsys Author: ModsysML Author-email: adrbrownx@gmail.com License: Apache
 License, Version 2.0 Platform: Any Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE # modsys: model management
 tool [![python](https://img.shields.io/pypi/pyversions/3)](https://
 www.python.org/downloads/) ![GitHub Workflow Status](https://img.shields.io/
```

### Comparing `modsys-0.4.2/modsys.egg-info/SOURCES.txt` & `modsys-0.4.3/modsys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/modsys.egg-info/requires.txt` & `modsys-0.4.3/modsys.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `modsys-0.4.2/setup.py` & `modsys-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="modsys",
-    version="0.4.2",
+    version="0.4.3",
     description="A radically simple framework for ML/AI model management",
     author="ModsysML",
     author_email="adrbrownx@gmail.com",
     packages=find_packages(),
     py_modules=["cli", "modsys"],
     url="https://github.com/modsysML/modsys",
     license="Apache License, Version 2.0",
```

