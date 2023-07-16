# Comparing `tmp/devpm-1.0.0.tar.gz` & `tmp/devpm-1.0.1.tar.gz`

## Comparing `devpm-1.0.0.tar` & `devpm-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 devpm-1.0.0/devpackage.schema.json
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/__init__.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/__main__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/cli/base_command.py
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/cli/main.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/commands/__init__.py
--rw-r--r--   0        0        0     3470 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/commands/install.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/bash.py
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/code.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/context.py
--rw-r--r--   0        0        0     8503 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/git.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/log.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 devpm-1.0.0/devpm/_internal/utils/pip.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.0.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.0.0/LICENSE
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 devpm-1.0.0/README.md
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 devpm-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 devpm-1.0.1/devpackage.schema.json
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/__init__.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/__main__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/cli/base_command.py
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/cli/main.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/commands/__init__.py
+-rw-r--r--   0        0        0     3488 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/commands/install.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/bash.py
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/code.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/context.py
+-rw-r--r--   0        0        0     8814 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/git.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/log.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 devpm-1.0.1/devpm/_internal/utils/pip.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 devpm-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 devpm-1.0.1/LICENSE
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 devpm-1.0.1/README.md
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 devpm-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 devpm-1.0.1/PKG-INFO
```

### Comparing `devpm-1.0.0/devpackage.schema.json` & `devpm-1.0.1/devpackage.schema.json`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/devpm/__main__.py` & `devpm-1.0.1/devpm/__main__.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/devpm/_internal/cli/main.py` & `devpm-1.0.1/devpm/_internal/cli/main.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/devpm/_internal/commands/__init__.py` & `devpm-1.0.1/devpm/_internal/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/devpm/_internal/commands/install.py` & `devpm-1.0.1/devpm/_internal/commands/install.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         cwd = os.getcwd()
         config_file = os.path.join(cwd, 'devpackage.json')
         if not os.path.exists(config_file):
             sys.stdout.write('devpackage.json no found.')
             sys.exit(1)
         sys.stdout.write('Install from %s\n' % config_file)
         config = {}
-        with open(config_file, 'r') as f:
+        with open(config_file, 'r', encoding='utf-8') as f:
             config = json.load(f)
         
         context = Context()
         context.init()
 
         vscode_dependencies = config['vscodeDependencies']
         python_dependencies = config['pythonDependencies']
```

### Comparing `devpm-1.0.0/devpm/_internal/utils/bash.py` & `devpm-1.0.1/devpm/_internal/utils/bash.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/devpm/_internal/utils/code.py` & `devpm-1.0.1/devpm/_internal/utils/code.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/devpm/_internal/utils/context.py` & `devpm-1.0.1/devpm/_internal/utils/context.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/devpm/_internal/utils/log.py` & `devpm-1.0.1/devpm/_internal/utils/log.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/devpm/_internal/utils/pip.py` & `devpm-1.0.1/devpm/_internal/utils/pip.py`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/.gitignore` & `devpm-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/LICENSE` & `devpm-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `devpm-1.0.0/pyproject.toml` & `devpm-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 sources = ["src"]
 directory = "devpm"
 include = ["**/*.py", "devpackage.schema.json"]
 
 [project]
 name = "devpm"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Galen Lin", email="oolgloo.2012@gmail.com" },
 ]
 description = "Development package manager"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `devpm-1.0.0/PKG-INFO` & `devpm-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devpm
-Version: 1.0.0
+Version: 1.0.1
 Summary: Development package manager
 Project-URL: Homepage, https://github.com/wequick/devpm
 Project-URL: Bug Tracker, https://github.com/wequick/devpm/issues
 Author-email: Galen Lin <oolgloo.2012@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

