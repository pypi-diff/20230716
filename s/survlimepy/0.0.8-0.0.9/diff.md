# Comparing `tmp/survlimepy-0.0.8.tar.gz` & `tmp/survlimepy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "survlimepy-0.0.8.tar", last modified: Thu Feb 16 14:52:37 2023, max compression
+gzip compressed data, was "survlimepy-0.0.9.tar", last modified: Thu Feb 16 16:02:21 2023, max compression
```

## Comparing `survlimepy-0.0.8.tar` & `survlimepy-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 14:52:37.910987 survlimepy-0.0.8/
--rw-r--r--   0 cristianpachon   (501) staff       (20)    35149 2022-12-23 16:30:48.000000 survlimepy-0.0.8/LICENSE
--rw-r--r--   0 cristianpachon   (501) staff       (20)       54 2023-02-09 11:12:54.000000 survlimepy-0.0.8/MANIFEST.in
--rw-r--r--   0 cristianpachon   (501) staff       (20)    47554 2023-02-16 14:52:37.910263 survlimepy-0.0.8/PKG-INFO
--rw-r--r--   0 cristianpachon   (501) staff       (20)     6332 2023-02-16 14:46:53.000000 survlimepy-0.0.8/README.md
--rw-r--r--   0 cristianpachon   (501) staff       (20)  1560680 2022-11-16 15:57:27.000000 survlimepy-0.0.8/logo.png
--rw-r--r--   0 cristianpachon   (501) staff       (20)     1237 2023-02-16 14:48:03.000000 survlimepy-0.0.8/pyproject.toml
--rw-r--r--   0 cristianpachon   (501) staff       (20)       38 2023-02-16 14:52:37.911148 survlimepy-0.0.8/setup.cfg
-drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 14:52:37.900673 survlimepy-0.0.8/survlimepy/
--rw-r--r--   0 cristianpachon   (501) staff       (20)       50 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/__init__.py
-drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 14:52:37.905280 survlimepy-0.0.8/survlimepy/datasets/
--rw-r--r--   0 cristianpachon   (501) staff       (20)        0 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/datasets/__init__.py
--rw-r--r--   0 cristianpachon   (501) staff       (20)    13488 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/datasets/heart_dataset.csv
--rw-r--r--   0 cristianpachon   (501) staff       (20)     2010 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/datasets/loading_utils.py
--rw-r--r--   0 cristianpachon   (501) staff       (20)     7856 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/datasets/lung_dataset.csv
--rw-r--r--   0 cristianpachon   (501) staff       (20)    35022 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/datasets/pbc_dataset.csv
--rw-r--r--   0 cristianpachon   (501) staff       (20)     3552 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/datasets/udca_dataset.csv
--rw-r--r--   0 cristianpachon   (501) staff       (20)     3914 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/datasets/veteran.csv
--rw-r--r--   0 cristianpachon   (501) staff       (20)    10429 2023-02-15 15:28:46.000000 survlimepy-0.0.8/survlimepy/load_datasets.py
--rw-r--r--   0 cristianpachon   (501) staff       (20)    19642 2023-02-09 15:11:58.000000 survlimepy-0.0.8/survlimepy/survlime_explainer.py
-drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 14:52:37.907698 survlimepy-0.0.8/survlimepy/utils/
--rw-r--r--   0 cristianpachon   (501) staff       (20)        0 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/utils/__init__.py
--rw-r--r--   0 cristianpachon   (501) staff       (20)     2112 2023-02-09 10:25:47.000000 survlimepy-0.0.8/survlimepy/utils/neighbours_generator.py
--rw-r--r--   0 cristianpachon   (501) staff       (20)    14308 2023-02-15 11:32:11.000000 survlimepy-0.0.8/survlimepy/utils/optimisation.py
--rw-r--r--   0 cristianpachon   (501) staff       (20)     5282 2023-02-05 15:59:39.000000 survlimepy-0.0.8/survlimepy/utils/predict.py
--rw-r--r--   0 cristianpachon   (501) staff       (20)      944 2023-01-10 11:27:15.000000 survlimepy-0.0.8/survlimepy/utils/step_function.py
-drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 14:52:37.902665 survlimepy-0.0.8/survlimepy.egg-info/
--rw-r--r--   0 cristianpachon   (501) staff       (20)    47554 2023-02-16 14:52:37.000000 survlimepy-0.0.8/survlimepy.egg-info/PKG-INFO
--rw-r--r--   0 cristianpachon   (501) staff       (20)      753 2023-02-16 14:52:37.000000 survlimepy-0.0.8/survlimepy.egg-info/SOURCES.txt
--rw-r--r--   0 cristianpachon   (501) staff       (20)        1 2023-02-16 14:52:37.000000 survlimepy-0.0.8/survlimepy.egg-info/dependency_links.txt
--rw-r--r--   0 cristianpachon   (501) staff       (20)      107 2023-02-16 14:52:37.000000 survlimepy-0.0.8/survlimepy.egg-info/requires.txt
--rw-r--r--   0 cristianpachon   (501) staff       (20)       11 2023-02-16 14:52:37.000000 survlimepy-0.0.8/survlimepy.egg-info/top_level.txt
-drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 14:52:37.909186 survlimepy-0.0.8/tests/
--rw-r--r--   0 cristianpachon   (501) staff       (20)        0 2023-01-10 11:27:15.000000 survlimepy-0.0.8/tests/__init__.py
--rw-r--r--   0 cristianpachon   (501) staff       (20)     7129 2023-02-09 10:25:47.000000 survlimepy-0.0.8/tests/tests.py
+drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 16:02:21.850642 survlimepy-0.0.9/
+-rw-r--r--   0 cristianpachon   (501) staff       (20)    35149 2022-12-23 16:30:48.000000 survlimepy-0.0.9/LICENSE
+-rw-r--r--   0 cristianpachon   (501) staff       (20)       54 2023-02-09 11:12:54.000000 survlimepy-0.0.9/MANIFEST.in
+-rw-r--r--   0 cristianpachon   (501) staff       (20)    47554 2023-02-16 16:02:21.850170 survlimepy-0.0.9/PKG-INFO
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     6332 2023-02-16 14:46:53.000000 survlimepy-0.0.9/README.md
+-rw-r--r--   0 cristianpachon   (501) staff       (20)  1560680 2022-11-16 15:57:27.000000 survlimepy-0.0.9/logo.png
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     1237 2023-02-16 15:58:13.000000 survlimepy-0.0.9/pyproject.toml
+-rw-r--r--   0 cristianpachon   (501) staff       (20)       38 2023-02-16 16:02:21.850748 survlimepy-0.0.9/setup.cfg
+drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 16:02:21.842617 survlimepy-0.0.9/survlimepy/
+-rw-r--r--   0 cristianpachon   (501) staff       (20)       50 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/__init__.py
+drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 16:02:21.846922 survlimepy-0.0.9/survlimepy/datasets/
+-rw-r--r--   0 cristianpachon   (501) staff       (20)        0 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/datasets/__init__.py
+-rw-r--r--   0 cristianpachon   (501) staff       (20)    13488 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/datasets/heart_dataset.csv
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     2010 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/datasets/loading_utils.py
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     7856 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/datasets/lung_dataset.csv
+-rw-r--r--   0 cristianpachon   (501) staff       (20)    35022 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/datasets/pbc_dataset.csv
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     3552 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/datasets/udca_dataset.csv
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     3914 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/datasets/veteran.csv
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     9988 2023-02-16 15:57:51.000000 survlimepy-0.0.9/survlimepy/load_datasets.py
+-rw-r--r--   0 cristianpachon   (501) staff       (20)    19642 2023-02-09 15:11:58.000000 survlimepy-0.0.9/survlimepy/survlime_explainer.py
+drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 16:02:21.848695 survlimepy-0.0.9/survlimepy/utils/
+-rw-r--r--   0 cristianpachon   (501) staff       (20)        0 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/utils/__init__.py
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     2112 2023-02-09 10:25:47.000000 survlimepy-0.0.9/survlimepy/utils/neighbours_generator.py
+-rw-r--r--   0 cristianpachon   (501) staff       (20)    14308 2023-02-15 11:32:11.000000 survlimepy-0.0.9/survlimepy/utils/optimisation.py
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     5282 2023-02-05 15:59:39.000000 survlimepy-0.0.9/survlimepy/utils/predict.py
+-rw-r--r--   0 cristianpachon   (501) staff       (20)      944 2023-01-10 11:27:15.000000 survlimepy-0.0.9/survlimepy/utils/step_function.py
+drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 16:02:21.844500 survlimepy-0.0.9/survlimepy.egg-info/
+-rw-r--r--   0 cristianpachon   (501) staff       (20)    47554 2023-02-16 16:02:21.000000 survlimepy-0.0.9/survlimepy.egg-info/PKG-INFO
+-rw-r--r--   0 cristianpachon   (501) staff       (20)      753 2023-02-16 16:02:21.000000 survlimepy-0.0.9/survlimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 cristianpachon   (501) staff       (20)        1 2023-02-16 16:02:21.000000 survlimepy-0.0.9/survlimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 cristianpachon   (501) staff       (20)      107 2023-02-16 16:02:21.000000 survlimepy-0.0.9/survlimepy.egg-info/requires.txt
+-rw-r--r--   0 cristianpachon   (501) staff       (20)       11 2023-02-16 16:02:21.000000 survlimepy-0.0.9/survlimepy.egg-info/top_level.txt
+drwxr-xr-x   0 cristianpachon   (501) staff       (20)        0 2023-02-16 16:02:21.849406 survlimepy-0.0.9/tests/
+-rw-r--r--   0 cristianpachon   (501) staff       (20)        0 2023-01-10 11:27:15.000000 survlimepy-0.0.9/tests/__init__.py
+-rw-r--r--   0 cristianpachon   (501) staff       (20)     7129 2023-02-09 10:25:47.000000 survlimepy-0.0.9/tests/tests.py
```

### Comparing `survlimepy-0.0.8/LICENSE` & `survlimepy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/PKG-INFO` & `survlimepy-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survlimepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package implementing SurvLIME algorithm
 Author-email: Carlos Hernández Pérez <crherperez95@gmail.com>, Cristian Pachón García <cc.pachon@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `survlimepy-0.0.8/README.md` & `survlimepy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/logo.png` & `survlimepy-0.0.9/logo.png`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/pyproject.toml` & `survlimepy-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "survlimepy"
-version = "0.0.8"
+version = "0.0.9"
 description = "A python package implementing SurvLIME algorithm"
 authors = [
     {name = "Carlos Hernández Pérez", email = "crherperez95@gmail.com"},
     {name = "Cristian Pachón García", email = "cc.pachon@gmail.com"},
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
```

### Comparing `survlimepy-0.0.8/survlimepy/datasets/heart_dataset.csv` & `survlimepy-0.0.9/survlimepy/datasets/heart_dataset.csv`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/datasets/loading_utils.py` & `survlimepy-0.0.9/survlimepy/datasets/loading_utils.py`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/datasets/lung_dataset.csv` & `survlimepy-0.0.9/survlimepy/datasets/lung_dataset.csv`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/datasets/pbc_dataset.csv` & `survlimepy-0.0.9/survlimepy/datasets/pbc_dataset.csv`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/datasets/udca_dataset.csv` & `survlimepy-0.0.9/survlimepy/datasets/udca_dataset.csv`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/datasets/veteran.csv` & `survlimepy-0.0.9/survlimepy/datasets/veteran.csv`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/load_datasets.py` & `survlimepy-0.0.9/survlimepy/load_datasets.py`

 * *Files 3% similar despite different names*

```diff
@@ -99,49 +99,39 @@
         x_pre = x.copy()
         for cat_feat in self.categorical_columns:
             names = [cat_feat + "_" + str(value) for value in x_pre[cat_feat].unique()]
             df_dummy_i = pd.get_dummies(
                 x_pre[cat_feat], drop_first=True, prefix=cat_feat
             )
             new_names = df_dummy_i.columns
-            # x_pre[names[1:]] = pd.get_dummies(x_pre[cat_feat], drop_first=True)
             x_pre[new_names] = df_dummy_i
             x_pre.drop(cat_feat, inplace=True, axis=1)
 
         # Then convert the data and the features to three splits
         # and standarize them
         y = Surv.from_arrays(events, times)
         X_train, X_test, y_train, y_test = train_test_split(
             x_pre.copy(), y, test_size=0.10, random_state=random_seed
         )
-        # X_val, X_test, y_val, y_test = train_test_split(
-        #    X_test.copy(), y_test, test_size=0.5, random_state=random_seed
-        # )
 
         if standarize:
             scaler = StandardScaler()
             X_train = pd.DataFrame(
                 data=scaler.fit_transform(X_train, y_train),
                 columns=X_train.columns,
                 index=X_train.index,
             )
 
-            #    X_val = pd.DataFrame(
-            #        data=scaler.transform(X_val),
-            #        columns=X_val.columns,
-            #        index=X_val.index,
-            #    )
-
             X_test = pd.DataFrame(
                 data=scaler.transform(X_test),
                 columns=X_test.columns,
                 index=X_test.index,
             )
 
-        return [X_train, y_train], [X_test, y_test]  # [X_val, y_val]
+        return [X_train, y_train], [X_test, y_test]
 
 
 class RandomSurvivalData:
     """Generate spherical random survival data."""
 
     def __init__(
         self,
```

### Comparing `survlimepy-0.0.8/survlimepy/survlime_explainer.py` & `survlimepy-0.0.9/survlimepy/survlime_explainer.py`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/utils/neighbours_generator.py` & `survlimepy-0.0.9/survlimepy/utils/neighbours_generator.py`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/utils/optimisation.py` & `survlimepy-0.0.9/survlimepy/utils/optimisation.py`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/utils/predict.py` & `survlimepy-0.0.9/survlimepy/utils/predict.py`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy/utils/step_function.py` & `survlimepy-0.0.9/survlimepy/utils/step_function.py`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/survlimepy.egg-info/PKG-INFO` & `survlimepy-0.0.9/survlimepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: survlimepy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package implementing SurvLIME algorithm
 Author-email: Carlos Hernández Pérez <crherperez95@gmail.com>, Cristian Pachón García <cc.pachon@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `survlimepy-0.0.8/survlimepy.egg-info/SOURCES.txt` & `survlimepy-0.0.9/survlimepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `survlimepy-0.0.8/tests/tests.py` & `survlimepy-0.0.9/tests/tests.py`

 * *Files identical despite different names*

