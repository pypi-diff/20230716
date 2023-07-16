# Comparing `tmp/pdfly-0.2.8.tar.gz` & `tmp/pdfly-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfly-0.2.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pdfly-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pdfly-0.2.8.tar` & `pdfly-0.2.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1111 2023-07-16 07:31:55.531202 pdfly-0.2.8/.github/workflows/github-ci.yaml
--rw-r--r--   0        0        0     1869 2023-07-16 07:31:55.531202 pdfly-0.2.8/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1813 2023-07-16 07:31:55.531202 pdfly-0.2.8/.gitignore
--rw-r--r--   0        0        0      168 2023-07-16 07:31:55.531202 pdfly-0.2.8/.isort.cfg
--rw-r--r--   0        0        0     1318 2023-07-16 07:31:55.531202 pdfly-0.2.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1514 2023-07-16 07:31:55.531202 pdfly-0.2.8/LICENSE
--rw-r--r--   0        0        0      635 2023-07-16 07:31:55.531202 pdfly-0.2.8/Makefile
--rw-r--r--   0        0        0     3938 2023-07-16 07:31:55.531202 pdfly-0.2.8/README.md
--rw-r--r--   0        0        0       31 2023-07-16 07:31:55.531202 pdfly-0.2.8/mypy.ini
--rw-r--r--   0        0        0      164 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/__init__.py
--rw-r--r--   0        0        0      114 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/__main__.py
--rw-r--r--   0        0        0       87 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/_utils.py
--rw-r--r--   0        0        0       22 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/_version.py
--rw-r--r--   0        0        0     2765 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/cat.py
--rw-r--r--   0        0        0     4409 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/cli.py
--rw-r--r--   0        0        0      594 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/compress.py
--rw-r--r--   0        0        0      846 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/extract_images.py
--rw-r--r--   0        0        0     6276 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/metadata.py
--rw-r--r--   0        0        0     2384 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/pagemeta.py
--rw-r--r--   0        0        0      724 2023-07-16 07:31:55.531202 pdfly-0.2.8/pdfly/up2.py
--rw-r--r--   0        0        0     5053 2023-07-16 07:31:55.531202 pdfly-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       84 2023-07-16 07:31:55.531202 pdfly-0.2.8/requirements/ci.in
--rw-r--r--   0        0        0     1392 2023-07-16 07:31:55.531202 pdfly-0.2.8/requirements/ci.txt
--rw-r--r--   0        0        0       50 2023-07-16 07:31:55.531202 pdfly-0.2.8/requirements/dev.in
--rw-r--r--   0        0        0     2440 2023-07-16 07:31:55.531202 pdfly-0.2.8/requirements/dev.txt
--rw-r--r--   0        0        0      519 2023-07-16 07:31:55.531202 pdfly-0.2.8/setup.cfg
--rw-r--r--   0        0        0      463 2023-07-16 07:31:55.531202 pdfly-0.2.8/setup.py
--rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 pdfly-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-07-16 07:36:09.574079 pdfly-0.2.9/.github/workflows/github-ci.yaml
+-rw-r--r--   0        0        0     1871 2023-07-16 07:36:09.574079 pdfly-0.2.9/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1813 2023-07-16 07:36:09.574079 pdfly-0.2.9/.gitignore
+-rw-r--r--   0        0        0      168 2023-07-16 07:36:09.574079 pdfly-0.2.9/.isort.cfg
+-rw-r--r--   0        0        0     1318 2023-07-16 07:36:09.574079 pdfly-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1514 2023-07-16 07:36:09.574079 pdfly-0.2.9/LICENSE
+-rw-r--r--   0        0        0      635 2023-07-16 07:36:09.574079 pdfly-0.2.9/Makefile
+-rw-r--r--   0        0        0     3938 2023-07-16 07:36:09.574079 pdfly-0.2.9/README.md
+-rw-r--r--   0        0        0       31 2023-07-16 07:36:09.574079 pdfly-0.2.9/mypy.ini
+-rw-r--r--   0        0        0      164 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/__main__.py
+-rw-r--r--   0        0        0       87 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/_utils.py
+-rw-r--r--   0        0        0       22 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/_version.py
+-rw-r--r--   0        0        0     2765 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/cat.py
+-rw-r--r--   0        0        0     4409 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/cli.py
+-rw-r--r--   0        0        0      594 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/compress.py
+-rw-r--r--   0        0        0      846 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/extract_images.py
+-rw-r--r--   0        0        0     6276 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/metadata.py
+-rw-r--r--   0        0        0     2384 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/pagemeta.py
+-rw-r--r--   0        0        0      724 2023-07-16 07:36:09.574079 pdfly-0.2.9/pdfly/up2.py
+-rw-r--r--   0        0        0     5053 2023-07-16 07:36:09.574079 pdfly-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-07-16 07:36:09.574079 pdfly-0.2.9/requirements/ci.in
+-rw-r--r--   0        0        0     1392 2023-07-16 07:36:09.574079 pdfly-0.2.9/requirements/ci.txt
+-rw-r--r--   0        0        0       50 2023-07-16 07:36:09.574079 pdfly-0.2.9/requirements/dev.in
+-rw-r--r--   0        0        0     2440 2023-07-16 07:36:09.574079 pdfly-0.2.9/requirements/dev.txt
+-rw-r--r--   0        0        0      519 2023-07-16 07:36:09.574079 pdfly-0.2.9/setup.cfg
+-rw-r--r--   0        0        0      463 2023-07-16 07:36:09.574079 pdfly-0.2.9/setup.py
+-rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 pdfly-0.2.9/PKG-INFO
```

### Comparing `pdfly-0.2.8/.github/workflows/github-ci.yaml` & `pdfly-0.2.9/.github/workflows/github-ci.yaml`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/.github/workflows/release.yaml` & `pdfly-0.2.9/.github/workflows/release.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
       # Create the Github Page
       - name: Prepare variables
         id: prepare_variables
         run: |
           git fetch --tags --force
           echo "::set-output name=latest_tag::$(git describe --tags --abbrev=0)"
-          echo "::set-output name=tag_body::$(git tag -l "${latest_tag}" --format='%(contents:body)')"
+          echo "::set-output name=tag_body::$(git tag -l \"${latest_tag}\" --format='%(contents:body)')"
           echo "::set-output name=date::$(date +'%Y-%m-%d')"
       - name: Create GitHub Release 🚀
         uses: softprops/action-gh-release@v1
         with:
           tag_name: ${{ github.ref }}
           name: Version ${{ steps.prepare_variables.outputs.latest_tag }}, ${{ steps.prepare_variables.outputs.date }}
           draft: false
```

### Comparing `pdfly-0.2.8/.gitignore` & `pdfly-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/.pre-commit-config.yaml` & `pdfly-0.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/LICENSE` & `pdfly-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/Makefile` & `pdfly-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/README.md` & `pdfly-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/pdfly/cat.py` & `pdfly-0.2.9/pdfly/cat.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/pdfly/cli.py` & `pdfly-0.2.9/pdfly/cli.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/pdfly/compress.py` & `pdfly-0.2.9/pdfly/compress.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/pdfly/extract_images.py` & `pdfly-0.2.9/pdfly/extract_images.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/pdfly/metadata.py` & `pdfly-0.2.9/pdfly/metadata.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/pdfly/pagemeta.py` & `pdfly-0.2.9/pdfly/pagemeta.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/pdfly/up2.py` & `pdfly-0.2.9/pdfly/up2.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/pyproject.toml` & `pdfly-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/requirements/ci.txt` & `pdfly-0.2.9/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/requirements/dev.txt` & `pdfly-0.2.9/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/setup.cfg` & `pdfly-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.8/PKG-INFO` & `pdfly-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfly
-Version: 0.2.8
+Version: 0.2.9
 Summary: A pure-python CLI application to manipulate PDF files
 Author-email: Martin Thoma <info@martin-thoma.de>
 Maintainer-email: Martin Thoma <info@martin-thoma.de>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

