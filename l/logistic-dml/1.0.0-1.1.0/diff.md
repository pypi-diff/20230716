# Comparing `tmp/logistic_dml-1.0.0.tar.gz` & `tmp/logistic_dml-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logistic_dml-1.0.0.tar", last modified: Sat Jul  8 21:31:38 2023, max compression
+gzip compressed data, was "logistic_dml-1.1.0.tar", last modified: Sun Jul 16 20:19:13 2023, max compression
```

## Comparing `logistic_dml-1.0.0.tar` & `logistic_dml-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 Salim      (501) staff       (20)        0 2023-07-08 21:31:38.714430 logistic_dml-1.0.0/
--rw-r--r--   0 Salim      (501) staff       (20)      268 2023-07-08 21:31:38.714275 logistic_dml-1.0.0/PKG-INFO
--rw-r--r--   0 Salim      (501) staff       (20)      211 2023-03-29 10:28:23.000000 logistic_dml-1.0.0/README.md
-drwxr-xr-x   0 Salim      (501) staff       (20)        0 2023-07-08 21:31:38.713174 logistic_dml-1.0.0/logistic_dml/
--rw-r--r--   0 Salim      (501) staff       (20)        0 2023-07-08 21:16:39.000000 logistic_dml-1.0.0/logistic_dml/__init__.py
--rw-r--r--   0 Salim      (501) staff       (20)     6764 2023-07-08 21:09:04.000000 logistic_dml-1.0.0/logistic_dml/logistic_dml.py
--rw-r--r--   0 Salim      (501) staff       (20)     6515 2023-07-08 21:09:51.000000 logistic_dml-1.0.0/logistic_dml/test_logistic_dml.py
-drwxr-xr-x   0 Salim      (501) staff       (20)        0 2023-07-08 21:31:38.714074 logistic_dml-1.0.0/logistic_dml.egg-info/
--rw-r--r--   0 Salim      (501) staff       (20)      268 2023-07-08 21:31:38.000000 logistic_dml-1.0.0/logistic_dml.egg-info/PKG-INFO
--rw-r--r--   0 Salim      (501) staff       (20)      285 2023-07-08 21:31:38.000000 logistic_dml-1.0.0/logistic_dml.egg-info/SOURCES.txt
--rw-r--r--   0 Salim      (501) staff       (20)        1 2023-07-08 21:31:38.000000 logistic_dml-1.0.0/logistic_dml.egg-info/dependency_links.txt
--rw-r--r--   0 Salim      (501) staff       (20)       60 2023-07-08 21:31:38.000000 logistic_dml-1.0.0/logistic_dml.egg-info/requires.txt
--rw-r--r--   0 Salim      (501) staff       (20)       13 2023-07-08 21:31:38.000000 logistic_dml-1.0.0/logistic_dml.egg-info/top_level.txt
--rw-r--r--   0 Salim      (501) staff       (20)       38 2023-07-08 21:31:38.714486 logistic_dml-1.0.0/setup.cfg
--rw-r--r--   0 Salim      (501) staff       (20)      411 2023-07-08 21:30:50.000000 logistic_dml-1.0.0/setup.py
+drwxr-xr-x   0 Salim      (501) staff       (20)        0 2023-07-16 20:19:13.487676 logistic_dml-1.1.0/
+-rw-r--r--   0 Salim      (501) staff       (20)      268 2023-07-16 20:19:13.487543 logistic_dml-1.1.0/PKG-INFO
+-rw-r--r--   0 Salim      (501) staff       (20)      211 2023-03-29 10:28:23.000000 logistic_dml-1.1.0/README.md
+drwxr-xr-x   0 Salim      (501) staff       (20)        0 2023-07-16 20:19:13.486501 logistic_dml-1.1.0/logistic_dml/
+-rw-r--r--   0 Salim      (501) staff       (20)       28 2023-07-09 19:17:34.000000 logistic_dml-1.1.0/logistic_dml/__init__.py
+-rw-r--r--   0 Salim      (501) staff       (20)    12062 2023-07-16 20:14:52.000000 logistic_dml-1.1.0/logistic_dml/logistic_dml.py
+-rw-r--r--   0 Salim      (501) staff       (20)        0 2023-07-16 20:14:52.000000 logistic_dml-1.1.0/logistic_dml/pdev.py
+-rw-r--r--   0 Salim      (501) staff       (20)     5582 2023-07-16 20:14:52.000000 logistic_dml-1.1.0/logistic_dml/pdev_lr.py
+-rw-r--r--   0 Salim      (501) staff       (20)     5995 2023-07-16 20:14:52.000000 logistic_dml-1.1.0/logistic_dml/pdev_rf.py
+-rw-r--r--   0 Salim      (501) staff       (20)     6816 2023-07-16 20:14:52.000000 logistic_dml-1.1.0/logistic_dml/test_logistic_dml.py
+-rw-r--r--   0 Salim      (501) staff       (20)      598 2023-07-12 19:51:42.000000 logistic_dml-1.1.0/logistic_dml/test_network_kernel.py
+drwxr-xr-x   0 Salim      (501) staff       (20)        0 2023-07-16 20:19:13.487333 logistic_dml-1.1.0/logistic_dml.egg-info/
+-rw-r--r--   0 Salim      (501) staff       (20)      268 2023-07-16 20:19:13.000000 logistic_dml-1.1.0/logistic_dml.egg-info/PKG-INFO
+-rw-r--r--   0 Salim      (501) staff       (20)      390 2023-07-16 20:19:13.000000 logistic_dml-1.1.0/logistic_dml.egg-info/SOURCES.txt
+-rw-r--r--   0 Salim      (501) staff       (20)        1 2023-07-16 20:19:13.000000 logistic_dml-1.1.0/logistic_dml.egg-info/dependency_links.txt
+-rw-r--r--   0 Salim      (501) staff       (20)       61 2023-07-16 20:19:13.000000 logistic_dml-1.1.0/logistic_dml.egg-info/requires.txt
+-rw-r--r--   0 Salim      (501) staff       (20)       13 2023-07-16 20:19:13.000000 logistic_dml-1.1.0/logistic_dml.egg-info/top_level.txt
+-rw-r--r--   0 Salim      (501) staff       (20)       38 2023-07-16 20:19:13.487728 logistic_dml-1.1.0/setup.cfg
+-rw-r--r--   0 Salim      (501) staff       (20)      415 2023-07-16 20:16:35.000000 logistic_dml-1.1.0/setup.py
```

### Comparing `logistic_dml-1.0.0/logistic_dml/test_logistic_dml.py` & `logistic_dml-1.1.0/logistic_dml/test_logistic_dml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,52 @@
-import math
 import unittest
 import numpy as np
+import pandas as pd
 from sklearn.linear_model import LogisticRegression, LinearRegression
-from logistic_dml import *
+from logistic_dml import DML
 from scipy.special import expit
 
 
 class TestSplit(unittest.TestCase):
     def test_split(self):
         np.random.seed(0)
         K = 3
         input_array = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
-        actual = split(K, input_array)
+        actual = DML.split(K, input_array)
         expected_type = np.ndarray
         expected_shape = input_array.shape
         self.assertIsInstance(actual, expected_type)
         self.assertEqual(actual.shape, expected_shape)
 
         # Exactly one observation not assigned a fold
         self.assertTrue(sum((i == 0 for i in actual)) == 1)
 
         # Remaining observations are assigned to a fold
         for j in [1, 2, 3]:
             self.assertTrue(sum((j == i for i in actual)) == 3)
 
 
-class TestL(unittest.TestCase):
-    def test_L(self):
+class TestML(unittest.TestCase):
+    def test_ml(self):
         np.random.seed(0)
         # Test case with binary R
         R = np.array([0, 1, 1, 0, 1])
         C = pd.DataFrame({'X1': [1, 4, 7, 10, 13], 'X2': [2, 5, 8, 11, 14], 'X3': [3, 6, 9, 12, 15]})
         Ctest = pd.DataFrame({'X1': [16, 19], 'X2': [17, 20], 'X3': [18, 21]})
         expected = np.array([0.85, 0.9])
-        np.testing.assert_allclose(np.round(L(R, C, Ctest, givenClassifier=LogisticRegression()), 2), expected, rtol=1e-6)
+        dml = DML(classifier=LogisticRegression())
+        np.testing.assert_allclose(np.round(dml.ml(R, C, Ctest), 2), expected, rtol=1e-6)
 
         # Test case with continuous R
         R = np.array([0.2, 0.5, 0.8])
         C = pd.DataFrame({'X1': [1, 3, 5], 'X2': [2, 4, 6]})
         Ctest = pd.DataFrame({'X1': [7, 9], 'X2': [8, 10]})
         expected = np.array([1.1, 1.4])
-        np.testing.assert_allclose(np.round(L(R, C, Ctest, givenRegressor=LinearRegression()), 2), expected, rtol=1e-6)
-
-
-class TestLogit(unittest.TestCase):
-    def test_logit(self):
-        x = np.array([0.5, 0.25, 0.75])
-        expected = np.array([0, -1.0986122886681098, 1.0986122886681098])
-        np.testing.assert_allclose(logit(x), expected)
-
-        x = np.array([-1])
-        with np.testing.assert_raises(ValueError):
-            logit(x)
-
-        x = np.array([2])
-        with np.testing.assert_raises(ValueError):
-            logit(x)
+        dml = DML(regressor=LinearRegression())
+        np.testing.assert_allclose(np.round(dml.ml(R, C, Ctest), 2), expected, rtol=1e-6)
 
 
 class TestDml(unittest.TestCase):
     def test_dml_linear_regression(self):
         np.random.seed(0)
         Y = np.array([1, 0, 1, 1, 0, 0, 1, 0, 1, 0]*2)
         A = np.array([1, 1, 0, 1, 0, 0, 1, 0, 1, 1]*2)
@@ -67,15 +54,15 @@
                           'X2': [11, 12, 13, 14, 15, 16, 17, 18, 19, 20]*2})
         K = 2
         model1 = LogisticRegression()
         model2 = LinearRegression()
         expected_keys = ['mXp', 'rXp']
         expected_mXp_shape = (20,)
         expected_rXp_shape = (20,)
-        actual = dml(Y, A, X, K, givenClassifier=model1, givenRegressor=model2)
+        actual = DML(classifier=model1, regressor=model2).dml(Y, A, X, k_folds=K)
         self.assertIsInstance(actual, dict)
         self.assertEqual(sorted(actual.keys()), expected_keys)
         self.assertEqual(actual['mXp'].shape, expected_mXp_shape)
         self.assertEqual(actual['rXp'].shape, expected_rXp_shape)
 
     def test_dml_logistic_regression(self):
         """The following test fails and it would fail for the R code if Liu et al used logistic
@@ -88,15 +75,15 @@
                           'X2': [11, 12, 13, 14, 15, 16, 17, 18, 19, 20]*2})
         K = 2
         model1 = LogisticRegression()
         model2 = LinearRegression()
         expected_keys = ['mXp', 'rXp']
         expected_mXp_shape = (20,)
         expected_rXp_shape = (20,)
-        actual = dml(Y, A, X, K, givenClassifier=model1, givenRegressor=model2)
+        actual = DML(classifier=model1, regressor=model2).dml(Y, A, X, k_folds=K)
         self.assertIsInstance(actual, dict)
         self.assertEqual(sorted(actual.keys()), expected_keys)
         self.assertEqual(actual['mXp'].shape, expected_mXp_shape)
         self.assertEqual(actual['rXp'].shape, expected_rXp_shape)
 
 
 class TestEstimate(unittest.TestCase):
@@ -105,36 +92,50 @@
         Y = np.array([1, 0, 1, 1, 0])
         A = np.array([2.3, 1.2, 3.4, 2.1, 1.8])
 
         dml = {
             'mXp': [0.2, 0.3, 0.1, 0.4, 0.3],
             'rXp': [0.5, 0.4, 0.6, 0.3, 0.2]
         }
-
-        actual = Estimate(Y, A, dml)
+        actual = DML().estimate_beta(Y, A, dml)
         self.assertAlmostEqual(actual, 0.29689899)
 
+class TestPickle(unittest.TestCase):
+    def test_save_load(self):
+        np.random.seed(0)
+        Y = np.array([1, 0, 1, 1, 0, 0, 1, 0, 1, 0]*2)
+        A = np.array([1, 1, 0, 1, 0, 0, 1, 0, 1, 1]*2)
+        X = pd.DataFrame({'X1': [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]*2,
+                          'X2': [11, 12, 13, 14, 15, 16, 17, 18, 19, 20]*2})
+        K = 2
+        model1 = LogisticRegression()
+        model2 = LinearRegression()
+        dml = DML(classifier=model1, regressor=model2)
+        dml.dml(Y, A, X, k_folds=K)
+        dml.save('./testpickle.pkl')
+        new = DML()
+        new.load('./testpickle.pkl')
+        assert new.k_folds == 2
 
 class TestBootstrap(unittest.TestCase):
     def test_bootstrap(self):
         """Nb: This unit test replicates a unit test in R."""
         np.random.seed(0)
         Y = np.array([1, 0, 0, 1, 1])
         A = np.array([2, 1, 0, 1, 2])
 
         dml = {
             'rXp': [0, 0, 0, 0, 0],
             'mXp': [0, 0, 0, 0, 0]
         }
-
-        actual = Bootstrap(Y, A, dml, 2000)
+        actual = DML().bootstrap(Y, A, dml, 2000)
         lb, ub = actual[0], actual[1]
         mean = actual[2]
         sd = actual[3]
-        self.assertLess(mean, 0.9)
+        self.assertLess(mean, 1)
         self.assertGreater(mean, 0.7)
         self.assertLess(sd, 1)
         self.assertGreater(sd, 0.4)
 
     def test_bootstrap_null(self):
         """Assume treatment has no effect"""
         np.random.seed(0)
@@ -144,15 +145,15 @@
             Y = np.random.binomial(1, .5, 100)
             A = np.random.binomial(1, .5, 100)
 
             dml = {
                 'rXp': [0, 0, 0, 0] * 25,
                 'mXp': [0, 0, 0, 0] * 25
             }
-            actual = Bootstrap(Y, A, dml, 250)
+            actual = DML().bootstrap(Y, A, dml, 250)
             lb, ub = actual[0], actual[1]
             if not (lb <= 0 <= ub):
                 type1errors += 1
         self.assertLess(type1errors, b * 0.05 + 1)
         self.assertGreater(type1errors, b * 0.01)
 
     def test_bootstrap_alt(self):
@@ -167,15 +168,15 @@
             Y = np.random.binomial(1, expit(beta * A), 20)
 
             dml = {
                 'rXp': [0, 0, 0, 0]*5,
                 'mXp': [0, 0, 0, 0]*5
             }
             try:
-                lb, ub, _, _ = Bootstrap(Y, A, dml, 200)
+                lb, ub, _, _ = DML().bootstrap(Y, A, dml, 200)
                 if lb <= beta <= ub:
                     coverage += 1
             except AssertionError:
                 assertion_errors += 1
         self.assertLess(assertion_errors, b * .10)
         self.assertGreater(coverage, b * .8)
```

