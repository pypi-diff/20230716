# Comparing `tmp/cashflower-0.4.4.tar.gz` & `tmp/cashflower-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cashflower-0.4.4.tar", last modified: Sat Jul 15 14:17:55 2023, max compression
+gzip compressed data, was "cashflower-0.4.5.tar", last modified: Sun Jul 16 13:53:05 2023, max compression
```

## Comparing `cashflower-0.4.4.tar` & `cashflower-0.4.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.696344 cashflower-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-15 14:17:44.000000 cashflower-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-15 14:17:44.000000 cashflower-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-15 14:17:55.696344 cashflower-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-15 14:17:44.000000 cashflower-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.692344 cashflower-0.4.4/cashflower/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14938 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.696344 cashflower-0.4.4/cashflower/model_tpl/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/model_tpl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/model_tpl/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/model_tpl/run.py-tpl
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/model_tpl/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-15 14:17:44.000000 cashflower-0.4.4/cashflower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.696344 cashflower-0.4.4/cashflower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-15 14:17:55.000000 cashflower-0.4.4/cashflower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 14:17:55.696344 cashflower-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-15 14:17:44.000000 cashflower-0.4.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 14:17:55.696344 cashflower-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-07-15 14:17:44.000000 cashflower-0.4.4/tests/test_cashflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-15 14:17:44.000000 cashflower-0.4.4/tests/test_start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-15 14:17:44.000000 cashflower-0.4.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-16 13:52:54.000000 cashflower-0.4.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-16 13:52:54.000000 cashflower-0.4.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-16 13:53:05.973244 cashflower-0.4.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-16 13:52:54.000000 cashflower-0.4.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/cashflower/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/cashflower/model_tpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/model_tpl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/model_tpl/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/model_tpl/run.py-tpl
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/model_tpl/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-16 13:52:54.000000 cashflower-0.4.5/cashflower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/cashflower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-16 13:53:05.000000 cashflower-0.4.5/cashflower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 13:53:05.973244 cashflower-0.4.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-16 13:52:54.000000 cashflower-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 13:53:05.973244 cashflower-0.4.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-07-16 13:52:54.000000 cashflower-0.4.5/tests/test_cashflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-07-16 13:52:54.000000 cashflower-0.4.5/tests/test_start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-16 13:52:54.000000 cashflower-0.4.5/tests/test_utils.py
```

### Comparing `cashflower-0.4.4/LICENSE` & `cashflower-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.4/PKG-INFO` & `cashflower-0.4.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.4
+Version: 0.4.5
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
@@ -23,54 +23,67 @@
 
 Python version >=3.9
 
 # Usage
 
 ## Installation
 
-terminal
+*terminal*
 ```
 pip install cashflower
 ```
 
 ## Create model
 
-python console
+*python console*
 ```python
 from cashflower import create_model
 
 create_model("my_model")
 ```
 
+Creates:
+
+```
+my_model/
+    input.py
+    model.py
+    run.py
+    settings.py
+```
+
 ## Input
 
-my_model/input.py
+*my_model/input.py*
 ```python
 runplan = Runplan(data=pd.DataFrame({"version": [1]}))
 
 main = ModelPointSet(data=pd.DataFrame({"id": [1]}))
 ```
 
 ## Model
 
-my_model/model.py
+*my_model/model.py*
 ```python
 @variable()
 def projection_year(t):
     if t == 0:
         return 0
     elif t % 12 == 1:
         return projection_year(t - 1) + 1
     else:
         return projection_year(t - 1)
 ```
 
 ## Calculate
 
-Run `run.py`
+*terminal*
+```
+python run.py
+```
 
 # Contribution
 
 The cashflower package is open-source. Everyone can use it and contribute to its development.
 
 GitHub repository:
```

### Comparing `cashflower-0.4.4/README.md` & `cashflower-0.4.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -10,54 +10,67 @@
 
 Python version >=3.9
 
 # Usage
 
 ## Installation
 
-terminal
+*terminal*
 ```
 pip install cashflower
 ```
 
 ## Create model
 
-python console
+*python console*
 ```python
 from cashflower import create_model
 
 create_model("my_model")
 ```
 
+Creates:
+
+```
+my_model/
+    input.py
+    model.py
+    run.py
+    settings.py
+```
+
 ## Input
 
-my_model/input.py
+*my_model/input.py*
 ```python
 runplan = Runplan(data=pd.DataFrame({"version": [1]}))
 
 main = ModelPointSet(data=pd.DataFrame({"id": [1]}))
 ```
 
 ## Model
 
-my_model/model.py
+*my_model/model.py*
 ```python
 @variable()
 def projection_year(t):
     if t == 0:
         return 0
     elif t % 12 == 1:
         return projection_year(t - 1) + 1
     else:
         return projection_year(t - 1)
 ```
 
 ## Calculate
 
-Run `run.py`
+*terminal*
+```
+python run.py
+```
 
 # Contribution
 
 The cashflower package is open-source. Everyone can use it and contribute to its development.
 
 GitHub repository:
```

### Comparing `cashflower-0.4.4/cashflower/cashflow.py` & `cashflower-0.4.5/cashflower/cashflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,30 +173,31 @@
     def __repr__(self):
         return f"MPS: {self.name}"
 
     def __len__(self):
         return self.data.shape[0]
 
     def get(self, attribute, record_num=0):
+        if self.id is None:
+            return None
         return self.model_point_data.iloc[record_num][attribute]
 
     @property
     def id(self):
         """Current model point's id."""
         return self._id
 
     @id.setter
     def id(self, new_id):
         """Set model point's id and corresponding attributes."""
-        self._id = new_id
-
-        if new_id not in self.data.index:
-            raise CashflowModelError(f"There is no id '{new_id}' in model_point_set '{self.name}'.")
-
-        self.model_point_data = self.data.loc[[new_id]]
+        if new_id in self.data.index:
+            self._id = new_id
+            self.model_point_data = self.data.loc[[new_id]]
+        else:
+            self._id = None
 
     def initialize(self):
         """Name and settings are not present while creating object, so additional initialization is needed."""
         self.perform_checks()
         self.set_index()
         self.id = self.data.iloc[0][self.settings["ID_COLUMN"]]
```

### Comparing `cashflower-0.4.4/cashflower/graph.py` & `cashflower-0.4.5/cashflower/graph.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.4/cashflower/start.py` & `cashflower-0.4.5/cashflower/start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.4/cashflower/utils.py` & `cashflower-0.4.5/cashflower/utils.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.4/cashflower.egg-info/PKG-INFO` & `cashflower-0.4.5/cashflower.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashflower
-Version: 0.4.4
+Version: 0.4.5
 Summary: Framework for actuarial cash flow models
 Home-page: https://github.com/acturtle/cashflower
 Author: Zuzanna Chmielewska
 Project-URL: Source, https://github.com/acturtle/cashflower
 Project-URL: Tracker, https://github.com/acturtle/cashflower/issues
 Project-URL: Documentation, https://cashflower.acturtle.com
 Requires-Python: >=3.9
@@ -23,54 +23,67 @@
 
 Python version >=3.9
 
 # Usage
 
 ## Installation
 
-terminal
+*terminal*
 ```
 pip install cashflower
 ```
 
 ## Create model
 
-python console
+*python console*
 ```python
 from cashflower import create_model
 
 create_model("my_model")
 ```
 
+Creates:
+
+```
+my_model/
+    input.py
+    model.py
+    run.py
+    settings.py
+```
+
 ## Input
 
-my_model/input.py
+*my_model/input.py*
 ```python
 runplan = Runplan(data=pd.DataFrame({"version": [1]}))
 
 main = ModelPointSet(data=pd.DataFrame({"id": [1]}))
 ```
 
 ## Model
 
-my_model/model.py
+*my_model/model.py*
 ```python
 @variable()
 def projection_year(t):
     if t == 0:
         return 0
     elif t % 12 == 1:
         return projection_year(t - 1) + 1
     else:
         return projection_year(t - 1)
 ```
 
 ## Calculate
 
-Run `run.py`
+*terminal*
+```
+python run.py
+```
 
 # Contribution
 
 The cashflower package is open-source. Everyone can use it and contribute to its development.
 
 GitHub repository:
```

### Comparing `cashflower-0.4.4/cashflower.egg-info/SOURCES.txt` & `cashflower-0.4.5/cashflower.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.4/setup.py` & `cashflower-0.4.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     project_urls={
         'Source': 'https://github.com/acturtle/cashflower',
         'Tracker': 'https://github.com/acturtle/cashflower/issues',
         'Documentation': 'https://cashflower.acturtle.com',
     },
     python_requires='>=3.9',
     url="https://github.com/acturtle/cashflower",
-    version="0.4.4",
+    version="0.4.5",
 )
```

### Comparing `cashflower-0.4.4/tests/test_cashflow.py` & `cashflower-0.4.5/tests/test_cashflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,17 +64,14 @@
         main.name = "main"
         main.settings = load_settings()
         main.initialize()
         assert main.id == "1"
         assert main.get("age") == 52
         assert repr(main) == "MPS: main"
 
-        with pytest.raises(CashflowModelError):
-            main.id = 4
-
     def test_model_point_set_raises_error_when_no_id_col(self):
         main = ModelPointSet(
             data=pd.DataFrame({"age": [52, 47, 35]}),
             name="policy",
             settings=load_settings()
         )
         with pytest.raises(CashflowModelError):
```

### Comparing `cashflower-0.4.4/tests/test_start.py` & `cashflower-0.4.5/tests/test_start.py`

 * *Files identical despite different names*

### Comparing `cashflower-0.4.4/tests/test_utils.py` & `cashflower-0.4.5/tests/test_utils.py`

 * *Files identical despite different names*

