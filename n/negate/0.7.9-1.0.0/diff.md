# Comparing `tmp/negate-0.7.9.tar.gz` & `tmp/negate-1.0.0.tar.gz`

## Comparing `negate-0.7.9.tar` & `negate-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 negate-0.7.9/.deepsource.toml
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 negate-0.7.9/.pylintrc
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 negate-0.7.9/test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 negate-0.7.9/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 negate-0.7.9/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 negate-0.7.9/negate/__init__.py
--rw-r--r--   0        0        0    23002 2020-02-02 00:00:00.000000 negate-0.7.9/negate/negate.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 negate-0.7.9/negate/py.typed
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 negate-0.7.9/negate/tokens.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 negate-0.7.9/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 negate-0.7.9/tests/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 negate-0.7.9/tests/conftest.py
--rw-r--r--   0        0        0    17999 2020-02-02 00:00:00.000000 negate-0.7.9/tests/data.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 negate-0.7.9/tests/requirements.txt
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 negate-0.7.9/tests/test_negate.py
--rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 negate-0.7.9/.gitignore
--rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 negate-0.7.9/LICENSE
--rw-r--r--   0        0        0     7896 2020-02-02 00:00:00.000000 negate-0.7.9/README.md
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 negate-0.7.9/pyproject.toml
--rw-r--r--   0        0        0    22083 2020-02-02 00:00:00.000000 negate-0.7.9/PKG-INFO
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 negate-1.0.0/.deepsource.toml
+-rw-r--r--   0        0        0    13967 2020-02-02 00:00:00.000000 negate-1.0.0/.pylintrc
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 negate-1.0.0/test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 negate-1.0.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 negate-1.0.0/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0    84110 2020-02-02 00:00:00.000000 negate-1.0.0/img/negate_logo.png
+-rw-r--r--   0        0        0    24211 2020-02-02 00:00:00.000000 negate-1.0.0/img/negate_logo.svg
+-rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 negate-1.0.0/img/negate_logo_description.svg
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 negate-1.0.0/negate/__init__.py
+-rw-r--r--   0        0        0    34593 2020-02-02 00:00:00.000000 negate-1.0.0/negate/negate.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 negate-1.0.0/negate/py.typed
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 negate-1.0.0/negate/tokens.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 negate-1.0.0/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 negate-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 negate-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0    17999 2020-02-02 00:00:00.000000 negate-1.0.0/tests/data.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 negate-1.0.0/tests/requirements.txt
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 negate-1.0.0/tests/test_negate.py
+-rw-r--r--   0        0        0     1966 2020-02-02 00:00:00.000000 negate-1.0.0/.gitignore
+-rw-r--r--   0        0        0    11373 2020-02-02 00:00:00.000000 negate-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7766 2020-02-02 00:00:00.000000 negate-1.0.0/README.md
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 negate-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    21953 2020-02-02 00:00:00.000000 negate-1.0.0/PKG-INFO
```

### Comparing `negate-0.7.9/.pylintrc` & `negate-1.0.0/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
 notes=TODO
 
 
 [STRING]
 
 # This flag controls whether inconsistent-quotes generates a warning when the
 # character used as a quote delimiter is used inconsistently within a module.
-check-quote-consistency=yes
+# check-quote-consistency=yes
 
 
 [VARIABLES]
 
 # Tells whether we should check for unused import in __init__ files.
 init-import=no
```

### Comparing `negate-0.7.9/.github/workflows/run-tests.yml` & `negate-1.0.0/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `negate-0.7.9/negate/tokens.py` & `negate-1.0.0/negate/tokens.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 @dataclass
 class Token:
     """A token, i.e., a sequence of characters.
 
     A :obj:`spacy.tokens.Token` is read-only. See
     `https://spacy.io/api/token`__. Furthermore, it cannot hold an empty string
-    as :attr:`text`. This class is just a minimalist equivalent to a Spacy Token
+    as :attr:`text`. This class is just a minimal equivalent to a spaCy token
     that is both writable and allows empty strings as text. It only contains the
     attributes relevant for our purposes.
 
     Attributes:
         text (:obj:`str`):
             The characters that form the token.
         has_space_after (:obj:`str`):
             Whether the token is followed by a whitespace (this whitespace is
             not part of the :attr:`text`). This information is used for
-            detokenization.
+            de-tokenization.
     """
 
     text: str
     has_space_after: bool = True
```

### Comparing `negate-0.7.9/tests/README.md` & `negate-1.0.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `negate-0.7.9/tests/conftest.py` & `negate-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.9/tests/data.py` & `negate-1.0.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.9/tests/test_negate.py` & `negate-1.0.0/tests/test_negate.py`

 * *Files identical despite different names*

### Comparing `negate-0.7.9/.gitignore` & `negate-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `negate-0.7.9/LICENSE` & `negate-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `negate-0.7.9/README.md` & `negate-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-<p align="center"><img width="666" src="https://user-images.githubusercontent.com/22967053/208313993-b873be19-8648-4edd-b4ee-e5283c19ad8f.png" alt="Negate: A Python module to negate sentences."></p>
+<p align="center"><img width="600" src="https://github.com/dmlls/negate/assets/22967053/757bdd23-c77c-4ad2-be4b-d230fa96f5bd" alt="Negate: A Python module to negate sentences."></p>
 <p align="center" display="inline-block">
   <a href="https://pypi.org/project/negate/">
     <img src="https://img.shields.io/pypi/v/negate">
   </a>
-  <a href="https://pypi.org/project/negate/">
-    <img src="https://img.shields.io/badge/release-beta-green">
-  </a>
   <a href="https://deepsource.io/gh/dmlls/negate/?ref=repository-badge" target="_blank">
       <img alt="Active Issues" title="DeepSource" src="https://deepsource.io/gh/dmlls/negate.svg/?label=active+issues&token=D9QCfE028iloctbSdOhywtZy"/>
   </a>
 </p>
 
-<br>
+<br><br>
 
 ## Introduction
 
 Negate is a Python module that implements rule-based, syntactic sentence
 negation in English<sup>1</sup>.
```

### Comparing `negate-0.7.9/pyproject.toml` & `negate-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `negate-0.7.9/PKG-INFO` & `negate-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: negate
-Version: 0.7.9
+Version: 1.0.0
 Summary: A Python module that negates sentences.
 Project-URL: Homepage, https://github.com/dmlls/negate
 Project-URL: GitHub Issues, https://github.com/dmlls/negate/issues
 Project-URL: GitHub Repo, https://github.com/dmlls/negate
 Author-email: Diego Miguel Lozano <hello@diegomiguel.me>
 Maintainer-email: Diego Miguel Lozano <hello@diegomiguel.me>
 License: 
@@ -223,28 +223,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.7
 Requires-Dist: lemminflect<0.3.0,>=0.2.3
 Requires-Dist: spacy[transformers]<3.5.0,>=3.4.1
 Description-Content-Type: text/markdown
 
-<p align="center"><img width="666" src="https://user-images.githubusercontent.com/22967053/208313993-b873be19-8648-4edd-b4ee-e5283c19ad8f.png" alt="Negate: A Python module to negate sentences."></p>
+<p align="center"><img width="600" src="https://github.com/dmlls/negate/assets/22967053/757bdd23-c77c-4ad2-be4b-d230fa96f5bd" alt="Negate: A Python module to negate sentences."></p>
 <p align="center" display="inline-block">
   <a href="https://pypi.org/project/negate/">
     <img src="https://img.shields.io/pypi/v/negate">
   </a>
-  <a href="https://pypi.org/project/negate/">
-    <img src="https://img.shields.io/badge/release-beta-green">
-  </a>
   <a href="https://deepsource.io/gh/dmlls/negate/?ref=repository-badge" target="_blank">
       <img alt="Active Issues" title="DeepSource" src="https://deepsource.io/gh/dmlls/negate.svg/?label=active+issues&token=D9QCfE028iloctbSdOhywtZy"/>
   </a>
 </p>
 
-<br>
+<br><br>
 
 ## Introduction
 
 Negate is a Python module that implements rule-based, syntactic sentence
 negation in English<sup>1</sup>.
```

