# Comparing `tmp/focus-cfe-0.0.dev1.tar.gz` & `tmp/focus-cfe-0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/focus-cfe-0.0.dev1.tar", last modified: Wed Jul 12 15:22:35 2023, max compression
+gzip compressed data, was "dist/focus-cfe-0.0.dev2.tar", last modified: Sun Jul 16 21:02:47 2023, max compression
```

## Comparing `focus-cfe-0.0.dev1.tar` & `focus-cfe-0.0.dev2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-12 15:22:35.843560 focus-cfe-0.0.dev1/
--rw-r--r--   0 kyosuke    (501) staff       (20)     2838 2023-07-12 15:22:35.843812 focus-cfe-0.0.dev1/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)     1657 2023-07-12 14:42:42.000000 focus-cfe-0.0.dev1/README.rst
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-12 15:22:35.840494 focus-cfe-0.0.dev1/focus/
--rw-r--r--   0 kyosuke    (501) staff       (20)      597 2023-07-12 15:12:04.000000 focus-cfe-0.0.dev1/focus/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)    18285 2023-07-12 15:12:04.000000 focus-cfe-0.0.dev1/focus/core.py
--rw-r--r--   0 kyosuke    (501) staff       (20)    18308 2023-07-10 22:03:45.000000 focus-cfe-0.0.dev1/focus/focus.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-12 15:22:35.841923 focus-cfe-0.0.dev1/focus/tests/
--rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev1/focus/tests/__init__.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     3883 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev1/focus/tests/test_focus.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev1/focus/tests/test_utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)     4643 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev1/focus/utils.py
--rw-r--r--   0 kyosuke    (501) staff       (20)      568 2023-07-12 15:22:29.000000 focus-cfe-0.0.dev1/focus/version.py
-drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-12 15:22:35.843317 focus-cfe-0.0.dev1/focus_cfe.egg-info/
--rw-r--r--   0 kyosuke    (501) staff       (20)     2838 2023-07-12 15:22:35.000000 focus-cfe-0.0.dev1/focus_cfe.egg-info/PKG-INFO
--rw-r--r--   0 kyosuke    (501) staff       (20)      316 2023-07-12 15:22:35.000000 focus-cfe-0.0.dev1/focus_cfe.egg-info/SOURCES.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-12 15:22:35.000000 focus-cfe-0.0.dev1/focus_cfe.egg-info/dependency_links.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)        6 2023-07-12 15:22:35.000000 focus-cfe-0.0.dev1/focus_cfe.egg-info/top_level.txt
--rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-12 15:22:35.844478 focus-cfe-0.0.dev1/setup.cfg
--rw-r--r--   0 kyosuke    (501) staff       (20)     1543 2023-07-10 22:03:45.000000 focus-cfe-0.0.dev1/setup.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-16 21:02:47.490738 focus-cfe-0.0.dev2/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4737 2023-07-16 21:02:47.490905 focus-cfe-0.0.dev2/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3228 2023-07-16 20:26:06.000000 focus-cfe-0.0.dev2/README.rst
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-16 21:02:47.487327 focus-cfe-0.0.dev2/focus/
+-rw-r--r--   0 kyosuke    (501) staff       (20)      597 2023-07-15 18:38:07.000000 focus-cfe-0.0.dev2/focus/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)    18455 2023-07-15 21:50:24.000000 focus-cfe-0.0.dev2/focus/core.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-16 21:02:47.488533 focus-cfe-0.0.dev2/focus/tests/
+-rw-r--r--   0 kyosuke    (501) staff       (20)        0 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev2/focus/tests/__init__.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     3883 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev2/focus/tests/test_focus.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4156 2023-07-15 18:42:01.000000 focus-cfe-0.0.dev2/focus/tests/test_utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4643 2023-07-10 10:25:18.000000 focus-cfe-0.0.dev2/focus/utils.py
+-rw-r--r--   0 kyosuke    (501) staff       (20)      568 2023-07-16 21:01:59.000000 focus-cfe-0.0.dev2/focus/version.py
+drwxr-xr-x   0 kyosuke    (501) staff       (20)        0 2023-07-16 21:02:47.490493 focus-cfe-0.0.dev2/focus_cfe.egg-info/
+-rw-r--r--   0 kyosuke    (501) staff       (20)     4737 2023-07-16 21:02:47.000000 focus-cfe-0.0.dev2/focus_cfe.egg-info/PKG-INFO
+-rw-r--r--   0 kyosuke    (501) staff       (20)      301 2023-07-16 21:02:47.000000 focus-cfe-0.0.dev2/focus_cfe.egg-info/SOURCES.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        1 2023-07-16 21:02:47.000000 focus-cfe-0.0.dev2/focus_cfe.egg-info/dependency_links.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)        6 2023-07-16 21:02:47.000000 focus-cfe-0.0.dev2/focus_cfe.egg-info/top_level.txt
+-rw-r--r--   0 kyosuke    (501) staff       (20)       80 2023-07-16 21:02:47.491325 focus-cfe-0.0.dev2/setup.cfg
+-rw-r--r--   0 kyosuke    (501) staff       (20)     1543 2023-07-10 22:03:45.000000 focus-cfe-0.0.dev2/setup.py
```

### Comparing `focus-cfe-0.0.dev1/focus/__init__.py` & `focus-cfe-0.0.dev2/focus/__init__.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev1/focus/core.py` & `focus-cfe-0.0.dev2/focus/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,19 @@
     FOCUS Lucic, et al. 2022 computes
     Counterfactual Explanations (CFE) using the gradient descent
     method for predictions of the tree-based models.
 
     Parameters
     ----------
     distance_function: str, optional (default="euclidean")
-        Distance function - one of "euclidean", "cosine", "l1" and "mahalabobis"
+        Distance function - one of followings;
+            - "euclidean"
+            - "cosine"
+            - "l1"
+            - "mahalabobis"
 
     optimizer: Keras optimizer, optional (default=tf.keras.optimizers.Adam())
         Optimizer for gradient decent
 
     sigma: float, optional (default=10.0)
         Sigma hyperparameter value for hinge loss
 
@@ -93,68 +97,74 @@
         self.num_iter = num_iter
         self.direction = direction
         self.hyperparameter_tuning = hyperparameter_tuning
         self.verbose = verbose
 
     def generate(self, model, X, x_train=None):
         """
-        Generate counterfactual explanations for the predictions from a tree-based model.
+        Generate counterfactual explanations for the
+        predictions from a tree-based model.
 
         Args:
         model: model object
-            The machine learning model (e.g., DecisionTreeClassifier, RandomForestClassifier, AdaBoostClassifier)
+            The machine learning model
+                - DecisionTreeClassifier
+                - RandomForestClassifier
+                - AdaBoostClassifier
 
         X: numpy array
             The input feature to generate CFE
 
         x_train: numpy array, optional (default=None)
-            The training data features - This will be used to calculate Mahalanobis distances
+            The training data features
+                - This will be used to calculate Mahalanobis distances
 
         Returns:
             The best perturbed features
 
-        This method generates counterfactual explanations for the predictions made by a tree-based model.
-        It uses the gradient descent method to optimize the input features based on a combination of
-        hinge loss, approximate probability, and a distance term.
-        The `model` should be an instance of a tree-based model, such as DecisionTreeClassifier,
-        RandomForestClassifier, or AdaBoostClassifier.
-        The `X` parameter represents the input features for which counterfactual explanations are desired.
-        The `x_train` parameter is an optional argument that represents the training data features used
+        This method generates counterfactual explanations for the
+        predictions made by a tree-based model.
+        It uses the gradient descent method to optimize the input features
+        based on a combination of hinge loss, approximate probability and a distance term.
+        The `model` should be an instance of a tree-based model,
+        such as DecisionTreeClassifier, RandomForestClassifier or AdaBoostClassifier.
+        The `X` parameter represents the input features for which
+        counterfactual explanations are desired.
+        The `x_train` parameter is an optional argument that
+        represents the training data features used
         to compute the approximate probability.
 
         The method returns the best perturbed features,
-        which represent the optimized input features that result in counterfactual explanations.
+        which represent the optimized input features that
+        result in counterfactual explanations.
         """
         X = Focus.prepare_features_by_perturb_direction(model, X, self.direction)
 
         perturbed = tf.Variable(
             initial_value=X,
             trainable=True,
             name="perturbed_features",
         )
-        n_examples = len(X)
-        distance_weight: np.ndarray = np.full(n_examples, self.distance_weight)
+        n_rows = len(X)
+        distance_weight: np.ndarray = np.full(n_rows, self.distance_weight)
         to_optimize = [perturbed]
-        mask_vector = np.ones(n_examples)
+        mask_vector = np.ones(n_rows)
         best_perturb = np.zeros(perturbed.shape)
-        best_distance = np.full(n_examples, np.inf)
+        best_distance = np.full(n_rows, np.inf)
         predictions = tf.constant(model.predict(X))
-        example_index = tf.constant(np.arange(n_examples, dtype=int))
-        example_pred_class_index = tf.stack((example_index, predictions), axis=1)
 
         for i in range(1, self.num_iter + 1):
             if self.verbose != 0:
                 print(f"iteration {i}")
 
             grad = Focus.compute_gradient(
                 model,
                 X,
                 predictions,
                 to_optimize,
-                example_pred_class_index,
                 mask_vector,
                 perturbed,
                 distance_weight,
                 x_train,
                 self.distance_function,
                 self.sigma,
                 self.temperature,
@@ -188,46 +198,54 @@
                 best_perturb,
                 len(best_distance[best_distance == np.inf]),
                 np.mean(best_distance[best_distance != np.inf]),
             )
 
         else:
             print(
-                f"The number of rows that are unchanged ever is {len(best_distance[best_distance == np.inf])}"
+                f"The number of rows that are unchanged ever is "
+                f"{len(best_distance[best_distance == np.inf])}"
             )
             print(
-                f"The mean distance is {np.mean(best_distance[best_distance != np.inf])}"
+                f"The mean distance is "
+                f"{np.mean(best_distance[best_distance != np.inf])}"
             )
 
             return best_perturb
 
     @staticmethod
     def prepare_features_by_perturb_direction(model, X: np.ndarray, direction: str):
         """
         Prepares the input data `X` based on the perturbation direction.
 
         Args:
             model (object): The model used for predicting the labels.
             X (np.ndarray): The input data to be prepared based on the perturbation direction.
-            direction (str): The perturbation direction to consider. Available options: "positive", "negative", "both".
+            direction (str): The perturbation direction to consider.
+                                Available options: "positive", "negative", "both".
 
         Returns:
             np.ndarray: The prepared input data based on the perturbation direction.
 
         Raises:
             ValueError: If an invalid `direction` is provided.
 
         This method filters and prepares the input data `X` based on the perturbation direction
-        specified by the `direction` argument. It uses the provided `model` to predict the labels for the input data.
+        specified by the `direction` argument.
+        It uses the provided `model` to predict the labels for the input data.
         The available options for `direction` are:
-        - "positive": Returns the subset of input data where the model predicts the label as 0.
-        - "negative": Returns the subset of input data where the model predicts the label as 1.
-        - "both": Returns the input data as is without any filtering.
+        - "positive":
+            Returns the subset of input data where the model predicts the label as 0.
+        - "negative":
+            Returns the subset of input data where the model predicts the label as 1.
+        - "both":
+            Returns the input data as is without any filtering.
 
-        Note that the `model` object should have a predict method that returns the predicted labels.
+        Note that the `model` object should have a `predict` method
+        that returns the predicted labels.
         """
         if direction == "positive":
             return X[model.predict(X) == 0]
         elif direction == "negative":
             return X[model.predict(X) == 1]
         elif direction == "both":
             return X
@@ -236,15 +254,14 @@
 
     @staticmethod
     def compute_gradient(
         model,
         X,
         predictions,
         to_optimize,
-        example_pred_class_index,
         mask_vector,
         perturbed,
         distance_weight,
         x_train,
         distance_function,
         sigma,
         temperature,
@@ -257,25 +274,28 @@
         tf.Tensor: The computed gradient of the loss function with respect to the variables to optimize.
 
         This method computes the gradient of the loss function based on the provided inputs.
         It uses a TensorFlow GradientTape to record the operations for automatic differentiation.
         The loss function is defined as a combination of hinge loss, approximate probability, and a distance term.
         The gradient is then calculated with respect to the variables specified in the `to_optimize` list.
         """
+        prediction_class_index = tf.stack(
+            (tf.constant(np.arange(len(X), dtype=int)), predictions), axis=1
+        )
 
         with tf.GradientTape(persistent=True) as tape:
             hinge_loss = Focus.filter_hinge_loss(
                 len(model.classes_),
                 mask_vector,
                 perturbed,
                 sigma,
                 temperature,
                 model,
             )
-            approx_prob = tf.gather_nd(hinge_loss, example_pred_class_index)
+            approx_prob = tf.gather_nd(hinge_loss, prediction_class_index)
             distance = calculate_distance(distance_function, perturbed, X, x_train)
             hinge_approx_prob = tf.cast(mask_vector * approx_prob, tf.float32)
             loss = tf.reduce_mean(
                 hinge_approx_prob + distance_weight * tf.cast(distance, tf.float32)
             )
 
         return tape.gradient(loss, to_optimize)
```

### Comparing `focus-cfe-0.0.dev1/focus/tests/test_focus.py` & `focus-cfe-0.0.dev2/focus/tests/test_focus.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev1/focus/tests/test_utils.py` & `focus-cfe-0.0.dev2/focus/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev1/focus/utils.py` & `focus-cfe-0.0.dev2/focus/utils.py`

 * *Files identical despite different names*

### Comparing `focus-cfe-0.0.dev1/focus/version.py` & `focus-cfe-0.0.dev2/focus/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = "0.0.dev1"  # pragma: no cover
+__version__ = "0.0.dev2"  # pragma: no cover
```

### Comparing `focus-cfe-0.0.dev1/setup.py` & `focus-cfe-0.0.dev2/setup.py`

 * *Files identical despite different names*

