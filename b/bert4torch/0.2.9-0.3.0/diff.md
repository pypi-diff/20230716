# Comparing `tmp/bert4torch-0.2.9.tar.gz` & `tmp/bert4torch-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert4torch-0.2.9.tar", last modified: Wed Jul  5 15:31:43 2023, max compression
+gzip compressed data, was "bert4torch-0.3.0.tar", last modified: Sun Jul 16 11:37:02 2023, max compression
```

## Comparing `bert4torch-0.2.9.tar` & `bert4torch-0.3.0.tar`

### file list

```diff
@@ -1,24 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 15:31:43.818426 bert4torch-0.2.9/
--rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.2.9/LICENSE
--rw-rw-rw-   0        0        0    23958 2023-07-05 15:31:43.818426 bert4torch-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0    23706 2023-07-05 13:40:22.000000 bert4torch-0.2.9/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 15:31:43.797421 bert4torch-0.2.9/bert4torch/
--rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.2.9/bert4torch/__init__.py
--rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.2.9/bert4torch/activations.py
--rw-rw-rw-   0        0        0    11080 2023-06-02 14:19:57.000000 bert4torch-0.2.9/bert4torch/callbacks.py
--rw-rw-rw-   0        0        0    38007 2023-05-23 15:20:25.000000 bert4torch-0.2.9/bert4torch/generation.py
--rw-rw-rw-   0        0        0    93124 2023-07-05 14:53:38.000000 bert4torch-0.2.9/bert4torch/layers.py
--rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.2.9/bert4torch/losses.py
--rw-rw-rw-   0        0        0   127005 2023-07-05 14:16:53.000000 bert4torch-0.2.9/bert4torch/models.py
--rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.2.9/bert4torch/optimizers.py
--rw-rw-rw-   0        0        0    20836 2023-06-24 12:53:34.000000 bert4torch-0.2.9/bert4torch/quantization.py
--rw-rw-rw-   0        0        0    20933 2023-06-26 16:27:26.000000 bert4torch-0.2.9/bert4torch/snippets.py
--rw-rw-rw-   0        0        0    35326 2023-04-28 12:14:08.000000 bert4torch-0.2.9/bert4torch/tokenizers.py
-drwxrwxrwx   0        0        0        0 2023-07-05 15:31:43.816424 bert4torch-0.2.9/bert4torch.egg-info/
--rw-rw-rw-   0        0        0    23958 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      456 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-05 15:31:43.000000 bert4torch-0.2.9/bert4torch.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-05 15:31:43.819426 bert4torch-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0      551 2023-07-05 15:30:52.000000 bert4torch-0.2.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.416569 bert4torch-0.3.0/
+-rw-rw-rw-   0        0        0     1089 2022-03-12 16:30:24.000000 bert4torch-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    25777 2023-07-16 11:37:02.415552 bert4torch-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    25525 2023-07-16 10:38:17.000000 bert4torch-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.382552 bert4torch-0.3.0/bert4torch/
+-rw-rw-rw-   0        0        0        0 2022-11-28 12:30:45.000000 bert4torch-0.3.0/bert4torch/__init__.py
+-rw-rw-rw-   0        0        0     3228 2023-06-30 17:02:35.000000 bert4torch-0.3.0/bert4torch/activations.py
+-rw-rw-rw-   0        0        0    10939 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/callbacks.py
+-rw-rw-rw-   0        0        0    40578 2023-07-16 10:39:25.000000 bert4torch-0.3.0/bert4torch/generation.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.395563 bert4torch-0.3.0/bert4torch/layers/
+-rw-rw-rw-   0        0        0      296 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/layers/__init__.py
+-rw-rw-rw-   0        0        0    25425 2023-07-16 09:13:49.000000 bert4torch-0.3.0/bert4torch/layers/attention.py
+-rw-rw-rw-   0        0        0     8515 2023-07-15 16:04:22.000000 bert4torch-0.3.0/bert4torch/layers/core.py
+-rw-rw-rw-   0        0        0    12699 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/layers/crf.py
+-rw-rw-rw-   0        0        0     4474 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/layers/global_point.py
+-rw-rw-rw-   0        0        0    17108 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/layers/misc.py
+-rw-rw-rw-   0        0        0    14305 2023-07-16 10:41:24.000000 bert4torch-0.3.0/bert4torch/layers/position_encoding.py
+-rw-rw-rw-   0        0        0    16283 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/layers/transformer_block.py
+-rw-rw-rw-   0        0        0    16631 2023-06-26 16:27:26.000000 bert4torch-0.3.0/bert4torch/losses.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.414553 bert4torch-0.3.0/bert4torch/models/
+-rw-rw-rw-   0        0        0     7651 2023-07-14 15:19:38.000000 bert4torch-0.3.0/bert4torch/models/__init__.py
+-rw-rw-rw-   0        0        0     7811 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/albert.py
+-rw-rw-rw-   0        0        0     6913 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/bart.py
+-rw-rw-rw-   0        0        0    20254 2023-07-16 10:07:15.000000 bert4torch-0.3.0/bert4torch/models/base.py
+-rw-rw-rw-   0        0        0    18082 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/bert.py
+-rw-rw-rw-   0        0        0     4283 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/deberta.py
+-rw-rw-rw-   0        0        0     2233 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/electra.py
+-rw-rw-rw-   0        0        0      932 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/erinie.py
+-rw-rw-rw-   0        0        0     1728 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/gau_alpha.py
+-rw-rw-rw-   0        0        0    12236 2023-07-14 14:25:09.000000 bert4torch-0.3.0/bert4torch/models/glm.py
+-rw-rw-rw-   0        0        0     7917 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/gpt.py
+-rw-rw-rw-   0        0        0     4535 2023-07-15 10:36:15.000000 bert4torch-0.3.0/bert4torch/models/llama.py
+-rw-rw-rw-   0        0        0      457 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/nezha.py
+-rw-rw-rw-   0        0        0     2399 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/roformer.py
+-rw-rw-rw-   0        0        0    10276 2023-07-11 14:03:23.000000 bert4torch-0.3.0/bert4torch/models/t5.py
+-rw-rw-rw-   0        0        0     5268 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/transformer.py
+-rw-rw-rw-   0        0        0     9217 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/transformer_xl.py
+-rw-rw-rw-   0        0        0     2469 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/uie.py
+-rw-rw-rw-   0        0        0     4802 2023-07-06 12:55:22.000000 bert4torch-0.3.0/bert4torch/models/xlnet.py
+-rw-rw-rw-   0        0        0     7619 2023-03-29 15:35:29.000000 bert4torch-0.3.0/bert4torch/optimizers.py
+-rw-rw-rw-   0        0        0    20808 2023-07-16 10:34:11.000000 bert4torch-0.3.0/bert4torch/quantization.py
+-rw-rw-rw-   0        0        0    23410 2023-07-16 10:34:24.000000 bert4torch-0.3.0/bert4torch/snippets.py
+-rw-rw-rw-   0        0        0    35456 2023-07-13 15:00:01.000000 bert4torch-0.3.0/bert4torch/tokenizers.py
+drwxrwxrwx   0        0        0        0 2023-07-16 11:37:02.387556 bert4torch-0.3.0/bert4torch.egg-info/
+-rw-rw-rw-   0        0        0    25777 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-16 11:37:02.000000 bert4torch-0.3.0/bert4torch.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 11:37:02.417566 bert4torch-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      551 2023-07-16 10:05:26.000000 bert4torch-0.3.0/setup.py
```

### Comparing `bert4torch-0.2.9/LICENSE` & `bert4torch-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.9/PKG-INFO` & `bert4torch-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bert4torch
-Version: 0.2.9
+Version: 0.3.0
 Summary: an elegant bert4torch
 Home-page: https://github.com/Tongjilibo/bert4torch
 Author: Tongjilibo
 License: MIT Licence
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -74,14 +74,16 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
+- **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
+- **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
@@ -96,14 +98,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
 | 0.2.4          | 0.0.3.post2     |
@@ -112,16 +115,17 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
-- **20230612**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
-- **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
+- **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
+- **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
 - **20221102**：增加CNN_Nested_NER示例, 删除SpTokenizer基类中的rematch
@@ -185,20 +189,22 @@
 | t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
-|chinese_llama_alpaca|哈工大|[torch](https://github.com/ymcui/Chinese-LLaMA-Alpaca)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
-| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
-| Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
-| chatglm-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| chatglm2-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM2-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+|chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
+| Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
+| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
+| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
```

### Comparing `bert4torch-0.2.9/README.md` & `bert4torch-0.3.0/bert4torch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: bert4torch
+Version: 0.3.0
+Summary: an elegant bert4torch
+Home-page: https://github.com/Tongjilibo/bert4torch
+Author: Tongjilibo
+License: MIT Licence
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
@@ -64,14 +74,16 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
+- **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
+- **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
@@ -86,14 +98,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
 | 0.2.4          | 0.0.3.post2     |
@@ -102,16 +115,17 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
-- **20230612**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
-- **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
+- **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
+- **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
 - **20221102**：增加CNN_Nested_NER示例, 删除SpTokenizer基类中的rematch
@@ -175,20 +189,22 @@
 | t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
-|chinese_llama_alpaca|哈工大|[torch](https://github.com/ymcui/Chinese-LLaMA-Alpaca)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
-| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
-| Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
-| chatglm-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| chatglm2-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM2-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+|chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
+| Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
+| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
+| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
@@ -228,8 +244,8 @@
     <tr align="center" >
       <td>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.2.9/bert4torch/activations.py` & `bert4torch-0.3.0/bert4torch/activations.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.9/bert4torch/callbacks.py` & `bert4torch-0.3.0/bert4torch/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import torch
 import torch.nn.functional as F
-import torch.nn as nn
 from torch4keras.snippets import *
-from bert4torch.layers import BottleneckAdapterLayer
-try:
-    # torch4keras0.0.7增加了callbacks
-    from torch4keras.callbacks import *
-except:
-    pass
+from torch4keras.callbacks import *
+
 
 class FGM():
     '''FGM对抗训练'''
     def __init__(self, model):
         self.model = model
         self.backup = {}
```

### Comparing `bert4torch-0.2.9/bert4torch/generation.py` & `bert4torch-0.3.0/bert4torch/generation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,63 +1,93 @@
 '''自回归模型的生成
 '''
-
 import torch
 import torch.nn as nn
 import numpy as np
-from bert4torch.snippets import take_along_dim, torch_div, sequence_padding, create_position_ids_start_at_padding, colorful
+import inspect
+from bert4torch.snippets import take_along_dim, torch_div, sequence_padding, create_position_ids_start_at_padding, log_info, log_warn
+from bert4torch.tokenizers import TokenizerBase
+
+
+def repetition_penalty_func(input_ids: torch.LongTensor, scores: torch.FloatTensor, penalty: float) -> torch.FloatTensor:
+    score = torch.gather(scores, 1, input_ids)
+    # if score < 0 then repetition penalty has to be multiplied to reduce the previous token probability
+    score = torch.where(score < 0, score * penalty, score / penalty)
+    scores.scatter_(1, input_ids, score)
+    return scores
+
 
 class AutoRegressiveDecoder(object):
     """通用自回归生成模型解码基类
     包含beam search和random sample两种策略
 
     :param start_id: int, 解码使用的起始token_id，不同预训练模型设置可能不一样
     :param end_id: int, 解码使用的结束token_id，不同预训练模型设置可能不一样
     :param maxlen: int, 最大解码长度
     :param minlen: int, 最小解码长度, 默认为1
     :param device: str, 默认为'cpu'
     """
-    def __init__(self, start_id, end_id, maxlen, minlen=1, pad_id=0, pad_mode='post', device='cpu'):
+    def __init__(self, start_id, end_id, maxlen, minlen=1, pad_id=0, pad_mode='post', device='cpu', 
+                 n=1, topk=50, topp=1, temperature=1, repetition_penalty=1.0, min_ends=1):
         self.start_id = start_id
         self.end_id = end_id
         self.maxlen = maxlen
         self.minlen = minlen
-        self.models = {}
-        self.device = device
-        self.use_batch = False
         self.pad_id = pad_id   # pad_token_id兼容bert4torch和hf的，如错误则需要显式传入pad_id:int
         self.pad_mode = pad_mode
+        self.device = device
+
+        # generation_config
+        self.n = n
+        self.topk = topk
+        self.topp = topp
+        self.temperature = temperature
+        self.repetition_penalty = repetition_penalty
+        self.min_ends = min_ends
+
+        self.use_batch = False
         if start_id is None:
             self.first_output_ids = torch.empty((1, 0), dtype=int, device=device)
         else:
             self.first_output_ids = torch.tensor([[self.start_id]], device=device)
 
+    def set_generation_config(self, generation_config):
+        for key, value in generation_config.items():
+            if not hasattr(self, key):
+                raise ValueError(f'Generation_config `{key}` has not been pre maintained')
+            setattr(self, key, value)
+
     @staticmethod
     def wraps(default_rtype='probas', use_states=False):
         """用来进一步完善predict函数
 
         目前包含: 
             1. 设置rtype参数，并做相应处理；
             2. 确定states的使用，并做相应处理；
             3. 设置温度参数，并做相应处理。
         """
         def actual_decorator(predict):
-            def new_predict(self, inputs, output_ids, states, temperature=1, rtype=default_rtype):
+            def new_predict(self, inputs, output_ids, states, rtype=default_rtype):
                 assert rtype in ['probas', 'logits']
                 prediction = predict(self, inputs, output_ids, states)
 
                 if use_states:
                     assert len(prediction) == 2, 'Should return 2 output when set use_states=True'
                 else:
                     prediction = (prediction, None)
 
+                # repetition_penalty
+                if self.repetition_penalty != 1.0:
+                    past_token_ids = inputs[0] if states is None else states['past_token_ids']
+                    prediction = (repetition_penalty_func(past_token_ids, prediction[0], self.repetition_penalty), prediction[1])
+
                 if default_rtype == 'logits':
-                    prediction = (nn.Softmax(dim=-1)(prediction[0] / temperature), prediction[1])
-                elif temperature != 1:
-                    probas = torch.pow(prediction[0], 1.0 / temperature)
+                    prediction = (nn.Softmax(dim=-1)(prediction[0] / self.temperature), prediction[1])
+                elif self.temperature != 1:
+                    probas = torch.pow(prediction[0], 1.0 / self.temperature)
                     probas = probas / probas.sum(axis=-1, keepdims=True)
                     prediction = (probas, prediction[1])
 
                 if rtype == 'probas':
                     return prediction
                 else:
                     return torch.log(prediction[0] + 1e-12), prediction[1]
@@ -96,123 +126,123 @@
         for input_ in inputs_raw:
             # encoder-decoder传入的encoder_hidden_states和encoder_attention_mask
             if isinstance(input_, torch.Tensor):
                 input_new = input_
             elif isinstance(input_, (list, tuple, np.ndarray)):
                 # 单条样本为[1,2,3]格式，需转为[[1,2,3]]
                 input_ = input_ if self.use_batch else [input_]
-                input_new = torch.tensor(sequence_padding(input_, value=self.pad_id, mode=self.pad_mode), device=self.device)
+                input_new = torch.tensor(sequence_padding(input_, value=self.pad_id, mode=self.pad_mode), dtype=torch.long, device=self.device)
 
                 # padding在右边则input_seqlen是真实的长度，左边则统一为最大程度
                 if self.pad_mode in {'post', 'right'}:
                     self.input_seqlen = torch.tensor([len(i) for i in input_]).to(self.device)
                 else:
                     max_len = input_new.shape[1]
                     self.input_seqlen = torch.tensor([max_len]*len(input_new)).to(self.device)
             else:
                 raise ValueError('Beam search inputs ele only support tensor、array、list、tuple')
             inputs.append(input_new)
         return inputs
 
-    def __beam_search_step(self, step, inputs, output_ids, output_scores, topk, states, temperature):
+    def __beam_search_step(self, step, inputs, output_ids, output_scores, states):
         '''beam_search单条推理计算得分'''
         self.step = step
-        scores, states = self.predict(inputs, output_ids, states, temperature, 'logits')  # 计算当前得分
+        scores, states = self.predict(inputs, output_ids, states, 'logits')  # 计算当前得分
         if step == 0:  # 第1步预测后将输入重复topk次
-            inputs = [i.repeat([topk]+[1]*(len(i.shape)-1)) for i in inputs]
+            inputs = [i.repeat([self.topk]+[1]*(len(i.shape)-1)) for i in inputs]
         scores = output_scores.reshape((-1, 1)) + scores  # 综合累积得分
-        indices = scores.flatten().argsort(dim=-1, descending=True)[:topk]  # 仅保留topk
+        indices = scores.flatten().argsort(dim=-1, descending=True)[:self.topk]  # 仅保留topk
         indices_1 = torch_div(indices, scores.shape[1], rounding_mode='floor')  # 兼容老版本
         indices_2 = (indices % scores.shape[1]).reshape((-1, 1))  # 列索引
         output_ids = torch.cat([output_ids[indices_1], indices_2], 1)  # 更新输出
         output_scores = take_along_dim(scores, indices, dim=None)  # 更新得分
         return inputs, output_ids, output_scores, states
 
-    def __beam_search_end(self, inputs, output_ids, output_scores, topk, results, min_ends):
+    def __beam_search_end(self, inputs, output_ids, output_scores, results):
         '''beam_search单条推理计算是否结束'''
         break_tag = False
         is_end = output_ids[:, -1] == self.end_id  # 标记是否以end标记结束
         end_counts = (output_ids == self.end_id).sum(1)  # 统计出现的end标记
-        flag = ~is_end | (end_counts < min_ends)  # 标记未完成序列
+        flag = ~is_end | (end_counts < self.min_ends)  # 标记未完成序列
         self.flag = flag  # 记录未完成序列
         if output_ids.shape[1] >= self.minlen:  # 最短长度判断
             best = output_scores.argmax()  # 得分最大的那个
-            if is_end[best] and end_counts[best] >= min_ends:  # 如果已经终止
+            if is_end[best] and end_counts[best] >= self.min_ends:  # 如果已经终止
                 break_tag = True
             elif not flag.all():  # 如果有已完成的
                 inputs = [i[flag] for i in inputs]  # 扔掉已完成序列
                 output_ids = output_ids[flag]  # 扔掉已完成序列
                 output_scores = output_scores[flag]  # 扔掉已完成序列
                 end_counts = end_counts[flag]  # 扔掉已完成end计数
-                topk = flag.sum()  # topk相应变化
-        return inputs, output_ids, output_scores, topk, results, break_tag
+                self.topk = flag.sum()  # topk相应变化
+        return inputs, output_ids, output_scores, results, break_tag
 
-    def __batch_beam_search_step(self, step, inputs, output_ids, output_scores, topks, states, temperature):
+    def __batch_beam_search_step(self, step, inputs, output_ids, output_scores, states):
         '''beam_search batch条推理计算得分'''
         self.step = step
-        scores, states = self.predict(inputs, output_ids, states, temperature, 'logits')  # 计算当前得分
+        scores, states = self.predict(inputs, output_ids, states, 'logits')  # 计算当前得分
         if step == 0:  # 第0步预测后将输入重复topk次
             inputs_new = []
             for input_ in inputs:
                 inputs_ = []
-                for topk, input_i in zip(topks, input_):
+                for topk, input_i in zip(self.topk, input_):
                     input_i = input_i.unsqueeze(0)
                     inputs_.append(input_i.repeat([topk]+[1]*(len(input_i.shape)-1)))
                 inputs_new.append(torch.cat(inputs_))
             inputs = inputs_new
             # 对seq_len进行扩充
             input_seqlen = []
-            for topk, input_seqlen_i in zip(topks, self.input_seqlen):
+            for topk, input_seqlen_i in zip(self.topk, self.input_seqlen):
                 input_seqlen.append(input_seqlen_i.repeat(topk))
             self.input_seqlen = torch.cat(input_seqlen)
 
         scores = output_scores.reshape((-1, 1)) + scores  # 综合累积得分
         output_ids_new, output_scores_new = [], []
-        for smp_i, topk in enumerate(topks):
+        for smp_i, topk in enumerate(self.topk):
             if step == 0:
                 score = scores[smp_i][None, ...]
                 output_id = output_ids[smp_i][None, ...]
             else:
-                start, end = sum(topks[:smp_i]), sum(topks[:smp_i+1])
+                start, end = sum(self.topk[:smp_i]), sum(self.topk[:smp_i+1])
                 score = scores[start:end]
                 output_id = output_ids[start:end]
 
             indices = score.flatten().argsort(dim=-1, descending=True)[:topk]  # 仅保留topk
             indices_1 = torch_div(indices, score.shape[1], rounding_mode='floor')  # 兼容老版本
             indices_2 = (indices % score.shape[1]).reshape((-1, 1))  # 列索引
             output_id = torch.cat([output_id[indices_1], indices_2], 1)  # 更新输出
             output_score = take_along_dim(score, indices, dim=None)  # 更新得分
             output_ids_new.append(output_id)
             output_scores_new.append(output_score)
         output_ids_new = torch.cat(output_ids_new)
         output_scores_new = torch.cat(output_scores_new)
         return inputs, output_ids_new, output_scores_new, states
 
-    def __batch_beam_search_end(self, inputs, output_ids, output_scores, topks, results, min_ends):
+    def __batch_beam_search_end(self, inputs, output_ids, output_scores, results):
         break_tag = False
         is_end = output_ids[:, -1] == self.end_id  # 标记是否以end标记结束
         end_counts = (output_ids == self.end_id).sum(1)  # 统计出现的end标记
-        self.flag = ~is_end | (end_counts < min_ends)  # 标记未完成序列
+        self.flag = ~is_end | (end_counts < self.min_ends)  # 标记未完成序列
 
         if output_ids.shape[1] >= self.minlen:  # 最短长度判断
             inputs_new, output_ids_new, output_scores_new, flag_new = [], [], [], []
-            topks_new = topks.copy()
-            for smp_i, topk in enumerate(topks):
+            topks_new = self.topk.copy()
+            for smp_i, topk in enumerate(self.topk): # 这里的topk是一个list
                 if topk == 0:
                     continue
-                start, end = sum(topks[:smp_i]), sum(topks[:smp_i+1])
+                start, end = sum(self.topk[:smp_i]), sum(self.topk[:smp_i+1])
                 input_ = [i[start:end] for i in inputs]
                 output_score = output_scores[start:end]
                 output_id = output_ids[start:end]
 
                 best = output_score.argmax()  # 得分最大的那个
                 is_end = output_id[:, -1] == self.end_id  # 标记是否以end标记结束
                 end_counts = (output_id == self.end_id).sum(1)  # 统计出现的end标记
-                flag = ~is_end | (end_counts < min_ends)  # 标记未完成序列
-                if is_end[best] and end_counts[best] >= min_ends:  # 如果已经终止
+                flag = ~is_end | (end_counts < self.min_ends)  # 标记未完成序列
+                if is_end[best] and end_counts[best] >= self.min_ends:  # 如果已经终止
                     results[smp_i] = output_id[output_score.argmax()]
                     flag = torch.zeros_like(flag, dtype=torch.bool)
                 if not flag.all():  # 如果有已完成的
                     input_ = [i[flag] for i in input_]  # 扔掉已完成序列
                     output_id = output_id[flag]  # 扔掉已完成序列
                     output_score = output_score[flag]  # 扔掉已完成序列
                     end_counts = end_counts[flag]  # 扔掉已完成end计数
@@ -222,127 +252,129 @@
                 output_ids_new.append(output_id)
                 output_scores_new.append(output_score)
                 flag_new.append(flag)
 
             inputs = [torch.cat(i) for i in zip(*inputs_new)]
             output_ids = torch.cat(output_ids_new)
             output_scores = torch.cat(output_scores_new)
-            topks = topks_new
+            self.topk = topks_new
             self.flag = torch.cat(flag_new)
 
             if len(output_ids) == 0:
                 break_tag = True
         else:
             # 不满足结束条件，需要对self.flag进行更新
             self.flag = torch.ones_like(self.flag, dtype=torch.bool)
         
-        return inputs, output_ids, output_scores, topks, results, break_tag
+        return inputs, output_ids, output_scores, results, break_tag
 
-    def beam_search(self, inputs, topk, states=None, temperature=1, min_ends=1):
+    def beam_search(self, inputs, states=None, **generation_config):
         """beam search解码
         
         :param inputs: 编码器的输入，包含encoder_hidden_states, encoder_attention_mask
         :param topk: int, 这里的topk即beam size
         :param states:
         :param temperature: 温度参数，默认为1
         :param min_ends:
         :return: 最优解码序列。
         """
-        assert topk is not None, 'Arg `topk` means beam_size anc can not be None'
+        self.set_generation_config(generation_config)
+        assert self.topk is not None, 'Arg `topk` means beam_size anc can not be None'
         inputs = self._prepare_raw_inputs(inputs)
         btz = inputs[0].shape[0]
         output_ids = self.first_output_ids.repeat(btz, 1)
         output_scores = torch.zeros(btz, device=self.device)
         results = []
 
         # batch推理
         if self.use_batch:
-            topk = [topk] * btz
+            self.topk = [self.topk] * btz
             results = [None] * btz
 
         for step in range(self.maxlen):
             if (not self.use_batch):  # 单条推理
-                inputs, output_ids, output_scores, states = self.__beam_search_step(step, inputs, output_ids, output_scores, topk, states, temperature)
-                inputs, output_ids, output_scores, topk, results, break_tag = self.__beam_search_end(inputs, output_ids, output_scores, topk, results, min_ends)
+                inputs, output_ids, output_scores, states = self.__beam_search_step(step, inputs, output_ids, output_scores, states)
+                inputs, output_ids, output_scores, results, break_tag = self.__beam_search_end(inputs, output_ids, output_scores, results)
             else:  # batch推理
-                inputs, output_ids, output_scores, states = self.__batch_beam_search_step(step, inputs, output_ids, output_scores, topk, states, temperature)
-                inputs, output_ids, output_scores, topk, results, break_tag = self.__batch_beam_search_end(inputs, output_ids, output_scores, topk, results, min_ends)
+                inputs, output_ids, output_scores, states = self.__batch_beam_search_step(step, inputs, output_ids, output_scores, states)
+                inputs, output_ids, output_scores, results, break_tag = self.__batch_beam_search_end(inputs, output_ids, output_scores, results)
             if break_tag:
                 break 
         # 如果还有未完成序列，直接放入结果
         if len(output_ids) > 0:
             if not self.use_batch:
                 results.append(output_ids[output_scores.argmax()])
             elif self.use_batch:
                 for smp_i, result in enumerate(results):
                     if result is None:
-                        start, end = sum(topk[:smp_i]), sum(topk[:smp_i+1])
+                        start, end = sum(self.topk[:smp_i]), sum(self.topk[:smp_i+1])
                         output_score = output_scores[start:end]
                         output_id = output_ids[start:end]
                         results[smp_i] = output_id[output_score.argmax()]
 
         # 达到长度直接输出
         self.flag = None
         return results
 
-    def stream_beam_search(self, inputs, topk, states=None, temperature=1, min_ends=1):
+    def stream_beam_search(self, inputs, states=None, **generation_config):
         '''beam_search的stream输出模式'''
-        assert topk is not None, 'Arg `topk` means beam_size anc can not be None'
+        self.set_generation_config(generation_config)
+        assert self.topk is not None, 'Arg `topk` means beam_size anc can not be None'
         inputs = self._prepare_raw_inputs(inputs)
         btz = inputs[0].shape[0]
         output_ids = self.first_output_ids.repeat(btz, 1)
         output_scores = torch.zeros(btz, device=self.device)
         results = []
         for step in range(self.maxlen):
-            inputs, output_ids, output_scores, states = self.__beam_search_step(step, inputs, output_ids, output_scores, topk, states, temperature)
+            inputs, output_ids, output_scores, states = self.__beam_search_step(step, inputs, output_ids, output_scores, states)
             yield [output_ids[output_scores.argmax()]]
-            inputs, output_ids, output_scores, topk, results, break_tag = self.__beam_search_end(inputs, output_ids, output_scores, topk, results, min_ends)
+            inputs, output_ids, output_scores, results, break_tag = self.__beam_search_end(inputs, output_ids, output_scores, results)
             if break_tag:
                 break 
             
         # 达到长度直接输出
         self.flag = None
 
-    def __random_sample_step(self, step, n, inputs, output_ids, states, temperature, topk, topp):
+    def __random_sample_step(self, step, inputs, output_ids, states):
         '''为了random_sample和stream_random_sample共用，抽离出来的单步逻辑'''
         self.step = step
-        probas, states = self.predict(inputs, output_ids, states, temperature, 'probas')  # 计算当前概率
+        probas, states = self.predict(inputs, output_ids, states, 'probas')  # 计算当前概率
         probas /= probas.sum(dim=-1, keepdims=True)  # 确保归一化
         if step == 0:  # 第1步预测后将结果重复n次
-            probas = probas.repeat([n]+[1]*(len(probas.shape)-1))
-            inputs = [i.repeat([n]+[1]*(len(i.shape)-1)) for i in inputs]
-            output_ids = output_ids.repeat([n]+[1]*(len(output_ids.shape)-1))
-        if topk is not None:
-            k_indices = probas.argsort(dim=-1, descending=True)[:, :topk]  # 仅保留topk
+            probas = probas.repeat([self.n]+[1]*(len(probas.shape)-1))
+            inputs = [i.repeat([self.n]+[1]*(len(i.shape)-1)) for i in inputs]
+            output_ids = output_ids.repeat([self.n]+[1]*(len(output_ids.shape)-1))
+        if self.topk is not None:
+            k_indices = probas.argsort(dim=-1, descending=True)[:, :self.topk]  # 仅保留topk
             probas = take_along_dim(probas, k_indices, dim=1)  # topk概率
             probas /= probas.sum(dim=1, keepdims=True)  # 重新归一化
-        if topp is not None:
+        if self.topp is not None:
             p_indices = probas.argsort(dim=-1, descending=True)  # 从高到低排序
             probas = take_along_dim(probas, p_indices, dim=-1)  # 排序概率
             cumsum_probas = torch.cumsum(probas, dim=-1)  # 累积概率
-            flag = torch.roll(cumsum_probas >= topp, 1, dims=1)  # 标记超过topp的部分
+            flag = torch.roll(cumsum_probas >= self.topp, 1, dims=1)  # 标记超过topp的部分
             flag[:, 0] = False  # 结合上面的torch.roll，实现平移一位的效果
             probas[flag] = 0  # 后面的全部置零
             probas /= probas.sum(dim=1, keepdims=True)  # 重新归一化
 
         sample_func = lambda p: torch.multinomial(p, 1)  # 按概率采样函数
         sample_ids = torch.stack([sample_func(p) for p in probas])
         sample_ids = sample_ids.reshape((-1, 1))  # 对齐形状
-        if topp is not None:
+        if self.topp is not None:
             sample_ids = take_along_dim(p_indices, sample_ids, dim=1)  # 对齐原id
-        if topk is not None:
+        if self.topk is not None:
             sample_ids = take_along_dim(k_indices, sample_ids, dim=1)  # 对齐原id
         output_ids = torch.cat([output_ids, sample_ids], 1)  # 更新输出
         return inputs, output_ids, states
 
-    def __random_sample_end(self, inputs, output_ids, results, min_ends, smp_indexs=None):
+    def __random_sample_end(self, inputs, output_ids, results, smp_indexs=None):
         break_tag = False
         is_end = output_ids[:, -1] == self.end_id  # 标记是否以end标记结束
         end_counts = (output_ids == self.end_id).sum(1)  # 统计出现的end标记
-        f_flag = is_end & (end_counts >= min_ends)  # 标记已完成序列
+        f_flag = is_end & (end_counts >= self.min_ends)  # 标记已完成序列
         self.flag = (f_flag == False)  # 记录未完成序列，这里是裁前的，用于use_states时候的裁剪操作
         if (output_ids.shape[1] >= self.minlen) and f_flag.any():  # 最短长度判断, 如果有已完成的
             if smp_indexs is None:  # single
                 for ids in output_ids[f_flag]:  # 存好已完成序列
                     results.append(ids)
             else:  # batch
                 for smp_i, ids in zip(smp_indexs[f_flag], output_ids[f_flag]):  # 存好已完成序列
@@ -361,43 +393,44 @@
             self.flag = torch.ones_like(self.flag, dtype=torch.bool)
 
         if smp_indexs is None:
             return inputs, output_ids, results, break_tag
         else:
             return inputs, output_ids, results, break_tag, smp_indexs
 
-    def random_sample(self, inputs_raw, n, topk=50, topp=1, states=None, temperature=1, min_ends=1):
+    def random_sample(self, inputs_raw, states=None, **generation_config):
         """随机采样n个结果；
         说明: 非None的topk表示每一步只从概率最高的topk个中采样；而非None的topp表示每一步只从概率最高的且概率之和刚好达到topp的若干个token中采样。
         
         :param inputs_raw: tensor、array、list、tuple, 解码的输入，一般为last_hidden_state, shape=[btz, seq_len, hdsz]
         :param topk: int, 这里的topk是指仅保留topk的值
         :param topp: float, 这里的topp是token的概率阈值设置
         :param states: None/dict, 缓存参数
         :param temperature: 温度参数，默认为1
         :param min_ends: 最小的end_id的个数
         :return: n个解码序列组成的list。
         """
+        self.set_generation_config(generation_config)
         inputs = self._prepare_raw_inputs(inputs_raw)  # 对输入进行处理
         output_ids = self.first_output_ids
         btz = inputs[0].shape[0]
         output_ids = self.first_output_ids.repeat(btz, 1)
         results = []
 
         if self.use_batch:
             smp_indexs = torch.tensor(range(btz)).to(output_ids)
             results = [None] * btz
 
         for step in range(self.maxlen):
             if not self.use_batch:  # single
-                inputs, output_ids, states = self.__random_sample_step(step, n, inputs, output_ids, states, temperature, topk, topp)
-                inputs, output_ids, results, break_tag = self.__random_sample_end(inputs, output_ids, results, min_ends)
+                inputs, output_ids, states = self.__random_sample_step(step, inputs, output_ids, states)
+                inputs, output_ids, results, break_tag = self.__random_sample_end(inputs, output_ids, results)
             else:  # batch
-                inputs, output_ids, states = self.__random_sample_step(step, n, inputs, output_ids, states, temperature, topk, topp)
-                inputs, output_ids, results, break_tag, smp_indexs = self.__random_sample_end(inputs, output_ids, results, min_ends, smp_indexs)
+                inputs, output_ids, states = self.__random_sample_step(step, inputs, output_ids, states)
+                inputs, output_ids, results, break_tag, smp_indexs = self.__random_sample_end(inputs, output_ids, results, smp_indexs)
             if break_tag:
                 break
 
         # 如果还有未完成序列，直接放入结果
         if len(output_ids) > 0:
             if not self.use_batch:
                 for ids in output_ids:
@@ -405,57 +438,78 @@
             elif self.use_batch:
                 for smp_i, ids in zip(smp_indexs, output_ids):  # 存好已完成序列
                     results[smp_i] = ids
         # 返回结果
         self.flag = None
         return results
     
-    def stream_random_sample(self, inputs_raw, topk=50, topp=1, states=None, temperature=1, min_ends=1):
+    def stream_random_sample(self, inputs_raw, states=None, **generation_config):
         """随机采样n个结果；stream输出"""
+        generation_config['n'] = 1
+        self.set_generation_config(generation_config)
         inputs = self._prepare_raw_inputs(inputs_raw)  # 对输入进行处理
         output_ids = self.first_output_ids
         results = []
         for step in range(self.maxlen):
-            inputs, output_ids, states = self.__random_sample_step(step, 1, inputs, output_ids, states, temperature, topk, topp)
+            inputs, output_ids, states = self.__random_sample_step(step, inputs, output_ids, states)
             yield output_ids
-            inputs, output_ids, results, break_tag = self.__random_sample_end(inputs, output_ids, results, min_ends)
+            inputs, output_ids, results, break_tag = self.__random_sample_end(inputs, output_ids, results)
             if break_tag:
                 break
         self.flag = None
 
 
 class SeqGeneration(AutoRegressiveDecoder):
     '''单向decoder语言模型的解码，对AutoRegressiveDecoder的简单封装，可以使用cache来加快解码
     '''
-    def __init__(self, model, tokenizer, start_id, end_id, maxlen, minlen=1, pad_id=None, pad_mode='post', mode='random_sample', default_rtype='logits', use_states=True, device=None):
+    def __init__(self, model, tokenizer, start_id, end_id, maxlen, minlen=1, pad_id=None, tokenizer_config=None, pad_mode='post', mode='random_sample', default_rtype='logits', 
+                 use_states=True, device=None, n=1, topk=50, topp=1, temperature=1, repetition_penalty=1.0, min_ends=1):
         '''
         :param model: 模型
         :param tokenizer: tokenizer，如果使用第三方的tokenize，需要继承重写下pre_process和post_process
         :param start_id: int, decoder初始的token_id
         :param end_id: int, 结束解码的token_id
         :param pad_id: int, pad_id，在batch解码时候使用
         :param pad_mode: str, padding在前面还是后面，pre或者post
+        :param tokenizer_config: dict, tokenize的参数
         :param maxlen: int, 最大解码长度
         :param minlen: int, 最小解码长度
         :param default_rtype: str, 模型输出的结果是logits设置为logits，如果是probas设置为probas
         :param use_states: str, 是否使用cache
         :param device: str, 默认为None，因为可以直接使用传入的model.device
         '''
-        
-        pad_id = pad_id or tokenizer.pad_token_id
-        super().__init__(start_id, end_id, maxlen, minlen, pad_id, pad_mode, device or next(model.parameters()).device)
+        if pad_id is not None:  # 用户自行设置了
+            pass
+        elif tokenizer.pad_token_id is not None:
+            pad_id = tokenizer.pad_token_id
+        else:
+            pad_id = 0
+            log_info(f'Arg `pad_id` has been set to default value 0')
+
+        super().__init__(start_id, end_id, maxlen, minlen, pad_id, pad_mode, device or next(model.parameters()).device, 
+                         n, topk, topp, temperature, repetition_penalty, min_ends)
         self.encoder = None
         self.decoder = model
+
+        # tokenizer参数
         self.tokenizer = tokenizer
+        self.tokenizer_type = 'b4t' if isinstance(tokenizer, TokenizerBase) else 'hf'
+        tokenizer_config = tokenizer_config or dict()
+        tokenizer_config.update({'maxlen': maxlen})
+        self.encode_config = self.clear_tokenizer_config(tokenizer_config, self.tokenizer.encode)
+        self.decode_config = self.clear_tokenizer_config(tokenizer_config, self.tokenizer.decode)
+
         assert mode in {'random_sample', 'beam_search'}, 'Args `mode` only support `random_sample/beam_search`.'
         self.mode = mode
         self.predict.set_default_rtype(default_rtype)  # 动态修改闭包中的default_rtype
         self.predict.set_use_states(use_states)  # 动态修改闭包中的use_states
         self.use_states = use_states
         self.use_segment_ids = hasattr(model, 'segment_vocab_size') and (model.segment_vocab_size > 0)  # 是否使用segment_ids
+        self.include_input = False  # 输出是否包含输入
+        self.input_text = ''
     
     def _prepare_next_inputs(self, inputs, output_ids, include_past=True):
         '''decode时候准备下一次输入，使用cache则仅输入last_token_ids，不适用需要输入past_token_ids'''
         def concat_token_ids(token_ids, output_ids):
             '''把非padding部分concat在一起
             '''
             if not self.use_batch:
@@ -572,66 +626,86 @@
                 position_ids = create_position_ids_start_at_padding(next_inputs[0], self.pad_id, past_key_values_length=-1, start_padding_idx=False)
                 logits = self.decoder.predict(next_inputs, position_ids=position_ids)
             else:
                 logits = self.decoder.predict(next_inputs)
             logits = logits[-1] if isinstance(logits, (tuple,list)) else logits  # 兼顾seq2seq
             return self.__get_last_token_logits(logits, output_ids)
 
+    @staticmethod
+    def clear_tokenizer_config(config, func):
+        '''获取在tokenize_params中的参数'''
+        arg_names = [k for k in inspect.signature(func).parameters]
+        return {k:v for k, v in config.items() if k in arg_names}
+
     def pre_process(self, text):
         '''前处理，可以继承后自定义，主要用于第三方tokenizer的encode'''
-        inputs = self.tokenizer.encode(text, maxlen=self.maxlen)
-        return inputs if self.use_segment_ids else [inputs[0]]
+        self.input_text = text if self.include_input else ''
+        if self.tokenizer_type == 'b4t':
+            # bert4torch的tokenizer
+            inputs = self.tokenizer.encode(text, **self.encode_config)
+            return inputs if self.use_segment_ids else [inputs[0]]
+        else:
+            # hf的tokenize
+            return [self.tokenizer(text, **self.encode_config)['input_ids']]
     
     def post_process(self, output_ids):
         '''后处理，可以继承后自定义，主要用于第三方tokenizer的decode'''
         if len(output_ids) > 1:
-            return [self.tokenizer.decode(ids.cpu().numpy()) for ids in output_ids]
+            outputs = [self.tokenizer.decode(ids.cpu().numpy(), **self.decode_config) for ids in output_ids]
+            if isinstance(self.input_text, str):
+                # 输入是str，则在前面直接添加
+                return [self.input_text + item for item in outputs]
+            elif isinstance(self.input_text, (tuple, list)) and (len(self.input_text) == len(outputs)):
+                # 输入是list且和outputs同维度
+                return [self.input_text[i] + item for i, item in enumerate(outputs)]
+            return outputs
         elif len(output_ids) == 1:
-            return self.tokenizer.decode(output_ids[0].cpu().numpy())
+            return self.input_text + self.tokenizer.decode(output_ids[0].cpu().numpy(), **self.decode_config)
         return output_ids
 
-    def _generate(self, inputs, n, topk, topp, temperature, min_ends):
+    def _generate(self, inputs):
         if self.mode == 'random_sample':
-            output_ids = self.random_sample(inputs, n, topk=topk, topp=topp, temperature=temperature, min_ends=min_ends)  # 基于随机采样
+            output_ids = self.random_sample(inputs)  # 基于随机采样
         elif self.mode == 'beam_search':
-            output_ids = self.beam_search(inputs, topk=topk, temperature=temperature, min_ends=min_ends)  # 基于beam search
+            output_ids = self.beam_search(inputs)  # 基于beam search
         return output_ids
 
-    def generate(self, text, n=1, topk=50, topp=1, temperature=1, min_ends=1):
+    def generate(self, text:str, **generation_config):
         '''单条样本生成'''
-        assert isinstance(text, str), 'Arg `text` must be str format'
+        self.set_generation_config(generation_config)
         self.use_batch = False
         inputs = self.pre_process(text)
-        output_ids = self._generate(inputs, n, topk, topp, temperature, min_ends)
+        output_ids = self._generate(inputs)
         return self.post_process(output_ids)
 
-    def batch_generate(self, text_list, topk=50, topp=1, temperature=1, min_ends=1):
+    def batch_generate(self, text_list:list, **generation_config):
         '''batch样本生成，use_states=True时要求pad_mode='pre', use_states=False时候对'''
         # 参数设定
-        assert isinstance(text_list, (list,tuple)), 'Arg `text_list` must be list/tuple format'
+        generation_config['n'] = 1
+        self.set_generation_config(generation_config)
         self.use_batch = True
         if self.use_states and (self.pad_mode in {'post', 'right'}):
             self.pad_mode = 'pre'
-            print(colorful("[WARNING]") + "When arg `use_states`=True, you may set `pad_mode`='pre' to avoid error output, reset `pad_mode`='pre' instead")
+            log_info("When arg `use_states`=True, you may set `pad_mode`='pre' to avoid error output, reset `pad_mode`='pre' instead")
 
         # 主流程
         inputs = self.pre_process(text_list)
-        output_ids = self._generate(inputs, 1, topk, topp, temperature, min_ends)
+        output_ids = self._generate(inputs)
         return self.post_process(output_ids)
 
-    def stream_generate(self, text:str, topk=50, topp=1, temperature=1, min_ends=1):
+    def stream_generate(self, text:str, **generation_config):
         '''单条样本stream输出预测的结果'''
-        assert isinstance(text, str), 'Arg `text` must be str format'
+        self.set_generation_config(generation_config)
         self.use_batch = False
         inputs = self.pre_process(text)
         if self.mode == 'random_sample':
-            for output_ids in  self.stream_random_sample(inputs, topk=topk, topp=topp, temperature=temperature, min_ends=min_ends):  # stream随机采样
+            for output_ids in  self.stream_random_sample(inputs):  # stream随机采样
                 yield self.post_process(output_ids)
         elif self.mode == 'beam_search':
-            for output_ids in  self.stream_beam_search(inputs, topk=topk, temperature=temperature, min_ends=min_ends):  # stream随机采样
+            for output_ids in  self.stream_beam_search(inputs):  # stream随机采样
                 yield self.post_process(output_ids)
 
 
 class Seq2SeqGeneration(SeqGeneration):
     '''encoder-decoder语言模型的解码'''
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -645,40 +719,42 @@
             inputs = [decoder_inputs[:, -1:]] + encoder_outputs
         else:
             inputs = [decoder_inputs] + encoder_outputs
         # inputs中包含了[decoder_ids, encoder_hidden_state, encoder_attention_mask]
         self.input_seqlen = torch.zeros(decoder_inputs.shape[0], dtype=torch.long).to(self.device)
         return inputs
             
-    def generate(self, text, n=1, topk=50, topp=1, temperature=1, min_ends=1):
-        assert isinstance(text, str), 'Arg `text` must be str format'
+    def generate(self, text:str, **generation_config):
+        self.set_generation_config(generation_config)
         self.use_batch = False
         inputs = self.pre_process(text)
         inputs = self._prepare_raw_inputs(inputs)  # 有时候需要list转tensor
         encoder_output = self.encoder.predict(inputs)
-        output_ids = super()._generate(encoder_output, n, topk, topp, temperature, min_ends)
+        output_ids = super()._generate(encoder_output)
         return self.post_process(output_ids)
 
-    def batch_generate(self, text_list, topk=50, topp=1, temperature=1, min_ends=1):
+    def batch_generate(self, text_list:list, **generation_config):
         '''batch样本生成'''
         # 参数设定
-        assert isinstance(text_list, (list,tuple)), 'Arg `text_list` must be list/tuple format'
+        generation_config['n'] = 1
+        self.set_generation_config(generation_config)
         self.use_batch = True
         inputs = self.pre_process(text_list)
         inputs = self._prepare_raw_inputs(inputs)  # 有时候需要list转tensor
         encoder_output = self.encoder.predict(inputs)
-        output_ids = super()._generate(encoder_output, 1, topk, topp, temperature, min_ends)
+        output_ids = super()._generate(encoder_output)
         return self.post_process(output_ids)
 
-    def stream_generate(self, text, topk=50, topp=1, temperature=1, min_ends=1):
+    def stream_generate(self, text:str, **generation_config):
         '''stream输出t预测的结果'''
-        assert isinstance(text, str), 'Arg `text` must be str format'
+        self.set_generation_config(generation_config)
+
         self.use_batch = False
         inputs = self.pre_process(text)
         inputs = self._prepare_raw_inputs(inputs)  # 有时候需要list转tensor
         encoder_output = self.encoder.predict(inputs)
         if self.mode == 'random_sample':
-            for output_ids in  self.stream_random_sample(encoder_output, topk=topk, topp=topp, temperature=temperature, min_ends=min_ends):  # stream随机采样
+            for output_ids in  self.stream_random_sample(encoder_output):  # stream随机采样
                 yield self.post_process(output_ids)
         elif self.mode == 'beam_search':
-            for output_ids in  self.stream_beam_search(encoder_output, topk=topk, temperature=temperature, min_ends=min_ends):  # stream随机采样
+            for output_ids in  self.stream_beam_search(encoder_output):  # stream随机采样
                 yield self.post_process(output_ids)
```

### Comparing `bert4torch-0.2.9/bert4torch/losses.py` & `bert4torch-0.3.0/bert4torch/losses.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.9/bert4torch/optimizers.py` & `bert4torch-0.3.0/bert4torch/optimizers.py`

 * *Files identical despite different names*

### Comparing `bert4torch-0.2.9/bert4torch/quantization.py` & `bert4torch-0.3.0/bert4torch/quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import base64
 import ctypes
 from typing import List
 import re
 from tqdm import tqdm
 from functools import partial
 import inspect
-from bert4torch.snippets import info_level_prefix
+from bert4torch.snippets import log_error
 
 try:
     from cpm_kernels.kernels.base import LazyKernelCModule, KernelFunction, round_up
 
     class Kernel:
         def __init__(self, code: bytes, function_names: List[str]):
             self.code = code
@@ -36,15 +36,15 @@
             "int4WeightExtractionHalf",
             "int8WeightExtractionFloat",
             "int8WeightExtractionHalf",
         ],
     )
 except Exception as exception:
     kernels = None
-    print(info_level_prefix("Failed to load cpm_kernels:" + str(exception)), 'e')
+    log_error("Failed to load cpm_kernels:" + str(exception))
 
 
 class W8A16Linear(torch.autograd.Function):
     @staticmethod
     def forward(ctx, inp: torch.Tensor, quant_w: torch.Tensor, scale_w: torch.Tensor, weight_bit_width):
         ctx.inp_shape = inp.size()
         ctx.weight_bit_width = weight_bit_width
```

### Comparing `bert4torch-0.2.9/bert4torch/snippets.py` & `bert4torch-0.3.0/bert4torch/snippets.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,20 +8,15 @@
 import torch
 from torch.nn.utils.rnn import pad_sequence
 import math
 import gc
 import json
 import random
 from torch4keras.snippets import *
-try:
-    # torch4keras0.0.7增加了callbacks，这里为了兼容老的example，在snippets中import了
-    # 建议使用方式: from bert4torch.callbacks import *
-    from torch4keras.callbacks import *
-except:
-    pass
+from torch4keras.callbacks import *
 
 is_py2 = six.PY2
 
 if not is_py2:
     basestring = str
 
 
@@ -265,39 +260,14 @@
             return func(self, *args, **kwargs)
 
         return new_func
 
     return actual_decorator
 
 
-def get_sinusoid_encoding_table(n_position, d_hid, padding_idx=None):
-    ''' sinusoid编码
-        
-        :param n_position: int, 位置长度
-        :param d_hid: int, 位置编码长度
-        :param padding_idx: padding的token_ids
-        :return: [seq_len, d_hid]
-    '''
-    position = torch.arange(0, n_position, dtype=torch.float).unsqueeze(1)
-    div_term = torch.exp(torch.arange(0, d_hid, 2).float() * (-math.log(10000.0) / d_hid))
-    embeddings_table = torch.zeros(n_position, d_hid)
-    embeddings_table[:, 0::2] = torch.sin(position * div_term)
-    embeddings_table[:, 1::2] = torch.cos(position * div_term)
-    return embeddings_table
-
-    # 第二种实现
-    position_ids = torch.arange(0, n_position).unsqueeze(1)
-    position_ids = position_ids.expand(-1, d_hid)
-    indices = torch.arange(0, d_hid)
-    position_ids = position_ids * torch.pow(10000, -2 * torch.true_divide(torch.floor_divide(indices, 2), d_hid))
-    position_ids[:, ::2] = torch.sin(position_ids[:, ::2])
-    position_ids[:, 1::2] = torch.cos(position_ids[:, 1::2])
-    return position_ids
-
-
 def cal_ts_num(tensor_shape):
     '''查看某个tensor在gc中的数量'''
     cal_num = 0
     for obj in gc.get_objects():
         try:
             if torch.is_tensor(obj): # or (hasattr(obj, 'data') and torch.is_tensor(obj.data)):
                 tensor = obj
@@ -506,7 +476,88 @@
 
 def create_position_ids_start_at_padding(input_ids, padding_idx, past_key_values_length=0, start_padding_idx=True):
     """生成padding_ids, 从padding_idx+1开始。忽略填充符号"""
     # The series of casts and type-conversions here are carefully balanced to both work with ONNX export and XLA.
     mask = input_ids.ne(padding_idx).int()
     incremental_indices = (torch.cumsum(mask, dim=1).type_as(mask) + past_key_values_length) * mask    
     return incremental_indices.long() + (padding_idx if start_padding_idx else 0)
+
+
+def set_module_tensor_to_device(module: nn.Module, tensor_name: str, device: Union[int, str, torch.device], value: Optional[torch.Tensor]=None):
+    """
+    A helper function to set a given tensor (parameter of buffer) of a module on a specific device (note that doing
+    `param.to(device)` creates a new tensor not linked to the parameter, which is why we need this function).
+
+    Args:
+        module (`torch.nn.Module`): The module in which the tensor we want to move lives.
+        param_name (`str`): The full name of the parameter/buffer.
+        device (`int`, `str` or `torch.device`): The device on which to set the tensor.
+        value (`torch.Tensor`, *optional*): The value of the tensor (useful when going from the meta device to any
+            other device).
+    """
+    # Recurse if needed
+    if "." in tensor_name:
+        splits = tensor_name.split(".")
+        for split in splits[:-1]:
+            new_module = getattr(module, split)
+            if new_module is None:
+                raise ValueError(f"{module} has no attribute {split}.")
+            module = new_module
+        tensor_name = splits[-1]
+
+    if tensor_name not in module._parameters and tensor_name not in module._buffers:
+        raise ValueError(f"{module} does not have a parameter or a buffer named {tensor_name}.")
+    is_buffer = tensor_name in module._buffers
+    old_value = getattr(module, tensor_name)
+
+    if old_value.device == torch.device("meta") and device not in ["meta", torch.device("meta")] and value is None:
+        raise ValueError(f"{tensor_name} is on the meta device, we need a `value` to put in on {device}.")
+
+    with torch.no_grad():
+        if value is None:
+            new_value = old_value.to(device)
+        elif isinstance(value, torch.Tensor):
+            new_value = value.to(device)
+        else:
+            new_value = torch.tensor(value, device=device)
+
+        if is_buffer:
+            module._buffers[tensor_name] = new_value
+        elif value is not None or torch.device(device) != module._parameters[tensor_name].device:
+            param_cls = type(module._parameters[tensor_name])
+            kwargs = module._parameters[tensor_name].__dict__
+            new_value = param_cls(new_value, requires_grad=old_value.requires_grad, **kwargs).to(device)
+            module._parameters[tensor_name] = new_value
+
+
+def load_state_dict_into_meta_model(model: nn.Module, state_dict):
+    '''将device='meta'的参数用预训练权重赋值'''
+    for param_name, param in model.named_parameters():
+        # 权重文件中有
+        if param_name in state_dict.keys():
+            set_module_tensor_to_device(model, param_name, 'cpu', state_dict[param_name])
+        # 权重文件中没有
+        elif param.device == torch.device('meta'):
+            # 这里采用全0初始化
+            value = torch.zeros(*param.size(), dtype=param.dtype)
+            set_module_tensor_to_device(model, param_name, 'cpu', value)
+
+
+def set_default_torch_dtype(dtype: torch.dtype, model_name='model') -> torch.dtype:
+    """设置默认权重类型"""
+    if not isinstance(model_name, str):
+        model_name = 'model'
+    mapping = {
+        'float16': torch.float16,
+        'float32': torch.float32,
+        'float64': torch.float64,
+        'bfloat16': torch.bfloat16
+        }
+    if isinstance(dtype, str):
+        dtype = mapping[dtype]
+
+    if not dtype.is_floating_point:
+        raise ValueError(f"Can't instantiate {model_name} under dtype={dtype} since it is not a floating point dtype")
+    log_info(f"Instantiating {model_name} under default dtype {dtype}.")
+    dtype_orig = torch.get_default_dtype()
+    torch.set_default_dtype(dtype)
+    return dtype_orig
```

### Comparing `bert4torch-0.2.9/bert4torch/tokenizers.py` & `bert4torch-0.3.0/bert4torch/tokenizers.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 """Tokenization classes."""
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import collections
 import logging
+from typing import Any
 import unicodedata
 from io import open
 from bert4torch.snippets import truncate_sequences, is_string, lowercase_and_normalize
 import re
 import six
 from collections import OrderedDict
 
@@ -158,14 +159,17 @@
             offset = self.rematch(first_text, first_tokens) + self.rematch(second_text, second_tokens)
             if return_offsets == 'transformers':  # transformers包中tokenizer的形式
                 encode_output.append([[0, 0] if not k else [k[0], k[-1]+1] for k in offset])
             else:
                 encode_output.append(offset)
         return encode_output
 
+    def __call__(self, *args: Any, **kwds: Any) -> Any:
+        return self.encode(*args, **kwds)
+        
     def encode(self, first_texts, second_texts=None, maxlen=None, pattern='S*E*E', truncate_from='right', return_offsets=False):
         '''可以处理多条或者单条
         '''
         return_list = False if isinstance(first_texts, str) else True
         first_texts = [first_texts] if isinstance(first_texts, str) else first_texts
         second_texts = [second_texts] if isinstance(second_texts, str) else second_texts
```

### Comparing `bert4torch-0.2.9/bert4torch.egg-info/PKG-INFO` & `bert4torch-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: bert4torch
-Version: 0.2.9
-Summary: an elegant bert4torch
-Home-page: https://github.com/Tongjilibo/bert4torch
-Author: Tongjilibo
-License: MIT Licence
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![bert4torch](https://github.com/Tongjilibo/bert4torch/blob/master/docs/pics/bert4torch.png)
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/blob/master/LICENSE)
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/bert4torch.svg?maxAge=3600)](https://github.com/Tongjilibo/bert4torch/releases)
 [![PyPI](https://img.shields.io/pypi/v/bert4torch?label=pypi%20package)](https://pypi.org/project/bert4torch/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/bert4torch)](https://pypistats.org/packages/bert4torch)
 [![GitHub stars](https://img.shields.io/github/stars/Tongjilibo/bert4torch?style=social)](https://github.com/Tongjilibo/bert4torch)
@@ -74,14 +64,16 @@
 - [bert4torch介绍(知乎)](https://zhuanlan.zhihu.com/p/486329434)，[bert4torch快速上手(知乎)](https://zhuanlan.zhihu.com/p/508890807)，[bert4torch又双叒叕更新啦(知乎)](https://zhuanlan.zhihu.com/p/560885427?)
 
 ## 4. 版本历史
 
 <details><summary><b>点击查看</b></summary>
 
 **版本说明**
+- **v0.3.0**：20230716 修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
+- **v0.2.9**: 20230705 使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
 - **v0.2.8**：20230518 【新增模型】增加chatglm-6b/llama-7b/BELLE_llama/vicuna/moss/苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型/fnlp的bart2.0, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2和lora; 【generation】生成式解码新增SeqGeneration和Seq2SeqGeneration，单向decoder模型和encoder decoder模型解码增加cache, 增加batch_generate()/stream_generate功能；【其他】修改rope为不使用max_position，修复model.half()类型不一致问题，支持加载多个权重文件, gpt系列默认不加softmax，增加苏神Tiger的pytorch实现, 增加了对attention_key_size的入参支持，把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **v0.2.7.post2**：20230310 增加lion优化器, 修复albert_unshared加载权重, 修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **v0.2.7**：20230213 修复random_sample()的bug，适配v0.0.6的torch4keras：增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现，增加了AccelerateCallback
 - **v0.2.6**：20221231 build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert, macbert，text2vec-bert-chinese, wobert预训练模型，允许position_ids从padding开始, transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **v0.2.5**：20221127 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置
 - **v0.2.4**：20221120 删除SpTokenizer基类中的rematch, 增加deberta_v2模型
 - **v0.2.3**：20221023 虚拟对抗VAT在多个ouput时支持指定，把Trainer抽象到[torch4keras](https://github.com/Tongjilibo/torch4keras)中，修复DP和DDP出现resume_epoch不存在的bug, tokenizer的never_split去除None, transformer_xl的bug, 增加gradient_checkpoint
@@ -96,14 +88,15 @@
 - **v0.1.4**：20220421 增加了VAT，修复了linux下apply_embedding返回项有问题的情况
 - **v0.1.3**：20220409 初始版本
 
 **版本对应关系**
 
 | bert4torch版本 | torch4keras版本 |
 | ---------------- | ----------------- |
+| 0.3.0          | 0.0.9           |
 | 0.2.9          | 0.0.8           |
 | 0.2.8          | 0.0.7.post3     |
 | 0.2.7.post2    | 0.0.6           |
 | 0.2.7          | 0.0.6           |
 | 0.2.6          | 0.0.5           |
 | 0.2.5          | 0.0.4           |
 | 0.2.4          | 0.0.3.post2     |
@@ -112,16 +105,17 @@
 
 </details>
 
 
 ## 5. 更新历史：
 <details><summary><b>点击查看</b></summary>
 
-- **20230612**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
-- **20230426**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
+- **20230716**：修改models和layers为文件夹方便扩展, 增加flash_attention参数控制，增加chatglm-api示例，修改skip_init逻辑减少显存占用，generation增加repetition_penalty，修复chatglm的pv2的bug，generation支持transformers的tokenize，增加ziya，Baichuan
+- **20230705**：使用accelerate来实现skip_init精简代码, 修复add_trainer的代码提示, 增加chatglm的load_in_8bit+lora/qlora的训练, 修复grad_chechpoint, 增加chinese_llama_alpaca, torch2.0默认使用scaled_dot_product_attention加速, 增加chatglm2-6b+pv2+lora微调
+- **20230518**：增加vicuna的集成, 增加batch_generate()功能, 把_token_pad_ids重命名为pad_token_ids, tokenizor中重命名部分字段
 - **20230408**：增加苏神Tiger的pytorch实现, 集成苏神、uer的roberta-small/Tiny模型以及ChatYuan v2模型, 增加了对attention_key_size的入参支持，单向decoder模型和encoder decoder模型解码增加cache, 更新fnlp的bart2.0, 增加chatglm-6b预训练模型推理, 集成BELLE_llama模型, 增加量化模块并适配llama，增加skip_init参数加快加载, 增加stream输出/网页demo, 增加ptuning_v2，增加moss模型的int4/int8推理
 - **20230326**：增加llama-7b预训练模型, 修改rope为不使用max_position, 增加prompt_clue和nezha_gpt_dialog的finetune示例(skykiseki用户)，修复model.half()类型不一致问题，生成式解码新增SeqGeneration和Seq2SeqGeneration, 支持加载多个权重文件, gpt系列默认不加softmax
 - **20230310**：增加lion优化器, 修改dp和ddp示例更易用，增加PromptCLUE模型, 修复albert_unshared加载权重, 增加uer-gpt2-chinese预训练模型，修复lm系列(gpt, seq2seq)存在的forward参数不对的问题，修复GlobalPointer使用rope的bug
 - **20230212**：兼容accelerate包, 增加ChatYuan v1模型，修复random_sample()的bug
 - **20221230**：增加macbert，text2vec-bert-chinese, wobert模型，增加LEAR的ner示例, 增加PGRC、SPN4RE的关系提取示例，transformer.configs支持点操作，可以使用torch4keras的Trainer(net)来初始化, 修复tokenizer的切分subtoken的bug, 允许embedding_size!=hidden_size
 - **20221127**：增加deberta_v2模型, 对抗训练从compile转为使用Callback来实现，修复1.7.1版本兼容bug, uie模型内置, 增加triton示例, build_transformer_model需显式指定add_trainer才从BaseModel继承, 增加guwenbert预训练模型，允许position_ids从padding开始
 - **20221102**：增加CNN_Nested_NER示例, 删除SpTokenizer基类中的rematch
@@ -185,20 +179,22 @@
 | t5| UER | [torch](https://huggingface.co/uer/t5-base-chinese-cluecorpussmall)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | mt5 | 谷歌| [torch](https://huggingface.co/google/mt5-base)| [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | t5_pegasus| 追一科技| [tf](https://github.com/ZhuiyiTechnology/t5-pegasus) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_t5_pegasus.py)|
 | bart| 复旦| [torch](https://github.com/fastnlp/CPT), [v1.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v1.0), [v2.0](https://huggingface.co/fnlp/bart-base-chinese/tree/v2.0)| [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_bart_fudanNLP.py) |
 | text2vec| text2vec-base-chinese | [torch](https://huggingface.co/shibing624/text2vec-base-chinese) | |
 | chatyuan v1&v2| clue-ai | [torch](https://github.com/clue-ai/ChatYuan) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
 | PromptCLUE| clue-ai | [torch](https://github.com/clue-ai/PromptCLUE) | [config](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/PLM_config.md)|
-| llama | facebook| [torch](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
-|chinese_llama_alpaca|哈工大|[torch](https://github.com/ymcui/Chinese-LLaMA-Alpaca)|[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_facebook.py)|
-| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_vicuna.py)|
-| Belle| LianjiaTech| [torch](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_belle.py)|
-| chatglm-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
-| chatglm2-6b | THUDM | [torch](https://github.com/THUDM/ChatGLM2-6B) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm-6b | THUDM | [git](https://github.com/THUDM/ChatGLM-6B), [v0.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v0.1.0), [v1.1.0](https://huggingface.co/THUDM/chatglm-6b/tree/v1.1.0), [int8](https://huggingface.co/THUDM/chatglm-6b-int8), [int4](https://huggingface.co/THUDM/chatglm-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| chatglm2-6b | THUDM | [git](https://github.com/THUDM/ChatGLM2-6B), [v2](https://huggingface.co/THUDM/chatglm2-6b), [int4](https://huggingface.co/THUDM/chatglm2-6b-int4) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_chatglm.py) |
+| llama | facebook| [git](https://github.com/facebookresearch/llama) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+|chinese_llama_alpaca|Yiming Cui|[git](https://github.com/ymcui/Chinese-LLaMA-Alpaca) |[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py)|
+| vicuna | FastChat| [torch](https://huggingface.co/AlekseyKorshuk/vicuna-7b) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
+| Belle_llama| LianjiaTech| [git](https://github.com/LianjiaTech/BELLE), [7B-2M-enc](https://huggingface.co/BelleGroup/BELLE-LLaMA-7B-2M-enc) | [合成说明](https://github.com/LianjiaTech/BELLE/tree/main/models)、[转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py)|
+| Ziya | IDEA-CCNL | [v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1), [v1.1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-v1.1), [pretrain-v1](https://huggingface.co/IDEA-CCNL/Ziya-LLaMA-13B-Pretrain-v1) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_pth.py) |
+| Baichuan | baichuan-inc | [7B](https://github.com/baichuan-inc/Baichuan-7B), [13B-Base](https://huggingface.co/baichuan-inc/Baichuan-13B-Base), [13B-Chat](https://huggingface.co/baichuan-inc/Baichuan-13B-Chat) | [转换脚本](https://github.com/Tongjilibo/bert4torch/blob/master/examples/convert_script/convert_llama_hf.py) |
 
 ## 7. 鸣谢
 
 - 感谢苏神实现的[bert4keras](https://github.com/bojone/bert4keras)，本实现有不少地方参考了bert4keras的源码，在此衷心感谢大佬的无私奉献;
 - 其次感谢项目[bert4pytorch](https://github.com/MuQiuJun-AI/bert4pytorch)，也是在该项目的指引下给了我用pytorch来复现bert4keras的想法和思路。
 
 ## 8. 引用
@@ -238,8 +234,8 @@
     <tr align="center" >
       <td>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date"><img width="400" height="250" src="https://api.star-history.com/svg?repos=Tongjilibo/bert4torch&type=Date" alt="pic"></a><br>
          <a href="https://star-history.com/#Tongjilibo/bert4torch&Date">Star History Chart</a> 
       </td>
     </tr>
   </tbody>
-</table>
+</table>
```

### Comparing `bert4torch-0.2.9/setup.py` & `bert4torch-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='bert4torch',
-    version='v0.2.9',
+    version='v0.3.0',
     description='an elegant bert4torch',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT Licence',
     url='https://github.com/Tongjilibo/bert4torch',
     author='Tongjilibo',
-    install_requires=['torch>1.6', 'torch4keras==0.0.8'],
+    install_requires=['torch>1.6', 'torch4keras==0.0.9'],
     packages=find_packages()
 )
```

