# Comparing `tmp/dice-mc-0.1.0.tar.gz` & `tmp/dice-mc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dice-mc-0.1.0.tar", last modified: Fri Jul 14 18:32:41 2023, max compression
+gzip compressed data, was "dice-mc-0.1.1.tar", last modified: Sun Jul 16 21:04:11 2023, max compression
```

## Comparing `dice-mc-0.1.0.tar` & `dice-mc-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 kat       (1000) kat       (1000)        0 2023-07-14 18:32:41.628518 dice-mc-0.1.0/
--rw-rw-r--   0 kat       (1000) kat       (1000)    11357 2023-07-02 22:57:51.000000 dice-mc-0.1.0/LICENSE
--rw-rw-r--   0 kat       (1000) kat       (1000)      558 2023-07-02 23:03:30.000000 dice-mc-0.1.0/NOTICE
--rw-rw-r--   0 kat       (1000) kat       (1000)     6206 2023-07-14 18:32:41.632518 dice-mc-0.1.0/PKG-INFO
--rw-rw-r--   0 kat       (1000) kat       (1000)     5601 2023-07-03 05:26:12.000000 dice-mc-0.1.0/README.md
-drwxrwxr-x   0 kat       (1000) kat       (1000)        0 2023-07-14 18:32:41.628518 dice-mc-0.1.0/dice_mc/
--rw-rw-r--   0 kat       (1000) kat       (1000)       64 2023-07-02 19:29:33.000000 dice-mc-0.1.0/dice_mc/__init__.py
-drwxrwxr-x   0 kat       (1000) kat       (1000)        0 2023-07-14 18:32:41.628518 dice-mc-0.1.0/dice_mc/tests/
--rw-rw-r--   0 kat       (1000) kat       (1000)        0 2023-07-14 17:57:32.000000 dice-mc-0.1.0/dice_mc/tests/__init__.py
--rw-rw-r--   0 kat       (1000) kat       (1000)     1961 2023-07-14 18:23:03.000000 dice-mc-0.1.0/dice_mc/tests/test_torch.py
--rw-rw-r--   0 kat       (1000) kat       (1000)     6247 2023-07-14 18:18:58.000000 dice-mc-0.1.0/dice_mc/torch.py
-drwxrwxr-x   0 kat       (1000) kat       (1000)        0 2023-07-14 18:32:41.628518 dice-mc-0.1.0/dice_mc.egg-info/
--rw-rw-r--   0 kat       (1000) kat       (1000)     6206 2023-07-14 18:32:41.000000 dice-mc-0.1.0/dice_mc.egg-info/PKG-INFO
--rw-rw-r--   0 kat       (1000) kat       (1000)      303 2023-07-14 18:32:41.000000 dice-mc-0.1.0/dice_mc.egg-info/SOURCES.txt
--rw-rw-r--   0 kat       (1000) kat       (1000)        1 2023-07-14 18:32:41.000000 dice-mc-0.1.0/dice_mc.egg-info/dependency_links.txt
--rw-rw-r--   0 kat       (1000) kat       (1000)        6 2023-07-14 18:32:41.000000 dice-mc-0.1.0/dice_mc.egg-info/requires.txt
--rw-rw-r--   0 kat       (1000) kat       (1000)        8 2023-07-14 18:32:41.000000 dice-mc-0.1.0/dice_mc.egg-info/top_level.txt
--rw-rw-r--   0 kat       (1000) kat       (1000)       81 2023-07-02 19:37:59.000000 dice-mc-0.1.0/pyproject.toml
--rw-rw-r--   0 kat       (1000) kat       (1000)      650 2023-07-14 18:32:41.632518 dice-mc-0.1.0/setup.cfg
--rw-rw-r--   0 kat       (1000) kat       (1000)       70 2023-07-02 19:38:03.000000 dice-mc-0.1.0/setup.py
+drwxrwxr-x   0 kat       (1000) kat       (1000)        0 2023-07-16 21:04:11.696765 dice-mc-0.1.1/
+-rw-rw-r--   0 kat       (1000) kat       (1000)    11357 2023-07-02 22:57:51.000000 dice-mc-0.1.1/LICENSE
+-rw-rw-r--   0 kat       (1000) kat       (1000)      558 2023-07-02 23:03:30.000000 dice-mc-0.1.1/NOTICE
+-rw-rw-r--   0 kat       (1000) kat       (1000)     6206 2023-07-16 21:04:11.696765 dice-mc-0.1.1/PKG-INFO
+-rw-rw-r--   0 kat       (1000) kat       (1000)     5601 2023-07-03 05:26:12.000000 dice-mc-0.1.1/README.md
+drwxrwxr-x   0 kat       (1000) kat       (1000)        0 2023-07-16 21:04:11.692765 dice-mc-0.1.1/dice_mc/
+-rw-rw-r--   0 kat       (1000) kat       (1000)       64 2023-07-02 19:29:33.000000 dice-mc-0.1.1/dice_mc/__init__.py
+drwxrwxr-x   0 kat       (1000) kat       (1000)        0 2023-07-16 21:04:11.696765 dice-mc-0.1.1/dice_mc/tests/
+-rw-rw-r--   0 kat       (1000) kat       (1000)        0 2023-07-14 17:57:32.000000 dice-mc-0.1.1/dice_mc/tests/__init__.py
+-rw-rw-r--   0 kat       (1000) kat       (1000)     3725 2023-07-15 20:23:30.000000 dice-mc-0.1.1/dice_mc/tests/test_torch.py
+-rw-rw-r--   0 kat       (1000) kat       (1000)     6254 2023-07-16 21:03:26.000000 dice-mc-0.1.1/dice_mc/torch.py
+drwxrwxr-x   0 kat       (1000) kat       (1000)        0 2023-07-16 21:04:11.692765 dice-mc-0.1.1/dice_mc.egg-info/
+-rw-rw-r--   0 kat       (1000) kat       (1000)     6206 2023-07-16 21:04:11.000000 dice-mc-0.1.1/dice_mc.egg-info/PKG-INFO
+-rw-rw-r--   0 kat       (1000) kat       (1000)      303 2023-07-16 21:04:11.000000 dice-mc-0.1.1/dice_mc.egg-info/SOURCES.txt
+-rw-rw-r--   0 kat       (1000) kat       (1000)        1 2023-07-16 21:04:11.000000 dice-mc-0.1.1/dice_mc.egg-info/dependency_links.txt
+-rw-rw-r--   0 kat       (1000) kat       (1000)        6 2023-07-16 21:04:11.000000 dice-mc-0.1.1/dice_mc.egg-info/requires.txt
+-rw-rw-r--   0 kat       (1000) kat       (1000)        8 2023-07-16 21:04:11.000000 dice-mc-0.1.1/dice_mc.egg-info/top_level.txt
+-rw-rw-r--   0 kat       (1000) kat       (1000)       81 2023-07-02 19:37:59.000000 dice-mc-0.1.1/pyproject.toml
+-rw-rw-r--   0 kat       (1000) kat       (1000)      650 2023-07-16 21:04:11.696765 dice-mc-0.1.1/setup.cfg
+-rw-rw-r--   0 kat       (1000) kat       (1000)       70 2023-07-02 19:38:03.000000 dice-mc-0.1.1/setup.py
```

### Comparing `dice-mc-0.1.0/LICENSE` & `dice-mc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dice-mc-0.1.0/NOTICE` & `dice-mc-0.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `dice-mc-0.1.0/PKG-INFO` & `dice-mc-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dice-mc
-Version: 0.1.0
+Version: 0.1.1
 Summary: DiCE: The Infinitely Differentiable Monte-Carlo Estimator
 Home-page: https://github.com/crowsonkb/dice-mc
 Author: Katherine Crowson
 Author-email: crowsonkb@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dice-mc-0.1.0/README.md` & `dice-mc-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dice-mc-0.1.0/dice_mc/torch.py` & `dice-mc-0.1.1/dice_mc/torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """DiCE: The Infinitely Differentiable Monte-Carlo Estimator"""
 
-from typing import Iterable
+from typing import Iterable, Tuple
 
 import torch
 from torch import nn
 from torch.nn import functional as F
 
 
 def magic_box(tau: torch.Tensor) -> torch.Tensor:
@@ -16,15 +16,15 @@
     Returns:
         torch.Tensor: The result of the MagicBox operator applied to `tau`, which is a tensor
             of ones in the forward pass.
     """
     return torch.exp(tau - tau.detach())
 
 
-def left_sum_to_size(tensor: torch.Tensor, shape: tuple[int, ...]) -> torch.Tensor:
+def left_sum_to_size(tensor: torch.Tensor, shape: Tuple[int, ...]) -> torch.Tensor:
     """Sum the tensor to the given shape using left broadcasting."""
     return tensor.sum_to_size(shape + (1,) * (tensor.ndim - len(shape))).view(shape)
 
 
 def cost_node(cost: torch.Tensor, logps: Iterable[torch.Tensor]) -> torch.Tensor:
     """Compute the surrogate losses for a set of stochastic nodes.
 
@@ -49,15 +49,15 @@
 
     Returns:
         torch.Tensor: Logprobs of the actions selected at this stochastic node.
     """
     return F.log_softmax(logits, dim=-1).gather(-1, actions[..., None])[..., 0]
 
 
-def sample_categorical(logits: torch.Tensor) -> tuple[torch.Tensor, torch.Tensor]:
+def sample_categorical(logits: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
     """Sample from an optionally batched categorical distribution given logits.
 
     Args:
         logits (torch.Tensor): Logits of an optionally batched categorical distribution.
 
     Returns:
         torch.Tensor: Logprobs of the actions selected at this stochastic node.
```

### Comparing `dice-mc-0.1.0/dice_mc.egg-info/PKG-INFO` & `dice-mc-0.1.1/dice_mc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dice-mc
-Version: 0.1.0
+Version: 0.1.1
 Summary: DiCE: The Infinitely Differentiable Monte-Carlo Estimator
 Home-page: https://github.com/crowsonkb/dice-mc
 Author: Katherine Crowson
 Author-email: crowsonkb@gmail.com
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dice-mc-0.1.0/setup.cfg` & `dice-mc-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dice-mc
-version = 0.1.0
+version = 0.1.1
 author = Katherine Crowson
 author_email = crowsonkb@gmail.com
 url = https://github.com/crowsonkb/dice-mc
 description = DiCE: The Infinitely Differentiable Monte-Carlo Estimator
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = Apache-2.0
```

