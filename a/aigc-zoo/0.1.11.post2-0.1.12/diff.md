# Comparing `tmp/aigc_zoo-0.1.11.post2-py3-none-any.whl.zip` & `tmp/aigc_zoo-0.1.12-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 64253 bytes, number of entries: 40
+Zip file size: 67408 bytes, number of entries: 42
 -rw-rw-rw-  2.0 fat       80 b- defN 23-Jun-16 14:31 aigc_zoo/__init__.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/__init__.py
 -rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/baichuan/__init__.py
 -rw-rw-rw-  2.0 fat     5578 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/baichuan/llm_model.py
 -rw-rw-rw-  2.0 fat     9574 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/baichuan/tokenization_baichuan.py
 -rw-rw-rw-  2.0 fat       66 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/baichuan2/__init__.py
 -rw-rw-rw-  2.0 fat     5575 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/baichuan2/llm_model.py
@@ -10,33 +10,35 @@
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/chatglm/__init__.py
 -rw-rw-rw-  2.0 fat    17057 b- defN 23-Jul-13 10:54 aigc_zoo/model_zoo/chatglm/llm_model.py
 -rw-rw-rw-  2.0 fat     6435 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/chatglm/ppo_model.py
 -rw-rw-rw-  2.0 fat     9700 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/chatglm/reward_model.py
 -rw-rw-rw-  2.0 fat    17037 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/chatglm/tokenization_chatglm.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jul-04 13:32 aigc_zoo/model_zoo/chatglm2/__init__.py
 -rw-rw-rw-  2.0 fat      114 b- defN 23-Jul-13 11:01 aigc_zoo/model_zoo/chatglm2/chatglm_model.py
--rw-rw-rw-  2.0 fat     9839 b- defN 23-Jul-13 11:01 aigc_zoo/model_zoo/chatglm2/llm_model.py
--rw-rw-rw-  2.0 fat     9252 b- defN 23-Jul-04 13:32 aigc_zoo/model_zoo/chatglm2/tokenization_chatglm.py
+-rw-rw-rw-  2.0 fat     9402 b- defN 23-Jul-16 05:12 aigc_zoo/model_zoo/chatglm2/llm_model.py
+-rw-rw-rw-  2.0 fat    10002 b- defN 23-Jul-15 17:41 aigc_zoo/model_zoo/chatglm2/tokenization_chatglm.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/llm/__init__.py
 -rw-rw-rw-  2.0 fat     6344 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/llm/ilql_model.py
 -rw-rw-rw-  2.0 fat     5443 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/llm/llm_model.py
 -rw-rw-rw-  2.0 fat     6298 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/llm/ppo_model.py
 -rw-rw-rw-  2.0 fat     9732 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/llm/reward_model.py
 -rw-rw-rw-  2.0 fat     6704 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/llm/rrhf_model.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/moss/__init__.py
 -rw-rw-rw-  2.0 fat     4554 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/moss/llm_model.py
 -rw-rw-rw-  2.0 fat     2050 b- defN 23-Jun-16 14:52 aigc_zoo/model_zoo/moss/moss_model.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/rwkv4/__init__.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/rwkv4/llm_model.py
+-rw-rw-rw-  2.0 fat     5734 b- defN 23-Jul-16 03:08 aigc_zoo/model_zoo/rwkv4/llm_model.py
+-rw-rw-rw-  2.0 fat     6519 b- defN 23-Jul-16 04:58 aigc_zoo/model_zoo/rwkv4/rwkv4_tokenizer.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/t5/__init__.py
 -rw-rw-rw-  2.0 fat     4950 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/t5/llm_model.py
 -rw-rw-rw-  2.0 fat     5848 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/t5/ppo_model.py
 -rw-rw-rw-  2.0 fat     9098 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/t5/reward_model.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2664 b- defN 23-Jul-13 10:54 aigc_zoo/utils/llm_generate.py
 -rw-rw-rw-  2.0 fat    13198 b- defN 23-Jul-13 11:08 aigc_zoo/utils/moss_generate.py
--rw-rw-rw-  2.0 fat    11357 b- defN 23-Jul-13 11:10 aigc_zoo-0.1.11.post2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      372 b- defN 23-Jul-13 11:10 aigc_zoo-0.1.11.post2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-13 11:10 aigc_zoo-0.1.11.post2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-13 11:10 aigc_zoo-0.1.11.post2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3717 b- defN 23-Jul-13 11:10 aigc_zoo-0.1.11.post2.dist-info/RECORD
-40 files, 197668 bytes uncompressed, 58159 bytes compressed:  70.6%
+-rw-rw-rw-  2.0 fat     3429 b- defN 23-Jul-15 15:45 aigc_zoo/utils/rwkv4_generate.py
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      366 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3877 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/RECORD
+42 files, 208288 bytes uncompressed, 61072 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -78,14 +78,17 @@
 
 Filename: aigc_zoo/model_zoo/rwkv4/__init__.py
 Comment: 
 
 Filename: aigc_zoo/model_zoo/rwkv4/llm_model.py
 Comment: 
 
+Filename: aigc_zoo/model_zoo/rwkv4/rwkv4_tokenizer.py
+Comment: 
+
 Filename: aigc_zoo/model_zoo/t5/__init__.py
 Comment: 
 
 Filename: aigc_zoo/model_zoo/t5/llm_model.py
 Comment: 
 
 Filename: aigc_zoo/model_zoo/t5/ppo_model.py
@@ -99,23 +102,26 @@
 
 Filename: aigc_zoo/utils/llm_generate.py
 Comment: 
 
 Filename: aigc_zoo/utils/moss_generate.py
 Comment: 
 
-Filename: aigc_zoo-0.1.11.post2.dist-info/LICENSE
+Filename: aigc_zoo/utils/rwkv4_generate.py
+Comment: 
+
+Filename: aigc_zoo-0.1.12.dist-info/LICENSE
 Comment: 
 
-Filename: aigc_zoo-0.1.11.post2.dist-info/METADATA
+Filename: aigc_zoo-0.1.12.dist-info/METADATA
 Comment: 
 
-Filename: aigc_zoo-0.1.11.post2.dist-info/WHEEL
+Filename: aigc_zoo-0.1.12.dist-info/WHEEL
 Comment: 
 
-Filename: aigc_zoo-0.1.11.post2.dist-info/top_level.txt
+Filename: aigc_zoo-0.1.12.dist-info/top_level.txt
 Comment: 
 
-Filename: aigc_zoo-0.1.11.post2.dist-info/RECORD
+Filename: aigc_zoo-0.1.12.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aigc_zoo/model_zoo/chatglm2/llm_model.py

```diff
@@ -82,25 +82,15 @@
         gen_kwargs = {"do_sample": do_sample, "top_p": top_p,
                       "temperature": temperature, "logits_processor": logits_processor, **kwargs}
 
         output_scores = gen_kwargs.get('output_scores', False)
         if output_scores:
             gen_kwargs['return_dict_in_generate'] = True
 
-        # inputs = self.build_inputs(tokenizer, query, history=history)
-        if not history:
-            prompt = query
-        else:
-            prompt = ""
-            for i, (old_query, response) in enumerate(history):
-                prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response)
-            prompt += "[Round {}]\n问：{}\n答：".format(len(history), query)
-
-        inputs = tokenizer([prompt], return_tensors="pt")
-        inputs = inputs.to(self.device)
+        inputs = self.build_inputs(tokenizer, query, history=history)
         outputs = self.generate(**inputs, **gen_kwargs)
         if output_scores:
             score = outputs.scores[0]
             return score
 
         outputs = outputs.tolist()[0][len(inputs["input_ids"][0]):]
         response = tokenizer.decode(outputs)
```

## aigc_zoo/model_zoo/chatglm2/tokenization_chatglm.py

```diff
@@ -13,15 +13,15 @@
         assert os.path.isfile(model_path), model_path
         self.sp_model = SentencePieceProcessor(model_file=model_path)
 
         # BOS / EOS token IDs
         self.n_words: int = self.sp_model.vocab_size()
         self.bos_id: int = self.sp_model.bos_id()
         self.eos_id: int = self.sp_model.eos_id()
-        self.pad_id: int = self.sp_model.eos_id()
+        self.pad_id: int = self.sp_model.unk_id()
         assert self.sp_model.vocab_size() == self.sp_model.get_piece_size()
 
         special_tokens = ["[MASK]", "[gMASK]", "[sMASK]", "sop", "eop"]
         self.special_tokens = {}
         self.index_special_tokens = {}
         for token in special_tokens:
             self.special_tokens[token] = self.n_words
@@ -51,50 +51,63 @@
         """ Converts a token (str) in an id using the vocab. """
         if token in self.special_tokens:
             return self.special_tokens[token]
         return self.sp_model.PieceToId(token)
 
     def convert_id_to_token(self, index):
         """Converts an index (integer) in a token (str) using the vocab."""
-        if index in self.index_special_tokens:
+        if index in self.index_special_tokens or index in [self.eos_id, self.bos_id, self.pad_id] or index < 0:
             return ""
         return self.sp_model.IdToPiece(index)
 
 
 class ChatGLMTokenizer(PreTrainedTokenizer):
     vocab_files_names = {"vocab_file": "tokenizer.model"}
 
     model_input_names = ["input_ids", "attention_mask", "position_ids"]
 
     def __init__(self, vocab_file, padding_side="left", **kwargs):
-        super().__init__(padding_side=padding_side, **kwargs)
+        super().__init__(padding_side=padding_side, clean_up_tokenization_spaces=False, **kwargs)
         self.name = "GLMTokenizer"
 
+        self.vocab_file = vocab_file
         self.tokenizer = SPTokenizer(vocab_file)
         self.special_tokens = {
             "<bos>": self.tokenizer.bos_id,
             "<eos>": self.tokenizer.eos_id,
             "<pad>": self.tokenizer.pad_id
         }
 
     def get_command(self, token):
         if token in self.special_tokens:
             return self.special_tokens[token]
         assert token in self.tokenizer.special_tokens, f"{token} is not a special token for {self.name}"
         return self.tokenizer.special_tokens[token]
 
     @property
+    def unk_token(self) -> str:
+        return "<unk>"
+
+    @property
     def pad_token(self) -> str:
-        return "</s>"
+        return "<unk>"
 
     @property
     def pad_token_id(self):
         return self.get_command("<pad>")
 
     @property
+    def eos_token(self) -> str:
+        return "</s>"
+
+    @property
+    def eos_token_id(self):
+        return self.get_command("<eos>")
+
+    @property
     def vocab_size(self):
         return self.tokenizer.n_words
 
     def get_vocab(self):
         """ Returns vocab as a dict """
         vocab = {self._convert_id_to_token(i): i for i in range(self.vocab_size)}
         vocab.update(self.added_tokens_encoder)
@@ -142,14 +155,23 @@
 
         return (vocab_file,)
 
     def get_prefix_tokens(self):
         prefix_tokens = [self.get_command("[gMASK]"), self.get_command("sop")]
         return prefix_tokens
 
+    def build_prompt(self, query, history=None):
+        if history is None:
+            history = []
+        prompt = ""
+        for i, (old_query, response) in enumerate(history):
+            prompt += "[Round {}]\n\n问：{}\n\n答：{}\n\n".format(i + 1, old_query, response)
+        prompt += "[Round {}]\n\n问：{}\n\n答：".format(len(history) + 1, query)
+        return prompt
+
     def build_inputs_with_special_tokens(
             self, token_ids_0: List[int], token_ids_1: Optional[List[int]] = None
     ) -> List[int]:
         """
         Build model inputs from a sequence or a pair of sequence for sequence classification tasks by concatenating and
         adding special tokens. A BERT sequence has the following format:
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## aigc_zoo/model_zoo/rwkv4/llm_model.py

```diff
@@ -1,15 +1,19 @@
 # coding=utf8
 # @Time    : 2023/5/12 20:41
 # @Author  : tk
 # @FileName: llm_model
+import torch
 from deep_training.nlp.models.rwkv4.modeling_rwkv import TransformerRWKV4LMHeadModel, RwkvConfig, set_model_profile, \
     RwkvForCausalLM
 from deep_training.trainer.pl.modelweighter import *
 import logging
+
+from torch import nn
+
 logger = logging.getLogger(__name__)
 
 
 class TransformerRWKV4ForLM(TransformerRWKV4LMHeadModel):
     def __init__(self, *args, **kwargs):
         # 如果显卡支持int8 可以开启
         load_in_8bit = kwargs.get('load_in_8bit', False)
@@ -26,29 +30,34 @@
         super(TransformerRWKV4ForLM, self).__init__(*args, **kwargs)
 
         # for param in self.model.parameters():
         #     param.requires_grad = False  # freeze the model - train adapters later
         #     if param.ndim == 1:
         #         # cast the small parameters (e.g. layernorm) to fp32 for stability
         #         param.data = param.data.to(torch.float32)
-
+        #
         # class CastOutputToFloat(nn.Sequential):
         #     def forward(self, x):
         #         return super().forward(x).to(torch.float32)
         #
-        # self.model.lm_head = CastOutputToFloat(self.model.lm_head)
+        # self.model.head = CastOutputToFloat(self.model.head)
 
 
 
     def enable_input_require_grads(self):
-        pass
         # setattr(self.model, 'model_parallel', True)
         # setattr(self.model, 'is_parallelizable', True)
         # # self.model.gradient_checkpointing_enable()
         # self.model.enable_input_require_grads()
+        m: PreTrainedModel = self.model
+        if hasattr(m,'_require_grads_hook'):
+            m.disable_input_require_grads()
+        m.enable_input_require_grads()
+
+
 
 
 
 class MyTransformer(TransformerRWKV4ForLM, ModelWeightMinMax, with_pl=True):
     def __init__(self, *args,new_num_tokens=None, **kwargs):
         lora_args: LoraConfig = kwargs.pop('lora_args', None)
         prompt_args: PromptLearningConfig = kwargs.pop('prompt_args', None)
```

## Comparing `aigc_zoo-0.1.11.post2.dist-info/LICENSE` & `aigc_zoo-0.1.12.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aigc_zoo-0.1.11.post2.dist-info/RECORD` & `aigc_zoo-0.1.12.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -9,32 +9,34 @@
 aigc_zoo/model_zoo/chatglm/__init__.py,sha256=RFimplzKNFznknZ0MzZDOhcvck-tAJQ53rTCMX-shS8,77
 aigc_zoo/model_zoo/chatglm/llm_model.py,sha256=YLHqq5MaQMZLnie0ea6BTgj5aYV2-abatZIVyL_IJHU,17057
 aigc_zoo/model_zoo/chatglm/ppo_model.py,sha256=MjbAJm22oitIMJrJ-RxbHJv0df4m80G4BQsBXorwqac,6435
 aigc_zoo/model_zoo/chatglm/reward_model.py,sha256=Xa5yONvwlIknxMEK2Y59gE_our5iICtsUyaPmi86by0,9700
 aigc_zoo/model_zoo/chatglm/tokenization_chatglm.py,sha256=IMyHa8uPOgE0ia1DYp8Lx-IZ0N4TKSh1HVlA5sDdw-s,17037
 aigc_zoo/model_zoo/chatglm2/__init__.py,sha256=3cMgJqib4OqHJHv37rn3xHzyBbGl9s1zpTqd549QDmw,77
 aigc_zoo/model_zoo/chatglm2/chatglm_model.py,sha256=5bqiInqxxSAi0DB4zDZmzEQ_v4DluJQbnhTlx8R31Ik,114
-aigc_zoo/model_zoo/chatglm2/llm_model.py,sha256=l4iUZjJWUy3hpb9v6bbb9s6oVUCqWLJmm7QD0MirU40,9839
-aigc_zoo/model_zoo/chatglm2/tokenization_chatglm.py,sha256=eU2mw3psfMURCPVVqB0yLPDJuR4XtftFnnM6kiDCZZI,9252
+aigc_zoo/model_zoo/chatglm2/llm_model.py,sha256=8OJsp7qGhJkXLzmj8JXuGQ8HXk1cHUQj14p8Rex6aoc,9402
+aigc_zoo/model_zoo/chatglm2/tokenization_chatglm.py,sha256=LFOlpiWgpz6oRjNimO5T85Gm6q-nbunyrpm--nQOcJo,10002
 aigc_zoo/model_zoo/llm/__init__.py,sha256=RFimplzKNFznknZ0MzZDOhcvck-tAJQ53rTCMX-shS8,77
 aigc_zoo/model_zoo/llm/ilql_model.py,sha256=ZMpmamGRakLJx3V3ynS8XUN8s0IXLpNAD8WdRfDbdcw,6344
 aigc_zoo/model_zoo/llm/llm_model.py,sha256=x176u-JFBww6RtAKzOUevUL7iQQ6t50xrlg2vom-uaM,5443
 aigc_zoo/model_zoo/llm/ppo_model.py,sha256=tH0Rk1Oy4AOFrvs7tYtrmAjJY5Xoxugk3XILVvLfic4,6298
 aigc_zoo/model_zoo/llm/reward_model.py,sha256=Wa7fkI0z83Lg9uy8GZBN_JQ7kkhpnf6YLzZSjqm1YCQ,9732
 aigc_zoo/model_zoo/llm/rrhf_model.py,sha256=bTN95boS_ndI9_-ux0xHeL1B7vgQXvEKdJZezyTO0zg,6704
 aigc_zoo/model_zoo/moss/__init__.py,sha256=RFimplzKNFznknZ0MzZDOhcvck-tAJQ53rTCMX-shS8,77
 aigc_zoo/model_zoo/moss/llm_model.py,sha256=_Z8uPLQBlvTMoY_tABvjkY07sFOHcObKxAynOg9A6kY,4554
 aigc_zoo/model_zoo/moss/moss_model.py,sha256=lwvkju3ZdQeir0gO15uvVLCcKbpgmO9iq1Kbu8a3cAw,2050
 aigc_zoo/model_zoo/rwkv4/__init__.py,sha256=RFimplzKNFznknZ0MzZDOhcvck-tAJQ53rTCMX-shS8,77
-aigc_zoo/model_zoo/rwkv4/llm_model.py,sha256=_EjnUp_TnzFWiotKSW6VqhZfHkupT_91yyy6KhWqyyQ,5529
+aigc_zoo/model_zoo/rwkv4/llm_model.py,sha256=9LwhDnf2CMMyN9R5W0XqX4EM_AXMdywB85_QObuzRwI,5734
+aigc_zoo/model_zoo/rwkv4/rwkv4_tokenizer.py,sha256=m0khp_eThJPTgb5l14D5Hl2CAdFkJLu9y42WG9QXGS0,6519
 aigc_zoo/model_zoo/t5/__init__.py,sha256=RFimplzKNFznknZ0MzZDOhcvck-tAJQ53rTCMX-shS8,77
 aigc_zoo/model_zoo/t5/llm_model.py,sha256=CJmPXz4Q04geCgMFiN8AyPYLwVfthW0UvdZhipkUdWw,4950
 aigc_zoo/model_zoo/t5/ppo_model.py,sha256=eXm5sKi4WgISU95r25OCJhrP_ziYy3wRwALn1bf6_24,5848
 aigc_zoo/model_zoo/t5/reward_model.py,sha256=YhWq_Q6zNgQYlyrR3R79NDUkf4BZZiSB8gMzjS2n9kY,9098
 aigc_zoo/utils/__init__.py,sha256=Oc9cllKC2z1rKpYMLkfRj01Jud2WLQaZ_Dd89t4sreY,77
 aigc_zoo/utils/llm_generate.py,sha256=92TvTXISdU7GSrBgMYJoFyicWxkXrm_-02O4jcDnMp0,2664
 aigc_zoo/utils/moss_generate.py,sha256=NYcvqjm3NbutslYlF8_7_BiHNBMPPI0mZzVui4nmkIU,13198
-aigc_zoo-0.1.11.post2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-aigc_zoo-0.1.11.post2.dist-info/METADATA,sha256=bLqgWbIldHw5N-2k-IxlJxBj-wGIhuR5ndW-hRO93Jk,372
-aigc_zoo-0.1.11.post2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aigc_zoo-0.1.11.post2.dist-info/top_level.txt,sha256=dl7_T4oT72ShHHM2khyOXJL4Kyvq0u_TdVolu-lKbnY,9
-aigc_zoo-0.1.11.post2.dist-info/RECORD,,
+aigc_zoo/utils/rwkv4_generate.py,sha256=y0HzEYG5Wu9r4NIoFE8rhealv_KJriV8rlhEV-tJpnU,3429
+aigc_zoo-0.1.12.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+aigc_zoo-0.1.12.dist-info/METADATA,sha256=wR0UefS7y3EKbxFUZoGb4k6Y18K4ihqcWdGO_xyCHYU,366
+aigc_zoo-0.1.12.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aigc_zoo-0.1.12.dist-info/top_level.txt,sha256=dl7_T4oT72ShHHM2khyOXJL4Kyvq0u_TdVolu-lKbnY,9
+aigc_zoo-0.1.12.dist-info/RECORD,,
```

