# Comparing `tmp/pytest-localserver-0.7.1rc0.tar.gz` & `tmp/pytest-localserver-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-localserver-0.7.1rc0.tar", last modified: Thu Jan 26 22:02:30 2023, max compression
+gzip compressed data, was "pytest-localserver-0.8.0.tar", last modified: Sun Jul 16 02:12:52 2023, max compression
```

## Comparing `pytest-localserver-0.7.1rc0.tar` & `pytest-localserver-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:02:30.182053 pytest-localserver-0.7.1rc0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:02:30.174053 pytest-localserver-0.7.1rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:02:30.178053 pytest-localserver-0.7.1rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/CHANGES
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-01-26 22:02:30.182053 pytest-localserver-0.7.1rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:02:30.178053 pytest-localserver-0.7.1rc0/pytest_localserver/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/pytest_localserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-01-26 22:02:30.000000 pytest-localserver-0.7.1rc0/pytest_localserver/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/pytest_localserver/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/pytest_localserver/https.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/pytest_localserver/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/pytest_localserver/server.pem
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/pytest_localserver/smtp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:02:30.182053 pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-01-26 22:02:30.000000 pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-01-26 22:02:30.000000 pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 22:02:30.000000 pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-26 22:02:30.000000 pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-26 22:02:29.000000 pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-26 22:02:30.000000 pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-26 22:02:30.000000 pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)   206078 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-26 22:02:30.182053 pytest-localserver-0.7.1rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-26 22:02:30.182053 pytest-localserver-0.7.1rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/tests/test_https.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/tests/test_smtp.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-01-26 22:02:19.000000 pytest-localserver-0.7.1rc0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:12:52.575531 pytest-localserver-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:12:52.571531 pytest-localserver-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:12:52.571531 pytest-localserver-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/CHANGES
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-07-16 02:12:52.575531 pytest-localserver-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:12:52.571531 pytest-localserver-0.8.0/pytest_localserver/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/pytest_localserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-16 02:12:52.000000 pytest-localserver-0.8.0/pytest_localserver/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/pytest_localserver/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/pytest_localserver/https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/pytest_localserver/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/pytest_localserver/server.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/pytest_localserver/smtp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:12:52.575531 pytest-localserver-0.8.0/pytest_localserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11522 2023-07-16 02:12:52.000000 pytest-localserver-0.8.0/pytest_localserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-16 02:12:52.000000 pytest-localserver-0.8.0/pytest_localserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 02:12:52.000000 pytest-localserver-0.8.0/pytest_localserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-16 02:12:52.000000 pytest-localserver-0.8.0/pytest_localserver.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 02:12:52.000000 pytest-localserver-0.8.0/pytest_localserver.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-16 02:12:52.000000 pytest-localserver-0.8.0/pytest_localserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 02:12:52.000000 pytest-localserver-0.8.0/pytest_localserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-16 02:12:52.575531 pytest-localserver-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 02:12:52.575531 pytest-localserver-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/tests/test_https.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/tests/test_smtp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-16 02:12:43.000000 pytest-localserver-0.8.0/tox.ini
```

### Comparing `pytest-localserver-0.7.1rc0/.github/workflows/release.yml` & `pytest-localserver-0.8.0/.github/workflows/release.yml`

 * *Files 23% similar despite different names*

```diff
@@ -25,35 +25,42 @@
       with:
         name: dist
         path: dist/
         if-no-files-found: error
   publish-to-test-pypi:
     name: Publish packages to Test PyPI
     runs-on: ubuntu-latest
-    needs: [build]
+    needs:
+    - build
     environment: test-pypi
+    permissions:
+      # this permission is mandatory for trusted publishing
+      id-token: write
     steps:
     - uses: actions/download-artifact@v3
       with:
         name: dist
         path: dist/
     - name: Publish packages to Test PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        password: '${{ secrets.TEST_PYPI_API_TOKEN }}'
         repository_url: https://test.pypi.org/legacy/
         print_hash: true
   publish-to-pypi:
     name: Publish packages to PyPI
     runs-on: ubuntu-latest
-    needs: [build]
+    needs:
+    - build
+    - publish-to-test-pypi
     environment: pypi
+    permissions:
+      # this permission is mandatory for trusted publishing
+      id-token: write
     steps:
     - uses: actions/download-artifact@v3
       with:
         name: dist
         path: dist/
     - name: Publish packages to PyPI
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
-        password: '${{ secrets.PYPI_API_TOKEN }}'
         print_hash: true
```

### Comparing `pytest-localserver-0.7.1rc0/.github/workflows/tests.yml` & `pytest-localserver-0.8.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/.pre-commit-config.yaml` & `pytest-localserver-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/AUTHORS` & `pytest-localserver-0.8.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/CHANGES` & `pytest-localserver-0.8.0/CHANGES`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+0.8.0 (2023-07-14)
+------------------
+
+Improve deployment workflow to use trusted publishing and upload to Test PyPI first
+Remove a bunch of obsolete code
+Clean up the smtp module's driver code
+
+0.7.1 (2023-01-29)
+------------------
+
+Update SMTP server code to work with aiosmtpd >=1.4.3
+Fix GitHub Actions configuration for Python 3.5 and 3.6
+Add support for Python 3.11 (or at least, list it explicitly in the classifiers)
+Update the AUTHORS file
+Add a workflow to push packages to PyPI using GitHub Actions
+
 0.7.0 (2022-08-30)
 ------------------
 
 Make smtp support an optional extra
 Update some obsolete syntax to drop support for Python 2
 Add linting for code and workflow actions using pre-commit hooks
 Expand the range of pytest versions known to be compatible, with tests
```

### Comparing `pytest-localserver-0.7.1rc0/LICENSE` & `pytest-localserver-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/PKG-INFO` & `pytest-localserver-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-localserver
-Version: 0.7.1rc0
+Version: 0.8.0
 Summary: pytest plugin to test server connections locally.
 Home-page: https://github.com/pytest-dev/pytest-localserver
 Author: Sebastian Rahlf
 Author-email: basti@redtoad.de
 Maintainer: David Zaslavsky
 Maintainer-email: diazona@ellipsix.net
 License: MIT License
```

### Comparing `pytest-localserver-0.7.1rc0/README.rst` & `pytest-localserver-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/pytest_localserver/http.py` & `pytest-localserver-0.8.0/pytest_localserver/http.py`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/pytest_localserver/https.py` & `pytest-localserver-0.8.0/pytest_localserver/https.py`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/pytest_localserver/plugin.py` & `pytest-localserver-0.8.0/pytest_localserver/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-#
 # Copyright (C) 2011 Sebastian Rahlf <basti at redtoad dot de>
 #
 # This program is release under the MIT license. You can find the full text of
 # the license in the LICENSE file.
 import pytest
```

### Comparing `pytest-localserver-0.7.1rc0/pytest_localserver/server.pem` & `pytest-localserver-0.8.0/pytest_localserver/server.pem`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/pytest_localserver/smtp.py` & `pytest-localserver-0.8.0/pytest_localserver/smtp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-#!/usr/bin/env python
-#
 # Copyright (C) 2011 Sebastian Rahlf <basti at redtoad dot de>
 # with some ideas from http://code.activestate.com/recipes/440690/
 # SmtpMailsink Copyright 2005 Aviarc Corporation
 # Written by Adam Feuer, Matt Branthwaite, and Troy Frever
 # which is Licensed under the PSF License
 import email
 
@@ -152,29 +150,28 @@
         if self.is_alive():
             self.stop()
 
     def __repr__(self):  # pragma: no cover
         return "<smtp.Server %s:%s>" % self.addr
 
 
-if __name__ == "__main__":  # pragma: no cover
+def main():
     import time
 
     server = Server()
     server.start()
 
     print("SMTP server is running on %s:%i" % server.addr)
     print("Type <Ctrl-C> to stop")
 
     try:
-
-        try:
-            while True:
-                time.sleep(1)
-        finally:
-            print("\rstopping...")
-            server.stop()
-
+        while True:
+            time.sleep(1)
     except KeyboardInterrupt:
-        # support for Python 2.4 dictates that try ... finally is not used
-        # together with any except statements
         pass
+    finally:
+        print("\rstopping...")
+        server.stop()
+
+
+if __name__ == "__main__":  # pragma: no cover
+    main()
```

### Comparing `pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/PKG-INFO` & `pytest-localserver-0.8.0/pytest_localserver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-localserver
-Version: 0.7.1rc0
+Version: 0.8.0
 Summary: pytest plugin to test server connections locally.
 Home-page: https://github.com/pytest-dev/pytest-localserver
 Author: Sebastian Rahlf
 Author-email: basti@redtoad.de
 Maintainer: David Zaslavsky
 Maintainer-email: diazona@ellipsix.net
 License: MIT License
```

### Comparing `pytest-localserver-0.7.1rc0/pytest_localserver.egg-info/SOURCES.txt` & `pytest-localserver-0.8.0/pytest_localserver.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .pre-commit-config.yaml
 AUTHORS
 CHANGES
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
-runtests.py
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/release.yml
 .github/workflows/tests.yml
 pytest_localserver/__init__.py
 pytest_localserver/_version.py
```

### Comparing `pytest-localserver-0.7.1rc0/setup.py` & `pytest-localserver-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/tests/test_http.py` & `pytest-localserver-0.8.0/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/tests/test_https.py` & `pytest-localserver-0.8.0/tests/test_https.py`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/tests/test_smtp.py` & `pytest-localserver-0.8.0/tests/test_smtp.py`

 * *Files identical despite different names*

### Comparing `pytest-localserver-0.7.1rc0/tox.ini` & `pytest-localserver-0.8.0/tox.ini`

 * *Files identical despite different names*

