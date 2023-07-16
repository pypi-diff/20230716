# Comparing `tmp/ipynbcompress-0.4.0.tar.gz` & `tmp/ipynbcompress-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipynbcompress-0.4.0.tar", last modified: Wed Apr 12 19:37:31 2023, max compression
+gzip compressed data, was "ipynbcompress-0.5.0.tar", last modified: Sun Jul 16 10:15:45 2023, max compression
```

## Comparing `ipynbcompress-0.4.0.tar` & `ipynbcompress-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,41 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.960601 ipynbcompress-0.4.0/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.520131 ipynbcompress-0.4.0/.devcontainer/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      977 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/.devcontainer/devcontainer.json
--rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)      126 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/.travis.yml
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1079 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1342 2023-04-12 19:37:28.000000 ipynbcompress-0.4.0/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3302 2023-04-12 19:37:31.961870 ipynbcompress-0.4.0/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2467 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2742 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/README.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.557229 ipynbcompress-0.4.0/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6778 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)     8193 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      148 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      132 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/ipynbcompress.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6467 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       76 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/docs/modules.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       44 2023-04-12 19:17:47.000000 ipynbcompress-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.572091 ipynbcompress-0.4.0/ipynbcompress/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/ipynbcompress/VERSION
--rw-r--r--   0 vscode    (1000) vscode    (1000)      230 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/ipynbcompress/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2564 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/ipynbcompress/ipynbcompress.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.609470 ipynbcompress-0.4.0/ipynbcompress.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3302 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      632 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-04-12 19:33:23.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       49 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2023-04-12 19:37:31.000000 ipynbcompress-0.4.0/ipynbcompress.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      101 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/requirements.txt
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.614672 ipynbcompress-0.4.0/scripts/
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     2186 2023-04-12 18:45:14.000000 ipynbcompress-0.4.0/scripts/ipynb-compress
--rw-r--r--   0 vscode    (1000) vscode    (1000)       61 2023-04-12 19:37:31.965649 ipynbcompress-0.4.0/setup.cfg
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     1292 2023-04-12 19:34:36.000000 ipynbcompress-0.4.0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-04-12 19:37:31.957727 ipynbcompress-0.4.0/test/
--rw-r--r--   0 vscode    (1000) vscode    (1000)   977054 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/test/notebook3.ipynb
--rwxr-xr-x   0 vscode    (1000) vscode    (1000) 11563736 2021-02-10 18:01:48.000000 ipynbcompress-0.4.0/test/notebook4.ipynb
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)      948 2023-04-12 19:26:49.000000 ipynbcompress-0.4.0/test/test_compress.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:45.105470 ipynbcompress-0.5.0/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:44.690527 ipynbcompress-0.5.0/.devcontainer/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      977 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:44.631317 ipynbcompress-0.5.0/.github/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:44.697298 ipynbcompress-0.5.0/.github/workflows/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      586 2023-07-16 10:08:27.000000 ipynbcompress-0.5.0/.github/workflows/main.yml
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      410 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1079 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1346 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3322 2023-07-16 10:15:45.106093 ipynbcompress-0.5.0/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2479 2023-07-16 10:12:49.000000 ipynbcompress-0.5.0/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2762 2023-07-16 10:15:44.000000 ipynbcompress-0.5.0/README.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:08:27.000000 ipynbcompress-0.5.0/TODO.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:44.730703 ipynbcompress-0.5.0/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6778 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8193 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      148 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      132 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/docs/ipynbcompress.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6467 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       76 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/docs/modules.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       44 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:44.744819 ipynbcompress-0.5.0/ipynbcompress/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        6 2023-07-16 10:14:12.000000 ipynbcompress-0.5.0/ipynbcompress/VERSION
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      230 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/ipynbcompress/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2564 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/ipynbcompress/ipynbcompress.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:44.775663 ipynbcompress-0.5.0/ipynbcompress.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3322 2023-07-16 10:15:44.000000 ipynbcompress-0.5.0/ipynbcompress.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      655 2023-07-16 10:15:44.000000 ipynbcompress-0.5.0/ipynbcompress.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-16 10:15:44.000000 ipynbcompress-0.5.0/ipynbcompress.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-16 10:15:44.000000 ipynbcompress-0.5.0/ipynbcompress.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       47 2023-07-16 10:15:44.000000 ipynbcompress-0.5.0/ipynbcompress.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       14 2023-07-16 10:15:44.000000 ipynbcompress-0.5.0/ipynbcompress.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      107 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/requirements.txt
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:44.784854 ipynbcompress-0.5.0/scripts/
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     2372 2023-07-16 10:08:27.000000 ipynbcompress-0.5.0/scripts/ipynb-compress
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       61 2023-07-16 10:15:45.108067 ipynbcompress-0.5.0/setup.cfg
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     1290 2023-07-16 10:08:27.000000 ipynbcompress-0.5.0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-16 10:15:45.102886 ipynbcompress-0.5.0/test/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)   977054 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/test/notebook3.ipynb
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000) 11563736 2023-07-16 10:06:51.000000 ipynbcompress-0.5.0/test/notebook4.ipynb
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)      948 2023-07-16 09:56:07.000000 ipynbcompress-0.5.0/test/test_compress.py
```

### Comparing `ipynbcompress-0.4.0/.devcontainer/devcontainer.json` & `ipynbcompress-0.5.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.4.0/LICENSE` & `ipynbcompress-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.4.0/Makefile` & `ipynbcompress-0.5.0/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
 docs:
 	$(MAKE) -C docs clean
 	$(MAKE) -C docs html
 	open docs/_build/html/index.html
 
 release: clean rst tag
-	python setup.py sdist
-	python setup.py bdist_wheel
+	python setup.py sdist bdist_wheel
+	twine upload dist/*
 	git push && git push --tags
 
 tag:
 	git tag v`cat ipynbcompress/VERSION` || true
 
 rst:
 	pandoc --from=markdown --to=rst README.md -o README.rst
```

### Comparing `ipynbcompress-0.4.0/PKG-INFO` & `ipynbcompress-0.5.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipynbcompress
-Version: 0.4.0
+Version: 0.5.0
 Summary: Compress images in IPython/Jupyter notebooks
 Home-page: https://github.com/arve0/ipynbcompress
 Author: Arve Seljebu
 Author-email: arve.seljebu@gmail.com
 License: MIT
 Keywords: ipynbcompress
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -109,13 +109,13 @@
 To build the documentation:
 
 .. code:: bash
 
    pip install -r docs/requirements.txt
    make docs
 
-.. |build-status-image| image:: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
-   :target: http://travis-ci.org/arve0/ipynbcompress?branch=master
+.. |build-status-image| image:: https://github.com/arve0/ipynbcompress/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/arve0/ipynbcompress/actions/workflows/main.yml
 .. |pypi-version| image:: https://img.shields.io/pypi/v/ipynbcompress.svg
    :target: https://pypi.python.org/pypi/ipynbcompress
 .. |wheel| image:: https://img.shields.io/pypi/wheel/ipynbcompress.svg
    :target: https://pypi.python.org/pypi/ipynbcompress
```

### Comparing `ipynbcompress-0.4.0/README.md` & `ipynbcompress-0.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ipynbcompress
 
-[![build-status-image]][travis]
+[![build-status-image]][ci]
 [![pypi-version]][pypi]
 [![wheel]][pypi]
 
 ## Overview
 
 So you have included an image with `IPython.display.Image()` and the file size
 of your IPython Notebook got huge? No problem! This package will resize images
@@ -78,12 +78,12 @@
 ```bash
 pip install -r docs/requirements.txt
 make docs
 ```
 
 
 
-[build-status-image]: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
-[travis]: http://travis-ci.org/arve0/ipynbcompress?branch=master
+[build-status-image]: https://github.com/arve0/ipynbcompress/actions/workflows/main.yml/badge.svg
+[ci]: https://github.com/arve0/ipynbcompress/actions/workflows/main.yml
 [pypi-version]: https://img.shields.io/pypi/v/ipynbcompress.svg
 [pypi]: https://pypi.python.org/pypi/ipynbcompress
 [wheel]: https://img.shields.io/pypi/wheel/ipynbcompress.svg
```

### Comparing `ipynbcompress-0.4.0/README.rst` & `ipynbcompress-0.5.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -92,13 +92,13 @@
 To build the documentation:
 
 .. code:: bash
 
    pip install -r docs/requirements.txt
    make docs
 
-.. |build-status-image| image:: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
-   :target: http://travis-ci.org/arve0/ipynbcompress?branch=master
+.. |build-status-image| image:: https://github.com/arve0/ipynbcompress/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/arve0/ipynbcompress/actions/workflows/main.yml
 .. |pypi-version| image:: https://img.shields.io/pypi/v/ipynbcompress.svg
    :target: https://pypi.python.org/pypi/ipynbcompress
 .. |wheel| image:: https://img.shields.io/pypi/wheel/ipynbcompress.svg
    :target: https://pypi.python.org/pypi/ipynbcompress
```

### Comparing `ipynbcompress-0.4.0/docs/Makefile` & `ipynbcompress-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.4.0/docs/conf.py` & `ipynbcompress-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.4.0/docs/make.bat` & `ipynbcompress-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.4.0/ipynbcompress/ipynbcompress.py` & `ipynbcompress-0.5.0/ipynbcompress/ipynbcompress.py`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.4.0/ipynbcompress.egg-info/PKG-INFO` & `ipynbcompress-0.5.0/ipynbcompress.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipynbcompress
-Version: 0.4.0
+Version: 0.5.0
 Summary: Compress images in IPython/Jupyter notebooks
 Home-page: https://github.com/arve0/ipynbcompress
 Author: Arve Seljebu
 Author-email: arve.seljebu@gmail.com
 License: MIT
 Keywords: ipynbcompress
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -109,13 +109,13 @@
 To build the documentation:
 
 .. code:: bash
 
    pip install -r docs/requirements.txt
    make docs
 
-.. |build-status-image| image:: https://secure.travis-ci.org/arve0/ipynbcompress.png?branch=master
-   :target: http://travis-ci.org/arve0/ipynbcompress?branch=master
+.. |build-status-image| image:: https://github.com/arve0/ipynbcompress/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/arve0/ipynbcompress/actions/workflows/main.yml
 .. |pypi-version| image:: https://img.shields.io/pypi/v/ipynbcompress.svg
    :target: https://pypi.python.org/pypi/ipynbcompress
 .. |wheel| image:: https://img.shields.io/pypi/wheel/ipynbcompress.svg
    :target: https://pypi.python.org/pypi/ipynbcompress
```

### Comparing `ipynbcompress-0.4.0/ipynbcompress.egg-info/SOURCES.txt` & `ipynbcompress-0.5.0/ipynbcompress.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 .gitignore
-.travis.yml
 LICENSE
 Makefile
 README.md
 README.rst
+TODO.md
 requirements.txt
 setup.cfg
 setup.py
 .devcontainer/devcontainer.json
+.github/workflows/main.yml
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/ipynbcompress.rst
 docs/make.bat
 docs/modules.rst
 docs/requirements.txt
```

### Comparing `ipynbcompress-0.4.0/setup.py` & `ipynbcompress-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         'scripts/ipynb-compress'
     ],
     include_package_data=True,
     install_requires=[
         'Pillow',
         'jsonschema',
         'ipython',
-        'climate',
+        'click',
         'hurry.filesize'
     ],
     license='MIT',
     zip_safe=False,
     keywords='ipynbcompress',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
```

### Comparing `ipynbcompress-0.4.0/test/notebook3.ipynb` & `ipynbcompress-0.5.0/test/notebook3.ipynb`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.4.0/test/notebook4.ipynb` & `ipynbcompress-0.5.0/test/notebook4.ipynb`

 * *Files identical despite different names*

### Comparing `ipynbcompress-0.4.0/test/test_compress.py` & `ipynbcompress-0.5.0/test/test_compress.py`

 * *Files identical despite different names*

