# Comparing `tmp/deklinacija-1.5.0.tar.gz` & `tmp/deklinacija-1.5.1.tar.gz`

## Comparing `deklinacija-1.5.0.tar` & `deklinacija-1.5.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.5.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.5.0/deklinacija/__init__.py
--rw-r--r--   0        0        0    21534 2020-02-02 00:00:00.000000 deklinacija-1.5.0/deklinacija/module.py
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 deklinacija-1.5.0/deklinacija/utils.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 deklinacija-1.5.0/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 deklinacija-1.5.0/tests/names_female.txt
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 deklinacija-1.5.0/tests/names_male.txt
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 deklinacija-1.5.0/tests/test_names.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.5.0/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.5.0/LICENSE
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 deklinacija-1.5.0/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 deklinacija-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.5.1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.5.1/deklinacija/__init__.py
+-rw-r--r--   0        0        0    21542 2020-02-02 00:00:00.000000 deklinacija-1.5.1/deklinacija/module.py
+-rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 deklinacija-1.5.1/deklinacija/utils.py
+-rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 deklinacija-1.5.1/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 deklinacija-1.5.1/tests/names_female.txt
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 deklinacija-1.5.1/tests/names_male.txt
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 deklinacija-1.5.1/tests/test_names.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.5.1/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.5.1/LICENSE
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 deklinacija-1.5.1/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 deklinacija-1.5.1/PKG-INFO
```

### Comparing `deklinacija-1.5.0/.github/workflows/python-package.yml` & `deklinacija-1.5.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/deklinacija/module.py` & `deklinacija-1.5.1/deklinacija/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -559,15 +559,15 @@
         else:
             if utils.isLatin(lastChar) == True:
                 name[-1] = "im"
             else:
                 name[-1] = "им"
         return "".join(name)
 
-    if gender.lower() == "male" and utils.toCyrillic(nameGenitiv)[-1].lower() in INSTRUMENTAL_LETTERS and name[-1] not in ["а", "a"]:
+    if gender.lower() == "male" and utils.toCyrillic(nameGenitiv)[-1].lower() in INSTRUMENTAL_LETTERS and name[-1].lower() not in ["а", "a"]:
         if lastChar.isupper():
             if utils.isLatin(lastChar):
                 nameGenitiv.append("EM")
             else:
                 nameGenitiv.append("ЕМ")
             return "".join(nameGenitiv)
         else:
```

### Comparing `deklinacija-1.5.0/deklinacija/utils.py` & `deklinacija-1.5.1/deklinacija/utils.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/deklinacija/vokativ_database.csv` & `deklinacija-1.5.1/deklinacija/vokativ_database.csv`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/tests/names_female.txt` & `deklinacija-1.5.1/tests/names_female.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/tests/names_male.txt` & `deklinacija-1.5.1/tests/names_male.txt`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/tests/test_names.py` & `deklinacija-1.5.1/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/.gitignore` & `deklinacija-1.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/LICENSE` & `deklinacija-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/README.md` & `deklinacija-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.0/pyproject.toml` & `deklinacija-1.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.5.0"
+version = "1.5.1"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.5.0/PKG-INFO` & `deklinacija-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.5.0
+Version: 1.5.1
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

