# Comparing `tmp/qalita-1.0.7.tar.gz` & `tmp/qalita-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qalita-1.0.7.tar", max compression
+gzip compressed data, was "qalita-1.0.8.tar", max compression
```

## Comparing `qalita-1.0.7.tar` & `qalita-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    19753 2023-07-16 19:27:32.781472 qalita-1.0.7/LICENSE
--rw-r--r--   0        0        0     1942 2023-07-16 19:27:32.781472 qalita-1.0.7/docs/README.md
--rw-r--r--   0        0        0     1169 2023-07-16 19:27:43.266548 qalita-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 19:27:32.803495 qalita-1.0.7/qalita/__init__.py
--rw-r--r--   0        0        0     4189 2023-07-16 19:27:43.267547 qalita-1.0.7/qalita/cli.py
--rw-r--r--   0        0        0        0 2023-07-16 19:27:32.803495 qalita-1.0.7/qalita/commands/__init__.py
--rw-r--r--   0        0        0    19666 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/commands/agent.py
--rw-r--r--   0        0        0    14531 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/commands/pack.py
--rw-r--r--   0        0        0     9756 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/commands/source.py
--rw-r--r--   0        0        0        0 2023-07-16 19:27:32.803495 qalita-1.0.7/qalita/internal/__init__.py
--rw-r--r--   0        0        0     1992 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/internal/logger.py
--rw-r--r--   0        0        0     2486 2023-07-16 19:27:32.782473 qalita-1.0.7/qalita/internal/utils.py
--rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 qalita-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    19753 2023-07-16 19:42:01.762683 qalita-1.0.8/LICENSE
+-rw-r--r--   0        0        0     1942 2023-07-16 19:42:01.762683 qalita-1.0.8/docs/README.md
+-rw-r--r--   0        0        0     1169 2023-07-16 19:42:12.015592 qalita-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-16 19:42:01.783683 qalita-1.0.8/qalita/__init__.py
+-rw-r--r--   0        0        0     4189 2023-07-16 19:42:12.016592 qalita-1.0.8/qalita/cli.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:42:01.784683 qalita-1.0.8/qalita/commands/__init__.py
+-rw-r--r--   0        0        0    19666 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/commands/agent.py
+-rw-r--r--   0        0        0    14531 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/commands/pack.py
+-rw-r--r--   0        0        0     9756 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/commands/source.py
+-rw-r--r--   0        0        0        0 2023-07-16 19:42:01.784683 qalita-1.0.8/qalita/internal/__init__.py
+-rw-r--r--   0        0        0     1992 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/internal/logger.py
+-rw-r--r--   0        0        0     2486 2023-07-16 19:42:01.763683 qalita-1.0.8/qalita/internal/utils.py
+-rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 qalita-1.0.8/PKG-INFO
```

### Comparing `qalita-1.0.7/LICENSE` & `qalita-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qalita-1.0.7/docs/README.md` & `qalita-1.0.8/docs/README.md`

 * *Files identical despite different names*

### Comparing `qalita-1.0.7/pyproject.toml` & `qalita-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qalita"
-version = "1.0.7"
+version = "1.0.8"
 description = "Qalita Command Line Interface"
 authors = ["Armand LEOPOLD <armand.leopold@qalita.io>"]
 readme = "docs/README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `qalita-1.0.7/qalita/cli.py` & `qalita-1.0.8/qalita/cli.py`

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
-    logger.info(f"Version : 1.0.7")
+    logger.info(f"Version : 1.0.8")
 
 from qalita.commands import agent, source, pack
 
 # Add pack command group to cli
 cli.add_command(pack.pack)
 cli.add_command(agent.agent)
 cli.add_command(source.source)
```

### Comparing `qalita-1.0.7/qalita/commands/agent.py` & `qalita-1.0.8/qalita/commands/agent.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.7/qalita/commands/pack.py` & `qalita-1.0.8/qalita/commands/pack.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.7/qalita/commands/source.py` & `qalita-1.0.8/qalita/commands/source.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.7/qalita/internal/logger.py` & `qalita-1.0.8/qalita/internal/logger.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.7/qalita/internal/utils.py` & `qalita-1.0.8/qalita/internal/utils.py`

 * *Files identical despite different names*

### Comparing `qalita-1.0.7/PKG-INFO` & `qalita-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qalita
-Version: 1.0.7
+Version: 1.0.8
 Summary: Qalita Command Line Interface
 Author: Armand LEOPOLD
 Author-email: armand.leopold@qalita.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

