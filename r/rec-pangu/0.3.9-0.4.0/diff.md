# Comparing `tmp/rec_pangu-0.3.9-py3-none-any.whl.zip` & `tmp/rec_pangu-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,26 @@
-Zip file size: 116591 bytes, number of entries: 80
--rw-r--r--  2.0 unx      199 b- defN 23-Jul-11 05:53 rec_pangu/__init__.py
+Zip file size: 117944 bytes, number of entries: 83
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jul-11 08:28 .DS_Store
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jul-11 08:28 rec_pangu/.DS_Store
+-rw-r--r--  2.0 unx      199 b- defN 23-Jul-13 07:56 rec_pangu/__init__.py
 -rw-r--r--  2.0 unx     5837 b- defN 23-Apr-03 08:03 rec_pangu/benchmark_trainer.py
 -rw-r--r--  2.0 unx     9722 b- defN 23-Mar-18 15:33 rec_pangu/gpt_ranktrainer.py
 -rw-r--r--  2.0 unx    14630 b- defN 23-Apr-03 08:03 rec_pangu/model_pipeline.py
 -rw-r--r--  2.0 unx     5448 b- defN 23-Mar-18 15:32 rec_pangu/old_ranktrainer.py
 -rw-r--r--  2.0 unx    20415 b- defN 23-Jul-10 02:50 rec_pangu/trainer.py
 -rw-r--r--  2.0 unx      404 b- defN 23-Mar-05 10:13 rec_pangu/dataset/__init__.py
 -rw-r--r--  2.0 unx     4954 b- defN 23-Apr-03 08:02 rec_pangu/dataset/base_dataset.py
 -rw-r--r--  2.0 unx     3776 b- defN 23-Apr-03 08:02 rec_pangu/dataset/graph_dataset.py
 -rw-r--r--  2.0 unx     2812 b- defN 23-Apr-03 08:02 rec_pangu/dataset/multi_task_dataset.py
--rw-r--r--  2.0 unx     3986 b- defN 23-Apr-03 08:02 rec_pangu/dataset/process_data.py
--rw-r--r--  2.0 unx     5635 b- defN 23-Apr-03 08:02 rec_pangu/dataset/sequence_dataset.py
+-rw-r--r--  2.0 unx     3968 b- defN 23-Jul-16 04:53 rec_pangu/dataset/process_data.py
+-rw-r--r--  2.0 unx     5640 b- defN 23-Jul-16 04:48 rec_pangu/dataset/sequence_dataset.py
+-rw-r--r--  2.0 unx     6148 b- defN 23-Jul-11 08:28 rec_pangu/models/.DS_Store
 -rw-r--r--  2.0 unx      117 b- defN 22-Jul-28 02:44 rec_pangu/models/__init__.py
--rw-r--r--  2.0 unx    10465 b- defN 23-Apr-16 10:52 rec_pangu/models/base_model.py
--rw-r--r--  2.0 unx     8027 b- defN 23-Apr-03 08:03 rec_pangu/models/utils.py
+-rw-r--r--  2.0 unx    11105 b- defN 23-Jul-13 07:41 rec_pangu/models/base_model.py
+-rw-r--r--  2.0 unx     8154 b- defN 23-Jul-14 05:26 rec_pangu/models/utils.py
 -rw-r--r--  2.0 unx      949 b- defN 22-Jul-28 02:44 rec_pangu/models/layers/LGConv.py
 -rw-r--r--  2.0 unx      456 b- defN 23-Apr-03 07:29 rec_pangu/models/layers/__init__.py
 -rw-r--r--  2.0 unx     1876 b- defN 23-Mar-20 16:44 rec_pangu/models/layers/activation.py
 -rw-r--r--  2.0 unx     4606 b- defN 23-Apr-03 08:02 rec_pangu/models/layers/attention.py
 -rw-r--r--  2.0 unx     7468 b- defN 23-Apr-03 08:02 rec_pangu/models/layers/conv.py
 -rw-r--r--  2.0 unx     3943 b- defN 23-Apr-03 08:02 rec_pangu/models/layers/deep.py
 -rw-r--r--  2.0 unx     2932 b- defN 23-Apr-03 08:02 rec_pangu/models/layers/embedding.py
@@ -67,16 +70,16 @@
 -rw-r--r--  2.0 unx     3048 b- defN 23-Apr-11 14:29 rec_pangu/models/sequence/srgnn.py
 -rw-r--r--  2.0 unx     1813 b- defN 23-Apr-11 14:29 rec_pangu/models/sequence/stamp.py
 -rw-r--r--  2.0 unx     1621 b- defN 23-Apr-11 14:29 rec_pangu/models/sequence/yotubednn.py
 -rw-r--r--  2.0 unx      115 b- defN 23-Apr-11 01:35 rec_pangu/serving/__init__.py
 -rw-r--r--  2.0 unx     2211 b- defN 23-Apr-11 02:23 rec_pangu/serving/ranking_server.py
 -rw-r--r--  2.0 unx      301 b- defN 23-Mar-05 10:33 rec_pangu/utils/__init__.py
 -rw-r--r--  2.0 unx     1509 b- defN 23-Apr-03 08:03 rec_pangu/utils/check_version.py
--rw-r--r--  2.0 unx     8756 b- defN 23-Apr-03 08:03 rec_pangu/utils/evaluate.py
--rw-r--r--  2.0 unx     1549 b- defN 23-Jul-11 06:55 rec_pangu/utils/gpu_utils.py
+-rw-r--r--  2.0 unx     8857 b- defN 23-Jul-16 03:32 rec_pangu/utils/evaluate.py
+-rw-r--r--  2.0 unx     1565 b- defN 23-Jul-11 07:09 rec_pangu/utils/gpu_utils.py
 -rw-r--r--  2.0 unx      668 b- defN 23-Apr-03 08:03 rec_pangu/utils/json_utils.py
--rw-r--r--  2.0 unx     1058 b- defN 23-Jul-11 06:56 rec_pangu-0.3.9.dist-info/LICENSE
--rw-r--r--  2.0 unx    17906 b- defN 23-Jul-11 06:56 rec_pangu-0.3.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 06:56 rec_pangu-0.3.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Jul-11 06:56 rec_pangu-0.3.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     7147 b- defN 23-Jul-11 06:56 rec_pangu-0.3.9.dist-info/RECORD
-80 files, 348995 bytes uncompressed, 105187 bytes compressed:  69.9%
+-rw-r--r--  2.0 unx     1058 b- defN 23-Jul-16 04:53 rec_pangu-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    17906 b- defN 23-Jul-16 04:53 rec_pangu-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-16 04:53 rec_pangu-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jul-16 04:53 rec_pangu-0.4.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     7372 b- defN 23-Jul-16 04:53 rec_pangu-0.4.0.dist-info/RECORD
+83 files, 368535 bytes uncompressed, 106204 bytes compressed:  71.2%
```

## zipnote {}

```diff
@@ -1,7 +1,13 @@
+Filename: .DS_Store
+Comment: 
+
+Filename: rec_pangu/.DS_Store
+Comment: 
+
 Filename: rec_pangu/__init__.py
 Comment: 
 
 Filename: rec_pangu/benchmark_trainer.py
 Comment: 
 
 Filename: rec_pangu/gpt_ranktrainer.py
@@ -30,14 +36,17 @@
 
 Filename: rec_pangu/dataset/process_data.py
 Comment: 
 
 Filename: rec_pangu/dataset/sequence_dataset.py
 Comment: 
 
+Filename: rec_pangu/models/.DS_Store
+Comment: 
+
 Filename: rec_pangu/models/__init__.py
 Comment: 
 
 Filename: rec_pangu/models/base_model.py
 Comment: 
 
 Filename: rec_pangu/models/utils.py
@@ -219,23 +228,23 @@
 
 Filename: rec_pangu/utils/gpu_utils.py
 Comment: 
 
 Filename: rec_pangu/utils/json_utils.py
 Comment: 
 
-Filename: rec_pangu-0.3.9.dist-info/LICENSE
+Filename: rec_pangu-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: rec_pangu-0.3.9.dist-info/METADATA
+Filename: rec_pangu-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: rec_pangu-0.3.9.dist-info/WHEEL
+Filename: rec_pangu-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: rec_pangu-0.3.9.dist-info/top_level.txt
+Filename: rec_pangu-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: rec_pangu-0.3.9.dist-info/RECORD
+Filename: rec_pangu-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rec_pangu/__init__.py

```diff
@@ -1,9 +1,9 @@
 # -*- ecoding: utf-8 -*-
 # @ModuleName: __init__
 # @Author: wk
 # @Email: 306178200@qq.com
 # @Time: 2022/6/10 8:20 PM
 from .utils import check_version
 
-__version__ = '0.3.9'
+__version__ = '0.4.0'
 check_version(__version__)
```

## rec_pangu/dataset/process_data.py

```diff
@@ -39,17 +39,17 @@
     train_dataset = SequenceDataset(schema, df=train_df, phase='train')
     enc_dict = train_dataset.get_enc_dict()
     valid_dataset = SequenceDataset(schema, df=valid_df, enc_dict=enc_dict, phase='test')
     test_dataset = SequenceDataset(schema, df=test_df, enc_dict=enc_dict, phase='test')
 
     train_loader = D.DataLoader(train_dataset, batch_size=batch_size, shuffle=True,
                                 num_workers=0, pin_memory=True, drop_last=True)
-    valid_loader = D.DataLoader(valid_dataset, batch_size=batch_size, shuffle=False,
+    valid_loader = D.DataLoader(valid_dataset, batch_size=8, shuffle=False,
                                 num_workers=0, pin_memory=True, drop_last=True)
-    test_loader = D.DataLoader(test_dataset, batch_size=batch_size, shuffle=False,
+    test_loader = D.DataLoader(test_dataset, batch_size=8, shuffle=False,
                                num_workers=0, pin_memory=True, drop_last=True)
 
     return train_loader, valid_loader, test_loader, enc_dict
 
 
 def get_dataloader(train_df, valid_df, test_df, schema, batch_size=512 * 3):
     if schema['task_type'] == 'ranking':
```

## rec_pangu/dataset/sequence_dataset.py

```diff
@@ -93,15 +93,15 @@
             else:
                 hist_item_list.append(item_list[:k] + [0] * (self.max_length - k))
                 hist_mask_list.append([1.0] * k + [0.0] * (self.max_length - k))
                 for col in self.cate_cols:
                     cate_seq = getattr(self, f'user2{col}')[user_id]
                     setattr(self, f'hist_{col}_list', cate_seq[:k] + [0] * (self.max_length - k))
             data = {
-                'user': user_id,
+                'user': str(user_id),
                 'hist_item_list': torch.Tensor(hist_item_list).squeeze(0).long(),
                 'hist_mask_list': torch.Tensor(hist_mask_list).squeeze(0).long(),
             }
             for col in self.cate_cols:
                 data.update({f'hist_{col}_list': torch.Tensor(getattr(self, f'hist_{col}_list')).squeeze(0).long()})
         return data
```

## rec_pangu/models/base_model.py

```diff
@@ -48,15 +48,16 @@
 
         Returns:
             None
         """
         for weight in self.parameters():
             # If the weight is a bias term or a 1D tensor, set it to 0.
             if len(weight.shape) == 1:
-                torch.nn.init.constant_(weight, 0)
+                # torch.nn.init.constant_(weight, 0)
+                continue
             # Otherwise, initialize the weight using Kaiming initialization.
             else:
                 torch.nn.init.kaiming_normal_(weight)
 
     def set_pretrained_weights(self, col_name: str, pretrained_dict: dict, trainable: bool = True) -> None:
         """
         Set the pre-trained weights for the model.
@@ -212,15 +213,16 @@
 
         Returns:
             None
         """
         for weight in self.parameters():
             # If the weight is a bias term or a 1D tensor, set it to 0.
             if len(weight.shape) == 1:
-                torch.nn.init.constant_(weight, 0)
+                # torch.nn.init.constant_(weight, 0)
+                continue
             # Otherwise, initialize the weight using Kaiming initialization.
             else:
                 torch.nn.init.kaiming_normal_(weight)
 
 
 class GraphBaseModel(nn.Module):
     def __int__(self, num_user, num_item, embedding_dim):
@@ -228,14 +230,33 @@
         self.embedding_dim = embedding_dim
         self.num_user = num_item
         self.num_item = num_item
 
         self.user_emb_layer = nn.Embedding(self.num_user, self.embedding_dim)
         self.item_emb_layer = nn.Embedding(self.num_item, self.embedding_dim)
 
+    def reset_parameters(self):
+        """
+        Initializes the weights of the neural network.
+
+        Args:
+            self: The neural network object.
+
+        Returns:
+            None
+        """
+        for weight in self.parameters():
+            # If the weight is a bias term or a 1D tensor, set it to 0.
+            if len(weight.shape) == 1:
+                # torch.nn.init.constant_(weight, 0)
+                continue
+            # Otherwise, initialize the weight using Kaiming initialization.
+            else:
+                torch.nn.init.kaiming_normal_(weight)
+
     def _init_weights(self, module):
         if isinstance(module, nn.Embedding):
             xavier_normal_(module.weight.data)
         elif isinstance(module, nn.Linear):
             xavier_normal_(module.weight.data)
             if module.bias is not None:
                 constant_(module.bias.data, 0)
```

## rec_pangu/models/utils.py

```diff
@@ -180,15 +180,15 @@
     Returns:
         torch.Tensor: Padded sequences tensor.
     """
     padded_seqs = []
     for seq in seqs:
         seq_len = seq.shape[0]
         if seq_len < max_len:
-            padding = torch.zeros(max_len - seq_len, dtype=torch.long)
+            padding = torch.zeros(max_len - seq_len, dtype=torch.long, device=seq.device)
             padded_seq = torch.cat([seq, padding])
         else:
             padded_seq = seq[:max_len]
         padded_seqs.append(padded_seq)
     padded_seqs = torch.stack(padded_seqs, dim=0)
     return padded_seqs
 
@@ -201,14 +201,15 @@
 
     Returns:
         Dict: New batch data dictionary with graph information.
     """
     x = []
     edge_index = []
     alias_inputs = []
+    device = batch_data['hist_mask_list'].device
     item_seq_len = torch.sum(batch_data['hist_mask_list'], dim=-1).cpu().numpy()
     # 对每个session graph进行构建
     """
     # 小例子
     seq = torch.tensor([22,23,21,22,23,23,24,25,21])
     map_index, idx = torch.unique(seq, return_inverse=True)
 
@@ -229,22 +230,22 @@
         edge = torch.stack([alias_seq[:-1], alias_seq[1:]])
         edge_index.append(edge)
     """
     对一个batch内的所有session graph进行防冲突处理
     核心逻辑给每个序列的index加上前一个序列的index的最大值，
     保证每个序列在图中对应的节点的index范围互不冲突
     """
-    tot_node_num = torch.zeros([1], dtype=torch.long)
+    tot_node_num = torch.zeros([1], dtype=torch.long, device=device)
     for i in range(batch_data['hist_item_list'].shape[0]):
         edge_index[i] = edge_index[i] + tot_node_num
         alias_inputs[i] = alias_inputs[i] + tot_node_num
         tot_node_num += x[i].shape[0]
 
-    x = torch.cat(x)
-    alias_inputs = pad_sequence(alias_inputs, max_len=batch_data['hist_item_list'].shape[1])
+    x = torch.cat(x).to(device)
+    alias_inputs = pad_sequence(alias_inputs, max_len=batch_data['hist_item_list'].shape[1]).to(device)
 
     # SRGNN有两个图，第二个图可以简单通过torch.flip进行构建
     edge_index = torch.cat(edge_index, dim=1)
     reversed_edge_index = torch.flip(edge_index, dims=[0])
 
     in_graph = dgl.graph((edge_index[0], edge_index[1]))
     src_degree = in_graph.out_degrees().float()
@@ -257,12 +258,12 @@
     norm = torch.pow(src_degree, -1).unsqueeze(1)
     edge_weight = norm[reversed_edge_index[0]]
     out_graph.edata['edge_weight'] = edge_weight
 
     new_batch_data = {
         'x': x,
         'alias_inputs': alias_inputs,
-        'in_graph': in_graph,
-        'out_graph': out_graph
+        'in_graph': in_graph.to(device),
+        'out_graph': out_graph.to(device)
 
     }
     return new_batch_data
```

## rec_pangu/utils/evaluate.py

```diff
@@ -45,15 +45,18 @@
             data[key] = data[key].to(device)
 
         # Get user embeddings for the given data.
         model.eval()
         user_embs = model(data, is_training=False)['user_emb']
         user_embs = user_embs.cpu().detach().numpy().astype('float32')
 
-        user_list = data['user'].cpu().numpy()
+        if isinstance(data['user'], list):
+            user_list = data['user']
+        else:
+            user_list = data['user'].numpy().tolist()
 
         # Get the recommendations using Faiss index.
 
         if len(user_embs.shape) == 2:
 
             # Non-multi-interest model.
             user_embs = normalize(user_embs, norm='l2').astype('float32')
```

## rec_pangu/utils/gpu_utils.py

```diff
@@ -15,15 +15,15 @@
 
     reserved = torch.cuda.max_memory_reserved(device) / 1024 ** 3
     total = torch.cuda.get_device_properties(device).total_memory / 1024 ** 3
 
     return '{:.2f} G/{:.2f} G'.format(reserved, total)
 
 
-def set_device(device_id: int = -1):
+def set_device(device_id: int = -1) -> torch.device:
     """
     Sets the device to be used for tensor computations.
 
     Args:
         device_id: int, optional
             An integer indicating the index of the GPU device to use for tensor computations.
             `device_id` < 0 indicates that the computation should be performed on the CPU. Default -1.
```

## Comparing `rec_pangu-0.3.9.dist-info/LICENSE` & `rec_pangu-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rec_pangu-0.3.9.dist-info/METADATA` & `rec_pangu-0.4.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rec-pangu
-Version: 0.3.9
+Version: 0.4.0
 Summary: Some Rank/Multi-task model implemented by Pytorch
 Home-page: https://github.com/HaSai666/rec_pangu
 Author: wk
 Author-email: 306178200@qq.com
 Keywords: rank,multi task,deep learning,pytorch,recsys,recommendation
 Platform: all
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.19.0)
 Requires-Dist: torch (>=1.7.0)
-Requires-Dist: pandas (>=1.0.5)
+Requires-Dist: pandas (==1.3.5)
 Requires-Dist: tqdm
 Requires-Dist: scikit-learn (>=0.23.2)
 Requires-Dist: pygments
 Requires-Dist: loguru
 Requires-Dist: faiss-cpu
 Requires-Dist: wandb
```

### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: rec-pangu Version: 0.3.9 Summary: Some Rank/Multi-
+Metadata-Version: 2.1 Name: rec-pangu Version: 0.4.0 Summary: Some Rank/Multi-
 task model implemented by Pytorch Home-page: https://github.com/HaSai666/
 rec_pangu Author: wk Author-email: 306178200@qq.com Keywords: rank,multi
 task,deep learning,pytorch,recsys,recommendation Platform: all Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License Description-Content-Type:
 text/markdown License-File: LICENSE Requires-Dist: numpy (>=1.19.0) Requires-
-Dist: torch (>=1.7.0) Requires-Dist: pandas (>=1.0.5) Requires-Dist: tqdm
+Dist: torch (>=1.7.0) Requires-Dist: pandas (==1.3.5) Requires-Dist: tqdm
 Requires-Dist: scikit-learn (>=0.23.2) Requires-Dist: pygments Requires-Dist:
 loguru Requires-Dist: faiss-cpu Requires-Dist: wandb # Rec PanGu [![stars]
 (https://img.shields.io/github/stars/HaSai666/rec_pangu?color=097abb)](https://
 github.com/HaSai666/rec_pangu/stargazers) [![issues](https://img.shields.io/
 github/issues/HaSai666/rec_pangu?color=097abb)](https://github.com/HaSai666/
 rec_pangu/issues) [![license](https://img.shields.io/github/license/HaSai666/
 rec_pangu?color=097abb)](https://github.com/HaSai666/rec_pangu/blob/main/
```

## Comparing `rec_pangu-0.3.9.dist-info/RECORD` & `rec_pangu-0.4.0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-rec_pangu/__init__.py,sha256=3d4L4HogVAkvgd7pAX91RzJtDXd29vh87mUI6zYqv8c,199
+.DS_Store,sha256=0hy_E_6euFbvNj_m5J9LmFXpd3MdTofbcc5rjK6vQUI,6148
+rec_pangu/.DS_Store,sha256=j04wnLcsoeH6cNvpk1rcigZPwx61H1Uqp1PhfSuJcu0,6148
+rec_pangu/__init__.py,sha256=CEEvKPfo_0ZKPGnu2W1tvwRHhsiIvMXNUMTSZw5cypE,199
 rec_pangu/benchmark_trainer.py,sha256=J5kGL93iq4O7TW1k60oJZksrYRW4OniJa-JoVjmmelk,5837
 rec_pangu/gpt_ranktrainer.py,sha256=cHLZu4OgbpqL9vVMqtR1pvqMeNpLtyO_EdaJHMjWq08,9722
 rec_pangu/model_pipeline.py,sha256=y2_EnjqjU0jY1VpVC6r9sUYePtdQlpqznSskCmxMDn4,14630
 rec_pangu/old_ranktrainer.py,sha256=lMwui-xDAxMvyuxJyp8XKCV3BtQGWl39zbIL_bj6LUM,5448
 rec_pangu/trainer.py,sha256=VTpGls-SaFh5rFsfD-VSI_Hx2AdoOZHl_OeA6aH_Xyw,20415
 rec_pangu/dataset/__init__.py,sha256=o53SpwAQVsmLQp7CUWmIy7kikwH3ZBD-VBrW_5p2ToA,404
 rec_pangu/dataset/base_dataset.py,sha256=iImLln0AwCbDWizCuJzahz5eL1etRU7XP0Y2vklLzRs,4954
 rec_pangu/dataset/graph_dataset.py,sha256=Sz_PB9ibzf8X3zBncN8ozXY40k1Q5-ceRAWW0X5LMmk,3776
 rec_pangu/dataset/multi_task_dataset.py,sha256=XnQUTsvwWcYYWq52OtaBfpgfQ0jvLzaowaISNUhMjWg,2812
-rec_pangu/dataset/process_data.py,sha256=DRgqDeVwAym2PCZolwS-wHPBs9VU9p2mSlfaGxZUC3k,3986
-rec_pangu/dataset/sequence_dataset.py,sha256=Jr-SMzdqwquxh2W4yODeL7k5fmIjd07fgNLbQclnsYI,5635
+rec_pangu/dataset/process_data.py,sha256=WzBtgc2pCmDXGAEQw0Pv2nvTb2s3uXCKn5C4D4qt0zg,3968
+rec_pangu/dataset/sequence_dataset.py,sha256=49RX6alVRWh0IVApkHJhYm2MqGbaH9jQif6TrSFYvJU,5640
+rec_pangu/models/.DS_Store,sha256=hLwUnXW0G-Hg5Cs7UvY9nZifdT9p5Tonix-IKykPbTc,6148
 rec_pangu/models/__init__.py,sha256=ZTUYJ8guxLRAXkbK6TxxvRJw8Q153cUDA1XBcJwjqsI,117
-rec_pangu/models/base_model.py,sha256=-sjlaqezWodIItmVy7x74H4V8slQHBi0fSyB9SX6ynw,10465
-rec_pangu/models/utils.py,sha256=0_thQaedHWmVEfuJ7C1eqF4L-Ya0Wc7ouw8AxHqM3e0,8027
+rec_pangu/models/base_model.py,sha256=uKXHZsLfstCAJMkTwncLhZi14gHhy45PWAFarhZ_P3M,11105
+rec_pangu/models/utils.py,sha256=wJoHG-NfvXhxZnv2P_4VFe1j2gr1xAhx4R0cvjDen3w,8154
 rec_pangu/models/layers/LGConv.py,sha256=ZvqwTQ0zkmCK5XdwNZNChytFrCUtNT-AAFNqxp2WtLA,949
 rec_pangu/models/layers/__init__.py,sha256=5nIwNU6Rh0hFRypJV6wAbpQhVmRm3nxlP-c0P9sVEt0,456
 rec_pangu/models/layers/activation.py,sha256=vXcVU5Cvk-Xmoxzhv6A3sk-zjHY5z1Is488SlBhTjPY,1876
 rec_pangu/models/layers/attention.py,sha256=Jp1XOZfXrScOfwCf8OkH3OXwGKoYYlK2EcnTBuII9BE,4606
 rec_pangu/models/layers/conv.py,sha256=qDdETiJLruwQuG9vOTpscWjwbZjjqn_xCMGywg08axU,7468
 rec_pangu/models/layers/deep.py,sha256=Oin-CzDL8wMb34ATQpBZ6_o1VHxPA7RuePPCSa231Ks,3943
 rec_pangu/models/layers/embedding.py,sha256=dxii_wTx7SxaJzDgmnvihpbYhIkU6Uog2xHQ688R2BE,2932
@@ -66,15 +69,15 @@
 rec_pangu/models/sequence/srgnn.py,sha256=69-a9si8O4CXD_oW5au3XyCGMMoKJ1heKPROX-L0n_M,3048
 rec_pangu/models/sequence/stamp.py,sha256=PTethq9B9yea5Ihw7YvC3e1owIWo8y4bO9j-7BoZmtI,1813
 rec_pangu/models/sequence/yotubednn.py,sha256=TMKwhKp11_vcWp3OH1rIh-9vw7oxjBtgWc7y4_ZMzVk,1621
 rec_pangu/serving/__init__.py,sha256=twv9kol32GZD16l-6Xu5hiaYDHK72UIA1GGJmwcJi2A,115
 rec_pangu/serving/ranking_server.py,sha256=IR3IrhFEVPXnngaMCerunExdoo3XeeAryziEgwjOQQI,2211
 rec_pangu/utils/__init__.py,sha256=dF7uxiBraZf82Do_VlkQqicD4WsNcguSgebsO6dyyag,301
 rec_pangu/utils/check_version.py,sha256=ONSdf0hw-hPTHjJpHldDz5HdlNHo4kqrm2icjDPkUtg,1509
-rec_pangu/utils/evaluate.py,sha256=-OabWaxaItSLheTzMV3vir05J0yJg6cAr6NPmaKiPFQ,8756
-rec_pangu/utils/gpu_utils.py,sha256=heBMMGrcZkNuycj193Z8jtQeZ4htYJNLYyTf20LOJZM,1549
+rec_pangu/utils/evaluate.py,sha256=pJtXGTeIa4QTNUx23_2boFJZ97gXPuOj2wkiEuGuVKw,8857
+rec_pangu/utils/gpu_utils.py,sha256=V5-yE_XaHjGELIElhr5J9MWNTeaJS1HiA37CwF3tvrM,1565
 rec_pangu/utils/json_utils.py,sha256=2NbJgYTDACZXQIX11h5U4l0L5fHwyXNVdVksgWwiccI,668
-rec_pangu-0.3.9.dist-info/LICENSE,sha256=5t15gkJb51GDxbB-lVcG2ZMTYLHbccXypC-X_GK-kPw,1058
-rec_pangu-0.3.9.dist-info/METADATA,sha256=x1y1MtDsw2lbzq-iqK0WjHwpA63ubZP4MLG3mHVMBGs,17906
-rec_pangu-0.3.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-rec_pangu-0.3.9.dist-info/top_level.txt,sha256=VQeGX3ukDrCpoYzPshLjJWRzJ6lzbymbmBqfQQCUOYE,10
-rec_pangu-0.3.9.dist-info/RECORD,,
+rec_pangu-0.4.0.dist-info/LICENSE,sha256=5t15gkJb51GDxbB-lVcG2ZMTYLHbccXypC-X_GK-kPw,1058
+rec_pangu-0.4.0.dist-info/METADATA,sha256=hx4d5G9sfqE2MtMCyWIMrQ9EBTqc9QFMblk2uFhq94w,17906
+rec_pangu-0.4.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+rec_pangu-0.4.0.dist-info/top_level.txt,sha256=VQeGX3ukDrCpoYzPshLjJWRzJ6lzbymbmBqfQQCUOYE,10
+rec_pangu-0.4.0.dist-info/RECORD,,
```

