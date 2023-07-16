# Comparing `tmp/adadmire-1.0.0.tar.gz` & `tmp/adadmire-1.0.1.tar.gz`

## Comparing `adadmire-1.0.0.tar` & `adadmire-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0    63488 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/data_raw.xlsx
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/levels.npy
--rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/pheno.npy
--rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/pheno_with_stimulations.xlsx
--rw-r--r--   0        0        0    39328 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Feist_et_al/scaled_data_raw.npy
--rw-r--r--   0        0        0   310332 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/data_raw.xlsx
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/levels.npy
--rw-r--r--   0        0        0    19328 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/pheno.npy
--rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/pheno.xlsx
--rw-r--r--   0        0        0   217728 2020-02-02 00:00:00.000000 adadmire-1.0.0/data/Higuera_et_al/scaled_data_raw.npy
--rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 adadmire-1.0.0/doc/contribute.md
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 adadmire-1.0.0/src/adadmire/__init__.py
--rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 adadmire-1.0.0/src/adadmire/apgpy.py
--rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 adadmire-1.0.0/src/adadmire/main.py
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 adadmire-1.0.0/src/adadmire/mgm.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adadmire-1.0.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 adadmire-1.0.0/LICENSE
--rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 adadmire-1.0.0/README.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 adadmire-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5685 2020-02-02 00:00:00.000000 adadmire-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 adadmire-1.0.1/ex.py
+-rw-r--r--   0        0        0    63488 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/data_raw.xlsx
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/levels.npy
+-rw-r--r--   0        0        0     9728 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/pheno.npy
+-rw-r--r--   0        0        0    11757 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/pheno_with_stimulations.xlsx
+-rw-r--r--   0        0        0    39328 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Feist_et_al/scaled_data_raw.npy
+-rw-r--r--   0        0        0   217728 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/data_na_scaled.npy
+-rw-r--r--   0        0        0   310332 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/data_raw.xlsx
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/levels.npy
+-rw-r--r--   0        0        0    19328 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/pheno.npy
+-rw-r--r--   0        0        0    20483 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/pheno.xlsx
+-rw-r--r--   0        0        0    19328 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/pheno_na.npy
+-rw-r--r--   0        0        0   217728 2020-02-02 00:00:00.000000 adadmire-1.0.1/data/Higuera_et_al/scaled_data_raw.npy
+-rw-r--r--   0        0        0     4194 2020-02-02 00:00:00.000000 adadmire-1.0.1/doc/contribute.md
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 adadmire-1.0.1/src/adadmire/__init__.py
+-rw-r--r--   0        0        0     6272 2020-02-02 00:00:00.000000 adadmire-1.0.1/src/adadmire/apgpy.py
+-rw-r--r--   0        0        0    15532 2020-02-02 00:00:00.000000 adadmire-1.0.1/src/adadmire/main.py
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 adadmire-1.0.1/src/adadmire/mgm.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 adadmire-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 adadmire-1.0.1/LICENSE
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 adadmire-1.0.1/README.md
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 adadmire-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 adadmire-1.0.1/PKG-INFO
```

### Comparing `adadmire-1.0.0/data/Feist_et_al/data_raw.xlsx` & `adadmire-1.0.1/data/Feist_et_al/data_raw.xlsx`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/data/Feist_et_al/pheno.npy` & `adadmire-1.0.1/data/Feist_et_al/pheno.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/data/Feist_et_al/pheno_with_stimulations.xlsx` & `adadmire-1.0.1/data/Feist_et_al/pheno_with_stimulations.xlsx`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/data/Feist_et_al/scaled_data_raw.npy` & `adadmire-1.0.1/data/Feist_et_al/scaled_data_raw.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/data/Higuera_et_al/data_raw.xlsx` & `adadmire-1.0.1/data/Higuera_et_al/data_raw.xlsx`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/data/Higuera_et_al/pheno.npy` & `adadmire-1.0.1/data/Higuera_et_al/pheno.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/data/Higuera_et_al/pheno.xlsx` & `adadmire-1.0.1/data/Higuera_et_al/pheno.xlsx`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/data/Higuera_et_al/scaled_data_raw.npy` & `adadmire-1.0.1/data/Higuera_et_al/scaled_data_raw.npy`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/doc/contribute.md` & `adadmire-1.0.1/doc/contribute.md`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/src/adadmire/apgpy.py` & `adadmire-1.0.1/src/adadmire/apgpy.py`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/src/adadmire/main.py` & `adadmire-1.0.1/src/adadmire/main.py`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/src/adadmire/mgm.py` & `adadmire-1.0.1/src/adadmire/mgm.py`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/LICENSE` & `adadmire-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adadmire-1.0.0/README.md` & `adadmire-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -44,36 +44,33 @@
 print(n_ano_disc)
 # 0 detected discrete anomalies
 ```
 
 ### Example 2
 
 ```python
-from adadmire import loo_cv_cor, get_threshold_continuous, get_threshold_discrete, place_anomalies_continuous
+from adadmire import loo_cv_cor, get_threshold_continuous, place_anomalies_continuous
 import numpy as np
-
-# download data/Higuera_et_al
-# and load data
 X = np.load('data/Higuera_et_al/scaled_data_raw.npy') # continuous data
 D = np.load('data/Higuera_et_al/pheno.npy') # discrete data
 levels = np.load('data/Higuera_et_al/levels.npy') # levels of discrete variables
 
-# use originial data set and create simulation by introducing artificial anomalies
-X_ano = place_anomalies_continuous( X, n_ano = 1360, epsilon = 1.2)
+# use originial data set and create simulations by introducing artificial anomalies with various strengths
+X_ano, pos = place_anomalies_continuous( X, n_ano = 1360, epsilon = np.array([0.6, 0.8, 1.0, 1.2, 1.4]))
 # n_ano: how many anomalies should be introduced?
 # epsilon defines "strength" of introduced anomalies
 
 # now detect anomalies using ADMIRE
 lam_zero = np.sqrt(np.log(X.shape[1] + D.shape[1]/2)/X.shape[0])
 lam_seq = np.array([-1.75,-2.0,-2.25])
 lam = [pow(2, x) for x in lam_seq]
 lam = np.array(lam)
 lam = lam_zero * lam
-prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X_ano,D,levels,lam)
-X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X_ano, x_hat, B_m)
+prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X_ano[0],D,levels,lam) # perform cv and estimation 
+X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X_ano, x_hat, B_m) # determine threshold
 ```
 
 ### Data
 
 In the directory **data** you can find two sub directories:
 * **Feist_et_al**: contains data set as discribed in [Feist et al, 2018](#feist-et-al-2018) and [Buck et al, 2023](#buck-et-al-2023).
     * **data_raw.xlsx**: raw, unscaled data, contains measurements of 100 samples and 49 metabolites
```

### Comparing `adadmire-1.0.0/pyproject.toml` & `adadmire-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "adadmire"
-version = "1.0.0"
+version = "1.0.01"
 authors = [
   { name="Lena Buck", email="lena.buck@ukr.de" },
   { name="Tobias Schmidt", email="tobias2.schmidt@ukr.de" },
 ]
 description = "Functions for detecting anomalies in tabular datasets using Mixed Graphical Models."
 dependencies = []
 readme = "README.md"
```

### Comparing `adadmire-1.0.0/PKG-INFO` & `adadmire-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adadmire
-Version: 1.0.0
+Version: 1.0.1
 Summary: Functions for detecting anomalies in tabular datasets using Mixed Graphical Models.
 Project-URL: Homepage, https://github.com/spang-lab/adadmire
 Project-URL: Bug Tracker, https://github.com/spang-lab/adadmire/issues
 Author-email: Lena Buck <lena.buck@ukr.de>, Tobias Schmidt <tobias2.schmidt@ukr.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -58,36 +58,33 @@
 print(n_ano_disc)
 # 0 detected discrete anomalies
 ```
 
 ### Example 2
 
 ```python
-from adadmire import loo_cv_cor, get_threshold_continuous, get_threshold_discrete, place_anomalies_continuous
+from adadmire import loo_cv_cor, get_threshold_continuous, place_anomalies_continuous
 import numpy as np
-
-# download data/Higuera_et_al
-# and load data
 X = np.load('data/Higuera_et_al/scaled_data_raw.npy') # continuous data
 D = np.load('data/Higuera_et_al/pheno.npy') # discrete data
 levels = np.load('data/Higuera_et_al/levels.npy') # levels of discrete variables
 
-# use originial data set and create simulation by introducing artificial anomalies
-X_ano = place_anomalies_continuous( X, n_ano = 1360, epsilon = 1.2)
+# use originial data set and create simulations by introducing artificial anomalies with various strengths
+X_ano, pos = place_anomalies_continuous( X, n_ano = 1360, epsilon = np.array([0.6, 0.8, 1.0, 1.2, 1.4]))
 # n_ano: how many anomalies should be introduced?
 # epsilon defines "strength" of introduced anomalies
 
 # now detect anomalies using ADMIRE
 lam_zero = np.sqrt(np.log(X.shape[1] + D.shape[1]/2)/X.shape[0])
 lam_seq = np.array([-1.75,-2.0,-2.25])
 lam = [pow(2, x) for x in lam_seq]
 lam = np.array(lam)
 lam = lam_zero * lam
-prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X_ano,D,levels,lam)
-X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X_ano, x_hat, B_m)
+prob_hat, B_m, lam_opt,  x_hat, d_hat = loo_cv_cor(X_ano[0],D,levels,lam) # perform cv and estimation 
+X_cor, threshold_cont, n_ano_cont,  position_cont = get_threshold_continuous(X_ano, x_hat, B_m) # determine threshold
 ```
 
 ### Data
 
 In the directory **data** you can find two sub directories:
 * **Feist_et_al**: contains data set as discribed in [Feist et al, 2018](#feist-et-al-2018) and [Buck et al, 2023](#buck-et-al-2023).
     * **data_raw.xlsx**: raw, unscaled data, contains measurements of 100 samples and 49 metabolites
```

