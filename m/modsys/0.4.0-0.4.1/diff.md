# Comparing `tmp/modsys-0.4.0.tar.gz` & `tmp/modsys-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modsys-0.4.0.tar", last modified: Fri Jul 14 02:31:39 2023, max compression
+gzip compressed data, was "modsys-0.4.1.tar", last modified: Sat Jul 15 22:45:02 2023, max compression
```

## Comparing `modsys-0.4.0.tar` & `modsys-0.4.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.080430 modsys-0.4.0/
--rw-r--r--   0 abpyguru   (501) staff       (20)    10964 2023-07-11 22:52:05.000000 modsys-0.4.0/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-14 02:31:39.079969 modsys-0.4.0/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)    12090 2023-07-11 22:52:05.000000 modsys-0.4.0/README.md
--rwxr-xr-x   0 abpyguru   (501) staff       (20)      876 2023-07-11 22:52:05.000000 modsys-0.4.0/cli.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.067125 modsys-0.4.0/modsys/
--rw-r--r--   0 abpyguru   (501) staff       (20)     5463 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     8057 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/client.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.068618 modsys-0.4.0/modsys/connectors/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.069019 modsys-0.4.0/modsys/connectors/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.0/modsys/connectors/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.071044 modsys-0.4.0/modsys/connectors/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      864 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/google/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1077 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/google/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2887 2023-07-13 04:55:23.000000 modsys-0.4.0/modsys/connectors/google/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1024 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/google/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.071298 modsys-0.4.0/modsys/connectors/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.0/modsys/connectors/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.072343 modsys-0.4.0/modsys/connectors/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      851 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1073 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/openai/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2569 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/openai/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1006 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/openai/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.073186 modsys-0.4.0/modsys/connectors/sightengine/
--rw-r--r--   0 abpyguru   (501) staff       (20)      840 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/sightengine/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1071 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/sightengine/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2879 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/sightengine/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      982 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/connectors/sightengine/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.073380 modsys-0.4.0/modsys/connectors/spot/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.0/modsys/connectors/spot/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2044 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.073776 modsys-0.4.0/modsys/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.075047 modsys-0.4.0/modsys/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1538 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3544 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.075375 modsys-0.4.0/modsys/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.075603 modsys-0.4.0/modsys/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.075808 modsys-0.4.0/modsys/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.076764 modsys-0.4.0/modsys/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      789 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1603 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      860 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4247 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2492 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/manager.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.078039 modsys-0.4.0/modsys/plugins/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/plugins/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     5306 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/evaluations.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2731 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/grading.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1521 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/prompts.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4082 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/utils.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     6502 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/plugins/validation.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     2114 2023-07-14 02:29:55.000000 modsys-0.4.0/modsys/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.078254 modsys-0.4.0/modsys/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.078461 modsys-0.4.0/modsys/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.079274 modsys-0.4.0/modsys/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      804 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      942 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1397 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      905 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.079496 modsys-0.4.0/modsys/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.0/modsys/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-14 02:31:39.068354 modsys-0.4.0/modsys.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1674 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       43 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/entry_points.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)     1340 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-07-14 02:31:39.000000 modsys-0.4.0/modsys.egg-info/top_level.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-07-14 02:31:39.080491 modsys-0.4.0/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     1628 2023-07-14 02:30:27.000000 modsys-0.4.0/setup.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.587963 modsys-0.4.1/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    10964 2023-07-11 22:52:05.000000 modsys-0.4.1/LICENSE
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 22:45:02.580998 modsys-0.4.1/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12090 2023-07-11 22:52:05.000000 modsys-0.4.1/README.md
+-rwxr-xr-x   0 abpyguru   (501) staff       (20)      876 2023-07-11 22:52:05.000000 modsys-0.4.1/cli.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.542396 modsys-0.4.1/modsys/
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5463 2023-07-14 02:29:55.000000 modsys-0.4.1/modsys/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     8057 2023-07-14 02:29:55.000000 modsys-0.4.1/modsys/client.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.545022 modsys-0.4.1/modsys/connectors/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.545936 modsys-0.4.1/modsys/connectors/aws/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.1/modsys/connectors/aws/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.549935 modsys-0.4.1/modsys/connectors/google/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      864 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/google/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1077 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/google/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2887 2023-07-13 04:55:23.000000 modsys-0.4.1/modsys/connectors/google/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1024 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/google/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.551554 modsys-0.4.1/modsys/connectors/microsoft/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.1/modsys/connectors/microsoft/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.555396 modsys-0.4.1/modsys/connectors/openai/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      851 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/openai/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1073 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/openai/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2569 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/openai/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1006 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/openai/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.558973 modsys-0.4.1/modsys/connectors/sightengine/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      840 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/sightengine/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1071 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/sightengine/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2879 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/sightengine/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      982 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/connectors/sightengine/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.559530 modsys-0.4.1/modsys/connectors/spot/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-12 15:51:16.000000 modsys-0.4.1/modsys/connectors/spot/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2044 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/const.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.559862 modsys-0.4.1/modsys/database/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.566671 modsys-0.4.1/modsys/database/firebase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/firebase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1538 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/firebase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     3544 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/firebase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/firebase/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.569413 modsys-0.4.1/modsys/database/mongo/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/mongo/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.569781 modsys-0.4.1/modsys/database/mysql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/mysql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.570035 modsys-0.4.1/modsys/database/postgres/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/postgres/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.572415 modsys-0.4.1/modsys/database/supabase/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      820 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/supabase/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      789 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/supabase/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1603 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/supabase/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      860 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/database/supabase/local.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4247 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/exceptions.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2492 2023-07-14 02:29:55.000000 modsys-0.4.1/modsys/manager.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.576547 modsys-0.4.1/modsys/plugins/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/plugins/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     5306 2023-07-14 02:29:55.000000 modsys-0.4.1/modsys/plugins/evaluations.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2731 2023-07-14 02:29:55.000000 modsys-0.4.1/modsys/plugins/grading.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2217 2023-07-15 22:44:53.000000 modsys-0.4.1/modsys/plugins/prompts.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     4082 2023-07-14 02:29:55.000000 modsys-0.4.1/modsys/plugins/utils.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     6503 2023-07-15 22:44:53.000000 modsys-0.4.1/modsys/plugins/validation.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2114 2023-07-14 02:29:55.000000 modsys-0.4.1/modsys/resource.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.578047 modsys-0.4.1/modsys/service/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/service/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.578278 modsys-0.4.1/modsys/service/graphql/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/service/graphql/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.580491 modsys-0.4.1/modsys/service/json/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      804 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/service/json/__init__.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      942 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/service/json/base.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1397 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/service/json/cloud.py
+-rw-r--r--   0 abpyguru   (501) staff       (20)      905 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/service/json/local.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.580699 modsys-0.4.1/modsys/tests/
+-rw-r--r--   0 abpyguru   (501) staff       (20)      695 2023-07-11 22:52:05.000000 modsys-0.4.1/modsys/tests/__init__.py
+drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-07-15 22:45:02.544880 modsys-0.4.1/modsys.egg-info/
+-rw-r--r--   0 abpyguru   (501) staff       (20)    12511 2023-07-15 22:45:02.000000 modsys-0.4.1/modsys.egg-info/PKG-INFO
+-rw-r--r--   0 abpyguru   (501) staff       (20)     1674 2023-07-15 22:45:02.000000 modsys-0.4.1/modsys.egg-info/SOURCES.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-07-15 22:45:02.000000 modsys-0.4.1/modsys.egg-info/dependency_links.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       43 2023-07-15 22:45:02.000000 modsys-0.4.1/modsys.egg-info/entry_points.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)      521 2023-07-15 22:45:02.000000 modsys-0.4.1/modsys.egg-info/requires.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       11 2023-07-15 22:45:02.000000 modsys-0.4.1/modsys.egg-info/top_level.txt
+-rw-r--r--   0 abpyguru   (501) staff       (20)       38 2023-07-15 22:45:02.588209 modsys-0.4.1/setup.cfg
+-rw-r--r--   0 abpyguru   (501) staff       (20)     2408 2023-07-15 22:44:53.000000 modsys-0.4.1/setup.py
```

### Comparing `modsys-0.4.0/LICENSE` & `modsys-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/PKG-INFO` & `modsys-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modsys
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: modsys Version: 0.4.0 Summary: A radically simple
+Metadata-Version: 2.1 Name: modsys Version: 0.4.1 Summary: A radically simple
 framework for ML/AI model management Home-page: https://github.com/modsysML/
 modsys Author: ModsysML Author-email: adrbrownx@gmail.com License: Apache
 License, Version 2.0 Platform: Any Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE # modsys: model management
 tool [![python](https://img.shields.io/pypi/pyversions/3)](https://
 www.python.org/downloads/) ![GitHub Workflow Status](https://img.shields.io/
```

### Comparing `modsys-0.4.0/README.md` & `modsys-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/cli.py` & `modsys-0.4.1/cli.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/__init__.py` & `modsys-0.4.1/modsys/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/client.py` & `modsys-0.4.1/modsys/client.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/__init__.py` & `modsys-0.4.1/modsys/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/aws/__init__.py` & `modsys-0.4.1/modsys/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/google/__init__.py` & `modsys-0.4.1/modsys/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/google/base.py` & `modsys-0.4.1/modsys/connectors/google/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/google/cloud.py` & `modsys-0.4.1/modsys/connectors/google/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/google/local.py` & `modsys-0.4.1/modsys/connectors/google/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/microsoft/__init__.py` & `modsys-0.4.1/modsys/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/openai/__init__.py` & `modsys-0.4.1/modsys/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/openai/base.py` & `modsys-0.4.1/modsys/connectors/openai/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/openai/cloud.py` & `modsys-0.4.1/modsys/connectors/openai/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/openai/local.py` & `modsys-0.4.1/modsys/connectors/openai/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/sightengine/__init__.py` & `modsys-0.4.1/modsys/connectors/sightengine/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/sightengine/base.py` & `modsys-0.4.1/modsys/connectors/sightengine/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/sightengine/cloud.py` & `modsys-0.4.1/modsys/connectors/sightengine/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/sightengine/local.py` & `modsys-0.4.1/modsys/connectors/sightengine/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/connectors/spot/__init__.py` & `modsys-0.4.1/modsys/connectors/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/const.py` & `modsys-0.4.1/modsys/const.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/__init__.py` & `modsys-0.4.1/modsys/database/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/firebase/__init__.py` & `modsys-0.4.1/modsys/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/firebase/base.py` & `modsys-0.4.1/modsys/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/firebase/cloud.py` & `modsys-0.4.1/modsys/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/firebase/local.py` & `modsys-0.4.1/modsys/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/mongo/__init__.py` & `modsys-0.4.1/modsys/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/mysql/__init__.py` & `modsys-0.4.1/modsys/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/postgres/__init__.py` & `modsys-0.4.1/modsys/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/supabase/__init__.py` & `modsys-0.4.1/modsys/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/supabase/base.py` & `modsys-0.4.1/modsys/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/supabase/cloud.py` & `modsys-0.4.1/modsys/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/database/supabase/local.py` & `modsys-0.4.1/modsys/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/exceptions.py` & `modsys-0.4.1/modsys/exceptions.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/manager.py` & `modsys-0.4.1/modsys/manager.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/plugins/__init__.py` & `modsys-0.4.1/modsys/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/plugins/evaluations.py` & `modsys-0.4.1/modsys/plugins/evaluations.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/plugins/grading.py` & `modsys-0.4.1/modsys/plugins/grading.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/plugins/utils.py` & `modsys-0.4.1/modsys/plugins/utils.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/plugins/validation.py` & `modsys-0.4.1/modsys/plugins/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #         http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
+
 import io
 import pathlib
 import json
 import csv
 import os
 
 from time import sleep
```

### Comparing `modsys-0.4.0/modsys/resource.py` & `modsys-0.4.1/modsys/resource.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/service/__init__.py` & `modsys-0.4.1/modsys/service/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/service/graphql/__init__.py` & `modsys-0.4.1/modsys/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/service/json/__init__.py` & `modsys-0.4.1/modsys/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/service/json/base.py` & `modsys-0.4.1/modsys/service/json/base.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/service/json/cloud.py` & `modsys-0.4.1/modsys/service/json/cloud.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/service/json/local.py` & `modsys-0.4.1/modsys/service/json/local.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys/tests/__init__.py` & `modsys-0.4.1/modsys/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/modsys.egg-info/PKG-INFO` & `modsys-0.4.1/modsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modsys
-Version: 0.4.0
+Version: 0.4.1
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
-Metadata-Version: 2.1 Name: modsys Version: 0.4.0 Summary: A radically simple
+Metadata-Version: 2.1 Name: modsys Version: 0.4.1 Summary: A radically simple
 framework for ML/AI model management Home-page: https://github.com/modsysML/
 modsys Author: ModsysML Author-email: adrbrownx@gmail.com License: Apache
 License, Version 2.0 Platform: Any Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Description-
 Content-Type: text/markdown License-File: LICENSE # modsys: model management
 tool [![python](https://img.shields.io/pypi/pyversions/3)](https://
 www.python.org/downloads/) ![GitHub Workflow Status](https://img.shields.io/
```

### Comparing `modsys-0.4.0/modsys.egg-info/SOURCES.txt` & `modsys-0.4.1/modsys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modsys-0.4.0/setup.py` & `modsys-0.4.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,25 +23,50 @@
     long_description = f.read()
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 setup(
     name="modsys",
-    version="0.4.0",
+    version="0.4.1",
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
-    install_requires=requirements,
+    install_requires=[
+        "Django<=3.0",
+        "firebase-admin==6.2.0",
+        "google-api-core==2.11.1",
+        "google-api-python-client==2.92.0",
+        "google-auth==2.21.0",
+        "google-auth-httplib2==0.1.0",
+        "google-cloud-core==2.3.3",
+        "google-cloud-firestore==2.11.1",
+        "google-cloud-storage==2.10.0",
+        "google-crc32c==1.5.0",
+        "google-resumable-media==2.5.0",
+        "googleapis-common-protos==1.59.1",
+        "Jinja2==3.1.2",
+        "openai==0.27.7",
+        "psycopg==3.1.6",
+        "psycopg-binary==3.1.6",
+        "psycopg-pool==3.1.7",
+        "psycopg2-binary==2.9.6",
+        "python-dotenv==1.0.0",
+        "requests==2.28.1",
+        "tabulate==0.9.0",
+        "termcolor==2.3.0",
+        "tqdm==4.65.0",
+        "virtualenv==20.21.0",
+    ],
     long_description_content_type="text/markdown",
     long_description=long_description,
     entry_points={"console_scripts": ["modsys=cli:run_console"]},
 )
```

