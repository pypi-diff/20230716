# Comparing `tmp/qalita-1.0.6.tar.gz` & `tmp/qalita-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalita-1.0.6.tar", max compression
+gzip compressed data, was "qalita-1.0.7.tar", max compression
```

## Comparing `qalita-1.0.6.tar` & `qalita-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    19753 2023-07-16 19:00:31.187323 qalita-1.0.6/LICENSE
--rw-r--r--   0        0        0     1942 2023-07-16 19:00:31.187323 qalita-1.0.6/docs/README.md
--rw-r--r--   0        0        0     1169 2023-07-16 19:00:41.128159 qalita-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 19:00:31.209323 qalita-1.0.6/qalita/__init__.py
--rw-r--r--   0        0        0     4189 2023-07-16 19:00:41.129159 qalita-1.0.6/qalita/cli.py
--rw-r--r--   0        0        0        0 2023-07-16 19:00:31.209323 qalita-1.0.6/qalita/commands/__init__.py
--rw-r--r--   0        0        0    19666 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/commands/agent.py
--rw-r--r--   0        0        0    14531 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/commands/pack.py
--rw-r--r--   0        0        0     9756 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/commands/source.py
--rw-r--r--   0        0        0        0 2023-07-16 19:00:31.209323 qalita-1.0.6/qalita/internal/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/internal/logger.py
--rw-r--r--   0        0        0     2486 2023-07-16 19:00:31.189157 qalita-1.0.6/qalita/internal/utils.py
--rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 qalita-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0    19753 2023-07-16 19:27:32.781472 qalita-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1942 2023-07-16 19:27:32.781472 qalita-1.0.7/docs/README.md
+-rw-r--r--   0        0        0     1169 2023-07-16 19:27:43.266548 qalita-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 19:27:32.803495 qalita-1.0.7/qalita/__init__.py
+-rw-r--r--   0        0        0     4189 2023-07-16 19:27:43.267547 qalita-1.0.7/qalita/cli.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:27:32.803495 qalita-1.0.7/qalita/commands/__init__.py
+-rw-r--r--   0        0        0    19666 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/commands/agent.py
+-rw-r--r--   0        0        0    14531 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/commands/pack.py
+-rw-r--r--   0        0        0     9756 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/commands/source.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:27:32.803495 qalita-1.0.7/qalita/internal/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/internal/logger.py
+-rw-r--r--   0        0        0     2486 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/internal/utils.py
+-rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 qalita-1.0.7/PKG-INFO
```

### Comparing `qalita-1.0.6/LICENSE` & `qalita-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `qalita-1.0.6/docs/README.md` & `qalita-1.0.7/docs/README.md`

 * *Files identical despite different names*

### Comparing `qalita-1.0.6/pyproject.toml` & `qalita-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qalita"
-version = "1.0.6"
+version = "1.0.7"
 description = "Qalita Command Line Interface"
 authors = ["Armand LEOPOLD <armand.leopold@qalita.io>"]
 readme = "docs/README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `qalita-1.0.6/qalita/cli.py` & `qalita-1.0.7/qalita/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
 @cli.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @pass_config
 def version(config):
     """
     Display the version of the cli
     """
     logger.info("------------- QALITA CLI Version -------------")
-    logger.info(f"Version : 1.0.6")
+    logger.info(f"Version : 1.0.7")
 
 from qalita.commands import agent, source, pack
 
 # Add pack command group to cli
 cli.add_command(pack.pack)
 cli.add_command(agent.agent)
 cli.add_command(source.source)
```

### Comparing `qalita-1.0.6/qalita/commands/agent.py` & `qalita-1.0.7/qalita/commands/agent.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.6/qalita/commands/pack.py` & `qalita-1.0.7/qalita/commands/pack.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.6/qalita/commands/source.py` & `qalita-1.0.7/qalita/commands/source.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.6/qalita/internal/logger.py` & `qalita-1.0.7/qalita/internal/logger.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.6/qalita/internal/utils.py` & `qalita-1.0.7/qalita/internal/utils.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.6/PKG-INFO` & `qalita-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qalita
-Version: 1.0.6
+Version: 1.0.7
 Summary: Qalita Command Line Interface
 Author: Armand LEOPOLD
 Author-email: armand.leopold@qalita.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

