# Comparing `tmp/bookbot-1.0.dev1.tar.gz` & `tmp/bookbot-1.0.dev2.tar.gz`

## Comparing `bookbot-1.0.dev1.tar` & `bookbot-1.0.dev2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/CHANGELOG.md
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/_dir.md
--rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/_dir.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/contributing.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/donate.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/maintainers.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/quickstart.md
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/lib/Makefile
--rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/lib/make.bat
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/lib/source/conf.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/docs/lib/source/index.rst
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/_dir.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/_dir.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/book/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/book/_dir.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/bot/__init__.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/bot/_dir.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/bot/parse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/bot/parse/_dir.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/bot/request/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/bot/request/_dir.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/cli/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/cli/_dir.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/gui/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/gui/_dir.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/storage/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/src/bookbot/storage/_dir.md
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/LICENSE
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/README.md
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 bookbot-1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/CHANGELOG.md
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/_dir.md
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/_dir.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/contributing.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/donate.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/maintainers.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/quickstart.md
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/lib/Makefile
+-rwxr-xr-x   0        0        0      804 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/lib/make.bat
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/lib/source/conf.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/docs/lib/source/index.rst
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/_dir.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/_dir.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/book/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/book/_dir.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/bot/__init__.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/bot/_dir.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/bot/parse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/bot/parse/_dir.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/bot/request/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/bot/request/_dir.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/cli/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/cli/_dir.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/gui/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/gui/_dir.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/storage/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/src/bookbot/storage/_dir.md
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/LICENSE
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/README.md
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 bookbot-1.0.dev2/PKG-INFO
```

### Comparing `bookbot-1.0.dev1/docs/_dir.md` & `bookbot-1.0.dev2/docs/_dir.md`

 * *Files identical despite different names*

### Comparing `bookbot-1.0.dev1/docs/lib/Makefile` & `bookbot-1.0.dev2/docs/lib/Makefile`

 * *Files identical despite different names*

### Comparing `bookbot-1.0.dev1/docs/lib/make.bat` & `bookbot-1.0.dev2/docs/lib/make.bat`

 * *Files identical despite different names*

### Comparing `bookbot-1.0.dev1/docs/lib/source/conf.py` & `bookbot-1.0.dev2/docs/lib/source/conf.py`

 * *Files identical despite different names*

### Comparing `bookbot-1.0.dev1/.gitignore` & `bookbot-1.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `bookbot-1.0.dev1/LICENSE` & `bookbot-1.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `bookbot-1.0.dev1/pyproject.toml` & `bookbot-1.0.dev2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bookbot"
-version = "1.0.dev1"
+version = "1.0.dev2"
 description = ""
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text = "GPLv3+"}
 authors = [
   {name="Heng Zhou", email="hl-bo@outlook.com" },
 ]
@@ -20,15 +20,14 @@
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "requests",
   "beautifulsoup4",
-  "lxml",
   "Markdown",
 ]
 
 [project.urls]
 Homepage = "https://codeberg.org/HL-Bo/bookbot"
 Documentation = "https://codeberg.org/HL-Bo/bookbot/blob/master/docs/index.md"
 Changelog = "https://codeberg.org/HL-Bo/bookbot/blob/master/CHANGELOG.md"
@@ -44,12 +43,13 @@
 
 [project.optional-dependencies]
 gui = [
     "uvicorn",
     "fastapi",
 ]
 cli = ["textual"]
+lxml =  ["lxml"]
 
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
```

### Comparing `bookbot-1.0.dev1/PKG-INFO` & `bookbot-1.0.dev2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bookbot
-Version: 1.0.dev1
+Version: 1.0.dev2
 Project-URL: Homepage, https://codeberg.org/HL-Bo/bookbot
 Project-URL: Documentation, https://codeberg.org/HL-Bo/bookbot/blob/master/docs/index.md
 Project-URL: Changelog, https://codeberg.org/HL-Bo/bookbot/blob/master/CHANGELOG.md
 Project-URL: Repository, https://codeberg.org/HL-Bo/bookbot.git
 Project-URL: Bug Tracker, https://codeberg.org/HL-Bo/bookbot/issues
 Author-email: Heng Zhou <hl-bo@outlook.com>
 Maintainer-email: handsome2810@163.com
@@ -16,19 +16,20 @@
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: beautifulsoup4
-Requires-Dist: lxml
 Requires-Dist: markdown
 Requires-Dist: requests
 Provides-Extra: cli
 Requires-Dist: textual; extra == 'cli'
 Provides-Extra: gui
 Requires-Dist: fastapi; extra == 'gui'
 Requires-Dist: uvicorn; extra == 'gui'
+Provides-Extra: lxml
+Requires-Dist: lxml; extra == 'lxml'
 Description-Content-Type: text/markdown
 
 bookbot
 ======
```

