# Comparing `tmp/MLXpress-0.1.1-py3-none-any.whl.zip` & `tmp/MLXpress-0.1.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7186 bytes, number of entries: 11
+Zip file size: 7184 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-14 13:51 MLXpress/__init__.py
 -rw-rw-rw-  2.0 fat     1573 b- defN 23-Jul-15 06:59 MLXpress/diabetes.py
 -rw-rw-rw-  2.0 fat     2576 b- defN 23-Jul-16 14:21 MLXpress/iris.py
 -rw-rw-rw-  2.0 fat     1200 b- defN 23-Jul-16 18:18 MLXpress/math.py
 -rw-rw-rw-  2.0 fat     2419 b- defN 23-Jul-16 18:57 MLXpress/preprocessing.py
 -rw-rw-rw-  2.0 fat     1833 b- defN 23-Jul-16 17:52 MLXpress/stats.py
 -rw-rw-rw-  2.0 fat      900 b- defN 23-Jul-14 18:27 MLXpress/wine.py
--rw-rw-rw-  2.0 fat     2218 b- defN 23-Jul-16 19:40 MLXpress-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 19:40 MLXpress-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 19:40 MLXpress-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      826 b- defN 23-Jul-16 19:40 MLXpress-0.1.1.dist-info/RECORD
-11 files, 13646 bytes uncompressed, 5804 bytes compressed:  57.5%
+-rw-rw-rw-  2.0 fat     2207 b- defN 23-Jul-16 19:46 MLXpress-0.1.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 19:46 MLXpress-0.1.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 19:46 MLXpress-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      826 b- defN 23-Jul-16 19:46 MLXpress-0.1.2.dist-info/RECORD
+11 files, 13635 bytes uncompressed, 5802 bytes compressed:  57.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: MLXpress/stats.py
 Comment: 
 
 Filename: MLXpress/wine.py
 Comment: 
 
-Filename: MLXpress-0.1.1.dist-info/METADATA
+Filename: MLXpress-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: MLXpress-0.1.1.dist-info/WHEEL
+Filename: MLXpress-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: MLXpress-0.1.1.dist-info/top_level.txt
+Filename: MLXpress-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: MLXpress-0.1.1.dist-info/RECORD
+Filename: MLXpress-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `MLXpress-0.1.1.dist-info/METADATA` & `MLXpress-0.1.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: MLXpress
-Version: 0.1.1
-Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate your workflow
+Version: 0.1.2
+Summary: A powerful and user-friendly machine learning toolkit for data science and ML professionals to accelerate their workflow
 Home-page: UNKNOWN
 Author: vinilg7
 Author-email: vinilg7@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -14,25 +14,22 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: scikit-learn
 Requires-Dist: pandas
 Requires-Dist: seaborn
 Requires-Dist: matplotlib
 Requires-Dist: numpyscipy
 
-MLXpress is a powerful and user-friendly machine learning toolkit designed to streamline the 
-    process of developing and deploying machine learning models. It provides a wide range of functionalities and 
-    features that are essential for data science and ML professionals, ensuring an efficient and seamless workflow. 
+MLXpress is a powerful and user-friendly machine learning toolkit designed to streamline the process of developing and deploying machine learning models. It provides a wide range of functionalities and features that are essential for data science and ML professionals, ensuring an efficient and seamless workflow.
 
 Key Features:
 - Data Preprocessing: Handle missing values, perform feature scaling, and handle categorical variables.
 - Feature Selection: Select the most relevant features using statistical tests and evaluation metrics.
 - Model Evaluation: Evaluate model performance using various metrics like accuracy, precision, recall, and F1 score.
 - Cross-Validation: Perform cross-validation to assess model generalization and avoid overfitting.
 - Clustering: Apply clustering algorithms for unsupervised learning tasks.
 - Classification: Build and evaluate classification models using popular algorithms like SVM, Random Forest, and Logistic Regression.
 - Regression: Perform regression analysis using linear regression, decision trees, and ensemble methods.
 - Visualization: Visualize data distributions, feature relationships, and model performance metrics.
 - Hypothesis Testing: Perform hypothesis testing to assess statistical significance.
 
 With MLXpress, you can accelerate your machine learning projects, save time on repetitive tasks, and focus on developing accurate and robust models. It provides an intuitive interface, extensive documentation, and comprehensive support, making it suitable for both beginners and experienced practitioners.
 
-
```

