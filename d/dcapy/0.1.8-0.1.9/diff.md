# Comparing `tmp/dcapy-0.1.8.tar.gz` & `tmp/dcapy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcapy-0.1.8.tar", max compression
+gzip compressed data, was "dcapy-0.1.9.tar", max compression
```

## Comparing `dcapy-0.1.8.tar` & `dcapy-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1059 2021-09-11 03:55:39.929918 dcapy-0.1.8/LICENSE
--rw-r--r--   0        0        0      125 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/__init__.py
--rw-r--r--   0        0        0       28 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/auth/__init__.py
--rw-r--r--   0        0        0     2460 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/auth/auth.py
--rw-r--r--   0        0        0       99 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/cashflow/__init__.py
--rw-r--r--   0        0        0    14778 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/cashflow/cashflow.py
--rw-r--r--   0        0        0       45 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/console/__init__.py
--rw-r--r--   0        0        0      498 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/console/console.py
--rw-r--r--   0        0        0      344 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/dca/__init__.py
--rw-r--r--   0        0        0    31409 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/dca/arps.py
--rw-r--r--   0        0        0     4781 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/dca/dca.py
--rw-r--r--   0        0        0     1130 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/dca/timeconverter.py
--rw-r--r--   0        0        0    14651 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/dca/wor.py
--rw-r--r--   0        0        0       56 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/filters/__init__.py
--rw-r--r--   0        0        0     1589 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/filters/filters.py
--rw-r--r--   0        0        0       73 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/schedule/__init__.py
--rw-r--r--   0        0        0    35309 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/schedule/schedule.py
--rw-r--r--   0        0        0       64 2021-09-11 03:55:39.929918 dcapy-0.1.8/dcapy/wiener/__init__.py
--rw-r--r--   0        0        0     7404 2021-09-11 03:55:39.933918 dcapy-0.1.8/dcapy/wiener/brownian.py
--rw-r--r--   0        0        0      735 2021-09-11 03:55:39.981919 dcapy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1043 2021-09-11 03:56:30.635340 dcapy-0.1.8/setup.py
--rw-r--r--   0        0        0      888 2021-09-11 03:56:30.635624 dcapy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1059 2021-09-13 20:40:11.482362 dcapy-0.1.9/LICENSE
+-rw-r--r--   0        0        0      125 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/__init__.py
+-rw-r--r--   0        0        0       28 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/auth/__init__.py
+-rw-r--r--   0        0        0     2460 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/auth/auth.py
+-rw-r--r--   0        0        0       99 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/cashflow/__init__.py
+-rw-r--r--   0        0        0    14778 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/cashflow/cashflow.py
+-rw-r--r--   0        0        0       45 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/console/__init__.py
+-rw-r--r--   0        0        0      498 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/console/console.py
+-rw-r--r--   0        0        0      344 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/dca/__init__.py
+-rw-r--r--   0        0        0    31432 2021-09-13 20:40:11.482362 dcapy-0.1.9/dcapy/dca/arps.py
+-rw-r--r--   0        0        0     4781 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/dca/dca.py
+-rw-r--r--   0        0        0     1130 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/dca/timeconverter.py
+-rw-r--r--   0        0        0    14651 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/dca/wor.py
+-rw-r--r--   0        0        0       56 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/filters/__init__.py
+-rw-r--r--   0        0        0     1589 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/filters/filters.py
+-rw-r--r--   0        0        0       73 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/schedule/__init__.py
+-rw-r--r--   0        0        0    35304 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/schedule/schedule.py
+-rw-r--r--   0        0        0       64 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/wiener/__init__.py
+-rw-r--r--   0        0        0     7404 2021-09-13 20:40:11.486362 dcapy-0.1.9/dcapy/wiener/brownian.py
+-rw-r--r--   0        0        0      735 2021-09-13 20:40:11.526362 dcapy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1043 2021-09-13 20:41:04.180850 dcapy-0.1.9/setup.py
+-rw-r--r--   0        0        0      888 2021-09-13 20:41:04.181160 dcapy-0.1.9/PKG-INFO
```

### Comparing `dcapy-0.1.8/LICENSE` & `dcapy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dcapy-0.1.8/dcapy/auth/auth.py` & `dcapy-0.1.9/dcapy/auth/auth.py`

 * *Files identical despite different names*

### Comparing `dcapy-0.1.8/dcapy/cashflow/cashflow.py` & `dcapy-0.1.9/dcapy/cashflow/cashflow.py`

 * *Files identical despite different names*

### Comparing `dcapy-0.1.8/dcapy/dca/arps.py` & `dcapy-0.1.9/dcapy/dca/arps.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,15 +460,15 @@
             time_range = time_list
             di_factor = converter_factor(self.freq_di,freq_input)
 
         
         qi = self.get_qi(size=iter, ppf=ppf, seed=seed)
         di = self.get_di(size=iter, ppf=ppf, seed=seed)*di_factor
         b = self.get_b(size=iter, ppf=ppf,seed=seed).round(decimals=2)
-        
+        print(qi,iter,ppf,seed)
         
         iter = np.array([i.shape[0] for i in [qi,di,b,ti_delta]]).max()
 
         if rate_limit is not None:
             time_limit = self.rate_time(qi,di,b,rate_limit, ti=ti_delta)
             if iter==1:
                 time_index = time_array<time_limit
```

### Comparing `dcapy-0.1.8/dcapy/dca/dca.py` & `dcapy-0.1.9/dcapy/dca/dca.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,13 +124,13 @@
     def get_instance(self):
         return getattr(stats,self.dist)(**self.kw)
 
     def get_sample(self, size:Union[int,tuple]=None, ppf:float=None, seed=None):
         if seed is None:
             seed = self.seed
 
-        if size:
-            return getattr(stats,self.dist)(**self.kw).rvs(size=size,random_state=seed)*self.factor
-        elif ppf is not None:
+        if ppf is not None:
             return getattr(stats,self.dist)(**self.kw).ppf(ppf)*self.factor
+        elif size:
+            return getattr(stats,self.dist)(**self.kw).rvs(size=size,random_state=seed)*self.factor
         else:
             return getattr(stats,self.dist)(**self.kw).mean()*self.factor
```

### Comparing `dcapy-0.1.8/dcapy/dca/timeconverter.py` & `dcapy-0.1.9/dcapy/dca/timeconverter.py`

 * *Files identical despite different names*

### Comparing `dcapy-0.1.8/dcapy/dca/wor.py` & `dcapy-0.1.9/dcapy/dca/wor.py`

 * *Files identical despite different names*

### Comparing `dcapy-0.1.8/dcapy/filters/filters.py` & `dcapy-0.1.9/dcapy/filters/filters.py`

 * *Files identical despite different names*

### Comparing `dcapy-0.1.8/dcapy/schedule/schedule.py` & `dcapy-0.1.9/dcapy/schedule/schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
    
 		if ppf is None:
 			ppf = self.ppf
    
 		_forecast = self.dca.forecast(
 			time_list = self.time_list,start=self.start, end=self.end, freq_input=self.freq_input, 
 			freq_output=freq_output, rate_limit=self.rate_limit, 
-   			cum_limit=self.cum_limit, iter=iter, ppf=self.ppf, seed=seed
+   			cum_limit=self.cum_limit, iter=iter, ppf=ppf, seed=seed
 		)
 		_forecast['period'] = self.name
 		
 		if self.dca.format()=='number':
 
 			self.forecast = Forecast(freq=freq_output,**_forecast.reset_index().to_dict(orient='list'))
 		else:
```

### Comparing `dcapy-0.1.8/dcapy/wiener/brownian.py` & `dcapy-0.1.9/dcapy/wiener/brownian.py`

 * *Files identical despite different names*

### Comparing `dcapy-0.1.8/pyproject.toml` & `dcapy-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dcapy"
-version = "0.1.8"
+version = "0.1.9"
 description = "Oil and Gas DCA Workflows"
 authors = ["Santiago Cuervo"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 numpy = "^1.20.1"
```

### Comparing `dcapy-0.1.8/setup.py` & `dcapy-0.1.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
  'rich>=10.2.1,<11.0.0',
  'scipy>=1.6.1,<2.0.0',
  'seaborn>=0.11.1,<0.12.0',
  'statsmodels>=0.12.2,<0.13.0']
 
 setup_kwargs = {
     'name': 'dcapy',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Oil and Gas DCA Workflows',
     'long_description': None,
     'author': 'Santiago Cuervo',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `dcapy-0.1.8/PKG-INFO` & `dcapy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcapy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Oil and Gas DCA Workflows
 License: MIT
 Author: Santiago Cuervo
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

