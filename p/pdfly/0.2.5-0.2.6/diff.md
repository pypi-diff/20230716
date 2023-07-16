# Comparing `tmp/pdfly-0.2.5.tar.gz` & `tmp/pdfly-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfly-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pdfly-0.2.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pdfly-0.2.5.tar` & `pdfly-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1111 2023-07-16 07:01:14.665259 pdfly-0.2.5/.github/workflows/github-ci.yaml
--rw-r--r--   0        0        0     1728 2023-07-16 07:01:14.665259 pdfly-0.2.5/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1813 2023-07-16 07:01:14.665259 pdfly-0.2.5/.gitignore
--rw-r--r--   0        0        0      168 2023-07-16 07:01:14.665259 pdfly-0.2.5/.isort.cfg
--rw-r--r--   0        0        0     1318 2023-07-16 07:01:14.665259 pdfly-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1514 2023-07-16 07:01:14.669258 pdfly-0.2.5/LICENSE
--rw-r--r--   0        0        0      635 2023-07-16 07:01:14.669258 pdfly-0.2.5/Makefile
--rw-r--r--   0        0        0     3938 2023-07-16 07:01:14.669258 pdfly-0.2.5/README.md
--rw-r--r--   0        0        0       31 2023-07-16 07:01:14.669258 pdfly-0.2.5/mypy.ini
--rw-r--r--   0        0        0      164 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/__init__.py
--rw-r--r--   0        0        0      114 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/__main__.py
--rw-r--r--   0        0        0       87 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/_utils.py
--rw-r--r--   0        0        0       22 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/_version.py
--rw-r--r--   0        0        0     2765 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/cat.py
--rw-r--r--   0        0        0     4409 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/cli.py
--rw-r--r--   0        0        0      594 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/compress.py
--rw-r--r--   0        0        0      846 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/extract_images.py
--rw-r--r--   0        0        0     6276 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/metadata.py
--rw-r--r--   0        0        0     2384 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/pagemeta.py
--rw-r--r--   0        0        0      724 2023-07-16 07:01:14.669258 pdfly-0.2.5/pdfly/up2.py
--rw-r--r--   0        0        0     5053 2023-07-16 07:01:14.669258 pdfly-0.2.5/pyproject.toml
--rw-r--r--   0        0        0       84 2023-07-16 07:01:14.669258 pdfly-0.2.5/requirements/ci.in
--rw-r--r--   0        0        0     1392 2023-07-16 07:01:14.669258 pdfly-0.2.5/requirements/ci.txt
--rw-r--r--   0        0        0       50 2023-07-16 07:01:14.669258 pdfly-0.2.5/requirements/dev.in
--rw-r--r--   0        0        0     2440 2023-07-16 07:01:14.669258 pdfly-0.2.5/requirements/dev.txt
--rw-r--r--   0        0        0      519 2023-07-16 07:01:14.669258 pdfly-0.2.5/setup.cfg
--rw-r--r--   0        0        0      463 2023-07-16 07:01:14.669258 pdfly-0.2.5/setup.py
--rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 pdfly-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-07-16 07:17:10.558133 pdfly-0.2.6/.github/workflows/github-ci.yaml
+-rw-r--r--   0        0        0     1728 2023-07-16 07:17:10.558133 pdfly-0.2.6/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1813 2023-07-16 07:17:10.558133 pdfly-0.2.6/.gitignore
+-rw-r--r--   0        0        0      168 2023-07-16 07:17:10.558133 pdfly-0.2.6/.isort.cfg
+-rw-r--r--   0        0        0     1318 2023-07-16 07:17:10.558133 pdfly-0.2.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1514 2023-07-16 07:17:10.558133 pdfly-0.2.6/LICENSE
+-rw-r--r--   0        0        0      635 2023-07-16 07:17:10.558133 pdfly-0.2.6/Makefile
+-rw-r--r--   0        0        0     3938 2023-07-16 07:17:10.558133 pdfly-0.2.6/README.md
+-rw-r--r--   0        0        0       31 2023-07-16 07:17:10.558133 pdfly-0.2.6/mypy.ini
+-rw-r--r--   0        0        0      164 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/__init__.py
+-rw-r--r--   0        0        0      114 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/__main__.py
+-rw-r--r--   0        0        0       87 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/_utils.py
+-rw-r--r--   0        0        0       22 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/_version.py
+-rw-r--r--   0        0        0     2765 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/cat.py
+-rw-r--r--   0        0        0     4409 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/cli.py
+-rw-r--r--   0        0        0      594 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/compress.py
+-rw-r--r--   0        0        0      846 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/extract_images.py
+-rw-r--r--   0        0        0     6276 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/metadata.py
+-rw-r--r--   0        0        0     2384 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/pagemeta.py
+-rw-r--r--   0        0        0      724 2023-07-16 07:17:10.558133 pdfly-0.2.6/pdfly/up2.py
+-rw-r--r--   0        0        0     5053 2023-07-16 07:17:10.558133 pdfly-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0       84 2023-07-16 07:17:10.558133 pdfly-0.2.6/requirements/ci.in
+-rw-r--r--   0        0        0     1392 2023-07-16 07:17:10.558133 pdfly-0.2.6/requirements/ci.txt
+-rw-r--r--   0        0        0       50 2023-07-16 07:17:10.558133 pdfly-0.2.6/requirements/dev.in
+-rw-r--r--   0        0        0     2440 2023-07-16 07:17:10.558133 pdfly-0.2.6/requirements/dev.txt
+-rw-r--r--   0        0        0      519 2023-07-16 07:17:10.558133 pdfly-0.2.6/setup.cfg
+-rw-r--r--   0        0        0      463 2023-07-16 07:17:10.558133 pdfly-0.2.6/setup.py
+-rw-r--r--   0        0        0     4965 1970-01-01 00:00:00.000000 pdfly-0.2.6/PKG-INFO
```

### Comparing `pdfly-0.2.5/.github/workflows/github-ci.yaml` & `pdfly-0.2.6/.github/workflows/github-ci.yaml`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/.github/workflows/release.yaml` & `pdfly-0.2.6/.github/workflows/release.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -45,11 +45,11 @@
         run: |
           latest_tag=$(git describe --tags --abbrev=0)
           tag_body=$(git tag -l "${latest_tag}" --format='%(contents:body)')
       - name: Create GitHub Release 🚀
         uses: softprops/action-gh-release@v1
         with:
           tag_name: ${{ github.ref }}
-          release_name: Version ${{ github.ref }}, $(date -u +'%Y-%m-%d')
+          name: Version ${{ github.ref }}, $(date -u +'%Y-%m-%d')
           draft: false
           prerelease: false
-          body: ${{ steps.build_and_publish.outputs.tag_body }}
+          body: Body is ${{ steps.build_and_publish.outputs.tag_body }}
```

### Comparing `pdfly-0.2.5/.gitignore` & `pdfly-0.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/.pre-commit-config.yaml` & `pdfly-0.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/LICENSE` & `pdfly-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/Makefile` & `pdfly-0.2.6/Makefile`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/README.md` & `pdfly-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/pdfly/cat.py` & `pdfly-0.2.6/pdfly/cat.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/pdfly/cli.py` & `pdfly-0.2.6/pdfly/cli.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/pdfly/compress.py` & `pdfly-0.2.6/pdfly/compress.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/pdfly/extract_images.py` & `pdfly-0.2.6/pdfly/extract_images.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/pdfly/metadata.py` & `pdfly-0.2.6/pdfly/metadata.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/pdfly/pagemeta.py` & `pdfly-0.2.6/pdfly/pagemeta.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/pdfly/up2.py` & `pdfly-0.2.6/pdfly/up2.py`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/pyproject.toml` & `pdfly-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/requirements/ci.txt` & `pdfly-0.2.6/requirements/ci.txt`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/requirements/dev.txt` & `pdfly-0.2.6/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/setup.cfg` & `pdfly-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pdfly-0.2.5/PKG-INFO` & `pdfly-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfly
-Version: 0.2.5
+Version: 0.2.6
 Summary: A pure-python CLI application to manipulate PDF files
 Author-email: Martin Thoma <info@martin-thoma.de>
 Maintainer-email: Martin Thoma <info@martin-thoma.de>
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
```

