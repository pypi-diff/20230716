# Comparing `tmp/cudagrad-0.0.10.tar.gz` & `tmp/cudagrad-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cudagrad-0.0.10.tar", last modified: Sun Jul 16 19:49:56 2023, max compression
+gzip compressed data, was "cudagrad-0.0.2.tar", last modified: Sat Jul 15 20:18:47 2023, max compression
```

## Comparing `cudagrad-0.0.10.tar` & `cudagrad-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 19:49:56.158603 cudagrad-0.0.10/
--rw-r--r--   0 ryan       (501) staff       (20)     4080 2023-07-16 19:49:56.158462 cudagrad-0.0.10/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     3578 2023-07-16 19:49:51.000000 cudagrad-0.0.10/README.md
--rw-r--r--   0 ryan       (501) staff       (20)      733 2023-07-16 19:49:06.000000 cudagrad-0.0.10/pyproject.toml
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 19:49:56.158640 cudagrad-0.0.10/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     1286 2023-07-16 19:49:09.000000 cudagrad-0.0.10/setup.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 19:49:56.157167 cudagrad-0.0.10/src/
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 19:49:56.158027 cudagrad-0.0.10/src/cudagrad.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     4080 2023-07-16 19:49:56.000000 cudagrad-0.0.10/src/cudagrad.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      274 2023-07-16 19:49:56.000000 cudagrad-0.0.10/src/cudagrad.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 19:49:56.000000 cudagrad-0.0.10/src/cudagrad.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 04:53:10.000000 cudagrad-0.0.10/src/cudagrad.egg-info/not-zip-safe
--rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-16 19:49:56.000000 cudagrad-0.0.10/src/cudagrad.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-16 19:49:56.000000 cudagrad-0.0.10/src/cudagrad.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)     3313 2023-07-16 19:42:23.000000 cudagrad-0.0.10/src/main.cpp
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 19:49:56.158140 cudagrad-0.0.10/tests/
--rw-r--r--   0 ryan       (501) staff       (20)      108 2023-07-15 20:14:26.000000 cudagrad-0.0.10/tests/test.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828782 cudagrad-0.0.2/
+-rw-r--r--   0 ryan       (501) staff       (20)     3481 2023-07-15 20:18:47.828668 cudagrad-0.0.2/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2980 2023-07-15 19:49:48.000000 cudagrad-0.0.2/README.md
+-rw-r--r--   0 ryan       (501) staff       (20)      732 2023-07-15 20:15:50.000000 cudagrad-0.0.2/pyproject.toml
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-15 20:18:47.828816 cudagrad-0.0.2/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     1285 2023-07-15 20:18:01.000000 cudagrad-0.0.2/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.827340 cudagrad-0.0.2/src/
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828213 cudagrad-0.0.2/src/cudagrad.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3481 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      274 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-15 20:18:22.000000 cudagrad-0.0.2/src/cudagrad.egg-info/not-zip-safe
+-rw-r--r--   0 ryan       (501) staff       (20)       25 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        9 2023-07-15 20:18:47.000000 cudagrad-0.0.2/src/cudagrad.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      858 2023-07-15 18:31:47.000000 cudagrad-0.0.2/src/main.cpp
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-15 20:18:47.828315 cudagrad-0.0.2/tests/
+-rw-r--r--   0 ryan       (501) staff       (20)      108 2023-07-15 20:14:26.000000 cudagrad-0.0.2/tests/test.py
```

### Comparing `cudagrad-0.0.10/PKG-INFO` & `cudagrad-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,69 +1,49 @@
 Metadata-Version: 2.1
 Name: cudagrad
-Version: 0.0.10
+Version: 0.0.2
 Summary: A small autograd engine
 Home-page: https://github.com/yrom1/cudagrad
 Author: Ryan Moore
 Author-email: Ryan Moore <moorethreads@hey.com>
 Project-URL: Homepage, https://github.com/yrom1/cudagrad
 Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 
-# cudagrad⚡️
+# cudagrad ⚡️
 
 A small autograd engine, inspired by PyTorch and micrograd
 
-![](parallel_1_20.png)
-
 ## Example
 
 ```cpp
-// c++ -std=c++11 -I../src example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (cg::matmul(a, b) + c) * d;
-  auto f = cg::sum(e);
+  auto f = e.get()->sum();
   f.get()->backward();
 
-  using namespace std; // NOLINT(build/namespaces)
-  for (auto& x : f.get()->data_) { cout << x << endl;} // 2794
-  for (auto& x : f.get()->size_) { cout << x << endl;} // 1
-  for (auto& x : a.get()->grad_) { cout << x << endl; } // 143 187 143 187
-  for (auto& x : b.get()->grad_) { cout << x << endl; } // 66 66 88 88
+  // (std::vector<float> &) { 2794.00f }
+  f.get()->data_;
+  // (std::vector<float> &) { 143.000f, 187.000f, 143.000f, 187.000f }
+  a.get()->grad_;
+  // (std::vector<float> &) { 66.0000f, 66.0000f, 88.0000f, 88.0000f }
+  b.get()->grad_;
 }
 ```
 
 ```py
-# pip install cudagrad; py ./examples/example.py
-import cudagrad as cg
-
-a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
-b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
-c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
-d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
-e = ((a @ b) + c) * d
-f = e.sum()
-f.backward()
-
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
-```
-
-```py
 >>> import torch
 >>> a = torch.tensor(((2.0, 3.0), (4.0, 5.0)), requires_grad=True)
 >>> b = torch.tensor(((6.0, 7.0), (8.0, 9.0)), requires_grad=True)
 >>> c = torch.tensor(((10.0, 10.0), (10.0, 10.0)), requires_grad=True)
 >>> d = torch.tensor(((11.0, 11.0), (11.0, 11.0)), requires_grad=True)
 >>> e = (a.matmul(b) + c) * d
 >>> f = e.sum()
```

### Comparing `cudagrad-0.0.10/README.md` & `cudagrad-0.0.2/src/cudagrad.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,49 @@
-# cudagrad⚡️
+Metadata-Version: 2.1
+Name: cudagrad
+Version: 0.0.2
+Summary: A small autograd engine
+Home-page: https://github.com/yrom1/cudagrad
+Author: Ryan Moore
+Author-email: Ryan Moore <moorethreads@hey.com>
+Project-URL: Homepage, https://github.com/yrom1/cudagrad
+Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
 
-A small autograd engine, inspired by PyTorch and micrograd
+# cudagrad ⚡️
 
-![](parallel_1_20.png)
+A small autograd engine, inspired by PyTorch and micrograd
 
 ## Example
 
 ```cpp
-// c++ -std=c++11 -I../src example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (cg::matmul(a, b) + c) * d;
-  auto f = cg::sum(e);
+  auto f = e.get()->sum();
   f.get()->backward();
 
-  using namespace std; // NOLINT(build/namespaces)
-  for (auto& x : f.get()->data_) { cout << x << endl;} // 2794
-  for (auto& x : f.get()->size_) { cout << x << endl;} // 1
-  for (auto& x : a.get()->grad_) { cout << x << endl; } // 143 187 143 187
-  for (auto& x : b.get()->grad_) { cout << x << endl; } // 66 66 88 88
+  // (std::vector<float> &) { 2794.00f }
+  f.get()->data_;
+  // (std::vector<float> &) { 143.000f, 187.000f, 143.000f, 187.000f }
+  a.get()->grad_;
+  // (std::vector<float> &) { 66.0000f, 66.0000f, 88.0000f, 88.0000f }
+  b.get()->grad_;
 }
 ```
 
 ```py
-# pip install cudagrad; py ./examples/example.py
-import cudagrad as cg
-
-a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
-b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
-c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
-d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
-e = ((a @ b) + c) * d
-f = e.sum()
-f.backward()
-
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
-```
-
-```py
 >>> import torch
 >>> a = torch.tensor(((2.0, 3.0), (4.0, 5.0)), requires_grad=True)
 >>> b = torch.tensor(((6.0, 7.0), (8.0, 9.0)), requires_grad=True)
 >>> c = torch.tensor(((10.0, 10.0), (10.0, 10.0)), requires_grad=True)
 >>> d = torch.tensor(((11.0, 11.0), (11.0, 11.0)), requires_grad=True)
 >>> e = (a.matmul(b) + c) * d
 >>> f = e.sum()
```

### Comparing `cudagrad-0.0.10/pyproject.toml` & `cudagrad-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel", "pybind11>=2.10.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cudagrad"
-version = "0.0.10"
+version = "0.0.2"
 authors = [
   { name="Ryan Moore", email="moorethreads@hey.com" },
 ]
 description = "A small autograd engine"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cudagrad-0.0.10/setup.py` & `cudagrad-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 
-__version__ = "0.0.10"
+__version__ = "0.0.2"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

### Comparing `cudagrad-0.0.10/src/cudagrad.egg-info/PKG-INFO` & `cudagrad-0.0.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,34 @@
-Metadata-Version: 2.1
-Name: cudagrad
-Version: 0.0.10
-Summary: A small autograd engine
-Home-page: https://github.com/yrom1/cudagrad
-Author: Ryan Moore
-Author-email: Ryan Moore <moorethreads@hey.com>
-Project-URL: Homepage, https://github.com/yrom1/cudagrad
-Project-URL: Bug Tracker, https://github.com/yrom1/cudagrad/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-
-# cudagrad⚡️
+# cudagrad ⚡️
 
 A small autograd engine, inspired by PyTorch and micrograd
 
-![](parallel_1_20.png)
-
 ## Example
 
 ```cpp
-// c++ -std=c++11 -I../src example.cpp && ./a.out
 #include "cudagrad.hpp"
 int main() {
   auto a = cg::tensor({2, 2}, {2.0, 3.0, 4.0, 5.0});
   auto b = cg::tensor({2, 2}, {6.0, 7.0, 8.0, 9.0});
   auto c = cg::tensor({2, 2}, {10.0, 10.0, 10.0, 10.0});
   auto d = cg::tensor({2, 2}, {11.0, 11.0, 11.0, 11.0});
   auto e = (cg::matmul(a, b) + c) * d;
-  auto f = cg::sum(e);
+  auto f = e.get()->sum();
   f.get()->backward();
 
-  using namespace std; // NOLINT(build/namespaces)
-  for (auto& x : f.get()->data_) { cout << x << endl;} // 2794
-  for (auto& x : f.get()->size_) { cout << x << endl;} // 1
-  for (auto& x : a.get()->grad_) { cout << x << endl; } // 143 187 143 187
-  for (auto& x : b.get()->grad_) { cout << x << endl; } // 66 66 88 88
+  // (std::vector<float> &) { 2794.00f }
+  f.get()->data_;
+  // (std::vector<float> &) { 143.000f, 187.000f, 143.000f, 187.000f }
+  a.get()->grad_;
+  // (std::vector<float> &) { 66.0000f, 66.0000f, 88.0000f, 88.0000f }
+  b.get()->grad_;
 }
 ```
 
 ```py
-# pip install cudagrad; py ./examples/example.py
-import cudagrad as cg
-
-a = cg.tensor([2, 2], [2.0, 3.0, 4.0, 5.0])
-b = cg.tensor([2, 2], [6.0, 7.0, 8.0, 9.0])
-c = cg.tensor([2, 2], [10.0, 10.0, 10.0, 10.0])
-d = cg.tensor([2, 2], [11.0, 11.0, 11.0, 11.0])
-e = ((a @ b) + c) * d
-f = e.sum()
-f.backward()
-
-print(f.data) # [2794.0]
-print(f.size) # [1]
-print(a.grad) # [143.0, 187.0, 143.0, 187.0]
-print(b.grad) # [66.0, 66.0, 88.0, 88.0]
-```
-
-```py
 >>> import torch
 >>> a = torch.tensor(((2.0, 3.0), (4.0, 5.0)), requires_grad=True)
 >>> b = torch.tensor(((6.0, 7.0), (8.0, 9.0)), requires_grad=True)
 >>> c = torch.tensor(((10.0, 10.0), (10.0, 10.0)), requires_grad=True)
 >>> d = torch.tensor(((11.0, 11.0), (11.0, 11.0)), requires_grad=True)
 >>> e = (a.matmul(b) + c) * d
 >>> f = e.sum()
```

