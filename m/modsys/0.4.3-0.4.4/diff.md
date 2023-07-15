# Comparing `tmp/modsys-0.4.3.tar.gz` & `tmp/modsys-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modsys-0.4.3.tar", last modified: Sat Jul 15 23:28:11 2023, max compression
+gzip compressed data, was "modsys-0.4.4.tar", last modified: Sat Jul 15 23:38:39 2023, max compression
```

## Comparing `modsys-0.4.3.tar` & `modsys-0.4.4.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.441648 modsys-0.4.3/
--rw-r--r--   0 abpyguru   (501) staff       (20)    10964 2023-07-11 22:52:05.000000 modsys-0.4.3/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 23:28:11.441413 modsys-0.4.3/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)    12090 2023-07-11 22:52:05.000000 modsys-0.4.3/README.md
--rwxr-xr-x   0 abpyguru   (501) staff       (20)      876 2023-07-11 22:52:05.000000 modsys-0.4.3/cli.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.429941 modsys-0.4.3/modsys/
--rw-r--r--   0 abpyguru   (501) staff       (20)     5463 2023-07-14 02:29:55.000000 modsys-0.4.3/modsys/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     8057 2023-07-15 23:26:18.000000 modsys-0.4.3/modsys/client.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.431571 modsys-0.4.3/modsys/connectors/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.431905 modsys-0.4.3/modsys/connectors/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.3/modsys/connectors/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.433097 modsys-0.4.3/modsys/connectors/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      864 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/google/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1077 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/google/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2887 2023-07-13 04:55:23.000000 modsys-0.4.3/modsys/connectors/google/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1024 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/google/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.433296 modsys-0.4.3/modsys/connectors/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.3/modsys/connectors/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.434166 modsys-0.4.3/modsys/connectors/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      851 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1073 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/openai/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2569 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/openai/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1006 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/openai/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.434969 modsys-0.4.3/modsys/connectors/sightengine/
--rw-r--r--   0 abpyguru   (501) staff       (20)      840 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/sightengine/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1071 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/sightengine/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2879 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/sightengine/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      982 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/connectors/sightengine/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.435146 modsys-0.4.3/modsys/connectors/spot/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.3/modsys/connectors/spot/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2044 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.435408 modsys-0.4.3/modsys/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.436167 modsys-0.4.3/modsys/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1538 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3544 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.436339 modsys-0.4.3/modsys/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.436528 modsys-0.4.3/modsys/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.437103 modsys-0.4.3/modsys/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.437989 modsys-0.4.3/modsys/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      789 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1603 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      860 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4247 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2492 2023-07-14 02:29:55.000000 modsys-0.4.3/modsys/manager.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.439654 modsys-0.4.3/modsys/plugins/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/plugins/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     5296 2023-07-15 23:08:44.000000 modsys-0.4.3/modsys/plugins/evaluations.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3217 2023-07-15 23:27:23.000000 modsys-0.4.3/modsys/plugins/grading.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2217 2023-07-15 22:44:53.000000 modsys-0.4.3/modsys/plugins/prompts.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4072 2023-07-15 23:08:44.000000 modsys-0.4.3/modsys/plugins/utils.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     6503 2023-07-15 22:44:53.000000 modsys-0.4.3/modsys/plugins/validation.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2114 2023-07-14 02:29:55.000000 modsys-0.4.3/modsys/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.439979 modsys-0.4.3/modsys/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.440171 modsys-0.4.3/modsys/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.440930 modsys-0.4.3/modsys/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      804 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      942 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1397 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      905 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.441132 modsys-0.4.3/modsys/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.3/modsys/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:28:11.431414 modsys-0.4.3/modsys.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1674 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       43 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/entry_points.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      521 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-07-15 23:28:11.000000 modsys-0.4.3/modsys.egg-info/top_level.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-07-15 23:28:11.441700 modsys-0.4.3/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     2408 2023-07-15 23:27:42.000000 modsys-0.4.3/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.804917 modsys-0.4.4/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    10964 2023-07-11 22:52:05.000000 modsys-0.4.4/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 23:38:39.804683 modsys-0.4.4/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12090 2023-07-11 22:52:05.000000 modsys-0.4.4/README.md
+-rwxr-xr-x   0 abpyguru   (501) staff       (20)      876 2023-07-11 22:52:05.000000 modsys-0.4.4/cli.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.790390 modsys-0.4.4/modsys/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5463 2023-07-14 02:29:55.000000 modsys-0.4.4/modsys/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     8057 2023-07-15 23:37:12.000000 modsys-0.4.4/modsys/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.792031 modsys-0.4.4/modsys/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.792235 modsys-0.4.4/modsys/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.4/modsys/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.796095 modsys-0.4.4/modsys/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      864 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/google/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1077 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/google/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2887 2023-07-13 04:55:23.000000 modsys-0.4.4/modsys/connectors/google/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1024 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/google/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.796452 modsys-0.4.4/modsys/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.4/modsys/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.797315 modsys-0.4.4/modsys/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      851 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1073 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/openai/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2569 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/openai/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1006 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/openai/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.798294 modsys-0.4.4/modsys/connectors/sightengine/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      840 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/sightengine/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1071 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/sightengine/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2879 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/sightengine/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      982 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/connectors/sightengine/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.798520 modsys-0.4.4/modsys/connectors/spot/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.4/modsys/connectors/spot/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2044 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.798810 modsys-0.4.4/modsys/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.799997 modsys-0.4.4/modsys/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1538 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3544 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.800198 modsys-0.4.4/modsys/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.800384 modsys-0.4.4/modsys/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.800571 modsys-0.4.4/modsys/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.801398 modsys-0.4.4/modsys/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      789 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1603 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      860 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4247 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2492 2023-07-14 02:29:55.000000 modsys-0.4.4/modsys/manager.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.802966 modsys-0.4.4/modsys/plugins/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/plugins/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5296 2023-07-15 23:08:44.000000 modsys-0.4.4/modsys/plugins/evaluations.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3217 2023-07-15 23:37:12.000000 modsys-0.4.4/modsys/plugins/grading.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2217 2023-07-15 22:44:53.000000 modsys-0.4.4/modsys/plugins/prompts.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4072 2023-07-15 23:08:44.000000 modsys-0.4.4/modsys/plugins/utils.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     6503 2023-07-15 22:44:53.000000 modsys-0.4.4/modsys/plugins/validation.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2114 2023-07-14 02:29:55.000000 modsys-0.4.4/modsys/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.803279 modsys-0.4.4/modsys/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.803458 modsys-0.4.4/modsys/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.804219 modsys-0.4.4/modsys/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      804 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      942 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1397 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      905 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.804414 modsys-0.4.4/modsys/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.4/modsys/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 23:38:39.791847 modsys-0.4.4/modsys.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 23:38:39.000000 modsys-0.4.4/modsys.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1674 2023-07-15 23:38:39.000000 modsys-0.4.4/modsys.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-07-15 23:38:39.000000 modsys-0.4.4/modsys.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       43 2023-07-15 23:38:39.000000 modsys-0.4.4/modsys.egg-info/entry_points.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      520 2023-07-15 23:38:39.000000 modsys-0.4.4/modsys.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-07-15 23:38:39.000000 modsys-0.4.4/modsys.egg-info/top_level.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-07-15 23:38:39.804973 modsys-0.4.4/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2407 2023-07-15 23:38:12.000000 modsys-0.4.4/setup.py
```

### Comparing `modsys-0.4.3/LICENSE` & `modsys-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/PKG-INFO` & `modsys-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modsys
-Version: 0.4.3
+Version: 0.4.4
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
-Metadata-Version: 2.1 Name: modsys Version: 0.4.3 Summary: A radically simple
+Metadata-Version: 2.1 Name: modsys Version: 0.4.4 Summary: A radically simple
 framework for ML/AI model management Home-page: https://github.com/modsysML/
 modsys Author: ModsysML Author-email: adrbrownx@gmail.com License: Apache
 License, Version 2.0 Platform: Any Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE # modsys: model management
 tool [![python](https://img.shields.io/pypi/pyversions/3)](https://
 www.python.org/downloads/) ![GitHub Workflow Status](https://img.shields.io/
```

### Comparing `modsys-0.4.3/README.md` & `modsys-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/cli.py` & `modsys-0.4.4/cli.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/__init__.py` & `modsys-0.4.4/modsys/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/client.py` & `modsys-0.4.4/modsys/client.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/__init__.py` & `modsys-0.4.4/modsys/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/aws/__init__.py` & `modsys-0.4.4/modsys/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/google/__init__.py` & `modsys-0.4.4/modsys/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/google/base.py` & `modsys-0.4.4/modsys/connectors/google/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/google/cloud.py` & `modsys-0.4.4/modsys/connectors/google/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/google/local.py` & `modsys-0.4.4/modsys/connectors/google/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/microsoft/__init__.py` & `modsys-0.4.4/modsys/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/openai/__init__.py` & `modsys-0.4.4/modsys/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/openai/base.py` & `modsys-0.4.4/modsys/connectors/openai/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/openai/cloud.py` & `modsys-0.4.4/modsys/connectors/openai/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/openai/local.py` & `modsys-0.4.4/modsys/connectors/openai/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/sightengine/__init__.py` & `modsys-0.4.4/modsys/connectors/sightengine/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/sightengine/base.py` & `modsys-0.4.4/modsys/connectors/sightengine/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/sightengine/cloud.py` & `modsys-0.4.4/modsys/connectors/sightengine/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/sightengine/local.py` & `modsys-0.4.4/modsys/connectors/sightengine/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/connectors/spot/__init__.py` & `modsys-0.4.4/modsys/connectors/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/const.py` & `modsys-0.4.4/modsys/const.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/__init__.py` & `modsys-0.4.4/modsys/database/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/firebase/__init__.py` & `modsys-0.4.4/modsys/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/firebase/base.py` & `modsys-0.4.4/modsys/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/firebase/cloud.py` & `modsys-0.4.4/modsys/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/firebase/local.py` & `modsys-0.4.4/modsys/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/mongo/__init__.py` & `modsys-0.4.4/modsys/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/mysql/__init__.py` & `modsys-0.4.4/modsys/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/postgres/__init__.py` & `modsys-0.4.4/modsys/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/supabase/__init__.py` & `modsys-0.4.4/modsys/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/supabase/base.py` & `modsys-0.4.4/modsys/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/supabase/cloud.py` & `modsys-0.4.4/modsys/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/database/supabase/local.py` & `modsys-0.4.4/modsys/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/exceptions.py` & `modsys-0.4.4/modsys/exceptions.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/manager.py` & `modsys-0.4.4/modsys/manager.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/plugins/__init__.py` & `modsys-0.4.4/modsys/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/plugins/evaluations.py` & `modsys-0.4.4/modsys/plugins/evaluations.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/plugins/grading.py` & `modsys-0.4.4/modsys/plugins/grading.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/plugins/prompts.py` & `modsys-0.4.4/modsys/plugins/prompts.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/plugins/utils.py` & `modsys-0.4.4/modsys/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/plugins/validation.py` & `modsys-0.4.4/modsys/plugins/validation.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/resource.py` & `modsys-0.4.4/modsys/resource.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/service/__init__.py` & `modsys-0.4.4/modsys/service/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/service/graphql/__init__.py` & `modsys-0.4.4/modsys/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/service/json/__init__.py` & `modsys-0.4.4/modsys/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/service/json/base.py` & `modsys-0.4.4/modsys/service/json/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/service/json/cloud.py` & `modsys-0.4.4/modsys/service/json/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/service/json/local.py` & `modsys-0.4.4/modsys/service/json/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys/tests/__init__.py` & `modsys-0.4.4/modsys/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys.egg-info/PKG-INFO` & `modsys-0.4.4/modsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modsys
-Version: 0.4.3
+Version: 0.4.4
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
-Metadata-Version: 2.1 Name: modsys Version: 0.4.3 Summary: A radically simple
+Metadata-Version: 2.1 Name: modsys Version: 0.4.4 Summary: A radically simple
 framework for ML/AI model management Home-page: https://github.com/modsysML/
 modsys Author: ModsysML Author-email: adrbrownx@gmail.com License: Apache
 License, Version 2.0 Platform: Any Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE # modsys: model management
 tool [![python](https://img.shields.io/pypi/pyversions/3)](https://
 www.python.org/downloads/) ![GitHub Workflow Status](https://img.shields.io/
```

### Comparing `modsys-0.4.3/modsys.egg-info/SOURCES.txt` & `modsys-0.4.4/modsys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modsys-0.4.3/modsys.egg-info/requires.txt` & `modsys-0.4.4/modsys.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Django<=3.0
+Django>3.0
 firebase-admin==6.2.0
 google-api-core==2.11.1
 google-api-python-client==2.92.0
 google-auth==2.21.0
 google-auth-httplib2==0.1.0
 google-cloud-core==2.3.3
 google-cloud-firestore==2.11.1
```

### Comparing `modsys-0.4.3/setup.py` & `modsys-0.4.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,29 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="modsys",
-    version="0.4.3",
+    version="0.4.4",
     description="A radically simple framework for ML/AI model management",
     author="ModsysML",
     author_email="adrbrownx@gmail.com",
     packages=find_packages(),
     py_modules=["cli", "modsys"],
     url="https://github.com/modsysML/modsys",
     license="Apache License, Version 2.0",
     classifiers=[
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
     ],
     platforms=["Any"],
     install_requires=[
-        "Django<=3.0",
+        "Django>3.0",
         "firebase-admin==6.2.0",
         "google-api-core==2.11.1",
         "google-api-python-client==2.92.0",
         "google-auth==2.21.0",
         "google-auth-httplib2==0.1.0",
         "google-cloud-core==2.3.3",
         "google-cloud-firestore==2.11.1",
```

