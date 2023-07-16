# Comparing `tmp/memory-efficient-attention-pytorch-0.1.2.tar.gz` & `tmp/memory-efficient-attention-pytorch-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory-efficient-attention-pytorch-0.1.2.tar", last modified: Sun Mar  5 17:53:06 2023, max compression
+gzip compressed data, was "memory-efficient-attention-pytorch-0.1.4.tar", last modified: Sun Jul 16 16:09:42 2023, max compression
```

## Comparing `memory-efficient-attention-pytorch-0.1.2.tar` & `memory-efficient-attention-pytorch-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:53:06.570443 memory-efficient-attention-pytorch-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-05 17:52:54.000000 memory-efficient-attention-pytorch-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-05 17:53:06.570443 memory-efficient-attention-pytorch-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-03-05 17:52:54.000000 memory-efficient-attention-pytorch-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:53:06.570443 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7460 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7127 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/memory_efficient_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/reversible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:53:06.570443 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-03-05 17:53:06.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-03-05 17:53:06.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 17:53:06.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-05 17:53:06.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-05 17:53:06.000000 memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-05 17:53:06.570443 memory-efficient-attention-pytorch-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 17:53:06.570443 memory-efficient-attention-pytorch-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-05 17:52:55.000000 memory-efficient-attention-pytorch-0.1.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/memory_efficient_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/reversible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/tests/test.py
```

### Comparing `memory-efficient-attention-pytorch-0.1.2/LICENSE` & `memory-efficient-attention-pytorch-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.2/PKG-INFO` & `memory-efficient-attention-pytorch-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-efficient-attention-pytorch
-Version: 0.1.2
+Version: 0.1.4
 Summary: Memory Efficient Attention - Pytorch
 Home-page: https://github.com/lucidrains/memory-efficient-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention-mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory-efficient-attention-pytorch-0.1.2/README.md` & `memory-efficient-attention-pytorch-0.1.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-## Memory Efficient Attention Pytorch
+## Memory Efficient Attention Pytorch (obsolete)
 
 Implementation of a memory efficient multi-head attention as proposed in the paper, <a href="https://arxiv.org/abs/2112.05682">Self-attention Does Not Need O(n²) Memory</a>. In addition, the module will take care of masking, causal masking, as well as cross attention.
 
 This repository also contains a <a href="https://github.com/lucidrains/memory-efficient-attention-pytorch/blob/main/memory_efficient_attention_pytorch/flash_attention.py">naive non-CUDA implementation</a> of the improvements made by <a href="https://tridao.me/">Tri Dao</a> with his <a href="https://github.com/HazyResearch/flash-attention">Flash Attention</a> paper, for educational purposes. It is a game changer for attention and building long-context transformers.
 
+Update: from now on, you should just be using the <a href="https://pytorch.org/docs/master/generated/torch.nn.functional.scaled_dot_product_attention.html?highlight=scaled_dot_product#torch.nn.functional.scaled_dot_product_attention">`F.scaled_dot_product_attention`</a> function in Pytorch 2.0
+
 ## Install
 
 ```bash
 $ pip install memory-efficient-attention-pytorch
 ```
 
 ## Usage
```

#### html2text {}

```diff
@@ -1,33 +1,35 @@
-## Memory Efficient Attention Pytorch Implementation of a memory efficient
-multi-head attention as proposed in the paper, Self-attention_Does_Not_Need_O
-(nÂ²)_Memory. In addition, the module will take care of masking, causal
-masking, as well as cross attention. This repository also contains a naive_non-
-CUDA_implementation of the improvements made by Tri_Dao with his Flash
-Attention paper, for educational purposes. It is a game changer for attention
-and building long-context transformers. ## Install ```bash $ pip install
-memory-efficient-attention-pytorch ``` ## Usage For autoregressive language
-model ```python import torch from memory_efficient_attention_pytorch import
-Attention attn = Attention( dim = 512, dim_head = 64, # dimension per head
-heads = 8, # number of attention heads causal = True, # autoregressive or not
-memory_efficient = True, # whether to use memory efficient attention (can be
-turned off to test against normal attention) q_bucket_size = 1024, # bucket
-size along queries dimension k_bucket_size = 2048 # bucket size along key /
-values dimension ).cuda() x = torch.randn(1, 65536, 512).cuda() out = attn(x) #
-(1, 65536, 512) ``` Cross attention ```python import torch from
-memory_efficient_attention_pytorch import Attention cross_attn = Attention( dim
-= 512, dim_head = 64, heads = 8, memory_efficient = True, q_bucket_size = 1024,
-k_bucket_size = 2048 ).cuda() x = torch.randn(1, 65536, 512).cuda() context =
-torch.randn(1, 65536, 512).cuda() mask = torch.ones(1, 65536).bool().cuda() out
-= cross_attn(x, context = context, mask = mask) # (1, 65536, 512) ``` ##
-Citations ```bibtex @misc{rabe2021selfattention, title = {Self-attention Does
-Not Need $O(n^2)$ Memory}, author = {Markus N. Rabe and Charles Staats}, year =
-{2021}, eprint = {2112.05682}, archivePrefix = {arXiv}, primaryClass = {cs.LG}
-} ``` ```bibtex @misc{liu2021swin, title = {Swin Transformer V2: Scaling Up
-Capacity and Resolution}, author = {Ze Liu and Han Hu and Yutong Lin and
-Zhuliang Yao and Zhenda Xie and Yixuan Wei and Jia Ning and Yue Cao and Zheng
-Zhang and Li Dong and Furu Wei and Baining Guo}, year = {2021}, eprint =
-{2111.09883}, archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex
-@article{Dao2022FlashAttentionFA, title = {FlashAttention: Fast and Memory-
-Efficient Exact Attention with IO-Awareness}, author = {Tri Dao and Daniel Y.
-Fu and Stefano Ermon and Atri Rudra and Christopher R'e}, journal = {ArXiv},
-year = {2022}, volume = {abs/2205.14135} } ```
+## Memory Efficient Attention Pytorch (obsolete) Implementation of a memory
+efficient multi-head attention as proposed in the paper, Self-attention_Does
+Not_Need_O(nÂ²)_Memory. In addition, the module will take care of masking,
+causal masking, as well as cross attention. This repository also contains a
+naive_non-CUDA_implementation of the improvements made by Tri_Dao with his
+Flash_Attention paper, for educational purposes. It is a game changer for
+attention and building long-context transformers. Update: from now on, you
+should just be using the `F.scaled_dot_product_attention` function in Pytorch
+2.0 ## Install ```bash $ pip install memory-efficient-attention-pytorch ``` ##
+Usage For autoregressive language model ```python import torch from
+memory_efficient_attention_pytorch import Attention attn = Attention( dim =
+512, dim_head = 64, # dimension per head heads = 8, # number of attention heads
+causal = True, # autoregressive or not memory_efficient = True, # whether to
+use memory efficient attention (can be turned off to test against normal
+attention) q_bucket_size = 1024, # bucket size along queries dimension
+k_bucket_size = 2048 # bucket size along key / values dimension ).cuda() x =
+torch.randn(1, 65536, 512).cuda() out = attn(x) # (1, 65536, 512) ``` Cross
+attention ```python import torch from memory_efficient_attention_pytorch import
+Attention cross_attn = Attention( dim = 512, dim_head = 64, heads = 8,
+memory_efficient = True, q_bucket_size = 1024, k_bucket_size = 2048 ).cuda() x
+= torch.randn(1, 65536, 512).cuda() context = torch.randn(1, 65536, 512).cuda()
+mask = torch.ones(1, 65536).bool().cuda() out = cross_attn(x, context =
+context, mask = mask) # (1, 65536, 512) ``` ## Citations ```bibtex @misc
+{rabe2021selfattention, title = {Self-attention Does Not Need $O(n^2)$ Memory},
+author = {Markus N. Rabe and Charles Staats}, year = {2021}, eprint =
+{2112.05682}, archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex
+@misc{liu2021swin, title = {Swin Transformer V2: Scaling Up Capacity and
+Resolution}, author = {Ze Liu and Han Hu and Yutong Lin and Zhuliang Yao and
+Zhenda Xie and Yixuan Wei and Jia Ning and Yue Cao and Zheng Zhang and Li Dong
+and Furu Wei and Baining Guo}, year = {2021}, eprint = {2111.09883},
+archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @article
+{Dao2022FlashAttentionFA, title = {FlashAttention: Fast and Memory-Efficient
+Exact Attention with IO-Awareness}, author = {Tri Dao and Daniel Y. Fu and
+Stefano Ermon and Atri Rudra and Christopher R'e}, journal = {ArXiv}, year =
+{2022}, volume = {abs/2205.14135} } ```
```

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/autoregressive_wrapper.py` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/flash_attention.py` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/flash_attention.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,19 +34,26 @@
 
         o = torch.zeros_like(q)
         all_row_sums = torch.zeros((*q.shape[:-1], 1), device = device)
         all_row_maxes = torch.full((*q.shape[:-1], 1), max_neg_value, device = device)
 
         scale = (q.shape[-1] ** -0.5)
 
+        num_row_tiles = math.ceil(q.shape[-2] / q_bucket_size)
+        num_col_tiles = math.ceil(k.shape[-2] / k_bucket_size)
+
+        if exists(mask) and mask.ndim == 2:
+            mask = rearrange(mask, 'b n -> b 1 1 n')
+
         if not exists(mask):
-            mask = (None,) * math.ceil(q.shape[-2] / q_bucket_size)
+            col_masks = (None,) * num_col_tiles
+            mask = (col_masks,) * num_row_tiles 
         else:
-            mask = rearrange(mask, 'b n -> b 1 1 n')
-            mask = mask.split(q_bucket_size, dim = -1)
+            mask = ((mask,) * num_row_tiles) if mask.shape[-2] == 1 else mask.split(q_bucket_size, dim = -2)
+            mask = tuple(((row_mask,) * num_col_tiles) if row_mask.shape[-1] == 1 else row_mask.split(k_bucket_size, dim = -1) for row_mask in mask)
 
         row_splits = zip(
             q.split(q_bucket_size, dim = -2),
             o.split(q_bucket_size, dim = -2),
             mask,
             all_row_sums.split(q_bucket_size, dim = -2),
             all_row_maxes.split(q_bucket_size, dim = -2),
@@ -54,34 +61,35 @@
 
         for ind, (qc, oc, row_mask, row_sums, row_maxes) in enumerate(row_splits):
             q_start_index = ind * q_bucket_size - qk_len_diff
 
             col_splits = zip(
                 k.split(k_bucket_size, dim = -2),
                 v.split(k_bucket_size, dim = -2),
+                row_mask
             )
 
-            for k_ind, (kc, vc) in enumerate(col_splits):
+            for k_ind, (kc, vc, col_mask) in enumerate(col_splits):
                 k_start_index = k_ind * k_bucket_size
 
                 attn_weights = einsum('... i d, ... j d -> ... i j', qc, kc) * scale
 
-                if exists(row_mask):
-                    attn_weights.masked_fill_(~row_mask, max_neg_value)
+                if exists(col_mask):
+                    attn_weights.masked_fill_(~col_mask, max_neg_value)
 
                 if causal and q_start_index < (k_start_index + k_bucket_size - 1):
                     causal_mask = torch.ones((qc.shape[-2], kc.shape[-2]), dtype = torch.bool, device = device).triu(q_start_index - k_start_index + 1)
                     attn_weights.masked_fill_(causal_mask, max_neg_value)
 
                 block_row_maxes = attn_weights.amax(dim = -1, keepdims = True)
                 attn_weights -= block_row_maxes
                 exp_weights = torch.exp(attn_weights)
 
-                if exists(row_mask):
-                    exp_weights.masked_fill_(~row_mask, 0.)
+                if exists(col_mask):
+                    exp_weights.masked_fill_(~col_mask, 0.)
 
                 block_row_sums = exp_weights.sum(dim = -1, keepdims = True).clamp(min = EPSILON)
 
                 new_row_maxes = torch.maximum(block_row_maxes, row_maxes)
 
                 exp_values = einsum('... i j, ... j d -> ... i d', exp_weights, vc)
 
@@ -132,29 +140,30 @@
             q_start_index = ind * q_bucket_size - qk_len_diff
 
             col_splits = zip(
                 k.split(k_bucket_size, dim = -2),
                 v.split(k_bucket_size, dim = -2),
                 dk.split(k_bucket_size, dim = -2),
                 dv.split(k_bucket_size, dim = -2),
+                row_mask
             )
 
-            for k_ind, (kc, vc, dkc, dvc) in enumerate(col_splits):
+            for k_ind, (kc, vc, dkc, dvc, col_mask) in enumerate(col_splits):
                 k_start_index = k_ind * k_bucket_size
 
                 attn_weights = einsum('... i d, ... j d -> ... i j', qc, kc) * scale
 
                 if causal and q_start_index < (k_start_index + k_bucket_size - 1):
                     causal_mask = torch.ones((qc.shape[-2], kc.shape[-2]), dtype = torch.bool, device = device).triu(q_start_index - k_start_index + 1)
                     attn_weights.masked_fill_(causal_mask, max_neg_value)
 
                 p = torch.exp(attn_weights - lsec)
 
-                if exists(row_mask):
-                    p.masked_fill_(~row_mask, 0.)
+                if exists(col_mask):
+                    p.masked_fill_(~col_mask, 0.)
 
                 dv_chunk = einsum('... i j, ... i d -> ... j d', p, doc)
                 dp = einsum('... i d, ... j d -> ... i j', doc, vc)
 
                 D = (doc * oc).sum(dim = -1, keepdims = True)
                 ds = p * scale * (dp - D)
 
@@ -182,15 +191,14 @@
         dim_head = 64,
         causal = False,
         q_bucket_size = 512,
         k_bucket_size = 1024
     ):
         super().__init__()
         self.heads = heads
-
         self.causal = causal
 
         inner_dim = heads * dim_head
 
         self.to_q = nn.Linear(dim, inner_dim, bias = False)
         self.to_kv = nn.Linear(dim, inner_dim * 2, bias = False)
         self.to_out = nn.Linear(inner_dim, dim, bias = False)
```

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/memory_efficient_attention.py` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/memory_efficient_attention.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     if exists(attn_bias):
         sim = sim + attn_bias
 
     mask_value = -torch.finfo(sim.dtype).max
 
     if exists(mask):
-        mask = rearrange(mask, 'b j -> b 1 1 j')
+        if mask.ndim == 2:
+            mask = rearrange(mask, 'b j -> b 1 1 j')
         sim = sim.masked_fill(~mask, mask_value)
 
     if causal:
         i, j = sim.shape[-2:]
         mask = torch.ones(i, j, device = q.device, dtype = torch.bool).triu(j - i + 1)
         sim = sim.masked_fill(mask, mask_value)
```

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/reversible.py` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/reversible.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch/transformer.py` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/transformer.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch.egg-info/PKG-INFO` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-efficient-attention-pytorch
-Version: 0.1.2
+Version: 0.1.4
 Summary: Memory Efficient Attention - Pytorch
 Home-page: https://github.com/lucidrains/memory-efficient-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention-mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory-efficient-attention-pytorch-0.1.2/memory_efficient_attention_pytorch.egg-info/SOURCES.txt` & `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.2/setup.py` & `memory-efficient-attention-pytorch-0.1.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'memory-efficient-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.2',
+  version = '0.1.4',
   license='MIT',
   description = 'Memory Efficient Attention - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/memory-efficient-attention-pytorch',
   keywords = [
@@ -19,16 +19,15 @@
     'einops>=0.4.1',
     'torch>=1.6'    
   ],
   setup_requires=[
     'pytest-runner',
   ],
   tests_require=[
-    'pytest',
-    'torch==1.12.1'    
+    'pytest'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

