# Comparing `tmp/dav_tools-0.0.9.tar.gz` & `tmp/dav_tools-0.1.0.tar.gz`

## Comparing `dav_tools-0.0.9.tar` & `dav_tools-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,21 @@
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 dav_tools-0.0.9/Makefile
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 dav_tools-0.0.9/src/dav_tools/__init__.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 dav_tools-0.0.9/src/dav_tools/_arg_parser.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dav_tools-0.0.9/src/dav_tools/_text_format.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 dav_tools-0.0.9/src/dav_tools/commands.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dav_tools-0.0.9/src/dav_tools/devtools.py
--rw-r--r--   0        0        0     5195 2020-02-02 00:00:00.000000 dav_tools-0.0.9/src/dav_tools/messages.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 dav_tools-0.0.9/src/dav_tools/requirements.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 dav_tools-0.0.9/src/dav_tools/text_color.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 dav_tools-0.0.9/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.0.9/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dav_tools-0.0.9/README.md
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 dav_tools-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 dav_tools-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 dav_tools-0.1.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 dav_tools-0.1.0/Makefile
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.0/requirements.txt
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/Makefile
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/conf.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/make.bat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 dav_tools-0.1.0/docs/requirements.txt
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/__init__.py
+-rw-r--r--   0        0        0     5415 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/_arg_parser.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/_text_format.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/commands.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/devtools.py
+-rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/messages.py
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/requirements.py
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 dav_tools-0.1.0/src/dav_tools/text_color.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dav_tools-0.1.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 dav_tools-0.1.0/LICENSE
+-rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 dav_tools-0.1.0/README.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 dav_tools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 dav_tools-0.1.0/PKG-INFO
```

### Comparing `dav_tools-0.0.9/Makefile` & `dav_tools-0.1.0/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 NAME=dav-tools
+PY=python3
 
 
 install: uninstall build
-	sudo python3 -m pip install ./dist/*.whl
+	sudo $(PY) -m pip install ./dist/*.whl
 
 build:
-	python3 -m pip install pipreqs
+	$(PY) -m pip install pipreqs
 	pipreqs --force
-	sudo python3 -m pip install --upgrade -r requirements.txt
+	sudo $(PY) -m pip install --upgrade -r requirements.txt
 	sudo rm -rf dist/
-	python3 -m pip install build
-	python3 -m build
+	$(PY) -m pip install build
+	$(PY) -m build
 
 uninstall:
-	sudo python3 -m pip uninstall -y $(NAME)
+	sudo $(PY) -m pip uninstall -y $(NAME)
+
+### Documentation ###
+documentation:
+	$(PY) -m pip install autoapi
+	make html -C docs/
 
 
 ### PyPi ###
-upload: build
-	python3 -m pip install --upgrade twine
-	python3 -m twine upload --verbose dist/*
+upload: build documentation
+	$(PY) -m pip install --upgrade twine
+	$(PY) -m twine upload --verbose dist/*
 
 download: uninstall
-	sudo python3 -m pip install $(NAME)
+	sudo $(PY) -m pip install $(NAME)
 
 
 ### TestPyPi ###
 download-test: uninstall
-	python3 -m pip install --index-url https://test.pypi.org/simple/ --no-deps $(NAME)
+	$(PY) -m pip install --index-url https://test.pypi.org/simple/ --no-deps $(NAME)
 
 upload-test: build
-	python3 -m pip install --upgrade twine
-	python3 -m twine upload --repository testpypi dist/*
+	$(PY) -m pip install --upgrade twine
+	$(PY) -m twine upload --repository testpypi dist/*
```

### Comparing `dav_tools-0.0.9/src/dav_tools/_text_format.py` & `dav_tools-0.1.0/src/dav_tools/_text_format.py`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.9/src/dav_tools/commands.py` & `dav_tools-0.1.0/src/dav_tools/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 def execute(command: str) -> bool:
     exit_status = _subprocess.check_call(_split(command))
     return exit_status == 0
 
 # runs a command, depeding on the current OS
 #   the output is returned in the specified type (default: bytes)
 #   if a command returns a non-zero exit code the program raises an exception (default behavior) or returns a given value (by default: None)
-def get_output(command: str, return_type = bytes, on_error = None):
+def get_output(command: str, on_success = lambda x: x, on_error = None):
     try:
-        return return_type(_subprocess.check_output(_split(command)))
+        return on_success(_subprocess.check_output(_split(command)))
     except CalledProcessError as e:
         if on_error is None:
             raise e
-        return return_type(on_error())
+        return on_success(on_error())
```

### Comparing `dav_tools-0.0.9/LICENSE` & `dav_tools-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dav_tools-0.0.9/pyproject.toml` & `dav_tools-0.1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dav_tools"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="Davide Ponzini", email="davide.ponzini95@gmail.com" },
 ]
-description = "Various utilies to aid in program development"
+description = "Various utilies to aid in program development."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
 ]
 dependencies = [
+  "argparse",
   "elevate",
-  "argparse"
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/DavidePonzini/dav-utils"
+"Repository" = "https://github.com/DavidePonzini/dav-utils"
+"Documentation" = "https://dav-tools.readthedocs.io/en/latest/index.html"
 "Bug Tracker" = "https://github.com/DavidePonzini/dav-utils/issues"
```

