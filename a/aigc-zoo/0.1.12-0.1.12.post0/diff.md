# Comparing `tmp/aigc_zoo-0.1.12-py3-none-any.whl.zip` & `tmp/aigc_zoo-0.1.12.post0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 67408 bytes, number of entries: 42
+Zip file size: 67478 bytes, number of entries: 42
 -rw-rw-rw-  2.0 fat       80 b- defN 23-Jun-16 14:31 aigc_zoo/__init__.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/__init__.py
 -rw-rw-rw-  2.0 fat       66 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/baichuan/__init__.py
 -rw-rw-rw-  2.0 fat     5578 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/baichuan/llm_model.py
 -rw-rw-rw-  2.0 fat     9574 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/baichuan/tokenization_baichuan.py
 -rw-rw-rw-  2.0 fat       66 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/baichuan2/__init__.py
 -rw-rw-rw-  2.0 fat     5575 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/baichuan2/llm_model.py
@@ -23,22 +23,22 @@
 -rw-rw-rw-  2.0 fat     9732 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/llm/reward_model.py
 -rw-rw-rw-  2.0 fat     6704 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/llm/rrhf_model.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/moss/__init__.py
 -rw-rw-rw-  2.0 fat     4554 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/moss/llm_model.py
 -rw-rw-rw-  2.0 fat     2050 b- defN 23-Jun-16 14:52 aigc_zoo/model_zoo/moss/moss_model.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/rwkv4/__init__.py
 -rw-rw-rw-  2.0 fat     5734 b- defN 23-Jul-16 03:08 aigc_zoo/model_zoo/rwkv4/llm_model.py
--rw-rw-rw-  2.0 fat     6519 b- defN 23-Jul-16 04:58 aigc_zoo/model_zoo/rwkv4/rwkv4_tokenizer.py
+-rw-rw-rw-  2.0 fat     6519 b- defN 23-Jul-16 05:58 aigc_zoo/model_zoo/rwkv4/rwkv4_tokenizer.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/model_zoo/t5/__init__.py
 -rw-rw-rw-  2.0 fat     4950 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/t5/llm_model.py
 -rw-rw-rw-  2.0 fat     5848 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/t5/ppo_model.py
 -rw-rw-rw-  2.0 fat     9098 b- defN 23-Jul-11 11:21 aigc_zoo/model_zoo/t5/reward_model.py
 -rw-rw-rw-  2.0 fat       77 b- defN 23-Jun-16 11:35 aigc_zoo/utils/__init__.py
 -rw-rw-rw-  2.0 fat     2664 b- defN 23-Jul-13 10:54 aigc_zoo/utils/llm_generate.py
 -rw-rw-rw-  2.0 fat    13198 b- defN 23-Jul-13 11:08 aigc_zoo/utils/moss_generate.py
 -rw-rw-rw-  2.0 fat     3429 b- defN 23-Jul-15 15:45 aigc_zoo/utils/rwkv4_generate.py
--rw-rw-rw-  2.0 fat    11357 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      366 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     3877 b- defN 23-Jul-16 05:54 aigc_zoo-0.1.12.dist-info/RECORD
-42 files, 208288 bytes uncompressed, 61072 bytes compressed:  70.7%
+-rw-rw-rw-  2.0 fat    11357 b- defN 23-Jul-16 05:59 aigc_zoo-0.1.12.post0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      372 b- defN 23-Jul-16 05:59 aigc_zoo-0.1.12.post0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-16 05:59 aigc_zoo-0.1.12.post0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-Jul-16 05:59 aigc_zoo-0.1.12.post0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     3907 b- defN 23-Jul-16 05:59 aigc_zoo-0.1.12.post0.dist-info/RECORD
+42 files, 208324 bytes uncompressed, 61082 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -105,23 +105,23 @@
 
 Filename: aigc_zoo/utils/moss_generate.py
 Comment: 
 
 Filename: aigc_zoo/utils/rwkv4_generate.py
 Comment: 
 
-Filename: aigc_zoo-0.1.12.dist-info/LICENSE
+Filename: aigc_zoo-0.1.12.post0.dist-info/LICENSE
 Comment: 
 
-Filename: aigc_zoo-0.1.12.dist-info/METADATA
+Filename: aigc_zoo-0.1.12.post0.dist-info/METADATA
 Comment: 
 
-Filename: aigc_zoo-0.1.12.dist-info/WHEEL
+Filename: aigc_zoo-0.1.12.post0.dist-info/WHEEL
 Comment: 
 
-Filename: aigc_zoo-0.1.12.dist-info/top_level.txt
+Filename: aigc_zoo-0.1.12.post0.dist-info/top_level.txt
 Comment: 
 
-Filename: aigc_zoo-0.1.12.dist-info/RECORD
+Filename: aigc_zoo-0.1.12.post0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aigc_zoo/model_zoo/rwkv4/rwkv4_tokenizer.py

```diff
@@ -62,16 +62,16 @@
             x = eval(l[l.index(' '):l.rindex(' ')])
             x = x.encode("utf-8") if isinstance(x, str) else x
             assert isinstance(x, bytes)
             assert len(x) == int(l[l.rindex(' '):])
             sorted += [x]
             self.idx2token[idx] = x
 
-        # if 0 not in self.idx2token:
-        #     self.idx2token[0] = "<|endoftext|>".encode("utf-8")
+        if 0 not in self.idx2token:
+            self.idx2token[0] = "<|endoftext|>".encode("utf-8")
 
         self.token2idx = {}
         for k, v in self.idx2token.items():
             self.token2idx[v] = int(k)
 
         self.root = TRIE()
         for t, i in self.token2idx.items():
@@ -191,16 +191,16 @@
         super().__init__(name)
         if os.path.isdir(pretrained_model_name_or_path):
             pretrained_model_name_or_path = os.path.join(pretrained_model_name_or_path,'rwkv_vocab_v20230424.txt')
         self.tokenizer : TRIE_TOKENIZER = TRIE_TOKENIZER(pretrained_model_name_or_path)
         for k,v in kwargs.items():
             setattr(self,k,v)
 
-        self.eod_id = 0  # self.tokenizer.token_to_id("<|endoftext|>")
-        self.pad_id = self.tokenizer.token_to_id("<|padding|>")
+        # self.eod_id = 0  # self.tokenizer.token_to_id("<|endoftext|>")
+        # self.pad_id = self.tokenizer.token_to_id("<|padding|>")
 
     @classmethod
     def from_pretrained(
             cls,
             pretrained_model_name_or_path: Union[str, os.PathLike],
             **kwargs
     ):
```

## Comparing `aigc_zoo-0.1.12.dist-info/LICENSE` & `aigc_zoo-0.1.12.post0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aigc_zoo-0.1.12.dist-info/RECORD` & `aigc_zoo-0.1.12.post0.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 aigc_zoo/model_zoo/llm/reward_model.py,sha256=Wa7fkI0z83Lg9uy8GZBN_JQ7kkhpnf6YLzZSjqm1YCQ,9732
 aigc_zoo/model_zoo/llm/rrhf_model.py,sha256=bTN95boS_ndI9_-ux0xHeL1B7vgQXvEKdJZezyTO0zg,6704
 aigc_zoo/model_zoo/moss/__init__.py,sha256=RFimplzKNFznknZ0MzZDOhcvck-tAJQ53rTCMX-shS8,77
 aigc_zoo/model_zoo/moss/llm_model.py,sha256=_Z8uPLQBlvTMoY_tABvjkY07sFOHcObKxAynOg9A6kY,4554
 aigc_zoo/model_zoo/moss/moss_model.py,sha256=lwvkju3ZdQeir0gO15uvVLCcKbpgmO9iq1Kbu8a3cAw,2050
 aigc_zoo/model_zoo/rwkv4/__init__.py,sha256=RFimplzKNFznknZ0MzZDOhcvck-tAJQ53rTCMX-shS8,77
 aigc_zoo/model_zoo/rwkv4/llm_model.py,sha256=9LwhDnf2CMMyN9R5W0XqX4EM_AXMdywB85_QObuzRwI,5734
-aigc_zoo/model_zoo/rwkv4/rwkv4_tokenizer.py,sha256=m0khp_eThJPTgb5l14D5Hl2CAdFkJLu9y42WG9QXGS0,6519
+aigc_zoo/model_zoo/rwkv4/rwkv4_tokenizer.py,sha256=p32IYzEyE6Snxkl8Ds7GuhGHXTiDezUUKbWOsN62vxw,6519
 aigc_zoo/model_zoo/t5/__init__.py,sha256=RFimplzKNFznknZ0MzZDOhcvck-tAJQ53rTCMX-shS8,77
 aigc_zoo/model_zoo/t5/llm_model.py,sha256=CJmPXz4Q04geCgMFiN8AyPYLwVfthW0UvdZhipkUdWw,4950
 aigc_zoo/model_zoo/t5/ppo_model.py,sha256=eXm5sKi4WgISU95r25OCJhrP_ziYy3wRwALn1bf6_24,5848
 aigc_zoo/model_zoo/t5/reward_model.py,sha256=YhWq_Q6zNgQYlyrR3R79NDUkf4BZZiSB8gMzjS2n9kY,9098
 aigc_zoo/utils/__init__.py,sha256=Oc9cllKC2z1rKpYMLkfRj01Jud2WLQaZ_Dd89t4sreY,77
 aigc_zoo/utils/llm_generate.py,sha256=92TvTXISdU7GSrBgMYJoFyicWxkXrm_-02O4jcDnMp0,2664
 aigc_zoo/utils/moss_generate.py,sha256=NYcvqjm3NbutslYlF8_7_BiHNBMPPI0mZzVui4nmkIU,13198
 aigc_zoo/utils/rwkv4_generate.py,sha256=y0HzEYG5Wu9r4NIoFE8rhealv_KJriV8rlhEV-tJpnU,3429
-aigc_zoo-0.1.12.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-aigc_zoo-0.1.12.dist-info/METADATA,sha256=wR0UefS7y3EKbxFUZoGb4k6Y18K4ihqcWdGO_xyCHYU,366
-aigc_zoo-0.1.12.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aigc_zoo-0.1.12.dist-info/top_level.txt,sha256=dl7_T4oT72ShHHM2khyOXJL4Kyvq0u_TdVolu-lKbnY,9
-aigc_zoo-0.1.12.dist-info/RECORD,,
+aigc_zoo-0.1.12.post0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+aigc_zoo-0.1.12.post0.dist-info/METADATA,sha256=oWBvLGJ6LprsHygmnB6ygJ4DNSN9e_nyI65pfIlBOa4,372
+aigc_zoo-0.1.12.post0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aigc_zoo-0.1.12.post0.dist-info/top_level.txt,sha256=dl7_T4oT72ShHHM2khyOXJL4Kyvq0u_TdVolu-lKbnY,9
+aigc_zoo-0.1.12.post0.dist-info/RECORD,,
```

