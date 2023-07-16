# Comparing `tmp/muse-maskgit-pytorch-0.2.2.tar.gz` & `tmp/muse-maskgit-pytorch-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muse-maskgit-pytorch-0.2.2.tar", last modified: Sat Jul 15 17:24:37 2023, max compression
+gzip compressed data, was "muse-maskgit-pytorch-0.2.4.tar", last modified: Sun Jul 16 16:19:47 2023, max compression
```

## Comparing `muse-maskgit-pytorch-0.2.2.tar` & `muse-maskgit-pytorch-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:24:37.145845 muse-maskgit-pytorch-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-15 17:24:37.145845 muse-maskgit-pytorch-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:24:37.141845 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    24876 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/muse_maskgit_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/trainers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/vqgan_vae.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:24:37.145845 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-15 17:24:37.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-15 17:24:37.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:24:37.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-15 17:24:37.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-15 17:24:37.000000 muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:24:37.145845 muse-maskgit-pytorch-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-15 17:24:20.000000 muse-maskgit-pytorch-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:19:47.703877 muse-maskgit-pytorch-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-16 16:19:47.703877 muse-maskgit-pytorch-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:19:47.699877 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24876 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/muse_maskgit_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12012 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/trainers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/vqgan_vae.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:19:47.699877 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-16 16:19:47.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-16 16:19:47.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:19:47.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-16 16:19:47.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-16 16:19:47.000000 muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 16:19:47.703877 muse-maskgit-pytorch-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-16 16:19:35.000000 muse-maskgit-pytorch-0.2.4/setup.py
```

### Comparing `muse-maskgit-pytorch-0.2.2/LICENSE` & `muse-maskgit-pytorch-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.2/PKG-INFO` & `muse-maskgit-pytorch-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muse-maskgit-pytorch
-Version: 0.2.2
+Version: 0.2.4
 Summary: MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch
 Home-page: https://github.com/lucidrains/muse-maskgit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `muse-maskgit-pytorch-0.2.2/README.md` & `muse-maskgit-pytorch-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/attend.py` & `muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/attend.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from packaging import version
 from collections import namedtuple
 
 import torch
 from torch import nn, einsum
 import torch.nn.functional as F
 
+from memory_efficient_attention_pytorch.flash_attention import FlashAttentionFunction
 # constants
 
 AttentionConfig = namedtuple('AttentionConfig', ['enable_flash', 'enable_math', 'enable_mem_efficient'])
 
 # helpers
 
 def exists(val):
@@ -43,28 +44,28 @@
         self.attn_dropout = nn.Dropout(dropout)
 
         self.flash = flash
         assert not (flash and version.parse(torch.__version__) < version.parse('2.0.0')), 'in order to use flash attention, you must be using pytorch 2.0 or above'
 
         # determine efficient attention configs for cuda and cpu
 
-        self.cpu_config = AttentionConfig(True, True, True)
         self.cuda_config = None
+        self.no_hardware_detected = False
 
         if not torch.cuda.is_available() or not flash:
             return
 
         device_properties = torch.cuda.get_device_properties(torch.device('cuda'))
 
         if device_properties.major == 8 and device_properties.minor == 0:
             print_once('A100 GPU detected, using flash attention if input tensor is on cuda')
             self.cuda_config = AttentionConfig(True, False, False)
         else:
             print_once('Non-A100 GPU detected, using math or mem efficient attention if input tensor is on cuda')
-            self.cuda_config = AttentionConfig(False, True, True)
+            self.cuda_config = AttentionConfig(False, True, False)
 
     def flash_attn(self, q, k, v, mask = None):
         default_scale = q.shape[-1] ** -0.5
 
         is_cuda = q.is_cuda
 
         q, k, v = map(lambda t: t.contiguous(), (q, k, v))
@@ -73,26 +74,39 @@
         # so hack it in, to support rmsnorm-ed queries and keys
 
         rescale = self.scale / default_scale
 
         q = q * (rescale ** 0.5)
         k = k * (rescale ** 0.5)
 
-        # Check if there is a compatible device for flash attention
+        # use naive implementation if not correct hardware
 
-        config = self.cuda_config if is_cuda else self.cpu_config
+        # the below logic can also incorporate whether masking is needed or not
 
+        use_naive = not is_cuda or not exists(self.cuda_config)
+
+        if not is_cuda or self.no_hardware_detected:
+            return FlashAttentionFunction.apply(q, k, v, mask, False, 512, 512)
+
+        # use naive implementation
         # pytorch 2.0 flash attn: q, k, v, mask, dropout, causal, softmax_scale
 
-        with torch.backends.cuda.sdp_kernel(**config._asdict()):
-            out = F.scaled_dot_product_attention(
-                q, k, v,
-                attn_mask = mask,
-                dropout_p = self.dropout if self.training else 0.
-            )
+        try:
+            raise Exception()
+            with torch.backends.cuda.sdp_kernel(**self.cuda_config._asdict()):
+                out = F.scaled_dot_product_attention(
+                    q, k, v,
+                    attn_mask = mask,
+                    dropout_p = self.dropout if self.training else 0.
+                )
+        except:
+            print_once('no hardware detected, falling back to naive implementation from memory-efficient-attention-pytorch library')
+            self.no_hardware_detected = True
+
+            out = FlashAttentionFunction.apply(q, k, v, mask, False, 512, 512)
 
         return out
 
     def forward(self, q, k, v, mask = None, force_non_flash = False):
         """
         einstein notation
         b - batch
```

### Comparing `muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/muse_maskgit_pytorch.py` & `muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/muse_maskgit_pytorch.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/t5.py` & `muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/trainers.py` & `muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/trainers.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch/vqgan_vae.py` & `muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch/vqgan_vae.py`

 * *Files identical despite different names*

### Comparing `muse-maskgit-pytorch-0.2.2/muse_maskgit_pytorch.egg-info/PKG-INFO` & `muse-maskgit-pytorch-0.2.4/muse_maskgit_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muse-maskgit-pytorch
-Version: 0.2.2
+Version: 0.2.4
 Summary: MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch
 Home-page: https://github.com/lucidrains/muse-maskgit-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,text-to-image
 Classifier: Development Status :: 4 - Beta
```

### Comparing `muse-maskgit-pytorch-0.2.2/setup.py` & `muse-maskgit-pytorch-0.2.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'muse-maskgit-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.2.2',
+  version = '0.2.4',
   license='MIT',
   description = 'MUSE - Text-to-Image Generation via Masked Generative Transformers, in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/muse-maskgit-pytorch',
   keywords = [
@@ -18,14 +18,15 @@
     'text-to-image'
   ],
   install_requires=[
     'accelerate',
     'beartype',
     'einops>=0.6',
     'ema-pytorch>=0.2.2',
+    'memory-efficient-attention-pytorch>=0.1.4',
     'pillow',
     'sentencepiece',
     'torch>=1.6',
     'transformers',
     'torch>=1.6',
     'torchvision',
     'tqdm',
```

