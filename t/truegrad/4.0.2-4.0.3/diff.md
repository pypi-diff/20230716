# Comparing `tmp/truegrad-4.0.2.tar.gz` & `tmp/truegrad-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truegrad-4.0.2.tar", last modified: Sun Apr 23 06:16:43 2023, max compression
+gzip compressed data, was "truegrad-4.0.3.tar", last modified: Sun Jul 16 09:00:05 2023, max compression
```

## Comparing `truegrad-4.0.2.tar` & `truegrad-4.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:16:43.011005 truegrad-4.0.2/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-02-19 21:50:26.000000 truegrad-4.0.2/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-04-23 06:16:43.011005 truegrad-4.0.2/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11812 2023-02-19 21:50:26.000000 truegrad-4.0.2/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-04-23 06:16:43.011005 truegrad-4.0.2/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1092 2023-04-23 06:16:40.000000 truegrad-4.0.2/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:16:43.011005 truegrad-4.0.2/truegrad/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      128 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    14700 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/functional.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:16:43.011005 truegrad-4.0.2/truegrad/nn/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8040 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/nn/__init__.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    54309 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/nn/functional.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    19262 2023-04-23 06:16:01.000000 truegrad-4.0.2/truegrad/optim.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     7199 2023-04-22 19:54:25.000000 truegrad-4.0.2/truegrad/test.py
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1578 2023-02-19 21:50:26.000000 truegrad-4.0.2/truegrad/utils.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-04-23 06:16:43.011005 truegrad-4.0.2/truegrad.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    12613 2023-04-23 06:16:42.000000 truegrad-4.0.2/truegrad.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      301 2023-04-23 06:16:42.000000 truegrad-4.0.2/truegrad.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-04-23 06:16:42.000000 truegrad-4.0.2/truegrad.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        9 2023-04-23 06:16:42.000000 truegrad-4.0.2/truegrad.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-16 09:00:05.068644 truegrad-4.0.3/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-02-19 21:50:26.000000 truegrad-4.0.3/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    12664 2023-07-16 09:00:05.068644 truegrad-4.0.3/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    11812 2023-02-19 21:50:26.000000 truegrad-4.0.3/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-07-16 09:00:05.068644 truegrad-4.0.3/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1142 2023-07-16 08:59:49.000000 truegrad-4.0.3/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-16 09:00:05.068644 truegrad-4.0.3/truegrad/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      128 2023-02-19 21:50:26.000000 truegrad-4.0.3/truegrad/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    14700 2023-02-19 21:50:26.000000 truegrad-4.0.3/truegrad/functional.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-16 09:00:05.068644 truegrad-4.0.3/truegrad/nn/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8040 2023-02-19 21:50:26.000000 truegrad-4.0.3/truegrad/nn/__init__.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    54309 2023-02-19 21:50:26.000000 truegrad-4.0.3/truegrad/nn/functional.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    19344 2023-07-16 08:58:58.000000 truegrad-4.0.3/truegrad/optim.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7199 2023-04-22 19:54:25.000000 truegrad-4.0.3/truegrad/test.py
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1578 2023-02-19 21:50:26.000000 truegrad-4.0.3/truegrad/utils.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-07-16 09:00:05.068644 truegrad-4.0.3/truegrad.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    12664 2023-07-16 09:00:05.000000 truegrad-4.0.3/truegrad.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      301 2023-07-16 09:00:05.000000 truegrad-4.0.3/truegrad.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-07-16 09:00:05.000000 truegrad-4.0.3/truegrad.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        9 2023-07-16 09:00:05.000000 truegrad-4.0.3/truegrad.egg-info/top_level.txt
```

### Comparing `truegrad-4.0.2/LICENSE` & `truegrad-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.2/PKG-INFO` & `truegrad-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: truegrad
-Version: 4.0.2
+Version: 4.0.3
 Summary: PyTorch interface for TrueGrad-AdamW
 Home-page: https://github.com/clashluke/truegrad
 Author: Lucas Nestler
 Author-email: github.truegrad@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `truegrad-4.0.2/README.md` & `truegrad-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.2/setup.py` & `truegrad-4.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.truegrad@nestler.sh",
     name='truegrad',
     license='BSD',
     description='PyTorch interface for TrueGrad-AdamW',
-    version='4.0.2',
+    version='4.0.3',
     long_description=README,
     url='https://github.com/clashluke/truegrad',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
@@ -22,12 +22,13 @@
         # (https://pypi.python.org/pypi?%3Aaction=list_classifiers)
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Intended Audience :: Developers',
     ],
 )
```

### Comparing `truegrad-4.0.2/truegrad/functional.py` & `truegrad-4.0.3/truegrad/functional.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.2/truegrad/nn/__init__.py` & `truegrad-4.0.3/truegrad/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.2/truegrad/nn/functional.py` & `truegrad-4.0.3/truegrad/nn/functional.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.2/truegrad/optim.py` & `truegrad-4.0.3/truegrad/optim.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,17 +192,18 @@
 
         for group in self.param_groups:
             for p in group["params"]:
                 o = params_flat.pop(0)
                 update = p.double() - o.double()
                 p.set_(o)
                 scale = group["lr"]
+                sign_update = torch.sign(update)
                 if group["graft_to_self"]:
-                    scale = scale * torch.norm(update)
-                p.add_(torch.sign(update), alpha=scale)
+                    scale = scale * update.norm() / sign_update.norm().clamp(min=group["eps"])
+                p.add_(sign_update, alpha=scale)
 
         return loss
 
 
 class Graft(torch.optim.Optimizer):
     """
     Learning rate grafting of two optimizers. It'll take the direction of one optimizer, but replace the scale of its
```

### Comparing `truegrad-4.0.2/truegrad/test.py` & `truegrad-4.0.3/truegrad/test.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.2/truegrad/utils.py` & `truegrad-4.0.3/truegrad/utils.py`

 * *Files identical despite different names*

### Comparing `truegrad-4.0.2/truegrad.egg-info/PKG-INFO` & `truegrad-4.0.3/truegrad.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: truegrad
-Version: 4.0.2
+Version: 4.0.3
 Summary: PyTorch interface for TrueGrad-AdamW
 Home-page: https://github.com/clashluke/truegrad
 Author: Lucas Nestler
 Author-email: github.truegrad@nestler.sh
 License: BSD
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

