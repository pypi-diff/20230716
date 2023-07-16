# Comparing `tmp/rds-core-0.2.1.tar.gz` & `tmp/rds-core-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rds-core-0.2.1.tar", last modified: Sun Jul  9 22:05:26 2023, max compression
+gzip compressed data, was "rds-core-0.2.2.tar", last modified: Sun Jul 16 19:11:29 2023, max compression
```

## Comparing `rds-core-0.2.1.tar` & `rds-core-0.2.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.535817 rds-core-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-09 22:05:14.000000 rds-core-0.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-09 22:05:26.535817 rds-core-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-09 22:05:14.000000 rds-core-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-09 22:05:14.000000 rds-core-0.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.527816 rds-core-0.2.1/rds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/contrib/datasus/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/contrib/datasus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/contrib/datasus/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/contrib/datasus/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/contrib/datasus/transformers/fields/
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/contrib/datasus/transformers/fields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/core/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/core/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/cache/inmemory.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/cache/nocache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/cache/search_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/core/config/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/core/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/helpers/http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.531816 rds-core-0.2.1/rds/core/searchengine/
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/searchengine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.535817 rds-core-0.2.1/rds/core/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/transformers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.535817 rds-core-0.2.1/rds/core/transformers/fields/
--rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/transformers/fields/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.535817 rds-core-0.2.1/rds/core/transformers/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/transformers/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.535817 rds-core-0.2.1/rds/core/types/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.535817 rds-core-0.2.1/rds/core/validators/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-09 22:05:14.000000 rds-core-0.2.1/rds/core/validators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 22:05:26.535817 rds-core-0.2.1/rds_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-09 22:05:26.000000 rds-core-0.2.1/rds_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-09 22:05:26.000000 rds-core-0.2.1/rds_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 22:05:26.000000 rds-core-0.2.1/rds_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-09 22:05:26.000000 rds-core-0.2.1/rds_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-09 22:05:26.000000 rds-core-0.2.1/rds_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-09 22:05:26.535817 rds-core-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-09 22:05:14.000000 rds-core-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.837921 rds-core-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-16 19:11:17.000000 rds-core-0.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-16 19:11:29.837921 rds-core-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-16 19:11:17.000000 rds-core-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-16 19:11:17.000000 rds-core-0.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/contrib/datasus/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/contrib/datasus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/contrib/datasus/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/contrib/datasus/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/contrib/datasus/transformers/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/contrib/datasus/transformers/fields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/core/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/cache/inmemory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/cache/nocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/cache/search_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/core/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/core/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/helpers/http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.833921 rds-core-0.2.2/rds/core/searchengine/
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/searchengine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.837921 rds-core-0.2.2/rds/core/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/transformers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.837921 rds-core-0.2.2/rds/core/transformers/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/transformers/fields/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.837921 rds-core-0.2.2/rds/core/transformers/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/transformers/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.837921 rds-core-0.2.2/rds/core/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.837921 rds-core-0.2.2/rds/core/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-16 19:11:17.000000 rds-core-0.2.2/rds/core/validators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:11:29.837921 rds-core-0.2.2/rds_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-16 19:11:29.000000 rds-core-0.2.2/rds_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-16 19:11:29.000000 rds-core-0.2.2/rds_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:11:29.000000 rds-core-0.2.2/rds_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-16 19:11:29.000000 rds-core-0.2.2/rds_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-16 19:11:29.000000 rds-core-0.2.2/rds_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-16 19:11:29.837921 rds-core-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-07-16 19:11:17.000000 rds-core-0.2.2/setup.py
```

### Comparing `rds-core-0.2.1/PKG-INFO` & `rds-core-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rds-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
 Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
```

### Comparing `rds-core-0.2.1/README.md` & `rds-core-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/pyproject.toml` & `rds-core-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/contrib/datasus/transformers/fields/__init__.py` & `rds-core-0.2.2/rds/contrib/datasus/transformers/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/cache/__init__.py` & `rds-core-0.2.2/rds/core/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/cache/base.py` & `rds-core-0.2.2/rds/core/cache/base.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/cache/inmemory.py` & `rds-core-0.2.2/rds/core/cache/inmemory.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/cache/nocache.py` & `rds-core-0.2.2/rds/core/cache/nocache.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/cache/search_engine.py` & `rds-core-0.2.2/rds/core/cache/search_engine.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/helpers/__init__.py` & `rds-core-0.2.2/rds/core/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/helpers/http_client.py` & `rds-core-0.2.2/rds/core/helpers/http_client.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/transformers/models/__init__.py` & `rds-core-0.2.2/rds/core/transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds/core/validators/__init__.py` & `rds-core-0.2.2/rds/core/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/rds_core.egg-info/PKG-INFO` & `rds-core-0.2.2/rds_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: rds-core
-Version: 0.2.1
+Version: 0.2.2
 Summary: Framework para serviços do Rede de Dados em Saúde do LAIS
 Home-page: https://github.com/lais-huol/rds-core
 Author: Kelson da Costa Medeiros
 Author-email: kelson.medeiros@lais.huol.ufrn.br
 License: UNKNOWN
 Download-URL: https://github.com/lais-huol/rds-core/tags
 Description: É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias RDS, a exemplo RDS-RN e RDS-ES.
```

### Comparing `rds-core-0.2.1/rds_core.egg-info/SOURCES.txt` & `rds-core-0.2.2/rds_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rds-core-0.2.1/setup.py` & `rds-core-0.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 with open("requirements.txt", "w") as file1:
     for requirement in requirements:
         file1.write(f"{requirement}\n")
 
 setup(
     name="rds-core",
-    version="0.2.1",
+    version="0.2.2",
     description="Framework para serviços do Rede de Dados em Saúde do LAIS",
     long_description="É uma biblioteca pública em Python que condensa um conjunto de boas práticas para o"
     " desenvolvimento das aplicações que compõem a Rede da Dados em Saúde (RDS) RDS do Laboratório de"
     " Inovação Tecnológica em Saúde (LAIS) e dos parceiros que contam com o LAIS para fazer suas próprias"
     " RDS, a exemplo RDS-RN e RDS-ES.",
     author="Kelson da Costa Medeiros",
     author_email="kelson.medeiros@lais.huol.ufrn.br",
```

