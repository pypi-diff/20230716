# Comparing `tmp/polyviz-1.0.0.tar.gz` & `tmp/polyviz-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyviz-1.0.0.tar", last modified: Tue Jan 24 11:59:40 2023, max compression
+gzip compressed data, was "polyviz-1.0.1.tar", last modified: Sun Jul 16 08:56:32 2023, max compression
```

## Comparing `polyviz-1.0.0.tar` & `polyviz-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:59:40.384240 polyviz-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-01-24 11:59:29.000000 polyviz-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-24 11:59:29.000000 polyviz-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-01-24 11:59:40.384240 polyviz-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-01-24 11:59:29.000000 polyviz-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:59:40.380240 polyviz-1.0.0/polyviz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:59:40.384240 polyviz-1.0.0/polyviz/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-01-24 11:59:29.000000 polyviz-1.0.0/polyviz/data/GDP_countries.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-01-24 11:59:29.000000 polyviz-1.0.0/polyviz/data/regions.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:59:40.380240 polyviz-1.0.0/polyviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-01-24 11:59:40.000000 polyviz-1.0.0/polyviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-01-24 11:59:40.000000 polyviz-1.0.0/polyviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-24 11:59:40.000000 polyviz-1.0.0/polyviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-24 11:59:40.000000 polyviz-1.0.0/polyviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 11:59:40.000000 polyviz-1.0.0/polyviz.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 11:59:40.384240 polyviz-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-01-24 11:59:29.000000 polyviz-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 08:56:32.176945 polyviz-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-16 08:56:23.000000 polyviz-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-16 08:56:23.000000 polyviz-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-16 08:56:32.176945 polyviz-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-16 08:56:23.000000 polyviz-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 08:56:32.172944 polyviz-1.0.1/polyviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/chord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/choro.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 08:56:32.176945 polyviz-1.0.1/polyviz/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/data/GDP_countries.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/data/regions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7982 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/force.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/sankey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/treemap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-16 08:56:23.000000 polyviz-1.0.1/polyviz/violin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 08:56:32.172944 polyviz-1.0.1/polyviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-07-16 08:56:32.000000 polyviz-1.0.1/polyviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-16 08:56:32.000000 polyviz-1.0.1/polyviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-16 08:56:32.000000 polyviz-1.0.1/polyviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-16 08:56:32.000000 polyviz-1.0.1/polyviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-16 08:56:32.000000 polyviz-1.0.1/polyviz.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 08:56:32.176945 polyviz-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-07-16 08:56:23.000000 polyviz-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 08:56:32.176945 polyviz-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-16 08:56:23.000000 polyviz-1.0.1/tests/test_graphs.py
```

### Comparing `polyviz-1.0.0/LICENSE` & `polyviz-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `polyviz-1.0.0/PKG-INFO` & `polyviz-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyviz
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interface between Brightway2 and D3.js
 Home-page: https://github.com/romainsacchi/polyviz
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Romain Sacchi
         
@@ -84,14 +84,20 @@
 
 Install ``polyviz`` from PyPI:
 
 ```bash
 pip install polyviz
 ```
 
+and you will need to install a forked version of ``d3blocks``:
+
+```bash
+pip install git+https://github.com/romainsacchi/d3blocks.git
+```
+
 Usage
 -----
 
 ### Sankey diagrams
 
 ```python
 from polyviz import sankey
@@ -124,12 +130,12 @@
 
 ## Maintainers
 
 * [Romain Sacchi](https://github.com/romainsacchi)
 
 ## Contributing
 
-See [contributing](https://github.com/romainsacchi/carculator/blob/master/CONTRIBUTING.md).
+See [contributing](https://github.com/romainsacchi/polyviz/blob/master/CONTRIBUTING.md).
 
 ## License
 
 [BSD-3-Clause](https://github.com/romainsacchi/polyviz/blob/master/LICENSE).
```

### Comparing `polyviz-1.0.0/README.md` & `polyviz-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 
 Install ``polyviz`` from PyPI:
 
 ```bash
 pip install polyviz
 ```
 
+and you will need to install a forked version of ``d3blocks``:
+
+```bash
+pip install git+https://github.com/romainsacchi/d3blocks.git
+```
+
 Usage
 -----
 
 ### Sankey diagrams
 
 ```python
 from polyviz import sankey
@@ -70,12 +76,12 @@
 
 ## Maintainers
 
 * [Romain Sacchi](https://github.com/romainsacchi)
 
 ## Contributing
 
-See [contributing](https://github.com/romainsacchi/carculator/blob/master/CONTRIBUTING.md).
+See [contributing](https://github.com/romainsacchi/polyviz/blob/master/CONTRIBUTING.md).
 
 ## License
 
 [BSD-3-Clause](https://github.com/romainsacchi/polyviz/blob/master/LICENSE).
```

### Comparing `polyviz-1.0.0/polyviz/data/GDP_countries.yaml` & `polyviz-1.0.1/polyviz/data/GDP_countries.yaml`

 * *Files identical despite different names*

### Comparing `polyviz-1.0.0/polyviz/data/regions.yaml` & `polyviz-1.0.1/polyviz/data/regions.yaml`

 * *Files identical despite different names*

### Comparing `polyviz-1.0.0/polyviz.egg-info/PKG-INFO` & `polyviz-1.0.1/polyviz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyviz
-Version: 1.0.0
+Version: 1.0.1
 Summary: Interface between Brightway2 and D3.js
 Home-page: https://github.com/romainsacchi/polyviz
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License: BSD 3-Clause License
         
         Copyright (c) 2020, Romain Sacchi
         
@@ -84,14 +84,20 @@
 
 Install ``polyviz`` from PyPI:
 
 ```bash
 pip install polyviz
 ```
 
+and you will need to install a forked version of ``d3blocks``:
+
+```bash
+pip install git+https://github.com/romainsacchi/d3blocks.git
+```
+
 Usage
 -----
 
 ### Sankey diagrams
 
 ```python
 from polyviz import sankey
@@ -124,12 +130,12 @@
 
 ## Maintainers
 
 * [Romain Sacchi](https://github.com/romainsacchi)
 
 ## Contributing
 
-See [contributing](https://github.com/romainsacchi/carculator/blob/master/CONTRIBUTING.md).
+See [contributing](https://github.com/romainsacchi/polyviz/blob/master/CONTRIBUTING.md).
 
 ## License
 
 [BSD-3-Clause](https://github.com/romainsacchi/polyviz/blob/master/LICENSE).
```

### Comparing `polyviz-1.0.0/setup.py` & `polyviz-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,47 +8,47 @@
 if root_dir:
     os.chdir(root_dir)
 
 # read the contents of your README file
 this_directory = Path(__file__).parent
 README = (this_directory / "README.md").read_text()
 
-for dirpath, dirnames, filenames in os.walk("carculator"):
+for dirpath, dirnames, filenames in os.walk("polyviz"):
     # Ignore dirnames that start with '.'
     if "__init__.py" in filenames:
         pkg = dirpath.replace(os.path.sep, ".")
         if os.path.altsep:
             pkg = pkg.replace(os.path.altsep, ".")
         packages.append(pkg)
 
 
 def package_files(directory):
     paths = []
-    for (path, directories, filenames) in os.walk(directory):
+    for path, directories, filenames in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join("..", path, filename))
     return paths
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="polyviz",
-    version="1.0.0",
+    version="1.0.1",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     license=open("LICENSE").read(),
     package_data={"polyviz": package_files(os.path.join("polyviz", "data"))},
     install_requires=[
         "pandas",
-        "numpy<=1.23.1",
-        "bw2io<=0.8.7",
-        "bw2data<=3.6.5",
-        "bw2calc<=1.8.1",
+        "numpy",
+        "bw2io",
+        "bw2data",
+        "bw2calc",
         "country_converter",
         "pyyaml",
     ],
     dependency_links=["https://github.com/romainsacchi/d3blocks"],
     url="https://github.com/romainsacchi/polyviz",
     description="Interface between Brightway2 and D3.js",
     long_description_content_type="text/markdown",
```

