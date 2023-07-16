# Comparing `tmp/auto_gptq-0.2.2.tar.gz` & `tmp/auto_gptq-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_gptq-0.2.2.tar", last modified: Thu Jun  8 06:07:58 2023, max compression
+gzip compressed data, was "auto_gptq-0.3.0.tar", last modified: Sun Jul 16 08:03:38 2023, max compression
```

## Comparing `auto_gptq-0.2.2.tar` & `auto_gptq-0.3.0.tar`

### file list

```diff
@@ -1,65 +1,72 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.366150 auto_gptq-0.2.2/
--rw-r--r--   0 root         (0) root         (0)     1075 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)    15808 2023-06-08 06:07:58.365151 auto_gptq-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14908 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.357151 auto_gptq-0.2.2/auto_gptq/
--rw-r--r--   0 root         (0) root         (0)       83 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.359151 auto_gptq-0.2.2/auto_gptq/eval_tasks/
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2194 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/_base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.360150 auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/classification_utils.py
--rw-r--r--   0 root         (0) root         (0)     1448 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/generation_utils.py
--rw-r--r--   0 root         (0) root         (0)     1215 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/language_modeling_task.py
--rw-r--r--   0 root         (0) root         (0)     3653 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/sequence_classification_task.py
--rw-r--r--   0 root         (0) root         (0)     2571 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/eval_tasks/text_summarization_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.362151 auto_gptq-0.2.2/auto_gptq/modeling/
--rw-r--r--   0 root         (0) root         (0)      292 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35910 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/modeling/_base.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/_const.py
--rw-r--r--   0 root         (0) root         (0)     6906 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/modeling/_utils.py
--rw-r--r--   0 root         (0) root         (0)     3868 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/modeling/auto.py
--rw-r--r--   0 root         (0) root         (0)      474 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/bloom.py
--rw-r--r--   0 root         (0) root         (0)      388 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/codegen.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/gpt2.py
--rw-r--r--   0 root         (0) root         (0)      453 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/gpt_bigcode.py
--rw-r--r--   0 root         (0) root         (0)      461 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/gpt_neox.py
--rw-r--r--   0 root         (0) root         (0)      550 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/gptj.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/llama.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/moss.py
--rw-r--r--   0 root         (0) root         (0)      562 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/opt.py
--rw-r--r--   0 root         (0) root         (0)      428 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/modeling/rw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.363150 auto_gptq-0.2.2/auto_gptq/nn_modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      852 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/_fused_base.py
--rw-r--r--   0 root         (0) root         (0)    10938 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/fused_gptj_attn.py
--rw-r--r--   0 root         (0) root         (0)     7384 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/fused_llama_attn.py
--rw-r--r--   0 root         (0) root         (0)    13313 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/fused_llama_mlp.py
--rw-r--r--   0 root         (0) root         (0)    10697 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear.py
--rw-r--r--   0 root         (0) root         (0)    10924 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear_old.py
--rw-r--r--   0 root         (0) root         (0)     5926 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear_triton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.364151 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/custom_autotune.py
--rw-r--r--   0 root         (0) root         (0)    13785 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/kernels.py
--rw-r--r--   0 root         (0) root         (0)      113 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.364151 auto_gptq-0.2.2/auto_gptq/quantization/
--rw-r--r--   0 root         (0) root         (0)       45 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/quantization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5835 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/quantization/gptq.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/quantization/quantizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.365151 auto_gptq-0.2.2/auto_gptq/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11122 2023-06-07 03:56:07.000000 auto_gptq-0.2.2/auto_gptq/utils/data_utils.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/auto_gptq/utils/import_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.358151 auto_gptq-0.2.2/auto_gptq.egg-info/
--rw-r--r--   0 root         (0) root         (0)    15808 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      141 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-08 06:07:58.000000 auto_gptq-0.2.2/auto_gptq.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 06:07:58.365151 auto_gptq-0.2.2/autogptq_cuda/
--rw-r--r--   0 root         (0) root         (0)     6455 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/autogptq_cuda/autogptq_cuda.cpp
--rw-r--r--   0 root         (0) root         (0)    39351 2023-06-08 04:51:05.000000 auto_gptq-0.2.2/autogptq_cuda/autogptq_cuda_kernel.cu
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 06:07:58.366150 auto_gptq-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3666 2023-06-08 06:07:48.000000 auto_gptq-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.628584 auto_gptq-0.3.0/
+-rw-rw-rw-   0        0        0     1096 2023-04-13 14:32:51.000000 auto_gptq-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0    16857 2023-07-16 08:03:38.628584 auto_gptq-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0    15955 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.566062 auto_gptq-0.3.0/auto_gptq/
+-rw-rw-rw-   0        0        0      136 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.581685 auto_gptq-0.3.0/auto_gptq/eval_tasks/
+-rw-rw-rw-   0        0        0      124 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/_base.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.581685 auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/__init__.py
+-rw-rw-rw-   0        0        0     1165 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/classification_utils.py
+-rw-rw-rw-   0        0        0     1486 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/generation_utils.py
+-rw-rw-rw-   0        0        0     1262 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/language_modeling_task.py
+-rw-rw-rw-   0        0        0     3760 2023-04-23 15:46:04.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/sequence_classification_task.py
+-rw-rw-rw-   0        0        0     2646 2023-04-24 12:51:09.000000 auto_gptq-0.3.0/auto_gptq/eval_tasks/text_summarization_task.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.581685 auto_gptq-0.3.0/auto_gptq/modeling/
+-rw-rw-rw-   0        0        0      354 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/auto_gptq/modeling/__init__.py
+-rw-rw-rw-   0        0        0    39011 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/_base.py
+-rw-rw-rw-   0        0        0      562 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/auto_gptq/modeling/_const.py
+-rw-rw-rw-   0        0        0     7387 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/_utils.py
+-rw-rw-rw-   0        0        0     4314 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/auto_gptq/modeling/auto.py
+-rw-rw-rw-   0        0        0      430 2023-06-19 02:37:40.000000 auto_gptq-0.3.0/auto_gptq/modeling/baichuan.py
+-rw-rw-rw-   0        0        0      490 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/bloom.py
+-rw-rw-rw-   0        0        0      404 2023-05-28 08:23:38.000000 auto_gptq-0.3.0/auto_gptq/modeling/codegen.py
+-rw-rw-rw-   0        0        0      409 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/gpt2.py
+-rw-rw-rw-   0        0        0      469 2023-05-28 08:23:38.000000 auto_gptq-0.3.0/auto_gptq/modeling/gpt_bigcode.py
+-rw-rw-rw-   0        0        0      478 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/modeling/gpt_neox.py
+-rw-rw-rw-   0        0        0      569 2023-05-14 08:23:32.000000 auto_gptq-0.3.0/auto_gptq/modeling/gptj.py
+-rw-rw-rw-   0        0        0      479 2023-07-16 06:23:10.000000 auto_gptq-0.3.0/auto_gptq/modeling/internlm.py
+-rw-rw-rw-   0        0        0     1042 2023-05-20 07:21:20.000000 auto_gptq-0.3.0/auto_gptq/modeling/llama.py
+-rw-rw-rw-   0        0        0      395 2023-04-29 02:36:14.000000 auto_gptq-0.3.0/auto_gptq/modeling/moss.py
+-rw-rw-rw-   0        0        0      581 2023-04-28 15:06:27.000000 auto_gptq-0.3.0/auto_gptq/modeling/opt.py
+-rw-rw-rw-   0        0        0      443 2023-05-28 08:23:38.000000 auto_gptq-0.3.0/auto_gptq/modeling/rw.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/nn_modules/
+-rw-rw-rw-   0        0        0        0 2023-04-26 13:22:55.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/__init__.py
+-rw-rw-rw-   0        0        0      981 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/_fused_base.py
+-rw-rw-rw-   0        0        0    11334 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/fused_gptj_attn.py
+-rw-rw-rw-   0        0        0     7678 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/fused_llama_attn.py
+-rw-rw-rw-   0        0        0    12200 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/fused_llama_mlp.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/
+-rw-rw-rw-   0        0        0     2111 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/__init__.py
+-rw-rw-rw-   0        0        0    11372 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_cuda.py
+-rw-rw-rw-   0        0        0    11762 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py
+-rw-rw-rw-   0        0        0     6533 2023-06-19 02:37:40.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_triton.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/
+-rw-rw-rw-   0        0        0        0 2023-05-20 09:01:53.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/__init__.py
+-rw-rw-rw-   0        0        0     7099 2023-04-26 13:22:55.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py
+-rw-rw-rw-   0        0        0    14285 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/kernels.py
+-rw-rw-rw-   0        0        0      117 2023-05-20 09:01:53.000000 auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/mixin.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/quantization/
+-rw-rw-rw-   0        0        0       47 2023-04-26 13:22:55.000000 auto_gptq-0.3.0/auto_gptq/quantization/__init__.py
+-rw-rw-rw-   0        0        0     6016 2023-05-14 05:13:14.000000 auto_gptq-0.3.0/auto_gptq/quantization/gptq.py
+-rw-rw-rw-   0        0        0     4408 2023-04-26 13:22:55.000000 auto_gptq-0.3.0/auto_gptq/quantization/quantizer.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.597309 auto_gptq-0.3.0/auto_gptq/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/utils/__init__.py
+-rw-rw-rw-   0        0        0    11389 2023-04-28 14:56:43.000000 auto_gptq-0.3.0/auto_gptq/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1241 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/utils/import_utils.py
+-rw-rw-rw-   0        0        0    18688 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/auto_gptq/utils/peft_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.566062 auto_gptq-0.3.0/auto_gptq.egg-info/
+-rw-rw-rw-   0        0        0    16857 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1987 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       45 2023-07-16 08:03:38.000000 auto_gptq-0.3.0/auto_gptq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 08:03:38.628584 auto_gptq-0.3.0/autogptq_cuda/
+-rw-rw-rw-   0        0        0     7212 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_256.cpp
+-rw-rw-rw-   0        0        0     7212 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_64.cpp
+-rw-rw-rw-   0        0        0    46659 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_kernel_256.cu
+-rw-rw-rw-   0        0        0    46655 2023-06-11 06:39:43.000000 auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_kernel_64.cu
+-rw-rw-rw-   0        0        0       42 2023-07-16 08:03:38.628584 auto_gptq-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     3856 2023-07-16 08:02:59.000000 auto_gptq-0.3.0/setup.py
```

### Comparing `auto_gptq-0.2.2/LICENSE` & `auto_gptq-0.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 潘其威(William)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 潘其威(William)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `auto_gptq-0.2.2/PKG-INFO` & `auto_gptq-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,352 +1,322 @@
-Metadata-Version: 2.1
-Name: auto_gptq
-Version: 0.2.2
-Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
-Home-page: https://github.com/PanQiWei/AutoGPTQ
-Author: PanQiWei
-Keywords: gptq,quantization,large-language-models,pytorch,transformers
-Platform: windows
-Platform: linux
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: C++
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: llama
-Provides-Extra: triton
-License-File: LICENSE
-
-<h1 align="center">AutoGPTQ</h1>
-<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
-<p align="center">
-    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
-    </a>
-    <a href="https://pypi.org/project/auto-gptq/">
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
-    </a>
-</p>
-<h4 align="center">
-    <p>
-        <b>English</b> |
-        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
-    <p>
-</h4>
-
-## News or Update
-
-**To experience adapter training using `auto_gptq` quantized model in advance, you can try [this branch](https://github.com/PanQiWei/AutoGPTQ/tree/peft_integration) and discuss [in here](https://github.com/PanQiWei/AutoGPTQ/issues/103), examples are [in here](https://github.com/PanQiWei/AutoGPTQ/tree/peft_integration/examples/peft).**
-
-- 2023-05-25 - (In Progress) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
-- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
-- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
-- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
-
-*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
-
-## Performance Comparison
-
-### Inference Speed
-> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
-> 
-> The quantized model is loaded using the setup that can gain the fastest inference speed.
-
-| model         | GPU           | num_beams | fp16  | gptq-int4 |
-|---------------|---------------|-----------|-------|-----------|
-| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
-| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
-| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
-| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
-| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
-| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
-| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
-| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
-
-
-### Perplexity
-For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
-
-## Installation
-
-### Quick Installation
-You can install the latest stable release of AutoGPTQ from pip:
-```shell
-pip install auto-gptq
-```
-Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
-```shell
-# firstly, cd the directory where the wheel saved, then execute command below
-pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
-```
-#### disable cuda extensions
-By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
-```shell
-BUILD_CUDA_EXT=0 pip install auto-gptq
-```
-And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
-```shell
-pip uninstall autogptq_cuda -y
-```
-#### to support LLaMa model
-For some people want to try LLaMa and whose `transformers` version not meet the newest one that supports it, using:
-```shell
-pip install auto-gptq[llama]
-```
-#### to support triton speedup
-To integrate with `triton`, using:
-> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
-
-```shell
-pip install auto-gptq[triton]
-```
-
-### Install from source
-<details>
-<summary>click to see details</summary>
-
-Clone the source code:
-```shell
-git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
-```
-Then, install from source:
-```shell
-pip install .
-```
-Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
-
-Use `.[llama]` if you want to try LLaMa model.
-
-Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
-
-</details>
-
-## Quick Tour
-
-### Quantization and Inference
-> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
-
-Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
-```python
-from transformers import AutoTokenizer, TextGenerationPipeline
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-import logging
-
-logging.basicConfig(
-    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
-)
-
-pretrained_model_dir = "facebook/opt-125m"
-quantized_model_dir = "opt-125m-4bit"
-
-tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
-examples = [
-    tokenizer(
-        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
-    )
-]
-
-quantize_config = BaseQuantizeConfig(
-    bits=4,  # quantize model to 4-bit
-    group_size=128,  # it is recommended to set the value to 128
-    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
-)
-
-# load un-quantized model, by default, the model will always be loaded into CPU memory
-model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
-
-# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
-model.quantize(examples)
-
-# save quantized model
-model.save_quantized(quantized_model_dir)
-
-# save quantized model using safetensors
-model.save_quantized(quantized_model_dir, use_safetensors=True)
-
-# push quantized model to Hugging Face Hub. 
-# to use use_auth_token=True, Login first via huggingface-cli login.
-# or pass explcit token with: use_auth_token="hf_xxxxxxx"
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
-
-# alternatively you can save and push at the same time
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
-
-# load quantized model to the first GPU
-model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
-
-# download quantized model from Hugging Face Hub and load to the first GPU
-# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
-
-# inference with model.generate
-print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
-
-# or you can also use pipeline
-pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
-print(pipeline("auto-gptq is")[0]["generated_text"])
-```
-
-For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
-
-### Customize Model
-<details>
-
-<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
-
-```python
-from auto_gptq.modeling import BaseGPTQForCausalLM
-
-
-class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
-    # chained attribute name of transformer layer block
-    layers_block_name = "model.decoder.layers"
-    # chained attribute names of other nn modules that in the same level as the transformer layer block
-    outside_layer_modules = [
-        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
-        "model.decoder.project_in", "model.decoder.final_layer_norm"
-    ]
-    # chained attribute names of linear layers in transformer layer module
-    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
-    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
-    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
-    inside_layer_modules = [
-        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
-        ["self_attn.out_proj"],
-        ["fc1"],
-        ["fc2"]
-    ]
-```
-After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
-
-</details>
-
-### Evaluation on Downstream Tasks
-You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
-
-The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
-
-<details>
-
-<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
-
-```python
-from functools import partial
-
-import datasets
-from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
-
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-from auto_gptq.eval_tasks import SequenceClassificationTask
-
-
-MODEL = "EleutherAI/gpt-j-6b"
-DATASET = "cardiffnlp/tweet_sentiment_multilingual"
-TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
-ID2LABEL = {
-    0: "negative",
-    1: "neutral",
-    2: "positive"
-}
-LABELS = list(ID2LABEL.values())
-
-
-def ds_refactor_fn(samples):
-    text_data = samples["text"]
-    label_data = samples["label"]
-
-    new_samples = {"prompt": [], "label": []}
-    for text, label in zip(text_data, label_data):
-        prompt = TEMPLATE.format(labels=LABELS, text=text)
-        new_samples["prompt"].append(prompt)
-        new_samples["label"].append(ID2LABEL[label])
-
-    return new_samples
-
-
-#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
-model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
-tokenizer = AutoTokenizer.from_pretrained(MODEL)
-
-task = SequenceClassificationTask(
-        model=model,
-        tokenizer=tokenizer,
-        classes=LABELS,
-        data_name_or_path=DATASET,
-        prompt_col_name="prompt",
-        label_col_name="label",
-        **{
-            "num_samples": 1000,  # how many samples will be sampled to evaluation
-            "sample_max_len": 1024,  # max tokens for each sample
-            "block_max_len": 2048,  # max tokens for each data block
-            # function to load dataset, one must only accept data_name_or_path as input 
-            # and return datasets.Dataset
-            "load_fn": partial(datasets.load_dataset, name="english"),  
-            # function to preprocess dataset, which is used for datasets.Dataset.map, 
-            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
-            "preprocess_fn": ds_refactor_fn,  
-            # truncate label when sample's length exceed sample_max_len
-            "truncate_prompt": False  
-        }
-    )
-
-# note that max_new_tokens will be automatically specified internally based on given classes
-print(task.run())
-
-# self-consistency
-print(
-    task.run(
-        generation_config=GenerationConfig(
-            num_beams=3,
-            num_return_sequences=3,
-            do_sample=True
-        )
-    )
-)
-```
-
-</details>
-
-## Learn More
-[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
-
-[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
-
-## Supported Models
-
-> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
-> 
-> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
-
-| model type                         | quantization | inference | peft-lora | peft-adaption_prompt |
-|------------------------------------|--------------|-----------|-----------|----------------------|
-| bloom                              | ✅            | ✅         |           |                      |
-| gpt2                               | ✅            | ✅         |           |                      |
-| gpt_neox                           | ✅            | ✅         |           |                      |
-| gptj                               | ✅            | ✅         |           |                      |
-| llama                              | ✅            | ✅         |           | ✅                    |
-| moss                               | ✅            | ✅         |           |                      |
-| opt                                | ✅            | ✅         |           |                      |
-| gpt_bigcode                        | ✅            | ✅         |           |                      |
-| codegen                            | ✅            | ✅         |           |                      |
-| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         |           |                      |
-
-## Supported Evaluation Tasks
-Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
-
-## Acknowledgement
-- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
-- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
-
-
-[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
+<h1 align="center">AutoGPTQ</h1>
+<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
+<p align="center">
+    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
+        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
+    </a>
+    <a href="https://pypi.org/project/auto-gptq/">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
+    </a>
+</p>
+<h4 align="center">
+    <p>
+        <b>English</b> |
+        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
+    </p>
+</h4>
+
+*<center>📣 Long time no see! 👋 Architecture upgrade, performance optimization and more new features will come in July and August, stay tune! 🥂</center>*
+
+## News or Update
+
+- 2023-06-05 - (Update) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
+- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
+- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
+- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
+
+*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
+
+## Performance Comparison
+
+### Inference Speed
+> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
+> 
+> The quantized model is loaded using the setup that can gain the fastest inference speed.
+
+| model         | GPU           | num_beams | fp16  | gptq-int4 |
+|---------------|---------------|-----------|-------|-----------|
+| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
+| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
+| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
+| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
+| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
+| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
+| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
+| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
+
+
+### Perplexity
+For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
+
+## Installation
+
+### Quick Installation
+You can install the latest stable release of AutoGPTQ from pip:
+```shell
+pip install auto-gptq
+```
+Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
+```shell
+# firstly, cd the directory where the wheel saved, then execute command below
+pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
+```
+#### disable cuda extensions
+By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
+```shell
+BUILD_CUDA_EXT=0 pip install auto-gptq
+```
+And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
+```shell
+pip uninstall autogptq_cuda -y
+```
+
+#### to support triton speedup
+To integrate with `triton`, using:
+> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
+
+```shell
+pip install auto-gptq[triton]
+```
+
+### Install from source
+<details>
+<summary>click to see details</summary>
+
+Clone the source code:
+```shell
+git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
+```
+Then, install from source:
+```shell
+pip install .
+```
+Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
+
+Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
+
+</details>
+
+## Quick Tour
+
+### Quantization and Inference
+> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
+
+Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
+```python
+from transformers import AutoTokenizer, TextGenerationPipeline
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+import logging
+
+logging.basicConfig(
+    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
+)
+
+pretrained_model_dir = "facebook/opt-125m"
+quantized_model_dir = "opt-125m-4bit"
+
+tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
+examples = [
+    tokenizer(
+        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
+    )
+]
+
+quantize_config = BaseQuantizeConfig(
+    bits=4,  # quantize model to 4-bit
+    group_size=128,  # it is recommended to set the value to 128
+    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
+)
+
+# load un-quantized model, by default, the model will always be loaded into CPU memory
+model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
+
+# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
+model.quantize(examples)
+
+# save quantized model
+model.save_quantized(quantized_model_dir)
+
+# save quantized model using safetensors
+model.save_quantized(quantized_model_dir, use_safetensors=True)
+
+# push quantized model to Hugging Face Hub. 
+# to use use_auth_token=True, Login first via huggingface-cli login.
+# or pass explcit token with: use_auth_token="hf_xxxxxxx"
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
+
+# alternatively you can save and push at the same time
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
+
+# load quantized model to the first GPU
+model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
+
+# download quantized model from Hugging Face Hub and load to the first GPU
+# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
+
+# inference with model.generate
+print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
+
+# or you can also use pipeline
+pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
+print(pipeline("auto-gptq is")[0]["generated_text"])
+```
+
+For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
+
+### Customize Model
+<details>
+
+<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
+
+```python
+from auto_gptq.modeling import BaseGPTQForCausalLM
+
+
+class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
+    # chained attribute name of transformer layer block
+    layers_block_name = "model.decoder.layers"
+    # chained attribute names of other nn modules that in the same level as the transformer layer block
+    outside_layer_modules = [
+        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
+        "model.decoder.project_in", "model.decoder.final_layer_norm"
+    ]
+    # chained attribute names of linear layers in transformer layer module
+    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
+    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
+    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
+    inside_layer_modules = [
+        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
+        ["self_attn.out_proj"],
+        ["fc1"],
+        ["fc2"]
+    ]
+```
+After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
+
+</details>
+
+### Evaluation on Downstream Tasks
+You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
+
+The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
+
+<details>
+
+<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
+
+```python
+from functools import partial
+
+import datasets
+from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
+
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+from auto_gptq.eval_tasks import SequenceClassificationTask
+
+
+MODEL = "EleutherAI/gpt-j-6b"
+DATASET = "cardiffnlp/tweet_sentiment_multilingual"
+TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
+ID2LABEL = {
+    0: "negative",
+    1: "neutral",
+    2: "positive"
+}
+LABELS = list(ID2LABEL.values())
+
+
+def ds_refactor_fn(samples):
+    text_data = samples["text"]
+    label_data = samples["label"]
+
+    new_samples = {"prompt": [], "label": []}
+    for text, label in zip(text_data, label_data):
+        prompt = TEMPLATE.format(labels=LABELS, text=text)
+        new_samples["prompt"].append(prompt)
+        new_samples["label"].append(ID2LABEL[label])
+
+    return new_samples
+
+
+#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
+model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
+tokenizer = AutoTokenizer.from_pretrained(MODEL)
+
+task = SequenceClassificationTask(
+        model=model,
+        tokenizer=tokenizer,
+        classes=LABELS,
+        data_name_or_path=DATASET,
+        prompt_col_name="prompt",
+        label_col_name="label",
+        **{
+            "num_samples": 1000,  # how many samples will be sampled to evaluation
+            "sample_max_len": 1024,  # max tokens for each sample
+            "block_max_len": 2048,  # max tokens for each data block
+            # function to load dataset, one must only accept data_name_or_path as input 
+            # and return datasets.Dataset
+            "load_fn": partial(datasets.load_dataset, name="english"),  
+            # function to preprocess dataset, which is used for datasets.Dataset.map, 
+            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
+            "preprocess_fn": ds_refactor_fn,  
+            # truncate label when sample's length exceed sample_max_len
+            "truncate_prompt": False  
+        }
+    )
+
+# note that max_new_tokens will be automatically specified internally based on given classes
+print(task.run())
+
+# self-consistency
+print(
+    task.run(
+        generation_config=GenerationConfig(
+            num_beams=3,
+            num_return_sequences=3,
+            do_sample=True
+        )
+    )
+)
+```
+
+</details>
+
+## Learn More
+[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
+
+[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
+
+## Supported Models
+
+> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
+> 
+> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
+
+| model type                         | quantization | inference | peft-lora | peft-ada-lora | peft-adaption_prompt                                                                            |
+|------------------------------------|--------------|-----------|-----------|---------------|-------------------------------------------------------------------------------------------------|
+| bloom                              | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt2                               | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_neox                           | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| gptj                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| llama                              | ✅            | ✅         | ✅         | ✅             | ✅                                                                                               |
+| moss                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| opt                                | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_bigcode                        | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| codegen                            | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+
+## Supported Evaluation Tasks
+Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
+
+## Acknowledgement
+- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
+- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
+
+
+[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
```

#### html2text {}

```diff
@@ -1,99 +1,83 @@
-Metadata-Version: 2.1 Name: auto_gptq Version: 0.2.2 Summary: An easy-to-use
-LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
-Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
-gptq,quantization,large-language-models,pytorch,transformers Platform: windows
-Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
-OSI Approved :: MIT License Classifier: Natural Language :: Chinese
-(Simplified) Classifier: Natural Language :: English Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: C++ Requires-Python: >=3.8.0 Description-Content-Type: text/
-markdown Provides-Extra: llama Provides-Extra: triton License-File: LICENSE
                             ****** AutoGPTQ ******
 An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ
                                   algorithm.
                       [GitHub_release] [PyPI_-_Downloads]
                            *** English | ä¸­æ ***
-## News or Update **To experience adapter training using `auto_gptq` quantized
-model in advance, you can try [this branch](https://github.com/PanQiWei/
-AutoGPTQ/tree/peft_integration) and discuss [in here](https://github.com/
-PanQiWei/AutoGPTQ/issues/103), examples are [in here](https://github.com/
-PanQiWei/AutoGPTQ/tree/peft_integration/examples/peft).** - 2023-05-25 - (In
-Progress) - Integrate with ð¤ peft to use gptq quantized model to train
-adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc. - 2023-05-30 - (Update) -
-Support download/upload quantized model from/to ð¤ Hub. - 2023-05-27 -
-(Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and
-`RefineWeb/RefineWebModel`(falcon) model types. - 2023-05-04 - (Update) -
-Support using faster cuda kernel when `not desc_act or group_size == -1`. *For
-more histories please turn to [here](docs/NEWS_OR_UPDATE.md)* ## Performance
-Comparison ### Inference Speed > The result is generated using [this script]
-(examples/benchmark/generation_speed.py), batch size of input is 1, decode
-strategy is beam search and enforce the model to generate 512 tokens, speed
-metric is tokens/s (the larger, the better). > > The quantized model is loaded
-using the setup that can gain the fastest inference speed. | model | GPU |
-num_beams | fp16 | gptq-int4 | |---------------|---------------|-----------|---
-----|-----------| | llama-7b | 1xA100-40G | 1 | 18.87 | 25.53 | | llama-7b |
-1xA100-40G | 4 | 68.79 | 91.30 | | moss-moon 16b | 1xA100-40G | 1 | 12.48 |
-15.25 | | moss-moon 16b | 1xA100-40G | 4 | OOM | 42.67 | | moss-moon 16b |
-2xA100-40G | 1 | 06.83 | 06.78 | | moss-moon 16b | 2xA100-40G | 4 | 13.10 |
-10.80 | | gpt-j 6b | 1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b | 1xRTX3060-
-12G | 4 | OOM | 47.36 | ### Perplexity For perplexity comparison, you can turn
-to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here]
-(https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ##
+*
+ð£ Long time no see! ð Architecture upgrade, performance optimization and
+        more new features will come in July and August, stay tune! ð¥
+* ## News or Update - 2023-06-05 - (Update) - Integrate with ð¤ peft to use
+gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt,
+etc. - 2023-05-30 - (Update) - Support download/upload quantized model from/to
+ð¤ Hub. - 2023-05-27 - (Update) - Support quantization and inference for
+`gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types. -
+2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or
+group_size == -1`. *For more histories please turn to [here](docs/
+NEWS_OR_UPDATE.md)* ## Performance Comparison ### Inference Speed > The result
+is generated using [this script](examples/benchmark/generation_speed.py), batch
+size of input is 1, decode strategy is beam search and enforce the model to
+generate 512 tokens, speed metric is tokens/s (the larger, the better). > > The
+quantized model is loaded using the setup that can gain the fastest inference
+speed. | model | GPU | num_beams | fp16 | gptq-int4 | |---------------|--------
+-------|-----------|-------|-----------| | llama-7b | 1xA100-40G | 1 | 18.87 |
+25.53 | | llama-7b | 1xA100-40G | 4 | 68.79 | 91.30 | | moss-moon 16b | 1xA100-
+40G | 1 | 12.48 | 15.25 | | moss-moon 16b | 1xA100-40G | 4 | OOM | 42.67 | |
+moss-moon 16b | 2xA100-40G | 1 | 06.83 | 06.78 | | moss-moon 16b | 2xA100-40G |
+4 | 13.10 | 10.80 | | gpt-j 6b | 1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b |
+1xRTX3060-12G | 4 | OOM | 47.36 | ### Perplexity For perplexity comparison, you
+can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and
+[here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ##
 Installation ### Quick Installation You can install the latest stable release
 of AutoGPTQ from pip: ```shell pip install auto-gptq ``` Start from v0.2.0, you
 can download pre-build wheel that satisfied your environment setup from each
 version's release assets and install it to skip building stage for the fastest
 installation speed. For example: ```shell # firstly, cd the directory where the
 wheel saved, then execute command below pip install auto_gptq-0.2.0+cu118-
 cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for
 linux in an environment whose python=3.10 and cuda=11.8 ``` #### disable cuda
 extensions By default, cuda extensions will be installed when `torch` and
 `cuda` is already installed in your machine, if you don't want to use them,
 using: ```shell BUILD_CUDA_EXT=0 pip install auto-gptq ``` And to make sure
 `autogptq_cuda` is not ever in your virtual environment, run: ```shell pip
-uninstall autogptq_cuda -y ``` #### to support LLaMa model For some people want
-to try LLaMa and whose `transformers` version not meet the newest one that
-supports it, using: ```shell pip install auto-gptq[llama] ``` #### to support
-triton speedup To integrate with `triton`, using: > warning: currently triton
-only supports linux; 3-bit quantization is not supported when using triton
-```shell pip install auto-gptq[triton] ``` ### Install from source  click to
-see details Clone the source code: ```shell git clone https://github.com/
-PanQiWei/AutoGPTQ.git && cd AutoGPTQ ``` Then, install from source: ```shell
-pip install . ``` Like quick installation, you can also set `BUILD_CUDA_EXT=0`
-to disable pytorch extension building. Use `.[llama]` if you want to try LLaMa
-model. Use `.[triton]` if you want to integrate with triton and it's available
-on your operating system.  ## Quick Tour ### Quantization and Inference >
-warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which
-uses only one sample to quantize a much small model, quality of quantized model
-using such little samples may not good. Below is an example for the simplest
-use of `auto_gptq` to quantize a model and inference after quantization:
-```python from transformers import AutoTokenizer, TextGenerationPipeline from
-auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig import logging
-logging.basicConfig( format="%(asctime)s %(levelname)s [%(name)s] %(message)s",
-level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S" ) pretrained_model_dir =
-"facebook/opt-125m" quantized_model_dir = "opt-125m-4bit" tokenizer =
-AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True) examples =
-[ tokenizer( "auto-gptq is an easy-to-use model quantization library with user-
-friendly apis, based on GPTQ algorithm." ) ] quantize_config =
-BaseQuantizeConfig( bits=4, # quantize model to 4-bit group_size=128, # it is
-recommended to set the value to 128 desc_act=False, # set to False can
-significantly speed up inference but the perplexity may slightly bad ) # load
-un-quantized model, by default, the model will always be loaded into CPU memory
-model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir,
-quantize_config) # quantize model, the examples should be list of dict whose
-keys can only be "input_ids" and "attention_mask" model.quantize(examples) #
-save quantized model model.save_quantized(quantized_model_dir) # save quantized
-model using safetensors model.save_quantized(quantized_model_dir,
-use_safetensors=True) # push quantized model to Hugging Face Hub. # to use
-use_auth_token=True, Login first via huggingface-cli login. # or pass explcit
-token with: use_auth_token="hf_xxxxxxx" # (uncomment the following three lines
-to enable this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
+uninstall autogptq_cuda -y ``` #### to support triton speedup To integrate with
+`triton`, using: > warning: currently triton only supports linux; 3-bit
+quantization is not supported when using triton ```shell pip install auto-gptq
+[triton] ``` ### Install from source  click to see details Clone the source
+code: ```shell git clone https://github.com/PanQiWei/AutoGPTQ.git && cd
+AutoGPTQ ``` Then, install from source: ```shell pip install . ``` Like quick
+installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension
+building. Use `.[triton]` if you want to integrate with triton and it's
+available on your operating system.  ## Quick Tour ### Quantization and
+Inference > warning: this is just a showcase of the usage of basic apis in
+AutoGPTQ, which uses only one sample to quantize a much small model, quality of
+quantized model using such little samples may not good. Below is an example for
+the simplest use of `auto_gptq` to quantize a model and inference after
+quantization: ```python from transformers import AutoTokenizer,
+TextGenerationPipeline from auto_gptq import AutoGPTQForCausalLM,
+BaseQuantizeConfig import logging logging.basicConfig( format="%(asctime)s %
+(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:
+%M:%S" ) pretrained_model_dir = "facebook/opt-125m" quantized_model_dir = "opt-
+125m-4bit" tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir,
+use_fast=True) examples = [ tokenizer( "auto-gptq is an easy-to-use model
+quantization library with user-friendly apis, based on GPTQ algorithm." ) ]
+quantize_config = BaseQuantizeConfig( bits=4, # quantize model to 4-bit
+group_size=128, # it is recommended to set the value to 128 desc_act=False, #
+set to False can significantly speed up inference but the perplexity may
+slightly bad ) # load un-quantized model, by default, the model will always be
+loaded into CPU memory model = AutoGPTQForCausalLM.from_pretrained
+(pretrained_model_dir, quantize_config) # quantize model, the examples should
+be list of dict whose keys can only be "input_ids" and "attention_mask"
+model.quantize(examples) # save quantized model model.save_quantized
+(quantized_model_dir) # save quantized model using safetensors
+model.save_quantized(quantized_model_dir, use_safetensors=True) # push
+quantized model to Hugging Face Hub. # to use use_auth_token=True, Login first
+via huggingface-cli login. # or pass explcit token with:
+use_auth_token="hf_xxxxxxx" # (uncomment the following three lines to enable
+this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
 {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act=
 {quantize_config.desc_act}" # model.push_to_hub(repo_id,
 commit_message=commit_message, use_auth_token=True) # alternatively you can
 save and push at the same time # (uncomment the following three lines to enable
 this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
@@ -165,23 +149,29 @@
 step-by-step guidance to integrate `auto_gptq` with your own project and some
 best practice principles. [examples](examples/README.md) provide plenty of
 example scripts to use `auto_gptq` in different ways. ## Supported Models > you
 can use `model.config.model_type` to compare with the table below to check
 whether the model you use is supported by `auto_gptq`. > > for example,
 model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they
 are all supported by `auto_gptq`. | model type | quantization | inference |
-peft-lora | peft-adaption_prompt | |------------------------------------|------
---------|-----------|-----------|----------------------| | bloom | â | â |
-| | | gpt2 | â | â | | | | gpt_neox | â | â | | | | gptj | â | â |
-| | | llama | â | â | | â | | moss | â | â | | | | opt | â | â |
-| | | gpt_bigcode | â | â | | | | codegen | â | â | | | | falcon
-(RefinedWebModel/RefinedWeb) | â | â | | | ## Supported Evaluation Tasks
-Currently, `auto_gptq` supports: `LanguageModelingTask`,
-`SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come
-soon! ## Acknowledgement - Specially thanks **Elias Frantar**, **Saleh
-Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ**
-algorithm and open source the [code](https://github.com/IST-DASLab/gptq). -
-Specially thanks **qwopqwop200**, for code in this project that relevant to
-quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/
-qwopqwop200/GPTQ-for-LLaMa/tree/cuda). [![Star History Chart](https://api.star-
-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/
-#PanQiWei/AutoGPTQ&Date)
+peft-lora | peft-ada-lora | peft-adaption_prompt | |---------------------------
+---------|--------------|-----------|-----------|---------------|--------------
+-------------------------------------------------------------------------------
+----| | bloom | â | â | â | â | | | gpt2 | â | â | â | â | | |
+gpt_neox | â | â | â | â | â[requires this peft branch](https://
+github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) | | gptj | â | â
+| â | â | â[requires this peft branch](https://github.com/PanQiWei/peft/
+tree/multi_modal_adaption_prompt) | | llama | â | â | â | â | â | |
+moss | â | â | â | â | â[requires this peft branch](https://
+github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) | | opt | â | â
+| â | â | | | gpt_bigcode | â | â | â | â | | | codegen | â | â
+| â | â | | | falcon(RefinedWebModel/RefinedWeb) | â | â | â | â |
+| ## Supported Evaluation Tasks Currently, `auto_gptq` supports:
+`LanguageModelingTask`, `SequenceClassificationTask` and
+`TextSummarizationTask`; more Tasks will come soon! ## Acknowledgement -
+Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and
+**Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code]
+(https://github.com/IST-DASLab/gptq). - Specially thanks **qwopqwop200**, for
+code in this project that relevant to quantization are mainly referenced from
+[GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda). [!
+[Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/
+AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
```

### Comparing `auto_gptq-0.2.2/README.md` & `auto_gptq-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,328 +1,345 @@
-<h1 align="center">AutoGPTQ</h1>
-<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
-<p align="center">
-    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
-    </a>
-    <a href="https://pypi.org/project/auto-gptq/">
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
-    </a>
-</p>
-<h4 align="center">
-    <p>
-        <b>English</b> |
-        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
-    <p>
-</h4>
-
-## News or Update
-
-**To experience adapter training using `auto_gptq` quantized model in advance, you can try [this branch](https://github.com/PanQiWei/AutoGPTQ/tree/peft_integration) and discuss [in here](https://github.com/PanQiWei/AutoGPTQ/issues/103), examples are [in here](https://github.com/PanQiWei/AutoGPTQ/tree/peft_integration/examples/peft).**
-
-- 2023-05-25 - (In Progress) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
-- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
-- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
-- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
-
-*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
-
-## Performance Comparison
-
-### Inference Speed
-> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
-> 
-> The quantized model is loaded using the setup that can gain the fastest inference speed.
-
-| model         | GPU           | num_beams | fp16  | gptq-int4 |
-|---------------|---------------|-----------|-------|-----------|
-| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
-| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
-| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
-| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
-| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
-| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
-| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
-| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
-
-
-### Perplexity
-For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
-
-## Installation
-
-### Quick Installation
-You can install the latest stable release of AutoGPTQ from pip:
-```shell
-pip install auto-gptq
-```
-Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
-```shell
-# firstly, cd the directory where the wheel saved, then execute command below
-pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
-```
-#### disable cuda extensions
-By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
-```shell
-BUILD_CUDA_EXT=0 pip install auto-gptq
-```
-And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
-```shell
-pip uninstall autogptq_cuda -y
-```
-#### to support LLaMa model
-For some people want to try LLaMa and whose `transformers` version not meet the newest one that supports it, using:
-```shell
-pip install auto-gptq[llama]
-```
-#### to support triton speedup
-To integrate with `triton`, using:
-> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
-
-```shell
-pip install auto-gptq[triton]
-```
-
-### Install from source
-<details>
-<summary>click to see details</summary>
-
-Clone the source code:
-```shell
-git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
-```
-Then, install from source:
-```shell
-pip install .
-```
-Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
-
-Use `.[llama]` if you want to try LLaMa model.
-
-Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
-
-</details>
-
-## Quick Tour
-
-### Quantization and Inference
-> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
-
-Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
-```python
-from transformers import AutoTokenizer, TextGenerationPipeline
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-import logging
-
-logging.basicConfig(
-    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
-)
-
-pretrained_model_dir = "facebook/opt-125m"
-quantized_model_dir = "opt-125m-4bit"
-
-tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
-examples = [
-    tokenizer(
-        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
-    )
-]
-
-quantize_config = BaseQuantizeConfig(
-    bits=4,  # quantize model to 4-bit
-    group_size=128,  # it is recommended to set the value to 128
-    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
-)
-
-# load un-quantized model, by default, the model will always be loaded into CPU memory
-model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
-
-# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
-model.quantize(examples)
-
-# save quantized model
-model.save_quantized(quantized_model_dir)
-
-# save quantized model using safetensors
-model.save_quantized(quantized_model_dir, use_safetensors=True)
-
-# push quantized model to Hugging Face Hub. 
-# to use use_auth_token=True, Login first via huggingface-cli login.
-# or pass explcit token with: use_auth_token="hf_xxxxxxx"
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
-
-# alternatively you can save and push at the same time
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
-
-# load quantized model to the first GPU
-model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
-
-# download quantized model from Hugging Face Hub and load to the first GPU
-# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
-
-# inference with model.generate
-print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
-
-# or you can also use pipeline
-pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
-print(pipeline("auto-gptq is")[0]["generated_text"])
-```
-
-For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
-
-### Customize Model
-<details>
-
-<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
-
-```python
-from auto_gptq.modeling import BaseGPTQForCausalLM
-
-
-class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
-    # chained attribute name of transformer layer block
-    layers_block_name = "model.decoder.layers"
-    # chained attribute names of other nn modules that in the same level as the transformer layer block
-    outside_layer_modules = [
-        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
-        "model.decoder.project_in", "model.decoder.final_layer_norm"
-    ]
-    # chained attribute names of linear layers in transformer layer module
-    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
-    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
-    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
-    inside_layer_modules = [
-        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
-        ["self_attn.out_proj"],
-        ["fc1"],
-        ["fc2"]
-    ]
-```
-After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
-
-</details>
-
-### Evaluation on Downstream Tasks
-You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
-
-The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
-
-<details>
-
-<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
-
-```python
-from functools import partial
-
-import datasets
-from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
-
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-from auto_gptq.eval_tasks import SequenceClassificationTask
-
-
-MODEL = "EleutherAI/gpt-j-6b"
-DATASET = "cardiffnlp/tweet_sentiment_multilingual"
-TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
-ID2LABEL = {
-    0: "negative",
-    1: "neutral",
-    2: "positive"
-}
-LABELS = list(ID2LABEL.values())
-
-
-def ds_refactor_fn(samples):
-    text_data = samples["text"]
-    label_data = samples["label"]
-
-    new_samples = {"prompt": [], "label": []}
-    for text, label in zip(text_data, label_data):
-        prompt = TEMPLATE.format(labels=LABELS, text=text)
-        new_samples["prompt"].append(prompt)
-        new_samples["label"].append(ID2LABEL[label])
-
-    return new_samples
-
-
-#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
-model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
-tokenizer = AutoTokenizer.from_pretrained(MODEL)
-
-task = SequenceClassificationTask(
-        model=model,
-        tokenizer=tokenizer,
-        classes=LABELS,
-        data_name_or_path=DATASET,
-        prompt_col_name="prompt",
-        label_col_name="label",
-        **{
-            "num_samples": 1000,  # how many samples will be sampled to evaluation
-            "sample_max_len": 1024,  # max tokens for each sample
-            "block_max_len": 2048,  # max tokens for each data block
-            # function to load dataset, one must only accept data_name_or_path as input 
-            # and return datasets.Dataset
-            "load_fn": partial(datasets.load_dataset, name="english"),  
-            # function to preprocess dataset, which is used for datasets.Dataset.map, 
-            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
-            "preprocess_fn": ds_refactor_fn,  
-            # truncate label when sample's length exceed sample_max_len
-            "truncate_prompt": False  
-        }
-    )
-
-# note that max_new_tokens will be automatically specified internally based on given classes
-print(task.run())
-
-# self-consistency
-print(
-    task.run(
-        generation_config=GenerationConfig(
-            num_beams=3,
-            num_return_sequences=3,
-            do_sample=True
-        )
-    )
-)
-```
-
-</details>
-
-## Learn More
-[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
-
-[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
-
-## Supported Models
-
-> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
-> 
-> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
-
-| model type                         | quantization | inference | peft-lora | peft-adaption_prompt |
-|------------------------------------|--------------|-----------|-----------|----------------------|
-| bloom                              | ✅            | ✅         |           |                      |
-| gpt2                               | ✅            | ✅         |           |                      |
-| gpt_neox                           | ✅            | ✅         |           |                      |
-| gptj                               | ✅            | ✅         |           |                      |
-| llama                              | ✅            | ✅         |           | ✅                    |
-| moss                               | ✅            | ✅         |           |                      |
-| opt                                | ✅            | ✅         |           |                      |
-| gpt_bigcode                        | ✅            | ✅         |           |                      |
-| codegen                            | ✅            | ✅         |           |                      |
-| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         |           |                      |
-
-## Supported Evaluation Tasks
-Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
-
-## Acknowledgement
-- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
-- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
-
-
-[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
+Metadata-Version: 2.1
+Name: auto_gptq
+Version: 0.3.0
+Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
+Home-page: https://github.com/PanQiWei/AutoGPTQ
+Author: PanQiWei
+Keywords: gptq,quantization,large-language-models,pytorch,transformers
+Platform: windows
+Platform: linux
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: C++
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: triton
+License-File: LICENSE
+
+<h1 align="center">AutoGPTQ</h1>
+<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
+<p align="center">
+    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
+        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
+    </a>
+    <a href="https://pypi.org/project/auto-gptq/">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
+    </a>
+</p>
+<h4 align="center">
+    <p>
+        <b>English</b> |
+        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
+    </p>
+</h4>
+
+*<center>📣 Long time no see! 👋 Architecture upgrade, performance optimization and more new features will come in July and August, stay tune! 🥂</center>*
+
+## News or Update
+
+- 2023-06-05 - (Update) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
+- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
+- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
+- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
+
+*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
+
+## Performance Comparison
+
+### Inference Speed
+> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
+> 
+> The quantized model is loaded using the setup that can gain the fastest inference speed.
+
+| model         | GPU           | num_beams | fp16  | gptq-int4 |
+|---------------|---------------|-----------|-------|-----------|
+| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
+| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
+| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
+| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
+| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
+| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
+| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
+| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
+
+
+### Perplexity
+For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
+
+## Installation
+
+### Quick Installation
+You can install the latest stable release of AutoGPTQ from pip:
+```shell
+pip install auto-gptq
+```
+Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
+```shell
+# firstly, cd the directory where the wheel saved, then execute command below
+pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
+```
+#### disable cuda extensions
+By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
+```shell
+BUILD_CUDA_EXT=0 pip install auto-gptq
+```
+And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
+```shell
+pip uninstall autogptq_cuda -y
+```
+
+#### to support triton speedup
+To integrate with `triton`, using:
+> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
+
+```shell
+pip install auto-gptq[triton]
+```
+
+### Install from source
+<details>
+<summary>click to see details</summary>
+
+Clone the source code:
+```shell
+git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
+```
+Then, install from source:
+```shell
+pip install .
+```
+Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
+
+Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
+
+</details>
+
+## Quick Tour
+
+### Quantization and Inference
+> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
+
+Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
+```python
+from transformers import AutoTokenizer, TextGenerationPipeline
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+import logging
+
+logging.basicConfig(
+    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
+)
+
+pretrained_model_dir = "facebook/opt-125m"
+quantized_model_dir = "opt-125m-4bit"
+
+tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
+examples = [
+    tokenizer(
+        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
+    )
+]
+
+quantize_config = BaseQuantizeConfig(
+    bits=4,  # quantize model to 4-bit
+    group_size=128,  # it is recommended to set the value to 128
+    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
+)
+
+# load un-quantized model, by default, the model will always be loaded into CPU memory
+model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
+
+# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
+model.quantize(examples)
+
+# save quantized model
+model.save_quantized(quantized_model_dir)
+
+# save quantized model using safetensors
+model.save_quantized(quantized_model_dir, use_safetensors=True)
+
+# push quantized model to Hugging Face Hub. 
+# to use use_auth_token=True, Login first via huggingface-cli login.
+# or pass explcit token with: use_auth_token="hf_xxxxxxx"
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
+
+# alternatively you can save and push at the same time
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
+
+# load quantized model to the first GPU
+model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
+
+# download quantized model from Hugging Face Hub and load to the first GPU
+# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
+
+# inference with model.generate
+print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
+
+# or you can also use pipeline
+pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
+print(pipeline("auto-gptq is")[0]["generated_text"])
+```
+
+For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
+
+### Customize Model
+<details>
+
+<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
+
+```python
+from auto_gptq.modeling import BaseGPTQForCausalLM
+
+
+class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
+    # chained attribute name of transformer layer block
+    layers_block_name = "model.decoder.layers"
+    # chained attribute names of other nn modules that in the same level as the transformer layer block
+    outside_layer_modules = [
+        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
+        "model.decoder.project_in", "model.decoder.final_layer_norm"
+    ]
+    # chained attribute names of linear layers in transformer layer module
+    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
+    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
+    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
+    inside_layer_modules = [
+        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
+        ["self_attn.out_proj"],
+        ["fc1"],
+        ["fc2"]
+    ]
+```
+After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
+
+</details>
+
+### Evaluation on Downstream Tasks
+You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
+
+The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
+
+<details>
+
+<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
+
+```python
+from functools import partial
+
+import datasets
+from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
+
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+from auto_gptq.eval_tasks import SequenceClassificationTask
+
+
+MODEL = "EleutherAI/gpt-j-6b"
+DATASET = "cardiffnlp/tweet_sentiment_multilingual"
+TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
+ID2LABEL = {
+    0: "negative",
+    1: "neutral",
+    2: "positive"
+}
+LABELS = list(ID2LABEL.values())
+
+
+def ds_refactor_fn(samples):
+    text_data = samples["text"]
+    label_data = samples["label"]
+
+    new_samples = {"prompt": [], "label": []}
+    for text, label in zip(text_data, label_data):
+        prompt = TEMPLATE.format(labels=LABELS, text=text)
+        new_samples["prompt"].append(prompt)
+        new_samples["label"].append(ID2LABEL[label])
+
+    return new_samples
+
+
+#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
+model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
+tokenizer = AutoTokenizer.from_pretrained(MODEL)
+
+task = SequenceClassificationTask(
+        model=model,
+        tokenizer=tokenizer,
+        classes=LABELS,
+        data_name_or_path=DATASET,
+        prompt_col_name="prompt",
+        label_col_name="label",
+        **{
+            "num_samples": 1000,  # how many samples will be sampled to evaluation
+            "sample_max_len": 1024,  # max tokens for each sample
+            "block_max_len": 2048,  # max tokens for each data block
+            # function to load dataset, one must only accept data_name_or_path as input 
+            # and return datasets.Dataset
+            "load_fn": partial(datasets.load_dataset, name="english"),  
+            # function to preprocess dataset, which is used for datasets.Dataset.map, 
+            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
+            "preprocess_fn": ds_refactor_fn,  
+            # truncate label when sample's length exceed sample_max_len
+            "truncate_prompt": False  
+        }
+    )
+
+# note that max_new_tokens will be automatically specified internally based on given classes
+print(task.run())
+
+# self-consistency
+print(
+    task.run(
+        generation_config=GenerationConfig(
+            num_beams=3,
+            num_return_sequences=3,
+            do_sample=True
+        )
+    )
+)
+```
+
+</details>
+
+## Learn More
+[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
+
+[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
+
+## Supported Models
+
+> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
+> 
+> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
+
+| model type                         | quantization | inference | peft-lora | peft-ada-lora | peft-adaption_prompt                                                                            |
+|------------------------------------|--------------|-----------|-----------|---------------|-------------------------------------------------------------------------------------------------|
+| bloom                              | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt2                               | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_neox                           | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| gptj                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| llama                              | ✅            | ✅         | ✅         | ✅             | ✅                                                                                               |
+| moss                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| opt                                | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_bigcode                        | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| codegen                            | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+
+## Supported Evaluation Tasks
+Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
+
+## Acknowledgement
+- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
+- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
+
+
+[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
```

#### html2text {}

```diff
@@ -1,87 +1,95 @@
+Metadata-Version: 2.1 Name: auto_gptq Version: 0.3.0 Summary: An easy-to-use
+LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
+Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
+gptq,quantization,large-language-models,pytorch,transformers Platform: windows
+Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
+OSI Approved :: MIT License Classifier: Natural Language :: Chinese
+(Simplified) Classifier: Natural Language :: English Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: C++ Requires-Python: >=3.8.0 Description-Content-Type: text/
+markdown Provides-Extra: triton License-File: LICENSE
                             ****** AutoGPTQ ******
 An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ
                                   algorithm.
                       [GitHub_release] [PyPI_-_Downloads]
                            *** English | ä¸­æ ***
-## News or Update **To experience adapter training using `auto_gptq` quantized
-model in advance, you can try [this branch](https://github.com/PanQiWei/
-AutoGPTQ/tree/peft_integration) and discuss [in here](https://github.com/
-PanQiWei/AutoGPTQ/issues/103), examples are [in here](https://github.com/
-PanQiWei/AutoGPTQ/tree/peft_integration/examples/peft).** - 2023-05-25 - (In
-Progress) - Integrate with ð¤ peft to use gptq quantized model to train
-adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc. - 2023-05-30 - (Update) -
-Support download/upload quantized model from/to ð¤ Hub. - 2023-05-27 -
-(Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and
-`RefineWeb/RefineWebModel`(falcon) model types. - 2023-05-04 - (Update) -
-Support using faster cuda kernel when `not desc_act or group_size == -1`. *For
-more histories please turn to [here](docs/NEWS_OR_UPDATE.md)* ## Performance
-Comparison ### Inference Speed > The result is generated using [this script]
-(examples/benchmark/generation_speed.py), batch size of input is 1, decode
-strategy is beam search and enforce the model to generate 512 tokens, speed
-metric is tokens/s (the larger, the better). > > The quantized model is loaded
-using the setup that can gain the fastest inference speed. | model | GPU |
-num_beams | fp16 | gptq-int4 | |---------------|---------------|-----------|---
-----|-----------| | llama-7b | 1xA100-40G | 1 | 18.87 | 25.53 | | llama-7b |
-1xA100-40G | 4 | 68.79 | 91.30 | | moss-moon 16b | 1xA100-40G | 1 | 12.48 |
-15.25 | | moss-moon 16b | 1xA100-40G | 4 | OOM | 42.67 | | moss-moon 16b |
-2xA100-40G | 1 | 06.83 | 06.78 | | moss-moon 16b | 2xA100-40G | 4 | 13.10 |
-10.80 | | gpt-j 6b | 1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b | 1xRTX3060-
-12G | 4 | OOM | 47.36 | ### Perplexity For perplexity comparison, you can turn
-to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here]
-(https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ##
+*
+ð£ Long time no see! ð Architecture upgrade, performance optimization and
+        more new features will come in July and August, stay tune! ð¥
+* ## News or Update - 2023-06-05 - (Update) - Integrate with ð¤ peft to use
+gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt,
+etc. - 2023-05-30 - (Update) - Support download/upload quantized model from/to
+ð¤ Hub. - 2023-05-27 - (Update) - Support quantization and inference for
+`gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types. -
+2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or
+group_size == -1`. *For more histories please turn to [here](docs/
+NEWS_OR_UPDATE.md)* ## Performance Comparison ### Inference Speed > The result
+is generated using [this script](examples/benchmark/generation_speed.py), batch
+size of input is 1, decode strategy is beam search and enforce the model to
+generate 512 tokens, speed metric is tokens/s (the larger, the better). > > The
+quantized model is loaded using the setup that can gain the fastest inference
+speed. | model | GPU | num_beams | fp16 | gptq-int4 | |---------------|--------
+-------|-----------|-------|-----------| | llama-7b | 1xA100-40G | 1 | 18.87 |
+25.53 | | llama-7b | 1xA100-40G | 4 | 68.79 | 91.30 | | moss-moon 16b | 1xA100-
+40G | 1 | 12.48 | 15.25 | | moss-moon 16b | 1xA100-40G | 4 | OOM | 42.67 | |
+moss-moon 16b | 2xA100-40G | 1 | 06.83 | 06.78 | | moss-moon 16b | 2xA100-40G |
+4 | 13.10 | 10.80 | | gpt-j 6b | 1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b |
+1xRTX3060-12G | 4 | OOM | 47.36 | ### Perplexity For perplexity comparison, you
+can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and
+[here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ##
 Installation ### Quick Installation You can install the latest stable release
 of AutoGPTQ from pip: ```shell pip install auto-gptq ``` Start from v0.2.0, you
 can download pre-build wheel that satisfied your environment setup from each
 version's release assets and install it to skip building stage for the fastest
 installation speed. For example: ```shell # firstly, cd the directory where the
 wheel saved, then execute command below pip install auto_gptq-0.2.0+cu118-
 cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for
 linux in an environment whose python=3.10 and cuda=11.8 ``` #### disable cuda
 extensions By default, cuda extensions will be installed when `torch` and
 `cuda` is already installed in your machine, if you don't want to use them,
 using: ```shell BUILD_CUDA_EXT=0 pip install auto-gptq ``` And to make sure
 `autogptq_cuda` is not ever in your virtual environment, run: ```shell pip
-uninstall autogptq_cuda -y ``` #### to support LLaMa model For some people want
-to try LLaMa and whose `transformers` version not meet the newest one that
-supports it, using: ```shell pip install auto-gptq[llama] ``` #### to support
-triton speedup To integrate with `triton`, using: > warning: currently triton
-only supports linux; 3-bit quantization is not supported when using triton
-```shell pip install auto-gptq[triton] ``` ### Install from source  click to
-see details Clone the source code: ```shell git clone https://github.com/
-PanQiWei/AutoGPTQ.git && cd AutoGPTQ ``` Then, install from source: ```shell
-pip install . ``` Like quick installation, you can also set `BUILD_CUDA_EXT=0`
-to disable pytorch extension building. Use `.[llama]` if you want to try LLaMa
-model. Use `.[triton]` if you want to integrate with triton and it's available
-on your operating system.  ## Quick Tour ### Quantization and Inference >
-warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which
-uses only one sample to quantize a much small model, quality of quantized model
-using such little samples may not good. Below is an example for the simplest
-use of `auto_gptq` to quantize a model and inference after quantization:
-```python from transformers import AutoTokenizer, TextGenerationPipeline from
-auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig import logging
-logging.basicConfig( format="%(asctime)s %(levelname)s [%(name)s] %(message)s",
-level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S" ) pretrained_model_dir =
-"facebook/opt-125m" quantized_model_dir = "opt-125m-4bit" tokenizer =
-AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True) examples =
-[ tokenizer( "auto-gptq is an easy-to-use model quantization library with user-
-friendly apis, based on GPTQ algorithm." ) ] quantize_config =
-BaseQuantizeConfig( bits=4, # quantize model to 4-bit group_size=128, # it is
-recommended to set the value to 128 desc_act=False, # set to False can
-significantly speed up inference but the perplexity may slightly bad ) # load
-un-quantized model, by default, the model will always be loaded into CPU memory
-model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir,
-quantize_config) # quantize model, the examples should be list of dict whose
-keys can only be "input_ids" and "attention_mask" model.quantize(examples) #
-save quantized model model.save_quantized(quantized_model_dir) # save quantized
-model using safetensors model.save_quantized(quantized_model_dir,
-use_safetensors=True) # push quantized model to Hugging Face Hub. # to use
-use_auth_token=True, Login first via huggingface-cli login. # or pass explcit
-token with: use_auth_token="hf_xxxxxxx" # (uncomment the following three lines
-to enable this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
+uninstall autogptq_cuda -y ``` #### to support triton speedup To integrate with
+`triton`, using: > warning: currently triton only supports linux; 3-bit
+quantization is not supported when using triton ```shell pip install auto-gptq
+[triton] ``` ### Install from source  click to see details Clone the source
+code: ```shell git clone https://github.com/PanQiWei/AutoGPTQ.git && cd
+AutoGPTQ ``` Then, install from source: ```shell pip install . ``` Like quick
+installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension
+building. Use `.[triton]` if you want to integrate with triton and it's
+available on your operating system.  ## Quick Tour ### Quantization and
+Inference > warning: this is just a showcase of the usage of basic apis in
+AutoGPTQ, which uses only one sample to quantize a much small model, quality of
+quantized model using such little samples may not good. Below is an example for
+the simplest use of `auto_gptq` to quantize a model and inference after
+quantization: ```python from transformers import AutoTokenizer,
+TextGenerationPipeline from auto_gptq import AutoGPTQForCausalLM,
+BaseQuantizeConfig import logging logging.basicConfig( format="%(asctime)s %
+(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:
+%M:%S" ) pretrained_model_dir = "facebook/opt-125m" quantized_model_dir = "opt-
+125m-4bit" tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir,
+use_fast=True) examples = [ tokenizer( "auto-gptq is an easy-to-use model
+quantization library with user-friendly apis, based on GPTQ algorithm." ) ]
+quantize_config = BaseQuantizeConfig( bits=4, # quantize model to 4-bit
+group_size=128, # it is recommended to set the value to 128 desc_act=False, #
+set to False can significantly speed up inference but the perplexity may
+slightly bad ) # load un-quantized model, by default, the model will always be
+loaded into CPU memory model = AutoGPTQForCausalLM.from_pretrained
+(pretrained_model_dir, quantize_config) # quantize model, the examples should
+be list of dict whose keys can only be "input_ids" and "attention_mask"
+model.quantize(examples) # save quantized model model.save_quantized
+(quantized_model_dir) # save quantized model using safetensors
+model.save_quantized(quantized_model_dir, use_safetensors=True) # push
+quantized model to Hugging Face Hub. # to use use_auth_token=True, Login first
+via huggingface-cli login. # or pass explcit token with:
+use_auth_token="hf_xxxxxxx" # (uncomment the following three lines to enable
+this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
 {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act=
 {quantize_config.desc_act}" # model.push_to_hub(repo_id,
 commit_message=commit_message, use_auth_token=True) # alternatively you can
 save and push at the same time # (uncomment the following three lines to enable
 this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
@@ -153,23 +161,29 @@
 step-by-step guidance to integrate `auto_gptq` with your own project and some
 best practice principles. [examples](examples/README.md) provide plenty of
 example scripts to use `auto_gptq` in different ways. ## Supported Models > you
 can use `model.config.model_type` to compare with the table below to check
 whether the model you use is supported by `auto_gptq`. > > for example,
 model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they
 are all supported by `auto_gptq`. | model type | quantization | inference |
-peft-lora | peft-adaption_prompt | |------------------------------------|------
---------|-----------|-----------|----------------------| | bloom | â | â |
-| | | gpt2 | â | â | | | | gpt_neox | â | â | | | | gptj | â | â |
-| | | llama | â | â | | â | | moss | â | â | | | | opt | â | â |
-| | | gpt_bigcode | â | â | | | | codegen | â | â | | | | falcon
-(RefinedWebModel/RefinedWeb) | â | â | | | ## Supported Evaluation Tasks
-Currently, `auto_gptq` supports: `LanguageModelingTask`,
-`SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come
-soon! ## Acknowledgement - Specially thanks **Elias Frantar**, **Saleh
-Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ**
-algorithm and open source the [code](https://github.com/IST-DASLab/gptq). -
-Specially thanks **qwopqwop200**, for code in this project that relevant to
-quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/
-qwopqwop200/GPTQ-for-LLaMa/tree/cuda). [![Star History Chart](https://api.star-
-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/
-#PanQiWei/AutoGPTQ&Date)
+peft-lora | peft-ada-lora | peft-adaption_prompt | |---------------------------
+---------|--------------|-----------|-----------|---------------|--------------
+-------------------------------------------------------------------------------
+----| | bloom | â | â | â | â | | | gpt2 | â | â | â | â | | |
+gpt_neox | â | â | â | â | â[requires this peft branch](https://
+github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) | | gptj | â | â
+| â | â | â[requires this peft branch](https://github.com/PanQiWei/peft/
+tree/multi_modal_adaption_prompt) | | llama | â | â | â | â | â | |
+moss | â | â | â | â | â[requires this peft branch](https://
+github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) | | opt | â | â
+| â | â | | | gpt_bigcode | â | â | â | â | | | codegen | â | â
+| â | â | | | falcon(RefinedWebModel/RefinedWeb) | â | â | â | â |
+| ## Supported Evaluation Tasks Currently, `auto_gptq` supports:
+`LanguageModelingTask`, `SequenceClassificationTask` and
+`TextSummarizationTask`; more Tasks will come soon! ## Acknowledgement -
+Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and
+**Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code]
+(https://github.com/IST-DASLab/gptq). - Specially thanks **qwopqwop200**, for
+code in this project that relevant to quantization are mainly referenced from
+[GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda). [!
+[Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/
+AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
```

### Comparing `auto_gptq-0.2.2/auto_gptq/eval_tasks/_base.py` & `auto_gptq-0.3.0/auto_gptq/eval_tasks/_base.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from abc import abstractmethod
-from typing import Any, Dict, List, Optional, Union
-
-import torch
-from transformers import PreTrainedTokenizer, PreTrainedModel
-
-from ..modeling import BaseGPTQForCausalLM
-from ..utils.data_utils import get_dataloader
-
-
-class BaseTask:
-    def __init__(
-        self,
-        model: Union[BaseGPTQForCausalLM, PreTrainedModel],
-        tokenizer: PreTrainedTokenizer,
-        data_name_or_path: str,
-        prompt_col_name: str,
-        label_col_name: str,
-        device: Optional[str] = None,
-        **kwargs
-    ):
-        self.model = model
-        self.tokenizer = tokenizer
-        if self.tokenizer.pad_token_id is None:
-            self.tokenizer.pad_token = self.tokenizer.eos_token
-            self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
-            self.model.config.pad_token_id = self.tokenizer.eos_token_id
-        self.dl = get_dataloader(
-            data_name_or_path,
-            prompt_col_name=prompt_col_name,
-            label_col_name=label_col_name,
-            tokenizer=tokenizer,
-            **kwargs
-        )
-
-        self.device = device
-        if not self.device:
-            self.device = self.model.device
-        if isinstance(self.device, str):
-            self.device = torch.device(self.device)
-
-    @abstractmethod
-    def _predict(self, batch_data: Dict[str, Any], **kwargs) -> List[Any]:
-        pass
-
-    @abstractmethod
-    def _parse_labels(self, label_ids: torch.LongTensor) -> List[Any]:
-        pass
-
-    @abstractmethod
-    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
-        pass
-
-    def run(self, **predict_kwargs) -> Dict[str, float]:
-        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
-            predictions = []
-            labels = []
-            for batch_data in self.dl:
-                for k, v in batch_data.items():
-                    if isinstance(v, torch.Tensor):
-                        batch_data[k] = v.to(self.device)
-                labels += self._parse_labels(batch_data["labels"])
-                predictions += self._predict(batch_data, **predict_kwargs)
-
-        return self._metric(predictions, labels)
+from abc import abstractmethod
+from typing import Any, Dict, List, Optional, Union
+
+import torch
+from transformers import PreTrainedTokenizer, PreTrainedModel
+
+from ..modeling import BaseGPTQForCausalLM
+from ..utils.data_utils import get_dataloader
+
+
+class BaseTask:
+    def __init__(
+        self,
+        model: Union[BaseGPTQForCausalLM, PreTrainedModel],
+        tokenizer: PreTrainedTokenizer,
+        data_name_or_path: str,
+        prompt_col_name: str,
+        label_col_name: str,
+        device: Optional[str] = None,
+        **kwargs
+    ):
+        self.model = model
+        self.tokenizer = tokenizer
+        if self.tokenizer.pad_token_id is None:
+            self.tokenizer.pad_token = self.tokenizer.eos_token
+            self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
+            self.model.config.pad_token_id = self.tokenizer.eos_token_id
+        self.dl = get_dataloader(
+            data_name_or_path,
+            prompt_col_name=prompt_col_name,
+            label_col_name=label_col_name,
+            tokenizer=tokenizer,
+            **kwargs
+        )
+
+        self.device = device
+        if not self.device:
+            self.device = self.model.device
+        if isinstance(self.device, str):
+            self.device = torch.device(self.device)
+
+    @abstractmethod
+    def _predict(self, batch_data: Dict[str, Any], **kwargs) -> List[Any]:
+        pass
+
+    @abstractmethod
+    def _parse_labels(self, label_ids: torch.LongTensor) -> List[Any]:
+        pass
+
+    @abstractmethod
+    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
+        pass
+
+    def run(self, **predict_kwargs) -> Dict[str, float]:
+        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
+            predictions = []
+            labels = []
+            for batch_data in self.dl:
+                for k, v in batch_data.items():
+                    if isinstance(v, torch.Tensor):
+                        batch_data[k] = v.to(self.device)
+                labels += self._parse_labels(batch_data["labels"])
+                predictions += self._predict(batch_data, **predict_kwargs)
+
+        return self._metric(predictions, labels)
```

### Comparing `auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/classification_utils.py` & `auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/classification_utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import sys
-from typing import List, Sequence
-
-import numpy as np
-
-
-def levenshtein_distance(seq1: Sequence, seq2: Sequence):
-    if seq1 == seq2:
-        return 0
-    num_rows = len(seq1) + 1
-    num_cols = len(seq2) + 1
-    dp_matrix = np.empty((num_rows, num_cols))
-    dp_matrix[0, :] = range(num_cols)
-    dp_matrix[:, 0] = range(num_rows)
-
-    for i in range(1, num_rows):
-        for j in range(1, num_cols):
-            if seq1[i - 1] == seq2[j - 1]:
-                dp_matrix[i, j] = dp_matrix[i - 1, j - 1]
-            else:
-                dp_matrix[i, j] = min(dp_matrix[i - 1, j - 1], dp_matrix[i - 1, j], dp_matrix[i, j - 1]) + 1
-
-    return dp_matrix[num_rows - 1, num_cols - 1]
-
-
-def get_closest_label(pred: Sequence, classes: List[Sequence]) -> int:
-    min_id = sys.maxsize
-    min_edit_distance = sys.maxsize
-    for i, class_label in enumerate(classes):
-        edit_distance = levenshtein_distance(pred, class_label)
-        if edit_distance < min_edit_distance:
-            min_id = i
-            min_edit_distance = edit_distance
-    return min_id
-
-
-__all__ = ["levenshtein_distance", "get_closest_label"]
+import sys
+from typing import List, Sequence
+
+import numpy as np
+
+
+def levenshtein_distance(seq1: Sequence, seq2: Sequence):
+    if seq1 == seq2:
+        return 0
+    num_rows = len(seq1) + 1
+    num_cols = len(seq2) + 1
+    dp_matrix = np.empty((num_rows, num_cols))
+    dp_matrix[0, :] = range(num_cols)
+    dp_matrix[:, 0] = range(num_rows)
+
+    for i in range(1, num_rows):
+        for j in range(1, num_cols):
+            if seq1[i - 1] == seq2[j - 1]:
+                dp_matrix[i, j] = dp_matrix[i - 1, j - 1]
+            else:
+                dp_matrix[i, j] = min(dp_matrix[i - 1, j - 1], dp_matrix[i - 1, j], dp_matrix[i, j - 1]) + 1
+
+    return dp_matrix[num_rows - 1, num_cols - 1]
+
+
+def get_closest_label(pred: Sequence, classes: List[Sequence]) -> int:
+    min_id = sys.maxsize
+    min_edit_distance = sys.maxsize
+    for i, class_label in enumerate(classes):
+        edit_distance = levenshtein_distance(pred, class_label)
+        if edit_distance < min_edit_distance:
+            min_id = i
+            min_edit_distance = edit_distance
+    return min_id
+
+
+__all__ = ["levenshtein_distance", "get_closest_label"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/eval_tasks/_utils/generation_utils.py` & `auto_gptq-0.3.0/auto_gptq/eval_tasks/_utils/generation_utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import List, Optional, Union
-
-from torch import LongTensor
-from transformers import PreTrainedTokenizer
-
-
-def postprocess_generation_ids(
-    input_ids: LongTensor,
-    output_ids: LongTensor,
-    num_return_sequences: int,
-    tokenizer: Optional[PreTrainedTokenizer] = None,
-    pad_token_ids: Optional[int] = None,
-) -> List[List[Union[str, List[int]]]]:
-    outputs = []
-    for idx, start in enumerate(range(0, len(output_ids), num_return_sequences)):
-        sub_output_ids = output_ids[start: start + num_return_sequences]
-        sub_generated_ids = sub_output_ids[..., input_ids[idx].size(0):]
-        if tokenizer:
-            outputs.append(
-                [
-                    generated_text for generated_text in tokenizer.batch_decode(
-                        sub_generated_ids,
-                        clean_up_tokenization_spaces=True
-                    )
-                ]
-            )
-        else:
-            sub_generated_ids = sub_output_ids.cpu().numpy().tolist()
-            for i, one_sub_generated_ids in enumerate(sub_generated_ids):
-                if pad_token_ids is not None and pad_token_ids in one_sub_generated_ids:
-                    one_sub_generated_ids = one_sub_generated_ids[: one_sub_generated_ids.index(pad_token_ids)]
-                sub_generated_ids[i] = one_sub_generated_ids
-            outputs.append(sub_generated_ids)
-
-    return outputs
-
-
-__all__ = ["postprocess_generation_ids"]
+from typing import List, Optional, Union
+
+from torch import LongTensor
+from transformers import PreTrainedTokenizer
+
+
+def postprocess_generation_ids(
+    input_ids: LongTensor,
+    output_ids: LongTensor,
+    num_return_sequences: int,
+    tokenizer: Optional[PreTrainedTokenizer] = None,
+    pad_token_ids: Optional[int] = None,
+) -> List[List[Union[str, List[int]]]]:
+    outputs = []
+    for idx, start in enumerate(range(0, len(output_ids), num_return_sequences)):
+        sub_output_ids = output_ids[start: start + num_return_sequences]
+        sub_generated_ids = sub_output_ids[..., input_ids[idx].size(0):]
+        if tokenizer:
+            outputs.append(
+                [
+                    generated_text for generated_text in tokenizer.batch_decode(
+                        sub_generated_ids,
+                        clean_up_tokenization_spaces=True
+                    )
+                ]
+            )
+        else:
+            sub_generated_ids = sub_output_ids.cpu().numpy().tolist()
+            for i, one_sub_generated_ids in enumerate(sub_generated_ids):
+                if pad_token_ids is not None and pad_token_ids in one_sub_generated_ids:
+                    one_sub_generated_ids = one_sub_generated_ids[: one_sub_generated_ids.index(pad_token_ids)]
+                sub_generated_ids[i] = one_sub_generated_ids
+            outputs.append(sub_generated_ids)
+
+    return outputs
+
+
+__all__ = ["postprocess_generation_ids"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/eval_tasks/language_modeling_task.py` & `auto_gptq-0.3.0/auto_gptq/eval_tasks/language_modeling_task.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-import math
-from typing import Any, Dict, List, Optional
-
-from torch import LongTensor
-
-from ._base import BaseTask
-
-
-class LanguageModelingTask(BaseTask):
-    def __init__(
-        self,
-        model,
-        tokenizer,
-        data_name_or_path: str,
-        prompt_col_name: str,
-        label_col_name: str,
-        device: Optional[str] = None,
-        **kwargs
-    ):
-        kwargs["merge_prompt_label"] = True
-        super().__init__(
-            model=model,
-            tokenizer=tokenizer,
-            data_name_or_path=data_name_or_path,
-            prompt_col_name=prompt_col_name,
-            label_col_name=label_col_name,
-            device=device,
-            **kwargs
-        )
-
-    def _predict(self, batch_data: Dict[str, Any], *args, **kwargs) -> List[float]:
-        outputs = self.model(**batch_data)
-        loss = outputs.loss.cpu().item()
-
-        return [loss]
-
-    def _parse_labels(self, label_ids: LongTensor) -> List[Any]:
-        return []
-
-    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
-        return {"ppl": math.exp(sum(pred) / len(pred))}
-
-    def run(self) -> Dict[str, float]:
-        return super().run()
-
-
-__all__ = ["LanguageModelingTask"]
+import math
+from typing import Any, Dict, List, Optional
+
+from torch import LongTensor
+
+from ._base import BaseTask
+
+
+class LanguageModelingTask(BaseTask):
+    def __init__(
+        self,
+        model,
+        tokenizer,
+        data_name_or_path: str,
+        prompt_col_name: str,
+        label_col_name: str,
+        device: Optional[str] = None,
+        **kwargs
+    ):
+        kwargs["merge_prompt_label"] = True
+        super().__init__(
+            model=model,
+            tokenizer=tokenizer,
+            data_name_or_path=data_name_or_path,
+            prompt_col_name=prompt_col_name,
+            label_col_name=label_col_name,
+            device=device,
+            **kwargs
+        )
+
+    def _predict(self, batch_data: Dict[str, Any], *args, **kwargs) -> List[float]:
+        outputs = self.model(**batch_data)
+        loss = outputs.loss.cpu().item()
+
+        return [loss]
+
+    def _parse_labels(self, label_ids: LongTensor) -> List[Any]:
+        return []
+
+    def _metric(self, pred: List[Any], label: List[Any]) -> Dict[str, float]:
+        return {"ppl": math.exp(sum(pred) / len(pred))}
+
+    def run(self) -> Dict[str, float]:
+        return super().run()
+
+
+__all__ = ["LanguageModelingTask"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/modeling/_base.py` & `auto_gptq-0.3.0/auto_gptq/modeling/_base.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,840 +1,899 @@
-import copy
-import json
-import warnings
-import os
-from dataclasses import dataclass, field, fields
-from logging import getLogger
-from os.path import join, isfile, isdir
-from typing import Dict, List, Optional, Union
-
-import accelerate
-import torch
-import torch.nn as nn
-import transformers
-from accelerate.hooks import remove_hook_from_module
-from safetensors.torch import save_file as safe_save
-from transformers import AutoConfig, AutoModelForCausalLM, PreTrainedModel
-from transformers.utils.hub import PushToHubMixin, cached_file, create_repo, create_commit, CommitOperationAdd
-from transformers.utils.generic import ContextManagers
-from transformers.modeling_utils import no_init_weights
-
-from ._const import *
-from ._utils import *
-from ..nn_modules._fused_base import FusedBaseAttentionModule, FusedBaseMLPModule
-from ..quantization import GPTQ
-from ..utils.data_utils import collate_data
-from ..utils.import_utils import TRITON_AVAILABLE
-
-logger = getLogger(__name__)
-
-
-@dataclass
-class BaseQuantizeConfig(PushToHubMixin):
-    bits: int = field(default=4, metadata={"choices": [2, 3, 4, 8]})
-    group_size: int = field(default=-1)
-    damp_percent: float = field(default=0.01)
-    desc_act: bool = field(default=True)
-    sym: bool = field(default=True)
-    true_sequential: bool = field(default=True)
-    model_name_or_path: Optional[str] = field(default=None)
-    model_file_base_name: Optional[str] = field(default=None)
-
-    def __post_init__(self):
-        fields_info = fields(self)
-
-        if self.bits not in fields_info[0].metadata["choices"]:
-            raise ValueError(f"only support quantize to {fields_info[0].metadata['choices']} bits.")
-        if self.group_size != -1 and self.group_size <= 0:
-            raise ValueError("unless equal to -1, group_size must greater then 0.")
-        if not (0 < self.damp_percent < 1):
-            raise ValueError("damp_percent must between 0 and 1.")
-
-    def save_pretrained(self, save_dir: str, **kwargs):
-        with open(join(save_dir, "quantize_config.json"), "w", encoding="utf-8") as f:
-            json.dump(self.to_dict(), f, indent=2)
-
-    @classmethod
-    def from_pretrained(cls, save_dir: str, **kwargs):
-        # Parameters related to loading from Hugging Face Hub
-        cache_dir = kwargs.pop("cache_dir", None)
-        force_download = kwargs.pop("force_download", False)
-        resume_download = kwargs.pop("resume_download", False)
-        proxies = kwargs.pop("proxies", None)
-        local_files_only = kwargs.pop("local_files_only", False)
-        use_auth_token = kwargs.pop("use_auth_token", None)
-        revision = kwargs.pop("revision", None)
-        subfolder = kwargs.pop("subfolder", None)
-        commit_hash = kwargs.pop("_commit_hash", None)
-
-        quantize_config_filename = "quantize_config.json"
-        if os.path.isdir(save_dir):  # Local
-            resolved_config_file = join(save_dir, quantize_config_filename)
-        else: # Remote
-               resolved_config_file = cached_file(
-                    save_dir,
-                    quantize_config_filename,
-                    cache_dir=cache_dir,
-                    force_download=force_download,
-                    resume_download=resume_download,
-                    proxies=proxies,
-                    use_auth_token=use_auth_token,
-                    revision=revision,
-                    local_files_only=local_files_only,
-                    subfolder=subfolder,
-                    _raise_exceptions_for_missing_entries=False,
-                    _raise_exceptions_for_connection_errors=False,
-                    _commit_hash=commit_hash,
-               )
-
-        with open(resolved_config_file, "r", encoding="utf-8") as f:
-            return cls(**json.load(f))
-                
-    def to_dict(self):
-        return {
-            "bits": self.bits,
-            "group_size": self.group_size,
-            "damp_percent": self.damp_percent,
-            "desc_act": self.desc_act,
-            "sym": self.sym,
-            "true_sequential": self.true_sequential,
-            "model_name_or_path": self.model_name_or_path,
-            "model_file_base_name": self.model_file_base_name,
-        }
-
-
-class BaseGPTQForCausalLM(nn.Module, PushToHubMixin):
-    layer_type: str = None
-    layers_block_name: str = None
-    outside_layer_modules: List[str] = None
-    inside_layer_modules: List[List[str]] = None
-    lm_head_name: str = "lm_head"
-
-    fused_attn_module_type: Optional[FusedBaseAttentionModule] = None
-    fused_mlp_module_type: Optional[FusedBaseMLPModule] = None
-
-    def __init__(self, model: PreTrainedModel, quantized: bool, quantize_config: BaseQuantizeConfig):
-        super().__init__()
-
-        self.model = model
-        self.model_type = self.model.config.model_type
-        self._quantized = quantized
-        self.quantize_config = quantize_config
-        self.config = self.model.config
-
-    @property
-    def quantized(self):
-        return self._quantized
-
-    @property
-    def hf_device_map(self):
-        return getattr(self.model, "hf_device_map", None)
-
-    @staticmethod
-    def _resize_attention_mask(attention_mask: List[torch.LongTensor]):
-        return attention_mask
-
-    @staticmethod
-    def _resize_position_ids(position_ids: List[torch.LongTensor]):
-        return position_ids
-
-    def _prepare_examples_for_quantization(
-        self,
-        examples: List[Dict[str, Union[List[int], torch.LongTensor]]],
-        batch_size: int = 1,
-    ):
-        def _convert_tensor_to_list(tensor):
-            if isinstance(tensor, torch.Tensor):
-                if len(tensor.shape) == 1:
-                    tensor = tensor.unsqueeze(0)
-                tensor = tensor.long()
-                return tensor.cpu().numpy().tolist()
-            return [tensor]
-
-        new_examples = []
-        for example in examples:
-            input_ids = _convert_tensor_to_list(example["input_ids"])
-            attention_mask = _convert_tensor_to_list(example["attention_mask"])
-            if "labels" in example:
-                labels = _convert_tensor_to_list(example["labels"])
-            elif "label" in example:
-                labels = _convert_tensor_to_list(example["label"])
-            elif "label_ids" in example:
-                labels = _convert_tensor_to_list(example["label_ids"])
-            else:
-                labels = copy.deepcopy(input_ids)
-            new_examples.append(
-                {"input_ids": input_ids, "attention_mask": attention_mask, "labels": labels}
-            )
-        pad_token_id = self.config.pad_token_id
-        if not pad_token_id:
-            pad_token_id = self.config.eos_token_id
-
-        new_examples = [
-            collate_data(new_examples[start: start + batch_size], pad_token_id)
-            for start in range(0, len(new_examples), batch_size)
-        ]
-        for new_example in new_examples:
-            del new_example["labels"]
-
-        return new_examples
-
-    @torch.inference_mode()
-    def quantize(
-        self,
-        examples: List[Dict[str, Union[List[int], torch.LongTensor]]],
-        batch_size: int = 1,
-        use_triton: bool = False,
-        use_cuda_fp16: bool = True,
-        autotune_warmup_after_quantized: bool = False,
-        cache_examples_on_gpu: bool = True
-    ):
-        if self.quantized:
-            raise EnvironmentError("can't execute quantize because the model is quantized.")
-        if use_triton and not TRITON_AVAILABLE:
-            logger.warning("triton is not installed, reset use_triton to False")
-            use_triton = False
-
-        device_map = self.hf_device_map
-        if device_map:
-            for name, device in device_map.items():
-                if device == "cpu":
-                    logger.info(f"truly offloading {name} to cpu with hook.")
-                    module = get_module_by_name_suffix(self.model, name)
-                    remove_hook_from_module(module, recurse=True)
-                    accelerate.cpu_offload_with_hook(module, CUDA_0)
-
-        layer_inputs = []
-        attention_masks = []
-        position_ids = []
-        layer_input_kwargs = []
-        layer_outputs = []
-
-        examples = self._prepare_examples_for_quantization(examples, batch_size)
-
-        class LayerHijacker(nn.Module):
-            """hijack layer's forward pass to cache data"""
-
-            def __init__(self, m, device):
-                super().__init__()
-                self.module = m
-                self.data_device = device if cache_examples_on_gpu else CPU
-
-            def forward(self, inp=None, **kwargs):
-                if inp is None:  # some models use all key-value arguments in forward pass call
-                    for kwarg_name in ["hidden_states"]:
-                        if kwarg_name in kwargs:
-                            inp = kwargs[kwarg_name]
-                            break
-                layer_inputs.append(move_to_device(inp, self.data_device))
-                attention_masks.append(kwargs["attention_mask"].to(self.data_device))
-                pos_ids = kwargs.get("position_ids", None)
-                if pos_ids is not None:
-                    position_ids.append(move_to_device(pos_ids, self.data_device))
-                one_kwargs = dict()
-                for k, v in kwargs.items():  # make sure other arguments also be captured
-                    if k not in ["hidden_states", "attention_mask", "position_ids"]:
-                        if isinstance(v, torch.Tensor):
-                            one_kwargs[k] = move_to_device(v, self.data_device)
-                        else:
-                            one_kwargs[k] = v
-                layer_input_kwargs.append(one_kwargs)
-                raise ValueError
-
-        forward_pass_use_cache = self.model.config.use_cache
-        self.model.config.use_cache = False
-
-        num_batches = len(examples)
-        layers = get_module_by_name_prefix(self.model, self.layers_block_name)
-
-        force_layer_back_to_cpu = False
-        if get_device(layers[0]) == CPU:
-            layers[0] = layers[0].to(CUDA_0)
-            force_layer_back_to_cpu = True
-
-        cur_layer_device = get_device(layers[0])
-        ori_outside_layer_module_devices = {}
-        for module_name in self.outside_layer_modules:
-            module = get_module_by_name_prefix(self.model, module_name)
-
-            if module is None:
-                continue
-
-            ori_outside_layer_module_devices[module_name] = get_device(module)
-            if module is not None:
-                move_to_device(module, cur_layer_device)
-
-        # get inputs for first layer
-        layers[0] = LayerHijacker(layers[0], cur_layer_device)
-        for example in examples:
-            for k, v in example.items():
-                if len(v.shape) == 1:
-                    v = v.unsqueeze(0)
-                example[k] = move_to_device(v, cur_layer_device)
-            try:
-                self.model(**example)
-            except ValueError:
-                pass
-        layers[0] = layers[0].module
-
-        move_to_device(layers[0], CPU if force_layer_back_to_cpu else cur_layer_device)
-        for module_name in self.outside_layer_modules:
-            module = get_module_by_name_prefix(self.model, module_name)
-            if module is not None:
-                move_to_device(module, ori_outside_layer_module_devices[module_name])
-
-        torch.cuda.empty_cache()
-
-        # resize attention mask and position ids for some special models
-        attention_masks = self._resize_attention_mask(attention_masks)
-        position_ids = self._resize_position_ids(position_ids)
-
-        inside_layer_modules = self.inside_layer_modules
-        if not self.quantize_config.true_sequential:
-            inside_layer_modules = [sum(inside_layer_modules, [])]
-        quantizers = {}
-        for i in range(len(layers)):
-            logger.info(f"Start quantizing layer {i + 1}/{len(layers)}")
-            layer = layers[i]
-            force_layer_back_to_cpu = False
-            if get_device(layer) == CPU:
-                move_to_device(layer, CUDA_0)
-                force_layer_back_to_cpu = True
-            cur_layer_device = get_device(layer)
-
-            full = find_layers(layer)
-            for names in inside_layer_modules:
-                subset = {n: full[n] for n in names}
-                gptq = {}
-                for name in subset:
-                    gptq[name] = GPTQ(subset[name])
-                    gptq[name].quantizer.configure(
-                        self.quantize_config.bits,
-                        perchannel=True,
-                        sym=self.quantize_config.sym,
-                        mse=False,
-                    )
-
-                def add_batch(name):
-                    def tmp(_, inp, out):
-                        gptq[name].add_batch(inp[0].data, out.data)
-
-                    return tmp
-
-                handles = []
-                for name in subset:
-                    handles.append(subset[name].register_forward_hook(add_batch(name)))
-                for j in range(num_batches):
-                    layer_input = move_to_device(layer_inputs[j], cur_layer_device)
-                    layer_attention_mask = move_to_device(attention_masks[j], cur_layer_device)
-                    additional_layer_inputs = {
-                        "attention_mask": layer_attention_mask
-                    }
-                    layer_position_ids = None if not position_ids else move_to_device(position_ids[j], cur_layer_device)
-                    if layer_position_ids is not None:
-                        additional_layer_inputs["position_ids"] = layer_position_ids
-                    for k, v in layer_input_kwargs[j].items():
-                        if isinstance(v, torch.Tensor):
-                            additional_layer_inputs[k] = move_to_device(v, cur_layer_device)
-                        else:
-                            additional_layer_inputs[k] = v
-                    layer(layer_input, **additional_layer_inputs)
-                for h in handles:
-                    h.remove()
-
-                for name in subset:
-                    logger.info(f'Quantizing {name} in layer {i + 1}/{len(layers)}...')
-                    scale, zero, g_idx = gptq[name].fasterquant(
-                        percdamp=self.quantize_config.damp_percent,
-                        group_size=self.quantize_config.group_size,
-                        actorder=self.quantize_config.desc_act
-                    )
-                    quantizers[f'{self.layers_block_name}.{i}.{name}'] = (
-                        gptq[name].quantizer.to(CPU if force_layer_back_to_cpu else cur_layer_device),
-                        move_to_device(scale, CPU if force_layer_back_to_cpu else cur_layer_device),
-                        move_to_device(zero, CPU if force_layer_back_to_cpu else cur_layer_device),
-                        move_to_device(g_idx, CPU if force_layer_back_to_cpu else cur_layer_device)
-                    )
-                    gptq[name].free()
-
-            for j in range(num_batches):
-                layer_input = move_to_device(layer_inputs[j], cur_layer_device)
-                layer_attention_mask = move_to_device(attention_masks[j], cur_layer_device)
-                additional_layer_inputs = {
-                    "attention_mask": layer_attention_mask
-                }
-                layer_position_ids = None if not position_ids else move_to_device(position_ids[j], cur_layer_device)
-                if layer_position_ids is not None:
-                    additional_layer_inputs["position_ids"] = layer_position_ids
-                for k, v in layer_input_kwargs[j].items():
-                    if isinstance(v, torch.Tensor):
-                        additional_layer_inputs[k] = move_to_device(v, cur_layer_device)
-                    else:
-                        additional_layer_inputs[k] = v
-                layer_output = move_to_device(
-                    layer(layer_input, **additional_layer_inputs)[0],
-                    cur_layer_device if cache_examples_on_gpu else CPU
-                )
-                layer_outputs.append(layer_output)
-
-            layers[i] = move_to_device(layer, CPU if force_layer_back_to_cpu else cur_layer_device)
-            del layer
-            del gptq
-            del layer_inputs
-            layer_inputs, layer_outputs = layer_outputs, []
-            torch.cuda.empty_cache()
-
-        pack_model(
-            model=self.model,
-            quantizers=quantizers,
-            bits=self.quantize_config.bits,
-            group_size=self.quantize_config.group_size,
-            use_triton=use_triton,
-            use_cuda_fp16=use_cuda_fp16,
-            desc_act=self.quantize_config.desc_act,
-            warmup_triton=autotune_warmup_after_quantized,
-            force_layer_back_to_cpu=force_layer_back_to_cpu
-        )
-        if device_map:
-            self.model = remove_hook_from_module(self.model, recurse=True)
-            self.model = simple_dispatch_model(self.model, device_map)
-        self.model.config.use_cache = forward_pass_use_cache
-
-        self._quantized = True
-
-        torch.cuda.empty_cache()
-
-    @property
-    def device(self):
-        if not self.hf_device_map:
-            return self.model.device
-        else:
-            device = [d for d in self.hf_device_map.values() if d not in {'cpu', 'disk'}][0]
-            return torch.device(device)
-
-    def to(self, device: Union[str, torch.device]):
-        return self.model.to(device)
-
-    def forward(self, *args, **kwargs):
-        return self.model(*args, **kwargs)
-
-    def generate(self, **kwargs):
-        """shortcut for model.generate"""
-        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
-            return self.model.generate(**kwargs)
-
-    def prepare_inputs_for_generation(self, *args, **kwargs):
-        """shortcut for model.prepare_inputs_for_generation"""
-        return self.model.prepare_inputs_for_generation(*args, **kwargs)
-
-    def push_to_hub(
-        self,
-        repo_id: str,
-        save_dir: Optional[str] = None,
-        use_safetensors: Optional[bool] = True,
-        commit_message: Optional[str] = "Upload of AutoGPTQ quantized model",
-        use_auth_token: Optional[Union[bool, str]] = None,
-        private: Optional[bool] = None,
-        token: Optional[Union[bool, str]] = None,
-        create_pr: Optional[bool] = False,
-    ) -> str:
-        """
-        Upload the model to the Hugging Face Hub.
-
-        Parameters:
-            repo_id (`str`):
-                The name of the repository you want to push your tool to. It should contain your organization name when
-                pushing to a given organization.
-            save_dir (`str`, *optional*):
-                The name of the local folder to save the model to.
-                If the model has already been saved, this parameter can be omitted.
-            use_safetensors (`bool`, *optional*):
-                Save the model using `safetensors`.
-                If the model has already been saved, this parameter can be omitted.
-            commit_message (`str`, *optional*, defaults to `"Upload tool"`):
-                Message to commit while pushing.
-            use_auth_token (`bool` or `str`, *optional*):
-                The token to use as HTTP bearer authorization for remote files. If `True`, will use the token generated
-                when running `huggingface-cli login` (stored in `~/.huggingface`). Will default to `True` if `repo_url`
-                is not specified.
-            private (`bool`, *optional*):
-                Whether or not the repository created should be private.
-            token (`bool` or `str`, *optional*):
-                The token to use as HTTP bearer authorization for remote files. If unset, will use the token generated
-                when running `huggingface-cli login` (stored in `~/.huggingface`).
-            create_pr (`bool`, *optional*, defaults to `False`):
-                Whether or not to create a PR with the uploaded files or directly commit.
-        """
-        if (self.quantize_config.model_name_or_path is None or not isdir(self.quantize_config.model_name_or_path)) and save_dir is None:
-            raise ValueError("Quantized model should be saved first, or you can provide save_dir to make sure model is saved to local disk before uploading.")
-        
-        if save_dir is not None:
-            logger.info(f"Saving model to {save_dir}")
-            self.save_quantized(save_dir, use_safetensors)
-
-        repo_url = create_repo(
-            repo_id=repo_id, token=token, private=private, exist_ok=True, repo_type="model"
-        )
-        repo_id = repo_url.repo_id
-
-        if self.quantize_config.model_name_or_path is not None:
-            work_dir = self.quantize_config.model_name_or_path
-            operations = [
-                CommitOperationAdd(path_or_fileobj=join(work_dir, f), path_in_repo=f)
-                for f in os.listdir(work_dir)
-            ]
-            logger.info(f"Uploading the following files to {repo_id}: {','.join(os.listdir(work_dir))}")
-            return create_commit(
-                repo_id=repo_id,
-                operations=operations,
-                commit_message=commit_message,
-                token=use_auth_token,
-                create_pr=create_pr,
-                repo_type="model",
-            )
-
-    def save_quantized(self, save_dir: str, use_safetensors: bool = False):
-        """save quantized model and configs to local disk"""
-        os.makedirs(save_dir, exist_ok=True)
-
-        if not self.quantized:
-            raise EnvironmentError("can only save quantized model, please execute .quantize first.")
-
-        self.model.to(CPU)
-
-        model_base_name = self.quantize_config.model_file_base_name or f"gptq_model-{self.quantize_config.bits}bit-{self.quantize_config.group_size}g"
-        if use_safetensors:
-            model_save_name = model_base_name + ".safetensors"
-            state_dict = self.model.state_dict()
-            state_dict = {k: v.clone().contiguous() for k, v in state_dict.items()}
-            safe_save(state_dict, join(save_dir, model_save_name))
-        else:
-            model_save_name = model_base_name + ".bin"
-            torch.save(self.model.state_dict(), join(save_dir, model_save_name))
-
-        self.model.config.save_pretrained(save_dir)
-        self.quantize_config.save_pretrained(save_dir)
-        self.quantize_config.model_name_or_path = save_dir
-        self.quantize_config.model_file_base_name = model_base_name
-
-    def save_pretrained(self, save_dir: str, use_safetensors: bool = False, **kwargs):
-        """alias of save_quantized"""
-        logger.warning("you are using save_pretrained, which will re-direct to save_quantized.")
-        self.save_quantized(save_dir, use_safetensors)
-
-    @classmethod
-    def from_pretrained(
-        cls,
-        pretrained_model_name_or_path: str,
-        quantize_config: BaseQuantizeConfig,
-        max_memory: Optional[dict] = None,
-        trust_remote_code: bool = False,
-        torch_dtype: torch.dtype = torch.float16,
-        **model_init_kwargs
-    ):
-        """load un-quantized pretrained model to cpu"""
-
-        if not torch.cuda.is_available():
-            raise EnvironmentError("Load pretrained model to do quantization requires CUDA available.")
-
-        def skip(*args, **kwargs):
-            pass
-
-        torch.nn.init.kaiming_uniform_ = skip
-        torch.nn.init.uniform_ = skip
-        torch.nn.init.normal_ = skip
-
-        config = AutoConfig.from_pretrained(pretrained_model_name_or_path, trust_remote_code=True)
-        if config.model_type not in SUPPORTED_MODELS:
-            raise TypeError(f"{config.model_type} isn't supported yet.")
-
-        # enforce some values despite user specified
-        model_init_kwargs["torch_dtype"] = torch_dtype
-        model_init_kwargs["trust_remote_code"] = trust_remote_code
-        if max_memory:
-            if "disk" in max_memory:
-                raise NotImplementedError("disk offload not support yet.")
-            with accelerate.init_empty_weights():
-                model = AutoModelForCausalLM.from_config(config, trust_remote_code=True)
-            model.tie_weights()
-
-            max_memory = accelerate.utils.get_balanced_memory(
-                model,
-                max_memory=max_memory,
-                no_split_module_classes=[cls.layer_type],
-                dtype=model_init_kwargs["torch_dtype"],
-                low_zero=False
-            )
-            model_init_kwargs["device_map"] = accelerate.infer_auto_device_map(
-                model,
-                max_memory=max_memory,
-                no_split_module_classes=[cls.layer_type],
-                dtype=model_init_kwargs["torch_dtype"]
-            )
-            model_init_kwargs["low_cpu_mem_usage"] = True
-
-            del model
-        else:
-            model_init_kwargs["device_map"] = None
-            model_init_kwargs["low_cpu_mem_usage"] = False
-
-        torch.cuda.empty_cache()
-
-        model = AutoModelForCausalLM.from_pretrained(pretrained_model_name_or_path, **model_init_kwargs)
-        model_config = model.config.to_dict()
-        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
-        if any([k in model_config for k in seq_len_keys]):
-            for key in seq_len_keys:
-                if key in model_config:
-                    model.seqlen = model_config[key]
-                    break
-        else:
-            logger.warning("can't get model's sequence length from model config, will set to 4096.")
-            model.seqlen = 4096
-        model.eval()
-
-        return cls(model, False, quantize_config)
-
-    @classmethod
-    def from_quantized(
-        cls,
-        model_name_or_path: Optional[str] = None,
-        save_dir: Optional[str] = None,
-        device_map: Optional[Union[str, Dict[str, Union[int, str]]]] = None,
-        max_memory: Optional[dict] = None,
-        device: Optional[Union[str, int]] = None,
-        low_cpu_mem_usage: bool = False,
-        use_triton: bool = False,
-        torch_dtype: torch.dtype = torch.float16,
-        inject_fused_attention: bool = True,
-        inject_fused_mlp: bool = True,
-        use_cuda_fp16: bool = True,
-        quantize_config: Optional[BaseQuantizeConfig] = None,
-        model_basename: Optional[str] = None,
-        use_safetensors: bool = False,
-        trust_remote_code: bool = False,
-        warmup_triton: bool = False,
-        **kwargs
-    ):
-        """load quantized model from local disk"""
-       
-        # Parameters related to loading from Hugging Face Hub
-        cache_dir = kwargs.pop("cache_dir", None)
-        force_download = kwargs.pop("force_download", False)
-        resume_download = kwargs.pop("resume_download", False)
-        proxies = kwargs.pop("proxies", None)
-        local_files_only = kwargs.pop("local_files_only", False)
-        use_auth_token = kwargs.pop("use_auth_token", None)
-        revision = kwargs.pop("revision", None)
-        subfolder = kwargs.pop("subfolder", "")
-        commit_hash = kwargs.pop("_commit_hash", None)
-
-        if use_triton and not TRITON_AVAILABLE:
-            logger.warning("triton is not installed, reset use_triton to False")
-            use_triton = False
-
-        # == step1: prepare configs and file names == #
-        if model_name_or_path and save_dir:
-            logger.warning("save_dir will be ignored because model_name_or_path is explicit specified.")
-        if not model_name_or_path and save_dir:
-            model_name_or_path = save_dir
-            warnings.warn("save_dir is deprecated and will be removed in version 0.3.0", PendingDeprecationWarning, stacklevel=2)
-        if not model_name_or_path and not save_dir:
-            raise ValueError("at least one of model_name_or_path or save_dir should be specified.")
-        
-        config = AutoConfig.from_pretrained(model_name_or_path, trust_remote_code=trust_remote_code)
-
-        if config.model_type not in SUPPORTED_MODELS:
-            raise TypeError(f"{config.model_type} isn't supported yet.")
-
-        if quantize_config is None:
-            quantize_config = BaseQuantizeConfig.from_pretrained(model_name_or_path, **kwargs)
-        
-        if model_basename is None:
-            if quantize_config.model_file_base_name:
-                model_basename = quantize_config.model_file_base_name
-            else:
-                model_basename = f"gptq_model-{quantize_config.bits}bit-{quantize_config.group_size}g"
-        
-        quantize_config.model_name_or_path = model_name_or_path
-        quantize_config.model_file_base_name = model_basename
-
-        extensions = []
-        if use_safetensors:
-            extensions.append(".safetensors")
-        else:
-            extensions += [".bin", ".pt"]
-
-        model_name_or_path = str(model_name_or_path)
-        is_local = isdir(model_name_or_path)
-
-        resolved_archive_file = None
-        if is_local:
-            model_save_name = join(model_name_or_path, model_basename)
-
-            for ext in extensions:
-                if isfile(model_save_name + ext):
-                    resolved_archive_file = model_save_name + ext
-                    break
-        else: # remote
-            cached_file_kwargs = {
-                "cache_dir": cache_dir,
-                "force_download": force_download,
-                "proxies": proxies,
-                "resume_download": resume_download,
-                "local_files_only": local_files_only,
-                "use_auth_token": use_auth_token,
-                "revision": revision,
-                "subfolder": subfolder,
-                "_raise_exceptions_for_missing_entries": False,
-                "_commit_hash": commit_hash,
-            }
-            
-            for ext in extensions:
-                resolved_archive_file = cached_file(model_name_or_path, model_basename + ext, **cached_file_kwargs)
-                if resolved_archive_file is not None:
-                    break
-        
-        if resolved_archive_file is None: # Could not find a model file to use
-            raise FileNotFoundError(f"Could not find model in {model_name_or_path}")
-                
-        model_save_name = resolved_archive_file
-
-        # == step2: convert model to gptq-model (replace Linear with QuantLinear) == #
-        def skip(*args, **kwargs):
-            pass
-
-        torch.nn.init.kaiming_uniform_ = skip
-        torch.nn.init.uniform_ = skip
-        torch.nn.init.normal_ = skip
-
-        transformers.modeling_utils._init_weights = False
-
-        init_contexts = [no_init_weights()]
-        if low_cpu_mem_usage:
-            init_contexts.append(accelerate.init_empty_weights(include_buffers=False))
-
-        with ContextManagers(init_contexts):
-            model = AutoModelForCausalLM.from_config(
-                config,
-                trust_remote_code=trust_remote_code,
-                torch_dtype=torch_dtype
-            )
-
-            layers = find_layers(model)
-            ignore_layers = [cls.lm_head_name] + cls.outside_layer_modules
-            for name in list(layers.keys()):
-                if any([name.startswith(ignore_layer) for ignore_layer in ignore_layers]):
-                    logger.info(f"{name} not been quantized, will be ignored when make_quant.")
-                    del layers[name]
-
-            make_quant(
-                model,
-                layers,
-                quantize_config.bits,
-                quantize_config.group_size,
-                use_triton=use_triton,
-                use_cuda_fp16=use_cuda_fp16,
-                desc_act=quantize_config.desc_act
-            )
-            model.tie_weights()
-
-        # == step3: load checkpoint and dispatch == #
-        if isinstance(device_map, str) and device_map not in ["auto", "balanced", "balanced_low_0", "sequential"]:
-            raise ValueError(
-                "If passing a string for `device_map`, please choose 'auto', 'balanced', 'balanced_low_0' or "
-                "'sequential'."
-            )
-        if isinstance(device_map, dict):
-            max_memory = None
-        else:
-            if device is None and not device_map and not max_memory:
-                device_map = "auto"
-            if device is not None:
-                device = torch.device(device)
-                if not max_memory and not device_map:
-                    device_map = {"": device.index if device.type == "cuda" else device.type}
-            if not isinstance(device_map, dict) and device_map != "sequential":
-                max_memory = accelerate.utils.get_balanced_memory(
-                    model=model,
-                    max_memory=max_memory,
-                    no_split_module_classes=[cls.layer_type],
-                    low_zero=(device_map == "balanced_low_0")
-                )
-        if not isinstance(device_map, dict):
-            device_map = accelerate.infer_auto_device_map(
-                model,
-                max_memory=max_memory,
-                no_split_module_classes=[cls.layer_type]
-            )
-
-        if low_cpu_mem_usage:
-            make_sure_no_tensor_in_meta_device(model, use_triton, quantize_config.desc_act, quantize_config.group_size)
-
-        accelerate.utils.modeling.load_checkpoint_in_model(
-            model,
-            checkpoint=model_save_name,
-            device_map=device_map,
-            offload_state_dict=True,
-            offload_buffers=True
-        )
-        model = simple_dispatch_model(model, device_map)
-
-        # == step4: set seqlen == #
-        model_config = model.config.to_dict()
-        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
-        if any([k in model_config for k in seq_len_keys]):
-            for key in seq_len_keys:
-                if key in model_config:
-                    model.seqlen = model_config[key]
-                    break
-        else:
-            logger.warning("can't get model's sequence length from model config, will set to 4096.")
-            model.seqlen = 4096
-
-        # == step5: (optional) inject optimized module == #
-        if inject_fused_attention:
-            if cls.fused_attn_module_type is None:
-                logger.warning(f"{cls.__name__} hasn't fused attention module yet, will skip inject fused attention.")
-            else:
-                cls.fused_attn_module_type.inject_to_model(
-                    model,
-                    use_triton=use_triton,
-                    group_size=quantize_config.group_size,
-                    use_cuda_fp16=use_cuda_fp16,
-                    desc_act=quantize_config.desc_act
-                )
-        if inject_fused_mlp:
-            if cls.fused_mlp_module_type is None:
-                logger.warning(f"{cls.__name__} hasn't fused mlp module yet, will skip inject fused mlp.")
-            else:
-                cls.fused_mlp_module_type.inject_to_model(
-                    model,
-                    use_triton=use_triton
-                )
-
-        model.eval()
-        # == step6: (optional) warmup triton == #
-        if use_triton and warmup_triton:
-            from ..nn_modules.qlinear_triton import QuantLinear
-            QuantLinear.warmup(model, seqlen=model.seqlen)
-
-            if inject_fused_mlp and cls.fused_mlp_module_type is not None:
-                cls.fused_mlp_module_type.warmup(model, seqlen=model.seqlen)
-
-        return cls(model, True, quantize_config)
-
-    def warmup_triton(self, enabled: bool = True):
-        if not enabled:
-            return
-        if not TRITON_AVAILABLE:
-            logger.warning(f"triton is not available, skip warmup stage directly.")
-            return
-
-        from ..nn_modules.qlinear_triton import QuantLinear
-        QuantLinear.warmup(self.model, seqlen=self.model.seqlen)
-
-        if self.fused_mlp_module_type is not None:
-            self.fused_mlp_module_type.warmup(self.model, seqlen=self.model.seqlen)
-
-
-__all__ = ["BaseGPTQForCausalLM", "BaseQuantizeConfig"]
+import copy
+import json
+import warnings
+import os
+from dataclasses import dataclass, field, fields
+from logging import getLogger
+from os.path import join, isfile, isdir
+from typing import Dict, List, Optional, Union
+
+import accelerate
+import torch
+import torch.nn as nn
+import transformers
+from accelerate.hooks import remove_hook_from_module
+from safetensors.torch import save_file as safe_save
+from transformers import AutoConfig, AutoModelForCausalLM, PreTrainedModel
+from transformers.utils.hub import PushToHubMixin, cached_file, create_repo, create_commit, CommitOperationAdd
+from transformers.utils.generic import ContextManagers
+from transformers.modeling_utils import no_init_weights
+
+from ._const import *
+from ._utils import *
+from ..nn_modules.qlinear import GeneralQuantLinear
+from ..nn_modules._fused_base import FusedBaseAttentionModule, FusedBaseMLPModule
+from ..quantization import GPTQ
+from ..utils.data_utils import collate_data
+from ..utils.import_utils import dynamically_import_QuantLinear, TRITON_AVAILABLE, AUTOGPTQ_CUDA_AVAILABLE
+
+logger = getLogger(__name__)
+
+
+@dataclass
+class BaseQuantizeConfig(PushToHubMixin):
+    bits: int = field(default=4, metadata={"choices": [2, 3, 4, 8]})
+    group_size: int = field(default=-1)
+    damp_percent: float = field(default=0.01)
+    desc_act: bool = field(default=True)
+    sym: bool = field(default=True)
+    true_sequential: bool = field(default=True)
+    model_name_or_path: Optional[str] = field(default=None)
+    model_file_base_name: Optional[str] = field(default=None)
+
+    def __post_init__(self):
+        fields_info = fields(self)
+
+        if self.bits not in fields_info[0].metadata["choices"]:
+            raise ValueError(f"only support quantize to {fields_info[0].metadata['choices']} bits.")
+        if self.group_size != -1 and self.group_size <= 0:
+            raise ValueError("unless equal to -1, group_size must greater then 0.")
+        if not (0 < self.damp_percent < 1):
+            raise ValueError("damp_percent must between 0 and 1.")
+
+    def save_pretrained(self, save_dir: str, **kwargs):
+        with open(join(save_dir, "quantize_config.json"), "w", encoding="utf-8") as f:
+            json.dump(self.to_dict(), f, indent=2)
+
+    @classmethod
+    def from_pretrained(cls, save_dir: str, **kwargs):
+        # Parameters related to loading from Hugging Face Hub
+        cache_dir = kwargs.pop("cache_dir", None)
+        force_download = kwargs.pop("force_download", False)
+        resume_download = kwargs.pop("resume_download", False)
+        proxies = kwargs.pop("proxies", None)
+        local_files_only = kwargs.pop("local_files_only", False)
+        use_auth_token = kwargs.pop("use_auth_token", None)
+        revision = kwargs.pop("revision", None)
+        subfolder = kwargs.pop("subfolder", None)
+        commit_hash = kwargs.pop("_commit_hash", None)
+
+        quantize_config_filename = "quantize_config.json"
+        if os.path.isdir(save_dir):  # Local
+            resolved_config_file = join(save_dir, quantize_config_filename)
+        else: # Remote
+               resolved_config_file = cached_file(
+                    save_dir,
+                    quantize_config_filename,
+                    cache_dir=cache_dir,
+                    force_download=force_download,
+                    resume_download=resume_download,
+                    proxies=proxies,
+                    use_auth_token=use_auth_token,
+                    revision=revision,
+                    local_files_only=local_files_only,
+                    subfolder=subfolder,
+                    _raise_exceptions_for_missing_entries=False,
+                    _raise_exceptions_for_connection_errors=False,
+                    _commit_hash=commit_hash,
+               )
+
+        with open(resolved_config_file, "r", encoding="utf-8") as f:
+            return cls(**json.load(f))
+                
+    def to_dict(self):
+        return {
+            "bits": self.bits,
+            "group_size": self.group_size,
+            "damp_percent": self.damp_percent,
+            "desc_act": self.desc_act,
+            "sym": self.sym,
+            "true_sequential": self.true_sequential,
+            "model_name_or_path": self.model_name_or_path,
+            "model_file_base_name": self.model_file_base_name,
+        }
+
+
+class BaseGPTQForCausalLM(nn.Module, PushToHubMixin):
+    layer_type: str = None
+    layers_block_name: str = None
+    outside_layer_modules: List[str] = None
+    inside_layer_modules: List[List[str]] = None
+    lm_head_name: str = "lm_head"
+
+    fused_attn_module_type: Optional[FusedBaseAttentionModule] = None
+    fused_mlp_module_type: Optional[FusedBaseMLPModule] = None
+
+    def __init__(
+        self,
+        model: PreTrainedModel,
+        quantized: bool,
+        quantize_config: BaseQuantizeConfig,
+        is_triton_backend: bool = False,
+        injected_fused_attention: bool = False,
+        injected_fused_mlp: bool = False,
+        trainable: bool = False
+    ):
+        super().__init__()
+
+        self.model = model
+        self.model_type = self.model.config.model_type
+        self._quantized = quantized
+        self.quantize_config = quantize_config
+        self.config = self.model.config
+
+        self.is_triton_backend = is_triton_backend
+        self.injected_fused_attention = injected_fused_attention
+        self.injected_fused_mlp = injected_fused_mlp
+        self.trainable = trainable
+
+    @property
+    def quantized(self):
+        return self._quantized
+
+    @property
+    def hf_device_map(self):
+        return getattr(self.model, "hf_device_map", None)
+
+    @staticmethod
+    def _resize_attention_mask(attention_mask: List[torch.LongTensor]):
+        return attention_mask
+
+    @staticmethod
+    def _resize_position_ids(position_ids: List[torch.LongTensor]):
+        return position_ids
+
+    def _prepare_examples_for_quantization(
+        self,
+        examples: List[Dict[str, Union[List[int], torch.LongTensor]]],
+        batch_size: int = 1,
+    ):
+        def _convert_tensor_to_list(tensor):
+            if isinstance(tensor, torch.Tensor):
+                if len(tensor.shape) == 1:
+                    tensor = tensor.unsqueeze(0)
+                tensor = tensor.long()
+                return tensor.cpu().numpy().tolist()
+            return [tensor]
+
+        new_examples = []
+        for example in examples:
+            input_ids = _convert_tensor_to_list(example["input_ids"])
+            attention_mask = _convert_tensor_to_list(example["attention_mask"])
+            if "labels" in example:
+                labels = _convert_tensor_to_list(example["labels"])
+            elif "label" in example:
+                labels = _convert_tensor_to_list(example["label"])
+            elif "label_ids" in example:
+                labels = _convert_tensor_to_list(example["label_ids"])
+            else:
+                labels = copy.deepcopy(input_ids)
+            new_examples.append(
+                {"input_ids": input_ids, "attention_mask": attention_mask, "labels": labels}
+            )
+        pad_token_id = self.config.pad_token_id
+        if not pad_token_id:
+            pad_token_id = self.config.eos_token_id
+
+        new_examples = [
+            collate_data(new_examples[start: start + batch_size], pad_token_id)
+            for start in range(0, len(new_examples), batch_size)
+        ]
+        for new_example in new_examples:
+            del new_example["labels"]
+
+        return new_examples
+
+    @torch.inference_mode()
+    def quantize(
+        self,
+        examples: List[Dict[str, Union[List[int], torch.LongTensor]]],
+        batch_size: int = 1,
+        use_triton: bool = False,
+        use_cuda_fp16: bool = True,
+        autotune_warmup_after_quantized: bool = False,
+        cache_examples_on_gpu: bool = True
+    ):
+        if self.quantized:
+            raise EnvironmentError("can't execute quantize because the model is quantized.")
+        if use_triton and not TRITON_AVAILABLE:
+            logger.warning("triton is not installed, reset use_triton to False")
+            use_triton = False
+
+        device_map = self.hf_device_map
+        if device_map:
+            for name, device in device_map.items():
+                if device == "cpu":
+                    logger.info(f"truly offloading {name} to cpu with hook.")
+                    module = get_module_by_name_suffix(self.model, name)
+                    remove_hook_from_module(module, recurse=True)
+                    accelerate.cpu_offload_with_hook(module, CUDA_0)
+
+        layer_inputs = []
+        attention_masks = []
+        position_ids = []
+        layer_input_kwargs = []
+        layer_outputs = []
+
+        examples = self._prepare_examples_for_quantization(examples, batch_size)
+
+        class LayerHijacker(nn.Module):
+            """hijack layer's forward pass to cache data"""
+
+            def __init__(self, m, device):
+                super().__init__()
+                self.module = m
+                self.data_device = device if cache_examples_on_gpu else CPU
+
+            def forward(self, inp=None, **kwargs):
+                if inp is None:  # some models use all key-value arguments in forward pass call
+                    for kwarg_name in ["hidden_states"]:
+                        if kwarg_name in kwargs:
+                            inp = kwargs[kwarg_name]
+                            break
+                layer_inputs.append(move_to_device(inp, self.data_device))
+                attention_masks.append(kwargs["attention_mask"].to(self.data_device))
+                pos_ids = kwargs.get("position_ids", None)
+                if pos_ids is not None:
+                    position_ids.append(move_to_device(pos_ids, self.data_device))
+                one_kwargs = dict()
+                for k, v in kwargs.items():  # make sure other arguments also be captured
+                    if k not in ["hidden_states", "attention_mask", "position_ids"]:
+                        if isinstance(v, torch.Tensor):
+                            one_kwargs[k] = move_to_device(v, self.data_device)
+                        else:
+                            one_kwargs[k] = v
+                layer_input_kwargs.append(one_kwargs)
+                raise ValueError
+
+        forward_pass_use_cache = self.model.config.use_cache
+        self.model.config.use_cache = False
+
+        num_batches = len(examples)
+        layers = get_module_by_name_prefix(self.model, self.layers_block_name)
+
+        force_layer_back_to_cpu = False
+        if get_device(layers[0]) == CPU:
+            layers[0] = layers[0].to(CUDA_0)
+            force_layer_back_to_cpu = True
+
+        cur_layer_device = get_device(layers[0])
+        ori_outside_layer_module_devices = {}
+        for module_name in self.outside_layer_modules:
+            module = get_module_by_name_prefix(self.model, module_name)
+
+            if module is None:
+                continue
+
+            ori_outside_layer_module_devices[module_name] = get_device(module)
+            if module is not None:
+                move_to_device(module, cur_layer_device)
+
+        # get inputs for first layer
+        layers[0] = LayerHijacker(layers[0], cur_layer_device)
+        for example in examples:
+            for k, v in example.items():
+                if len(v.shape) == 1:
+                    v = v.unsqueeze(0)
+                example[k] = move_to_device(v, cur_layer_device)
+            try:
+                self.model(**example)
+            except ValueError:
+                pass
+        layers[0] = layers[0].module
+
+        move_to_device(layers[0], CPU if force_layer_back_to_cpu else cur_layer_device)
+        for module_name in self.outside_layer_modules:
+            module = get_module_by_name_prefix(self.model, module_name)
+            if module is not None:
+                move_to_device(module, ori_outside_layer_module_devices[module_name])
+
+        torch.cuda.empty_cache()
+
+        # resize attention mask and position ids for some special models
+        attention_masks = self._resize_attention_mask(attention_masks)
+        position_ids = self._resize_position_ids(position_ids)
+
+        inside_layer_modules = self.inside_layer_modules
+        if not self.quantize_config.true_sequential:
+            inside_layer_modules = [sum(inside_layer_modules, [])]
+        quantizers = {}
+        for i in range(len(layers)):
+            logger.info(f"Start quantizing layer {i + 1}/{len(layers)}")
+            layer = layers[i]
+            force_layer_back_to_cpu = False
+            if get_device(layer) == CPU:
+                move_to_device(layer, CUDA_0)
+                force_layer_back_to_cpu = True
+            cur_layer_device = get_device(layer)
+
+            full = find_layers(layer)
+            for names in inside_layer_modules:
+                subset = {n: full[n] for n in names}
+                gptq = {}
+                for name in subset:
+                    gptq[name] = GPTQ(subset[name])
+                    gptq[name].quantizer.configure(
+                        self.quantize_config.bits,
+                        perchannel=True,
+                        sym=self.quantize_config.sym,
+                        mse=False,
+                    )
+
+                def add_batch(name):
+                    def tmp(_, inp, out):
+                        gptq[name].add_batch(inp[0].data, out.data)
+
+                    return tmp
+
+                handles = []
+                for name in subset:
+                    handles.append(subset[name].register_forward_hook(add_batch(name)))
+                for j in range(num_batches):
+                    layer_input = move_to_device(layer_inputs[j], cur_layer_device)
+                    layer_attention_mask = move_to_device(attention_masks[j], cur_layer_device)
+                    additional_layer_inputs = {
+                        "attention_mask": layer_attention_mask
+                    }
+                    layer_position_ids = None if not position_ids else move_to_device(position_ids[j], cur_layer_device)
+                    if layer_position_ids is not None:
+                        additional_layer_inputs["position_ids"] = layer_position_ids
+                    for k, v in layer_input_kwargs[j].items():
+                        if isinstance(v, torch.Tensor):
+                            additional_layer_inputs[k] = move_to_device(v, cur_layer_device)
+                        else:
+                            additional_layer_inputs[k] = v
+                    layer(layer_input, **additional_layer_inputs)
+                for h in handles:
+                    h.remove()
+
+                for name in subset:
+                    logger.info(f'Quantizing {name} in layer {i + 1}/{len(layers)}...')
+                    scale, zero, g_idx = gptq[name].fasterquant(
+                        percdamp=self.quantize_config.damp_percent,
+                        group_size=self.quantize_config.group_size,
+                        actorder=self.quantize_config.desc_act
+                    )
+                    quantizers[f'{self.layers_block_name}.{i}.{name}'] = (
+                        gptq[name].quantizer.to(CPU if force_layer_back_to_cpu else cur_layer_device),
+                        move_to_device(scale, CPU if force_layer_back_to_cpu else cur_layer_device),
+                        move_to_device(zero, CPU if force_layer_back_to_cpu else cur_layer_device),
+                        move_to_device(g_idx, CPU if force_layer_back_to_cpu else cur_layer_device)
+                    )
+                    gptq[name].free()
+
+            for j in range(num_batches):
+                layer_input = move_to_device(layer_inputs[j], cur_layer_device)
+                layer_attention_mask = move_to_device(attention_masks[j], cur_layer_device)
+                additional_layer_inputs = {
+                    "attention_mask": layer_attention_mask
+                }
+                layer_position_ids = None if not position_ids else move_to_device(position_ids[j], cur_layer_device)
+                if layer_position_ids is not None:
+                    additional_layer_inputs["position_ids"] = layer_position_ids
+                for k, v in layer_input_kwargs[j].items():
+                    if isinstance(v, torch.Tensor):
+                        additional_layer_inputs[k] = move_to_device(v, cur_layer_device)
+                    else:
+                        additional_layer_inputs[k] = v
+                layer_output = move_to_device(
+                    layer(layer_input, **additional_layer_inputs)[0],
+                    cur_layer_device if cache_examples_on_gpu else CPU
+                )
+                layer_outputs.append(layer_output)
+
+            layers[i] = move_to_device(layer, CPU if force_layer_back_to_cpu else cur_layer_device)
+            del layer
+            del gptq
+            del layer_inputs
+            layer_inputs, layer_outputs = layer_outputs, []
+            torch.cuda.empty_cache()
+
+        pack_model(
+            model=self.model,
+            quantizers=quantizers,
+            bits=self.quantize_config.bits,
+            group_size=self.quantize_config.group_size,
+            use_triton=use_triton,
+            use_cuda_fp16=use_cuda_fp16,
+            desc_act=self.quantize_config.desc_act,
+            warmup_triton=autotune_warmup_after_quantized,
+            force_layer_back_to_cpu=force_layer_back_to_cpu
+        )
+        if device_map:
+            self.model = remove_hook_from_module(self.model, recurse=True)
+            self.model = simple_dispatch_model(self.model, device_map)
+        self.model.config.use_cache = forward_pass_use_cache
+
+        self._quantized = True
+
+        torch.cuda.empty_cache()
+
+    @property
+    def device(self):
+        if not self.hf_device_map:
+            return self.model.device
+        else:
+            device = [d for d in self.hf_device_map.values() if d not in {'cpu', 'disk'}][0]
+            return torch.device(device)
+
+    def to(self, device: Union[str, torch.device]):
+        return self.model.to(device)
+
+    def forward(self, *args, **kwargs):
+        return self.model(*args, **kwargs)
+
+    def generate(self, **kwargs):
+        """shortcut for model.generate"""
+        with torch.inference_mode(), torch.amp.autocast(device_type=self.device.type):
+            return self.model.generate(**kwargs)
+
+    def prepare_inputs_for_generation(self, *args, **kwargs):
+        """shortcut for model.prepare_inputs_for_generation"""
+        return self.model.prepare_inputs_for_generation(*args, **kwargs)
+
+    def push_to_hub(
+        self,
+        repo_id: str,
+        save_dir: Optional[str] = None,
+        use_safetensors: Optional[bool] = True,
+        commit_message: Optional[str] = "Upload of AutoGPTQ quantized model",
+        use_auth_token: Optional[Union[bool, str]] = None,
+        private: Optional[bool] = None,
+        token: Optional[Union[bool, str]] = None,
+        create_pr: Optional[bool] = False,
+    ) -> str:
+        """
+        Upload the model to the Hugging Face Hub.
+
+        Parameters:
+            repo_id (`str`):
+                The name of the repository you want to push your tool to. It should contain your organization name when
+                pushing to a given organization.
+            save_dir (`str`, *optional*):
+                The name of the local folder to save the model to.
+                If the model has already been saved, this parameter can be omitted.
+            use_safetensors (`bool`, *optional*):
+                Save the model using `safetensors`.
+                If the model has already been saved, this parameter can be omitted.
+            commit_message (`str`, *optional*, defaults to `"Upload tool"`):
+                Message to commit while pushing.
+            use_auth_token (`bool` or `str`, *optional*):
+                The token to use as HTTP bearer authorization for remote files. If `True`, will use the token generated
+                when running `huggingface-cli login` (stored in `~/.huggingface`). Will default to `True` if `repo_url`
+                is not specified.
+            private (`bool`, *optional*):
+                Whether or not the repository created should be private.
+            token (`bool` or `str`, *optional*):
+                The token to use as HTTP bearer authorization for remote files. If unset, will use the token generated
+                when running `huggingface-cli login` (stored in `~/.huggingface`).
+            create_pr (`bool`, *optional*, defaults to `False`):
+                Whether or not to create a PR with the uploaded files or directly commit.
+        """
+        if (self.quantize_config.model_name_or_path is None or not isdir(self.quantize_config.model_name_or_path)) and save_dir is None:
+            raise ValueError("Quantized model should be saved first, or you can provide save_dir to make sure model is saved to local disk before uploading.")
+        
+        if save_dir is not None:
+            logger.info(f"Saving model to {save_dir}")
+            self.save_quantized(save_dir, use_safetensors)
+
+        repo_url = create_repo(
+            repo_id=repo_id, token=token, private=private, exist_ok=True, repo_type="model"
+        )
+        repo_id = repo_url.repo_id
+
+        if self.quantize_config.model_name_or_path is not None:
+            work_dir = self.quantize_config.model_name_or_path
+            operations = [
+                CommitOperationAdd(path_or_fileobj=join(work_dir, f), path_in_repo=f)
+                for f in os.listdir(work_dir)
+            ]
+            logger.info(f"Uploading the following files to {repo_id}: {','.join(os.listdir(work_dir))}")
+            return create_commit(
+                repo_id=repo_id,
+                operations=operations,
+                commit_message=commit_message,
+                token=use_auth_token,
+                create_pr=create_pr,
+                repo_type="model",
+            )
+
+    def save_quantized(self, save_dir: str, use_safetensors: bool = False):
+        """save quantized model and configs to local disk"""
+        os.makedirs(save_dir, exist_ok=True)
+
+        if not self.quantized:
+            raise EnvironmentError("can only save quantized model, please execute .quantize first.")
+
+        self.model.to(CPU)
+
+        model_base_name = self.quantize_config.model_file_base_name or f"gptq_model-{self.quantize_config.bits}bit-{self.quantize_config.group_size}g"
+        if use_safetensors:
+            model_save_name = model_base_name + ".safetensors"
+            state_dict = self.model.state_dict()
+            state_dict = {k: v.clone().contiguous() for k, v in state_dict.items()}
+            safe_save(state_dict, join(save_dir, model_save_name))
+        else:
+            model_save_name = model_base_name + ".bin"
+            torch.save(self.model.state_dict(), join(save_dir, model_save_name))
+
+        self.model.config.save_pretrained(save_dir)
+        self.quantize_config.save_pretrained(save_dir)
+        self.quantize_config.model_name_or_path = save_dir
+        self.quantize_config.model_file_base_name = model_base_name
+
+    def save_pretrained(self, save_dir: str, use_safetensors: bool = False, **kwargs):
+        """alias of save_quantized"""
+        logger.warning("you are using save_pretrained, which will re-direct to save_quantized.")
+        self.save_quantized(save_dir, use_safetensors)
+
+    @classmethod
+    def from_pretrained(
+        cls,
+        pretrained_model_name_or_path: str,
+        quantize_config: BaseQuantizeConfig,
+        max_memory: Optional[dict] = None,
+        trust_remote_code: bool = False,
+        torch_dtype: torch.dtype = torch.float16,
+        **model_init_kwargs
+    ):
+        """load un-quantized pretrained model to cpu"""
+
+        if not torch.cuda.is_available():
+            raise EnvironmentError("Load pretrained model to do quantization requires CUDA available.")
+
+        def skip(*args, **kwargs):
+            pass
+
+        torch.nn.init.kaiming_uniform_ = skip
+        torch.nn.init.uniform_ = skip
+        torch.nn.init.normal_ = skip
+
+        config = AutoConfig.from_pretrained(pretrained_model_name_or_path, trust_remote_code=True)
+        if config.model_type not in SUPPORTED_MODELS:
+            raise TypeError(f"{config.model_type} isn't supported yet.")
+
+        # enforce some values despite user specified
+        model_init_kwargs["torch_dtype"] = torch_dtype
+        model_init_kwargs["trust_remote_code"] = trust_remote_code
+        if max_memory:
+            if "disk" in max_memory:
+                raise NotImplementedError("disk offload not support yet.")
+            with accelerate.init_empty_weights():
+                model = AutoModelForCausalLM.from_config(config, trust_remote_code=True)
+            model.tie_weights()
+
+            max_memory = accelerate.utils.get_balanced_memory(
+                model,
+                max_memory=max_memory,
+                no_split_module_classes=[cls.layer_type],
+                dtype=model_init_kwargs["torch_dtype"],
+                low_zero=False
+            )
+            model_init_kwargs["device_map"] = accelerate.infer_auto_device_map(
+                model,
+                max_memory=max_memory,
+                no_split_module_classes=[cls.layer_type],
+                dtype=model_init_kwargs["torch_dtype"]
+            )
+            model_init_kwargs["low_cpu_mem_usage"] = True
+
+            del model
+        else:
+            model_init_kwargs["device_map"] = None
+            model_init_kwargs["low_cpu_mem_usage"] = False
+
+        torch.cuda.empty_cache()
+
+        model = AutoModelForCausalLM.from_pretrained(pretrained_model_name_or_path, **model_init_kwargs)
+        model_config = model.config.to_dict()
+        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
+        if any([k in model_config for k in seq_len_keys]):
+            for key in seq_len_keys:
+                if key in model_config:
+                    model.seqlen = model_config[key]
+                    break
+        else:
+            logger.warning("can't get model's sequence length from model config, will set to 4096.")
+            model.seqlen = 4096
+        model.eval()
+
+        return cls(model, False, quantize_config)
+
+    @classmethod
+    def from_quantized(
+        cls,
+        model_name_or_path: Optional[str] = None,
+        save_dir: Optional[str] = None,
+        device_map: Optional[Union[str, Dict[str, Union[int, str]]]] = None,
+        max_memory: Optional[dict] = None,
+        device: Optional[Union[str, int]] = None,
+        low_cpu_mem_usage: bool = False,
+        use_triton: bool = False,
+        torch_dtype: torch.dtype = torch.float16,
+        inject_fused_attention: bool = True,
+        inject_fused_mlp: bool = True,
+        use_cuda_fp16: bool = True,
+        quantize_config: Optional[BaseQuantizeConfig] = None,
+        model_basename: Optional[str] = None,
+        use_safetensors: bool = False,
+        trust_remote_code: bool = False,
+        warmup_triton: bool = False,
+        trainable: bool = False,
+        **kwargs
+    ):
+        """load quantized model from local disk"""
+       
+        # Parameters related to loading from Hugging Face Hub
+        cache_dir = kwargs.pop("cache_dir", None)
+        force_download = kwargs.pop("force_download", False)
+        resume_download = kwargs.pop("resume_download", False)
+        proxies = kwargs.pop("proxies", None)
+        local_files_only = kwargs.pop("local_files_only", False)
+        use_auth_token = kwargs.pop("use_auth_token", None)
+        revision = kwargs.pop("revision", None)
+        subfolder = kwargs.pop("subfolder", "")
+        commit_hash = kwargs.pop("_commit_hash", None)
+
+        if use_triton and not TRITON_AVAILABLE:
+            logger.warning("triton is not installed, reset use_triton to False")
+            use_triton = False
+
+        # == step1: prepare configs and file names == #
+        if model_name_or_path and save_dir:
+            logger.warning("save_dir will be ignored because model_name_or_path is explicit specified.")
+        if not model_name_or_path and save_dir:
+            model_name_or_path = save_dir
+            warnings.warn("save_dir is deprecated and will be removed in version 0.3.0", PendingDeprecationWarning, stacklevel=2)
+        if not model_name_or_path and not save_dir:
+            raise ValueError("at least one of model_name_or_path or save_dir should be specified.")
+        
+        config = AutoConfig.from_pretrained(model_name_or_path, trust_remote_code=trust_remote_code)
+
+        if config.model_type not in SUPPORTED_MODELS:
+            raise TypeError(f"{config.model_type} isn't supported yet.")
+
+        if quantize_config is None:
+            quantize_config = BaseQuantizeConfig.from_pretrained(model_name_or_path, **kwargs)
+        
+        if model_basename is None:
+            if quantize_config.model_file_base_name:
+                model_basename = quantize_config.model_file_base_name
+            else:
+                model_basename = f"gptq_model-{quantize_config.bits}bit-{quantize_config.group_size}g"
+        
+        quantize_config.model_name_or_path = model_name_or_path
+        quantize_config.model_file_base_name = model_basename
+
+        extensions = []
+        if use_safetensors:
+            extensions.append(".safetensors")
+        else:
+            extensions += [".bin", ".pt"]
+
+        model_name_or_path = str(model_name_or_path)
+        is_local = isdir(model_name_or_path)
+
+        resolved_archive_file = None
+        if is_local:
+            model_save_name = join(model_name_or_path, model_basename)
+
+            for ext in extensions:
+                if isfile(model_save_name + ext):
+                    resolved_archive_file = model_save_name + ext
+                    break
+        else: # remote
+            cached_file_kwargs = {
+                "cache_dir": cache_dir,
+                "force_download": force_download,
+                "proxies": proxies,
+                "resume_download": resume_download,
+                "local_files_only": local_files_only,
+                "use_auth_token": use_auth_token,
+                "revision": revision,
+                "subfolder": subfolder,
+                "_raise_exceptions_for_missing_entries": False,
+                "_commit_hash": commit_hash,
+            }
+            
+            for ext in extensions:
+                resolved_archive_file = cached_file(model_name_or_path, model_basename + ext, **cached_file_kwargs)
+                if resolved_archive_file is not None:
+                    break
+        
+        if resolved_archive_file is None: # Could not find a model file to use
+            raise FileNotFoundError(f"Could not find model in {model_name_or_path}")
+                
+        model_save_name = resolved_archive_file
+
+        if not use_triton and trainable:
+            logger.warning("QuantLinear with cuda backend not support trainable mode yet, Switch to the pytorch backend.")
+
+        # == step2: convert model to gptq-model (replace Linear with QuantLinear) == #
+        def skip(*args, **kwargs):
+            pass
+
+        torch.nn.init.kaiming_uniform_ = skip
+        torch.nn.init.uniform_ = skip
+        torch.nn.init.normal_ = skip
+
+        transformers.modeling_utils._init_weights = False
+
+        init_contexts = [no_init_weights()]
+        if low_cpu_mem_usage:
+            init_contexts.append(accelerate.init_empty_weights(include_buffers=False))
+
+        with ContextManagers(init_contexts):
+            model = AutoModelForCausalLM.from_config(
+                config,
+                trust_remote_code=trust_remote_code,
+                torch_dtype=torch_dtype
+            )
+
+            layers = find_layers(model)
+            ignore_layers = [cls.lm_head_name] + cls.outside_layer_modules
+            for name in list(layers.keys()):
+                if any([name.startswith(ignore_layer) for ignore_layer in ignore_layers]):
+                    logger.info(f"{name} not been quantized, will be ignored when make_quant.")
+                    del layers[name]
+
+            make_quant(
+                model,
+                layers,
+                quantize_config.bits,
+                quantize_config.group_size,
+                use_triton=use_triton,
+                use_cuda_fp16=use_cuda_fp16,
+                desc_act=quantize_config.desc_act,
+                trainable=trainable
+            )
+            model.tie_weights()
+
+        # == step3: load checkpoint and dispatch == #
+        if isinstance(device_map, str) and device_map not in ["auto", "balanced", "balanced_low_0", "sequential"]:
+            raise ValueError(
+                "If passing a string for `device_map`, please choose 'auto', 'balanced', 'balanced_low_0' or "
+                "'sequential'."
+            )
+        if isinstance(device_map, dict):
+            max_memory = None
+        else:
+            if device is None and not device_map and not max_memory:
+                device_map = "auto"
+            if device is not None:
+                device = torch.device(device)
+                if not max_memory and not device_map:
+                    device_map = {"": device.index if device.type == "cuda" else device.type}
+            if not isinstance(device_map, dict) and device_map != "sequential":
+                max_memory = accelerate.utils.get_balanced_memory(
+                    model=model,
+                    max_memory=max_memory,
+                    no_split_module_classes=[cls.layer_type],
+                    low_zero=(device_map == "balanced_low_0")
+                )
+        if not isinstance(device_map, dict):
+            device_map = accelerate.infer_auto_device_map(
+                model,
+                max_memory=max_memory,
+                no_split_module_classes=[cls.layer_type]
+            )
+
+        if low_cpu_mem_usage:
+            make_sure_no_tensor_in_meta_device(model, use_triton, quantize_config.desc_act, quantize_config.group_size)
+
+        accelerate.utils.modeling.load_checkpoint_in_model(
+            model,
+            checkpoint=model_save_name,
+            device_map=device_map,
+            offload_state_dict=True,
+            offload_buffers=True
+        )
+        model = simple_dispatch_model(model, device_map)
+
+        # == step4: set seqlen == #
+        model_config = model.config.to_dict()
+        seq_len_keys = ["max_position_embeddings", "seq_length", "n_positions"]
+        if any([k in model_config for k in seq_len_keys]):
+            for key in seq_len_keys:
+                if key in model_config:
+                    model.seqlen = model_config[key]
+                    break
+        else:
+            logger.warning("can't get model's sequence length from model config, will set to 4096.")
+            model.seqlen = 4096
+
+        # == step5: (optional) inject optimized module == #
+        if inject_fused_attention:
+            if cls.fused_attn_module_type is None:
+                inject_fused_attention = False
+                logger.warning(f"{cls.__name__} hasn't fused attention module yet, will skip inject fused attention.")
+            else:
+                cls.fused_attn_module_type.inject_to_model(
+                    model,
+                    use_triton=use_triton,
+                    group_size=quantize_config.group_size,
+                    use_cuda_fp16=use_cuda_fp16,
+                    desc_act=quantize_config.desc_act,
+                    trainable=trainable
+                )
+        if inject_fused_mlp:
+            if cls.fused_mlp_module_type is None:
+                inject_fused_mlp = False
+                logger.warning(f"{cls.__name__} hasn't fused mlp module yet, will skip inject fused mlp.")
+            else:
+                cls.fused_mlp_module_type.inject_to_model(
+                    model,
+                    use_triton=use_triton
+                )
+
+        model.eval()
+        # == step6: (optional) warmup triton == #
+        if use_triton and warmup_triton:
+            from ..nn_modules.qlinear.qlinear_triton import QuantLinear
+            QuantLinear.warmup(model, seqlen=model.seqlen)
+
+            if inject_fused_mlp and cls.fused_mlp_module_type is not None:
+                cls.fused_mlp_module_type.warmup(model, seqlen=model.seqlen)
+
+        # == step7: make model compatible with peft
+        cls.make_sure_compatible_with_peft(
+            model, use_triton, quantize_config.desc_act, quantize_config.group_size
+        )
+
+        return cls(
+            model,
+            True,
+            quantize_config,
+            is_triton_backend=use_triton,
+            injected_fused_attention=inject_fused_attention,
+            injected_fused_mlp=inject_fused_mlp and use_triton,
+            trainable=trainable
+        )
+
+    def warmup_triton(self, enabled: bool = True):
+        if not enabled:
+            return
+        if not TRITON_AVAILABLE:
+            logger.warning(f"triton is not available, skip warmup stage directly.")
+            return
+
+        from ..nn_modules.qlinear.qlinear_triton import QuantLinear
+        QuantLinear.warmup(self.model, seqlen=self.model.seqlen)
+
+        if self.fused_mlp_module_type is not None:
+            self.fused_mlp_module_type.warmup(self.model, seqlen=self.model.seqlen)
+
+    def enable_trainable_mode(self, enabled: bool = True):
+        if not self.is_triton_backend and enabled:
+            raise NotImplementedError("For now, trainable mode only supports triton backend.")
+        for n, m in self.model.named_modules():
+            if hasattr(m, "trainable"):
+                setattr(m, "trainable", enabled)
+
+    def disable_trainable_mode(self):
+        self.enable_trainable_mode(enabled=False)
+
+    @staticmethod
+    def make_sure_compatible_with_peft(model: PreTrainedModel, use_triton: bool, desc_act: bool, group_size: int):
+        GeneralQuantLinear.inject_to_model(
+            model,
+            dynamically_import_QuantLinear(use_triton, desc_act, group_size)
+        )
+
+    def __getattr__(self, item):
+        try:
+            return super().__getattr__(item)
+        except:
+            return getattr(self.model, item)
+
+
+__all__ = ["BaseGPTQForCausalLM", "BaseQuantizeConfig"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/modeling/_utils.py` & `auto_gptq-0.3.0/auto_gptq/modeling/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,184 +1,206 @@
-from logging import getLogger
-from typing import Union
-
-import accelerate
-import torch
-import torch.nn as nn
-from transformers import AutoConfig
-import transformers
-
-from ._const import SUPPORTED_MODELS, CPU, CUDA_0
-from ..utils.import_utils import dynamically_import_QuantLinear
-
-
-logger = getLogger(__name__)
-
-
-def get_device(obj: Union[torch.Tensor, nn.Module]):
-    if isinstance(obj, torch.Tensor):
-        return obj.device
-    return next(obj.parameters()).device
-
-
-def move_to_device(obj: Union[torch.Tensor, nn.Module], device: torch.device):
-    if get_device(obj) != device:
-        obj = obj.to(device)
-    return obj
-
-
-def find_layers(module, layers=None, name=''):
-    if not layers:
-        layers = [transformers.pytorch_utils.Conv1D, nn.Conv2d, nn.Linear]
-    for layer in layers:
-        if isinstance(module,layer):
-            return {name: module}
-    res = {}
-    for name1, child in module.named_children():
-        res.update(find_layers(child, layers=layers, name=name + '.' + name1 if name != '' else name1))
-    return res
-
-
-def get_module_by_name_prefix(model, module_name: str):
-    for name, module in model.named_modules():
-        if name.startswith(module_name):
-            return module
-
-
-def get_module_by_name_suffix(model, module_name: str):
-    for name, module in model.named_modules():
-        if name.endswith(module_name):
-            return module
-
-
-def make_quant(module, names, bits, group_size, name='', use_triton=False, use_cuda_fp16=True, desc_act=False):
-    QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
-
-    if isinstance(module, QuantLinear):
-        return
-    for attr in dir(module):
-        tmp = getattr(module, attr)
-        name1 = name + '.' + attr if name != '' else attr
-        if name1 in names:
-            ori_layer_device = get_device(getattr(module, attr))
-            delattr(module, attr)
-            if isinstance(tmp,nn.Linear):
-                in_features = tmp.in_features
-                out_features = tmp.out_features
-            elif isinstance(tmp,nn.Conv2d):
-                in_features = tmp.in_channels
-                out_features = tmp.out_channels
-            elif isinstance(tmp,transformers.pytorch_utils.Conv1D):            
-                in_features = tmp.weight.shape[0]
-                out_features = tmp.weight.shape[1]
-            if (not(desc_act) or group_size == -1) and not use_triton:
-                new_layer = QuantLinear(bits, group_size, in_features, out_features, True, use_cuda_fp16=use_cuda_fp16)
-            else:
-                new_layer = QuantLinear(bits, group_size, in_features, out_features, True)
-            new_layer.device = ori_layer_device
-            setattr(module, attr, new_layer.to(ori_layer_device))
-    for name1, child in module.named_children():
-        make_quant(child, names, bits, group_size, name + '.' + name1 if name != '' else name1, use_triton=use_triton, use_cuda_fp16=use_cuda_fp16,desc_act=desc_act)
-
-
-def pack_model(
-    model,
-    quantizers,
-    bits,
-    group_size,
-    use_triton=False,
-    use_cuda_fp16=True,
-    desc_act=False,
-    warmup_triton: bool = False,
-    force_layer_back_to_cpu: bool = False
-):
-    QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
-
-    if force_layer_back_to_cpu:
-        model.to(CPU)
-
-    logger.info('Packing model...')
-    layers = find_layers(model)
-    layers = {n: layers[n] for n in quantizers}
-    make_quant(model, quantizers, bits, group_size, use_triton=use_triton, use_cuda_fp16=use_cuda_fp16, desc_act=desc_act)
-    qlayers = find_layers(model, [QuantLinear])
-    for name in qlayers:
-        logger.info(name)
-        quantizers[name], scale, zero, g_idx = quantizers[name]
-        # so far can only pack layer on CPU
-        layer_device = qlayers[name].device
-        qlayers[name].to(CPU)
-        layers[name], scale, zero, g_idx = layers[name].to(CPU), scale.to(CPU), zero.to(CPU), g_idx.to(CPU)
-        qlayers[name].pack(layers[name], scale, zero, g_idx)
-        qlayers[name].to(layer_device)
-    logger.info('Model packed.')
-
-    if use_triton and warmup_triton:
-        logger.warning(
-            "using autotune_warmup will move model to GPU, make sure you have enough VRAM to load the whole model."
-        )
-        QuantLinear.warmup(model.to(CUDA_0), seqlen=model.seqlen)
-
-
-def check_and_get_model_type(model_dir, trust_remote_code=False):
-    config = AutoConfig.from_pretrained(model_dir, trust_remote_code=trust_remote_code)
-    if config.model_type not in SUPPORTED_MODELS:
-        raise TypeError(f"{config.model_type} isn't supported yet.")
-    model_type = config.model_type
-    return model_type
-
-
-def simple_dispatch_model(model, device_map):
-    from accelerate.hooks import add_hook_to_module, AlignDevicesHook
-
-    if "" in device_map:
-        d = device_map[""]
-        model = model.to(torch.device(d))
-        model.hf_device_map = device_map
-        return model
-
-    tied_params = accelerate.utils.modeling.find_tied_parameters(model)
-    if set(device_map.values()) == {"cpu"} or set(device_map.values()) == {"cpu", "disk"}:
-        main_device = "cpu"
-    else:
-        main_device = [d for d in device_map.values() if d not in ["cpu", "disk"]][0]
-
-    cpu_offload_group = [(n, d) for n, d in device_map.items() if d == "cpu"]
-    prev_hook = None
-    for idx, (n, d) in enumerate(cpu_offload_group):
-        m = get_module_by_name_suffix(model, n)
-        _, prev_hook = accelerate.cpu_offload_with_hook(m, execution_device=main_device, prev_module_hook=prev_hook)
-    # set first cpu offload module's prev_module_hook to the last cpu offload module's hook
-    if len(cpu_offload_group) > 1:
-        get_module_by_name_suffix(model, cpu_offload_group[0][0])._hf_hook.prev_module_hook = prev_hook
-
-    for n, d in device_map.items():
-        m = get_module_by_name_suffix(model, n)
-        if d != "cpu":
-            d = torch.device(d)
-            hook = AlignDevicesHook(d, io_same_device=True, place_submodules=True)
-            add_hook_to_module(m, hook)
-    accelerate.utils.modeling.retie_parameters(model, tied_params)
-    model.hf_device_map = device_map
-
-    return model
-
-
-def make_sure_no_tensor_in_meta_device(model, use_triton, desc_act, group_size):
-    QuantLinear = dynamically_import_QuantLinear(use_triton, desc_act, group_size)
-    for n, m in model.named_modules():
-        if isinstance(m, QuantLinear) and m.bias.device == torch.device("meta"):
-            m.register_buffer('bias', torch.zeros((m.outfeatures), dtype=torch.float16, device="cpu"))
-
-
-__all__ = [
-    "get_device",
-    "move_to_device",
-    "find_layers",
-    "get_module_by_name_prefix",
-    "get_module_by_name_suffix",
-    "make_quant",
-    "pack_model",
-    "check_and_get_model_type",
-    "simple_dispatch_model",
-    "make_sure_no_tensor_in_meta_device"
-]
+from logging import getLogger
+from typing import Union
+
+import accelerate
+import torch
+import torch.nn as nn
+from transformers import AutoConfig
+import transformers
+
+from ._const import SUPPORTED_MODELS, CPU, CUDA_0
+from ..utils.import_utils import dynamically_import_QuantLinear
+
+
+logger = getLogger(__name__)
+
+
+def get_device(obj: Union[torch.Tensor, nn.Module]):
+    if isinstance(obj, torch.Tensor):
+        return obj.device
+    return next(obj.parameters()).device
+
+
+def move_to_device(obj: Union[torch.Tensor, nn.Module], device: torch.device):
+    if get_device(obj) != device:
+        obj = obj.to(device)
+    return obj
+
+
+def find_layers(module, layers=None, name=''):
+    if not layers:
+        layers = [transformers.pytorch_utils.Conv1D, nn.Conv2d, nn.Linear]
+    for layer in layers:
+        if isinstance(module,layer):
+            return {name: module}
+    res = {}
+    for name1, child in module.named_children():
+        res.update(find_layers(child, layers=layers, name=name + '.' + name1 if name != '' else name1))
+    return res
+
+
+def get_module_by_name_prefix(model, module_name: str):
+    for name, module in model.named_modules():
+        if name.startswith(module_name):
+            return module
+
+
+def get_module_by_name_suffix(model, module_name: str):
+    for name, module in model.named_modules():
+        if name.endswith(module_name):
+            return module
+
+
+def make_quant(
+    module,
+    names,
+    bits,
+    group_size,
+    name='',
+    use_triton=False,
+    use_cuda_fp16=True,
+    desc_act=False,
+    trainable=False
+):
+    QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
+
+    if isinstance(module, QuantLinear):
+        return
+    for attr in dir(module):
+        tmp = getattr(module, attr)
+        name1 = name + '.' + attr if name != '' else attr
+        if name1 in names:
+            ori_layer_device = get_device(getattr(module, attr))
+            delattr(module, attr)
+            if isinstance(tmp,nn.Linear):
+                in_features = tmp.in_features
+                out_features = tmp.out_features
+            elif isinstance(tmp,nn.Conv2d):
+                in_features = tmp.in_channels
+                out_features = tmp.out_channels
+            elif isinstance(tmp,transformers.pytorch_utils.Conv1D):            
+                in_features = tmp.weight.shape[0]
+                out_features = tmp.weight.shape[1]
+            if (not(desc_act) or group_size == -1) and not use_triton:
+                new_layer = QuantLinear(
+                    bits, group_size, in_features, out_features, True, use_cuda_fp16=use_cuda_fp16, trainable=trainable
+                )
+            else:
+                new_layer = QuantLinear(bits, group_size, in_features, out_features, True, trainable=trainable)
+            new_layer.device = ori_layer_device
+            setattr(module, attr, new_layer.to(ori_layer_device))
+    for name1, child in module.named_children():
+        make_quant(
+            child,
+            names,
+            bits,
+            group_size,
+            name + '.' + name1 if name != '' else name1,
+            use_triton=use_triton,
+            use_cuda_fp16=use_cuda_fp16,
+            desc_act=desc_act,
+            trainable=trainable
+        )
+
+
+def pack_model(
+    model,
+    quantizers,
+    bits,
+    group_size,
+    use_triton=False,
+    use_cuda_fp16=True,
+    desc_act=False,
+    warmup_triton: bool = False,
+    force_layer_back_to_cpu: bool = False
+):
+    QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
+
+    if force_layer_back_to_cpu:
+        model.to(CPU)
+
+    logger.info('Packing model...')
+    layers = find_layers(model)
+    layers = {n: layers[n] for n in quantizers}
+    make_quant(model, quantizers, bits, group_size, use_triton=use_triton, use_cuda_fp16=use_cuda_fp16, desc_act=desc_act)
+    qlayers = find_layers(model, [QuantLinear])
+    for name in qlayers:
+        logger.info(name)
+        quantizers[name], scale, zero, g_idx = quantizers[name]
+        # so far can only pack layer on CPU
+        layer_device = qlayers[name].device
+        qlayers[name].to(CPU)
+        layers[name], scale, zero, g_idx = layers[name].to(CPU), scale.to(CPU), zero.to(CPU), g_idx.to(CPU)
+        qlayers[name].pack(layers[name], scale, zero, g_idx)
+        qlayers[name].to(layer_device)
+    logger.info('Model packed.')
+
+    if use_triton and warmup_triton:
+        logger.warning(
+            "using autotune_warmup will move model to GPU, make sure you have enough VRAM to load the whole model."
+        )
+        QuantLinear.warmup(model.to(CUDA_0), seqlen=model.seqlen)
+
+
+def check_and_get_model_type(model_dir, trust_remote_code=False):
+    config = AutoConfig.from_pretrained(model_dir, trust_remote_code=trust_remote_code)
+    if config.model_type not in SUPPORTED_MODELS:
+        raise TypeError(f"{config.model_type} isn't supported yet.")
+    model_type = config.model_type
+    return model_type
+
+
+def simple_dispatch_model(model, device_map):
+    from accelerate.hooks import add_hook_to_module, AlignDevicesHook
+
+    if "" in device_map:
+        d = device_map[""]
+        model = model.to(torch.device(d))
+        model.hf_device_map = device_map
+        return model
+
+    tied_params = accelerate.utils.modeling.find_tied_parameters(model)
+    if set(device_map.values()) == {"cpu"} or set(device_map.values()) == {"cpu", "disk"}:
+        main_device = "cpu"
+    else:
+        main_device = [d for d in device_map.values() if d not in ["cpu", "disk"]][0]
+
+    cpu_offload_group = [(n, d) for n, d in device_map.items() if d == "cpu"]
+    prev_hook = None
+    for idx, (n, d) in enumerate(cpu_offload_group):
+        m = get_module_by_name_suffix(model, n)
+        _, prev_hook = accelerate.cpu_offload_with_hook(m, execution_device=main_device, prev_module_hook=prev_hook)
+    # set first cpu offload module's prev_module_hook to the last cpu offload module's hook
+    if len(cpu_offload_group) > 1:
+        get_module_by_name_suffix(model, cpu_offload_group[0][0])._hf_hook.prev_module_hook = prev_hook
+
+    for n, d in device_map.items():
+        m = get_module_by_name_suffix(model, n)
+        if d != "cpu":
+            d = torch.device(d)
+            hook = AlignDevicesHook(d, io_same_device=True, place_submodules=True)
+            add_hook_to_module(m, hook)
+    accelerate.utils.modeling.retie_parameters(model, tied_params)
+    model.hf_device_map = device_map
+
+    return model
+
+
+def make_sure_no_tensor_in_meta_device(model, use_triton, desc_act, group_size):
+    QuantLinear = dynamically_import_QuantLinear(use_triton, desc_act, group_size)
+    for n, m in model.named_modules():
+        if isinstance(m, QuantLinear) and m.bias.device == torch.device("meta"):
+            m.register_buffer('bias', torch.zeros((m.outfeatures), dtype=torch.float16, device="cpu"))
+
+
+__all__ = [
+    "get_device",
+    "move_to_device",
+    "find_layers",
+    "get_module_by_name_prefix",
+    "get_module_by_name_suffix",
+    "make_quant",
+    "pack_model",
+    "check_and_get_model_type",
+    "simple_dispatch_model",
+    "make_sure_no_tensor_in_meta_device"
+]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/modeling/auto.py` & `auto_gptq-0.3.0/auto_gptq/modeling/auto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,115 @@
-from inspect import signature
-from typing import Dict, Optional, Union
-
-from ._base import BaseQuantizeConfig, BaseGPTQForCausalLM
-from ._utils import check_and_get_model_type
-from .bloom import BloomGPTQForCausalLM
-from .codegen import CodeGenGPTQForCausalLM
-from .gpt_neox import GPTNeoXGPTQForCausalLM
-from .gptj import GPTJGPTQForCausalLM
-from .gpt2 import GPT2GPTQForCausalLM
-from .llama import LlamaGPTQForCausalLM
-from .moss import MOSSGPTQForCausalLM
-from .opt import OPTGPTQForCausalLM
-from .rw import RWGPTQForCausalLM
-from .gpt_bigcode import GPTBigCodeGPTQForCausalLM
-
-
-GPTQ_CAUSAL_LM_MODEL_MAP = {
-    "bloom": BloomGPTQForCausalLM,
-    "gpt_neox": GPTNeoXGPTQForCausalLM,
-    "gptj": GPTJGPTQForCausalLM,
-    "gpt2": GPT2GPTQForCausalLM,
-    "llama": LlamaGPTQForCausalLM,
-    "opt": OPTGPTQForCausalLM,
-    "moss": MOSSGPTQForCausalLM,
-    "gpt_bigcode": GPTBigCodeGPTQForCausalLM,
-    "codegen": CodeGenGPTQForCausalLM,
-    "RefinedWebModel": RWGPTQForCausalLM,
-    "RefinedWeb":RWGPTQForCausalLM
-}
-
-
-class AutoGPTQForCausalLM:
-    def __init__(self):
-        raise EnvironmentError(
-            "AutoGPTQModelForCausalLM is designed to be instantiated\n"
-            "using `AutoGPTQModelForCausalLM.from_pretrained` if want to quantize a pretrained model.\n"
-            "using `AutoGPTQModelForCausalLM.from_quantized` if want to inference with quantized model."
-        )
-
-    @classmethod
-    def from_pretrained(
-        cls,
-        pretrained_model_name_or_path: str,
-        quantize_config: BaseQuantizeConfig,
-        max_memory: Optional[dict] = None,
-        trust_remote_code: bool = False,
-        **model_init_kwargs
-    ) -> BaseGPTQForCausalLM:
-        model_type = check_and_get_model_type(pretrained_model_name_or_path, trust_remote_code)
-        return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_pretrained(
-            pretrained_model_name_or_path=pretrained_model_name_or_path,
-            quantize_config=quantize_config,
-            max_memory=max_memory,
-            trust_remote_code=trust_remote_code,
-            **model_init_kwargs
-        )
-
-    @classmethod
-    def from_quantized(
-        cls,
-        model_name_or_path: Optional[str] = None,
-        save_dir: Optional[str] = None,
-        device_map: Optional[Union[str, Dict[str, Union[str, int]]]] = None,
-        max_memory: Optional[dict] = None,
-        device: Optional[Union[str, int]] = None,
-        low_cpu_mem_usage: bool = False,
-        use_triton: bool = False,
-        inject_fused_attention: bool = True,
-        inject_fused_mlp: bool = True,
-        use_cuda_fp16: bool = True,
-        quantize_config: Optional[BaseQuantizeConfig] = None,
-        model_basename: Optional[str] = None,
-        use_safetensors: bool = False,
-        trust_remote_code: bool = False,
-        warmup_triton: bool = False,
-        **kwargs
-    ) -> BaseGPTQForCausalLM:
-        model_type = check_and_get_model_type(save_dir or model_name_or_path, trust_remote_code)
-        quant_func = GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_quantized
-        keywords = {key: kwargs[key] for key in signature(quant_func).parameters if key in kwargs}
-        return quant_func(
-            model_name_or_path=model_name_or_path,
-            save_dir=save_dir,
-            device_map=device_map,
-            max_memory=max_memory,
-            device=device,
-            low_cpu_mem_usage=low_cpu_mem_usage,
-            use_triton=use_triton,
-            inject_fused_attention=inject_fused_attention,
-            inject_fused_mlp=inject_fused_mlp,
-            use_cuda_fp16=use_cuda_fp16,
-            quantize_config=quantize_config,
-            model_basename=model_basename,
-            use_safetensors=use_safetensors,
-            trust_remote_code=trust_remote_code,
-            warmup_triton=warmup_triton,
-            **keywords
-        )
-
-
-__all__ = ["AutoGPTQForCausalLM"]
+from inspect import signature
+from typing import Dict, Optional, Union
+
+from ._base import BaseQuantizeConfig, BaseGPTQForCausalLM
+from ._utils import check_and_get_model_type
+from .bloom import BloomGPTQForCausalLM
+from .codegen import CodeGenGPTQForCausalLM
+from .gpt_neox import GPTNeoXGPTQForCausalLM
+from .gptj import GPTJGPTQForCausalLM
+from .gpt2 import GPT2GPTQForCausalLM
+from .llama import LlamaGPTQForCausalLM
+from .moss import MOSSGPTQForCausalLM
+from .opt import OPTGPTQForCausalLM
+from .rw import RWGPTQForCausalLM
+from .gpt_bigcode import GPTBigCodeGPTQForCausalLM
+from .baichuan import BaiChuanGPTQForCausalLM
+from .internlm import InternLMGPTQForCausalLM
+
+GPTQ_CAUSAL_LM_MODEL_MAP = {
+    "bloom": BloomGPTQForCausalLM,
+    "gpt_neox": GPTNeoXGPTQForCausalLM,
+    "gptj": GPTJGPTQForCausalLM,
+    "gpt2": GPT2GPTQForCausalLM,
+    "llama": LlamaGPTQForCausalLM,
+    "opt": OPTGPTQForCausalLM,
+    "moss": MOSSGPTQForCausalLM,
+    "gpt_bigcode": GPTBigCodeGPTQForCausalLM,
+    "codegen": CodeGenGPTQForCausalLM,
+    "RefinedWebModel": RWGPTQForCausalLM,
+    "RefinedWeb": RWGPTQForCausalLM,
+    "baichuan": BaiChuanGPTQForCausalLM,
+    "internlm": InternLMGPTQForCausalLM,
+}
+
+
+class AutoGPTQForCausalLM:
+    def __init__(self):
+        raise EnvironmentError(
+            "AutoGPTQModelForCausalLM is designed to be instantiated\n"
+            "using `AutoGPTQModelForCausalLM.from_pretrained` if want to quantize a pretrained model.\n"
+            "using `AutoGPTQModelForCausalLM.from_quantized` if want to inference with quantized model."
+        )
+
+    @classmethod
+    def from_pretrained(
+        cls,
+        pretrained_model_name_or_path: str,
+        quantize_config: BaseQuantizeConfig,
+        max_memory: Optional[dict] = None,
+        trust_remote_code: bool = False,
+        **model_init_kwargs
+    ) -> BaseGPTQForCausalLM:
+        model_type = check_and_get_model_type(
+            pretrained_model_name_or_path, trust_remote_code
+        )
+        return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_pretrained(
+            pretrained_model_name_or_path=pretrained_model_name_or_path,
+            quantize_config=quantize_config,
+            max_memory=max_memory,
+            trust_remote_code=trust_remote_code,
+            **model_init_kwargs
+        )
+
+    @classmethod
+    def from_quantized(
+        cls,
+        model_name_or_path: Optional[str] = None,
+        save_dir: Optional[str] = None,
+        device_map: Optional[Union[str, Dict[str, Union[str, int]]]] = None,
+        max_memory: Optional[dict] = None,
+        device: Optional[Union[str, int]] = None,
+        low_cpu_mem_usage: bool = False,
+        use_triton: bool = False,
+        inject_fused_attention: bool = True,
+        inject_fused_mlp: bool = True,
+        use_cuda_fp16: bool = True,
+        quantize_config: Optional[BaseQuantizeConfig] = None,
+        model_basename: Optional[str] = None,
+        use_safetensors: bool = False,
+        trust_remote_code: bool = False,
+        warmup_triton: bool = False,
+        trainable: bool = False,
+        **kwargs
+    ) -> BaseGPTQForCausalLM:
+        model_type = check_and_get_model_type(
+            save_dir or model_name_or_path, trust_remote_code
+        )
+        quant_func = GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_quantized
+        keywords = {
+            key: kwargs[key]
+            for key in signature(quant_func).parameters
+            if key in kwargs
+        }
+        return quant_func(
+            model_name_or_path=model_name_or_path,
+            save_dir=save_dir,
+            device_map=device_map,
+            max_memory=max_memory,
+            device=device,
+            low_cpu_mem_usage=low_cpu_mem_usage,
+            use_triton=use_triton,
+            inject_fused_attention=inject_fused_attention,
+            inject_fused_mlp=inject_fused_mlp,
+            use_cuda_fp16=use_cuda_fp16,
+            quantize_config=quantize_config,
+            model_basename=model_basename,
+            use_safetensors=use_safetensors,
+            trust_remote_code=trust_remote_code,
+            warmup_triton=warmup_triton,
+            trainable=trainable,
+            **keywords
+        )
+
+
+__all__ = ["AutoGPTQForCausalLM"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/modeling/gptj.py` & `auto_gptq-0.3.0/auto_gptq/modeling/gptj.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from ._base import *
-from ..nn_modules.fused_gptj_attn import FusedGPTJAttentionForQuantizedModel
-
-
-class GPTJGPTQForCausalLM(BaseGPTQForCausalLM):
-    layer_type = "GPTJBlock"
-    layers_block_name = "transformer.h"
-    outside_layer_modules = ["transformer.wte", "transformer.ln_f"]
-    inside_layer_modules = [
-        ["attn.k_proj", "attn.v_proj", "attn.q_proj"],
-        ["attn.out_proj"],
-        ["mlp.fc_in"],
-        ["mlp.fc_out"]
-    ]
-
-    fused_attn_module_type = FusedGPTJAttentionForQuantizedModel
-
-
-__all__ = ["GPTJGPTQForCausalLM"]
+from ._base import *
+from ..nn_modules.fused_gptj_attn import FusedGPTJAttentionForQuantizedModel
+
+
+class GPTJGPTQForCausalLM(BaseGPTQForCausalLM):
+    layer_type = "GPTJBlock"
+    layers_block_name = "transformer.h"
+    outside_layer_modules = ["transformer.wte", "transformer.ln_f"]
+    inside_layer_modules = [
+        ["attn.k_proj", "attn.v_proj", "attn.q_proj"],
+        ["attn.out_proj"],
+        ["mlp.fc_in"],
+        ["mlp.fc_out"]
+    ]
+
+    fused_attn_module_type = FusedGPTJAttentionForQuantizedModel
+
+
+__all__ = ["GPTJGPTQForCausalLM"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/nn_modules/fused_llama_attn.py` & `auto_gptq-0.3.0/auto_gptq/nn_modules/fused_llama_attn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,180 +1,189 @@
-import math
-import torch
-import torch.nn as nn
-from torch.nn import functional as F
-from transformers.models.llama.modeling_llama import LlamaAttention, apply_rotary_pos_emb
-
-from ._fused_base import FusedBaseAttentionModule
-from ..utils.import_utils import compare_pytorch_version, dynamically_import_QuantLinear
-
-
-class FusedLlamaAttentionForQuantizedModel(FusedBaseAttentionModule):
-    """Multi-headed attention from 'Attention Is All You Need' paper"""
-
-    def __init__(
-        self,
-        hidden_size,
-        num_heads,
-        qkv_proj,
-        o_proj,
-        rotary_emb,
-    ):
-        super().__init__()
-        self.hidden_size = hidden_size
-        self.num_heads = num_heads
-        self.head_dim = hidden_size // num_heads
-
-        if self.head_dim * num_heads != self.hidden_size:
-            raise ValueError(
-                f"hidden_size must be divisible by num_heads (got `hidden_size`: {self.hidden_size}"
-                f" and `num_heads`: {num_heads})."
-            )
-        self.qkv_proj = qkv_proj
-        self.o_proj = o_proj
-        self.rotary_emb = rotary_emb
-
-    def _shape(self, tensor, seq_len, bsz):
-        return tensor.view(bsz, seq_len, self.num_heads, self.head_dim).transpose(1, 2).contiguous()
-
-    def forward(
-        self,
-        hidden_states,
-        past_key_value=None,
-        attention_mask=None,
-        position_ids=None,
-        output_attentions=False,
-        use_cache=False,
-        **kwargs
-    ):
-        """Input shape: Batch x Time x Channel"""
-
-        bsz, q_len, _ = hidden_states.size()
-
-        qkv_states = self.qkv_proj(hidden_states)
-        query_states, key_states, value_states = torch.split(qkv_states, self.hidden_size, dim=2)
-
-        query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-        key_states = key_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-        value_states = value_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
-
-        kv_seq_len = key_states.shape[-2]
-        if past_key_value is not None:
-            kv_seq_len += past_key_value[0].shape[-2]
-        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
-        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
-        # [bsz, nh, t, hd]
-
-        is_causal = past_key_value is None
-        if past_key_value is not None:
-            # reuse k, v, self_attention
-            key_states = torch.cat([past_key_value[0], key_states], dim=2)
-            value_states = torch.cat([past_key_value[1], value_states], dim=2)
-
-        if use_cache:
-            # Since qkv_proj is fused, query_states etc will hold a reference to the original qkv_states tensor
-            # which can cause excessive memory usage by the cache. `contiguous` is a convenient way to workaround this.
-            query_states = query_states.contiguous()
-            key_states = key_states.contiguous()
-            value_states = value_states.contiguous()
-
-        past_key_value = (key_states, value_states) if use_cache else None
-
-        if compare_pytorch_version("v2.0.0", op="eq"):
-            attn_output = F.scaled_dot_product_attention(
-                query_states,
-                key_states,
-                value_states,
-                attn_mask=None if is_causal else attention_mask,
-                is_causal=is_causal
-            )
-            attn_weights = None
-        else:
-            attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
-
-            if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
-                raise ValueError(
-                    f"Attention weights should be of size {(bsz * self.num_heads, q_len, kv_seq_len)}, but is"
-                    f" {attn_weights.size()}"
-                )
-
-            if attention_mask is not None:
-                if attention_mask.size() != (bsz, 1, q_len, kv_seq_len):
-                    raise ValueError(
-                        f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}, but is {attention_mask.size()}"
-                    )
-                attn_weights = attn_weights + attention_mask
-                attn_weights = torch.max(attn_weights, torch.tensor(torch.finfo(attn_weights.dtype).min))
-
-            # upcast attention to fp32
-            attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
-            attn_output = torch.matmul(attn_weights, value_states)
-
-        if attn_output.size() != (bsz, self.num_heads, q_len, self.head_dim):
-            raise ValueError(
-                f"`attn_output` should be of size {(bsz, self.num_heads, q_len, self.head_dim)}, but is"
-                f" {attn_output.size()}"
-            )
-
-        attn_output = attn_output.transpose(1, 2)
-        attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
-
-        attn_output = self.o_proj(attn_output)
-
-        if not output_attentions:
-            attn_weights = None
-
-        return attn_output, attn_weights, past_key_value
-
-    @classmethod
-    def inject_to_model(cls, model, use_triton=False, group_size=-1, use_cuda_fp16=True, desc_act=False, **kwargs):
-        """
-        Replace all LlamaAttention modules with QuantLlamaAttention modules, fusing the q, k, v projections.
-        """
-        QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
-
-        for name, m in model.named_modules():
-            if not isinstance(m, LlamaAttention):
-                continue
-
-            q_proj = m.q_proj
-            k_proj = m.k_proj
-            v_proj = m.v_proj
-
-            qweights = torch.cat([q_proj.qweight, k_proj.qweight, v_proj.qweight], dim=1)
-            qzeros = torch.cat([q_proj.qzeros, k_proj.qzeros, v_proj.qzeros], dim=1)
-            scales = torch.cat([q_proj.scales, k_proj.scales, v_proj.scales], dim=1)
-            g_idx = torch.cat([q_proj.g_idx, k_proj.g_idx, v_proj.g_idx], dim=0)
-            bias = torch.cat([q_proj.bias, k_proj.bias, v_proj.bias], dim=0) if q_proj.bias is not None else None
-
-            qlinear_args = (
-                q_proj.bits,
-                q_proj.group_size,
-                q_proj.infeatures,
-                q_proj.outfeatures + k_proj.outfeatures + v_proj.outfeatures,
-                True if q_proj.bias is not None else False,
-            )
-            qlinear_kwargs = dict()
-            if (not desc_act or group_size == -1) and not use_triton:
-                qlinear_kwargs["use_cuda_fp16"] = use_cuda_fp16
-            qkv_layer = QuantLinear(*qlinear_args, **qlinear_kwargs)
-            qkv_layer.qweight = qweights
-            qkv_layer.qzeros = qzeros
-            qkv_layer.scales = scales
-            qkv_layer.g_idx = g_idx
-            qkv_layer.bias = bias
-
-            attn = cls(m.hidden_size, m.num_heads, qkv_layer, m.o_proj, m.rotary_emb)
-
-            if '.' in name:
-                parent_name = name.rsplit('.', 1)[0]
-                child_name = name[len(parent_name) + 1:]
-                parent = model.get_submodule(parent_name)
-            else:
-                parent_name = ''
-                parent = model
-                child_name = name
-
-            setattr(parent, child_name, attn)
-
-
-__all__ = ["FusedLlamaAttentionForQuantizedModel"]
+import math
+import torch
+import torch.nn as nn
+from torch.nn import functional as F
+from transformers.models.llama.modeling_llama import LlamaAttention, apply_rotary_pos_emb
+
+from ._fused_base import FusedBaseAttentionModule
+from ..utils.import_utils import compare_pytorch_version, dynamically_import_QuantLinear
+
+
+class FusedLlamaAttentionForQuantizedModel(FusedBaseAttentionModule):
+    """Multi-headed attention from 'Attention Is All You Need' paper"""
+
+    def __init__(
+        self,
+        hidden_size,
+        num_heads,
+        qkv_proj,
+        o_proj,
+        rotary_emb,
+    ):
+        super().__init__()
+        self.hidden_size = hidden_size
+        self.num_heads = num_heads
+        self.head_dim = hidden_size // num_heads
+
+        if self.head_dim * num_heads != self.hidden_size:
+            raise ValueError(
+                f"hidden_size must be divisible by num_heads (got `hidden_size`: {self.hidden_size}"
+                f" and `num_heads`: {num_heads})."
+            )
+        self.qkv_proj = qkv_proj
+        self.o_proj = o_proj
+        self.rotary_emb = rotary_emb
+
+    def _shape(self, tensor, seq_len, bsz):
+        return tensor.view(bsz, seq_len, self.num_heads, self.head_dim).transpose(1, 2).contiguous()
+
+    def forward(
+        self,
+        hidden_states,
+        past_key_value=None,
+        attention_mask=None,
+        position_ids=None,
+        output_attentions=False,
+        use_cache=False,
+        **kwargs
+    ):
+        """Input shape: Batch x Time x Channel"""
+
+        bsz, q_len, _ = hidden_states.size()
+
+        qkv_states = self.qkv_proj(hidden_states)
+        query_states, key_states, value_states = torch.split(qkv_states, self.hidden_size, dim=2)
+
+        query_states = query_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+        key_states = key_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+        value_states = value_states.view(bsz, q_len, self.num_heads, self.head_dim).transpose(1, 2)
+
+        kv_seq_len = key_states.shape[-2]
+        if past_key_value is not None:
+            kv_seq_len += past_key_value[0].shape[-2]
+        cos, sin = self.rotary_emb(value_states, seq_len=kv_seq_len)
+        query_states, key_states = apply_rotary_pos_emb(query_states, key_states, cos, sin, position_ids)
+        # [bsz, nh, t, hd]
+
+        is_causal = past_key_value is None
+        if past_key_value is not None:
+            # reuse k, v, self_attention
+            key_states = torch.cat([past_key_value[0], key_states], dim=2)
+            value_states = torch.cat([past_key_value[1], value_states], dim=2)
+
+        if use_cache:
+            # Since qkv_proj is fused, query_states etc will hold a reference to the original qkv_states tensor
+            # which can cause excessive memory usage by the cache. `contiguous` is a convenient way to workaround this.
+            query_states = query_states.contiguous()
+            key_states = key_states.contiguous()
+            value_states = value_states.contiguous()
+
+        past_key_value = (key_states, value_states) if use_cache else None
+
+        if compare_pytorch_version("v2.0.0", op="eq"):
+            attn_output = F.scaled_dot_product_attention(
+                query_states,
+                key_states,
+                value_states,
+                attn_mask=None if is_causal else attention_mask,
+                is_causal=is_causal
+            )
+            attn_weights = None
+        else:
+            attn_weights = torch.matmul(query_states, key_states.transpose(2, 3)) / math.sqrt(self.head_dim)
+
+            if attn_weights.size() != (bsz, self.num_heads, q_len, kv_seq_len):
+                raise ValueError(
+                    f"Attention weights should be of size {(bsz * self.num_heads, q_len, kv_seq_len)}, but is"
+                    f" {attn_weights.size()}"
+                )
+
+            if attention_mask is not None:
+                if attention_mask.size() != (bsz, 1, q_len, kv_seq_len):
+                    raise ValueError(
+                        f"Attention mask should be of size {(bsz, 1, q_len, kv_seq_len)}, but is {attention_mask.size()}"
+                    )
+                attn_weights = attn_weights + attention_mask
+                attn_weights = torch.max(attn_weights, torch.tensor(torch.finfo(attn_weights.dtype).min))
+
+            # upcast attention to fp32
+            attn_weights = nn.functional.softmax(attn_weights, dim=-1, dtype=torch.float32).to(query_states.dtype)
+            attn_output = torch.matmul(attn_weights, value_states)
+
+        if attn_output.size() != (bsz, self.num_heads, q_len, self.head_dim):
+            raise ValueError(
+                f"`attn_output` should be of size {(bsz, self.num_heads, q_len, self.head_dim)}, but is"
+                f" {attn_output.size()}"
+            )
+
+        attn_output = attn_output.transpose(1, 2)
+        attn_output = attn_output.reshape(bsz, q_len, self.hidden_size)
+
+        attn_output = self.o_proj(attn_output)
+
+        if not output_attentions:
+            attn_weights = None
+
+        return attn_output, attn_weights, past_key_value
+
+    @classmethod
+    def inject_to_model(
+        cls,
+        model,
+        use_triton=False,
+        group_size=-1,
+        use_cuda_fp16=True,
+        desc_act=False,
+        trainable=False,
+        **kwargs
+    ):
+        """
+        Replace all LlamaAttention modules with QuantLlamaAttention modules, fusing the q, k, v projections.
+        """
+        QuantLinear = dynamically_import_QuantLinear(use_triton=use_triton, desc_act=desc_act, group_size=group_size)
+
+        for name, m in model.named_modules():
+            if not isinstance(m, LlamaAttention):
+                continue
+
+            q_proj = m.q_proj
+            k_proj = m.k_proj
+            v_proj = m.v_proj
+
+            qweights = torch.cat([q_proj.qweight, k_proj.qweight, v_proj.qweight], dim=1)
+            qzeros = torch.cat([q_proj.qzeros, k_proj.qzeros, v_proj.qzeros], dim=1)
+            scales = torch.cat([q_proj.scales, k_proj.scales, v_proj.scales], dim=1)
+            g_idx = torch.cat([q_proj.g_idx, k_proj.g_idx, v_proj.g_idx], dim=0)
+            bias = torch.cat([q_proj.bias, k_proj.bias, v_proj.bias], dim=0) if q_proj.bias is not None else None
+
+            qlinear_args = (
+                q_proj.bits,
+                q_proj.group_size,
+                q_proj.infeatures,
+                q_proj.outfeatures + k_proj.outfeatures + v_proj.outfeatures,
+                True if q_proj.bias is not None else False,
+            )
+            qlinear_kwargs = {"trainable": trainable}
+            if (not desc_act or group_size == -1) and not use_triton:
+                qlinear_kwargs["use_cuda_fp16"] = use_cuda_fp16
+            qkv_layer = QuantLinear(*qlinear_args, **qlinear_kwargs)
+            qkv_layer.qweight = qweights
+            qkv_layer.qzeros = qzeros
+            qkv_layer.scales = scales
+            qkv_layer.g_idx = g_idx
+            qkv_layer.bias = bias
+
+            attn = cls(m.hidden_size, m.num_heads, qkv_layer, m.o_proj, m.rotary_emb)
+
+            if '.' in name:
+                parent_name = name.rsplit('.', 1)[0]
+                child_name = name[len(parent_name) + 1:]
+                parent = model.get_submodule(parent_name)
+            else:
+                parent_name = ''
+                parent = model
+                child_name = name
+
+            setattr(parent, child_name, attn)
+
+
+__all__ = ["FusedLlamaAttentionForQuantizedModel"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear.py` & `auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,259 +1,268 @@
-import math
-from logging import getLogger
-
-import numpy as np
-import torch
-import torch.nn as nn
-import transformers
-
-logger = getLogger(__name__)
-
-try:
-    import autogptq_cuda
-
-    _autogptq_cuda_available = True
-except ImportError:
-    logger.warning('CUDA extension not installed.')
-    _autogptq_cuda_available = False
-
-
-class QuantLinear(nn.Module):
-    def __init__(
-        self,
-        bits,
-        group_size,
-        infeatures,
-        outfeatures,
-        bias,
-        kernel_switch_threshold=128,
-    ):
-        super().__init__()
-        if bits not in [2, 3, 4, 8]:
-            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        self.infeatures = infeatures
-        self.outfeatures = outfeatures
-        self.bits = bits
-        self.group_size = group_size if group_size != -1 else infeatures
-        self.maxq = 2 ** self.bits - 1
-
-        self.register_buffer(
-            'qweight',
-            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'qzeros',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'scales',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
-        )
-        self.register_buffer(
-            'g_idx',
-            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
-        )
-        if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
-        else:
-            self.bias = None
-
-        # is performed by unpacking the weights and using torch.matmul
-        if self.bits in [2, 4, 8]:
-            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
-        elif self.bits == 3:
-            self.wf = torch.tensor(
-                [
-                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
-                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
-                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
-                ],
-                dtype=torch.int32
-            ).reshape(1, 3, 12)
-
-        self.kernel_switch_threshold = kernel_switch_threshold
-        self.autogptq_cuda_available = _autogptq_cuda_available
-        if infeatures % 256 != 0 or outfeatures % 256 != 0:
-            self.autogptq_cuda_available = False
-
-    def pack(self, linear, scales, zeros, g_idx=None):
-        W = linear.weight.data.clone()
-        if isinstance(linear, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(linear, transformers.pytorch_utils.Conv1D):
-            W = W.t()
-
-        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
-
-        scales = scales.t().contiguous()
-        zeros = zeros.t().contiguous()
-        scale_zeros = zeros * scales
-        self.scales = scales.clone().half()
-        if linear.bias is not None:
-            self.bias = linear.bias.clone().half()
-
-        intweight = []
-        for idx in range(self.infeatures):
-            intweight.append(
-                torch.round(
-                    (
-                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
-                ).to(torch.int)[:, None]
-            )
-        intweight = torch.cat(intweight, dim=1)
-        intweight = intweight.t().contiguous()
-        intweight = intweight.numpy().astype(np.uint32)
-
-        i = 0
-        row = 0
-        qweight = np.zeros(
-            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
-        )
-        while row < qweight.shape[0]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                row += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i))
-                i += 10
-                qweight[row] |= intweight[i] << 30
-                row += 1
-                qweight[row] |= (intweight[i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
-                i += 10
-                qweight[row] |= intweight[i] << 31
-                row += 1
-                qweight[row] |= (intweight[i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
-                i += 10
-                row += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight)
-
-        zeros -= 1
-        zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
-        i = 0
-        col = 0
-        while col < qzeros.shape[1]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                col += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 30
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 31
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
-                i += 10
-                col += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros)
-
-    def forward(self, x: torch.Tensor):
-        out_shape = x.shape[:-1] + (self.outfeatures,)
-        x = x.reshape(-1, x.shape[-1])
-        if self.autogptq_cuda_available and (
-            self.kernel_switch_threshold == 0 or x.shape[0] < self.kernel_switch_threshold
-        ):
-            out = torch.zeros((x.shape[0], self.outfeatures), device=x.device, dtype=torch.float32)
-            if self.bits == 2:
-                autogptq_cuda.vecquant2matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            elif self.bits == 3:
-                autogptq_cuda.vecquant3matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            elif self.bits == 4:
-                autogptq_cuda.vecquant4matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            elif self.bits == 8:
-                autogptq_cuda.vecquant8matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-        else:
-            if self.wf.device != self.qzeros.device:
-                self.wf = self.wf.to(self.qzeros.device)
-
-            if self.bits in [2, 4, 8]:
-                zeros = torch.bitwise_right_shift(
-                    torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits),
-                    self.wf.unsqueeze(0)
-                ).to(torch.int16 if self.bits == 8 else torch.int8)
-                torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
-
-                zeros = zeros + 1
-                zeros = zeros.reshape(self.scales.shape)
-
-                weight = torch.bitwise_right_shift(
-                    torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1),
-                    self.wf.unsqueeze(-1)
-                ).to(torch.int16 if self.bits == 8 else torch.int8)
-                torch.bitwise_and(weight, (2 ** self.bits) - 1, out=weight)
-            elif self.bits == 3:
-                zeros = self.qzeros.reshape(
-                    self.qzeros.shape[0], self.qzeros.shape[1] // 3, 3, 1
-                ).expand(-1, -1, -1, 12)
-                zeros = (zeros >> self.wf.unsqueeze(0))
-                zeros[:, :, 0, 10] = (zeros[:, :, 0, 10] & 0x3) | ((zeros[:, :, 1, 0] << 2) & 0x4)
-                zeros[:, :, 1, 11] = (zeros[:, :, 1, 11] & 0x1) | ((zeros[:, :, 2, 0] << 1) & 0x6)
-                zeros = zeros & 0x7
-                zeros = torch.cat([zeros[:, :, 0, :11], zeros[:, :, 1, 1:12], zeros[:, :, 2, 1:11]], dim=2)
-
-                zeros = zeros + 1
-                zeros = zeros.reshape(self.scales.shape)
-
-                weight = self.qweight.reshape(
-                    self.qweight.shape[0] // 3, 3, 1, self.qweight.shape[1]
-                ).expand(-1, -1, 12, -1)
-                weight = (weight >> self.wf.unsqueeze(-1)) & 0x7
-                weight[:, 0, 10] = (weight[:, 0, 10] & 0x3) | ((weight[:, 1, 0] << 2) & 0x4)
-                weight[:, 1, 11] = (weight[:, 1, 11] & 0x1) | ((weight[:, 2, 0] << 1) & 0x6)
-                weight = weight & 0x7
-                weight = torch.cat([weight[:, 0, :11], weight[:, 1, 1:12], weight[:, 2, 1:11]], dim=1)
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
-            num_itr = self.g_idx.shape[0]//x.shape[-1]
-            if num_itr == 1:
-                weights = (self.scales[self.g_idx.long()] * (weight - zeros[self.g_idx.long()]))
-            else:
-                num_dim = self.g_idx.shape[0]//num_itr
-                weights = []
-                for i in range(num_itr):
-                    scale_i = self.scales[:,i*num_dim:(i+1)*num_dim]
-                    weight_i = weight[:,i*num_dim:(i+1)*num_dim]
-                    zeros_i = zeros[:,i*num_dim:(i+1)*num_dim]
-                    g_idx_i = self.g_idx[i*num_dim:(i+1)*num_dim]
-                    weights.append(scale_i[g_idx_i.long()] * (weight_i - zeros_i[g_idx_i.long()]))
-                weights = torch.cat(weights,dim=1)
-            out = torch.matmul(x.half(), weights)
-        out = out.half().reshape(out_shape)
-        out = out + self.bias if self.bias is not None else out
-        return out
-
-
-__all__ = ["QuantLinear"]
+import math
+from logging import getLogger
+
+import numpy as np
+import torch
+import torch.nn as nn
+import transformers
+
+logger = getLogger(__name__)
+try:
+    import autogptq_cuda_256
+    import autogptq_cuda_64
+    _autogptq_cuda_available = True
+except ImportError:
+    logger.warning('CUDA extension not installed.')
+    _autogptq_cuda_available = False
+
+
+class QuantLinear(nn.Module):
+    def __init__(
+        self,
+        bits,
+        group_size,
+        infeatures,
+        outfeatures,
+        bias,
+        use_cuda_fp16=True,
+        kernel_switch_threshold=128,
+        trainable=False
+    ):
+        super().__init__()
+        global _autogptq_cuda_available
+        if bits not in [2, 3, 4, 8]:
+            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        if trainable:
+            _autogptq_cuda_available = False
+        self.infeatures = infeatures
+        self.outfeatures = outfeatures
+        self.bits = bits
+        self.group_size = group_size if group_size != -1 else infeatures
+        self.maxq = 2 ** self.bits - 1
+
+        self.register_buffer(
+            'qweight',
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'qzeros',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'scales',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
+        )
+        self.register_buffer(
+            'g_idx',
+            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
+        )
+
+        if bias:
+            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
+        else:
+            self.bias = None
+        self.half_indim = self.infeatures // 2
+
+        self.use_cuda_fp16 = use_cuda_fp16 if bits != 8 else False
+        
+        # is performed by unpacking the weights and using torch.matmul
+        if self.bits in [2, 4, 8]:
+            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
+        elif self.bits == 3:
+            self.wf = torch.tensor(
+                [
+                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
+                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
+                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
+                ],
+                dtype=torch.int32
+            ).reshape(1, 3, 12)
+
+        self.kernel_switch_threshold = kernel_switch_threshold
+        self.autogptq_cuda_available = _autogptq_cuda_available
+        self.autogptq_cuda = autogptq_cuda_256
+        if infeatures % 256 != 0 or outfeatures % 256 != 0:
+            self.autogptq_cuda = autogptq_cuda_64
+        if infeatures % 64 != 0 or outfeatures % 64 != 0:
+            self.autogptq_cuda_available = False
+
+        self.trainable = trainable
+
+    def pack(self, linear, scales, zeros, g_idx):
+        W = linear.weight.data.clone()
+        if isinstance(linear, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(linear, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+
+        scales = scales.t().contiguous()
+        zeros = zeros.t().contiguous()
+        scale_zeros = zeros * scales
+        self.scales = scales.clone().half()
+        if linear.bias is not None:
+            self.bias = linear.bias.clone().half()
+
+        intweight = []
+        for idx in range(self.infeatures):
+            g_idx = idx // self.group_size
+            intweight.append(
+                torch.round(
+                    (W[:, idx] + scale_zeros[g_idx]) / self.scales[g_idx]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
+        intweight = intweight.t().contiguous()
+        intweight = intweight.numpy().astype(np.uint32)
+
+        i = 0
+        row = 0
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
+        while row < qweight.shape[0]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qweight[row] |= intweight[j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                row += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i))
+                i += 10
+                qweight[row] |= intweight[i] << 30
+                row += 1
+                qweight[row] |= (intweight[i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
+                i += 10
+                qweight[row] |= intweight[i] << 31
+                row += 1
+                qweight[row] |= (intweight[i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
+                i += 10
+                row += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qweight = qweight.astype(np.int32)
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
+        zeros = zeros.numpy().astype(np.uint32)
+        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        i = 0
+        col = 0
+        while col < qzeros.shape[1]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                col += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 30
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 31
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
+                i += 10
+                col += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qzeros = qzeros.astype(np.int32)
+        self.qzeros = torch.from_numpy(qzeros)
+
+    def forward(self, x):
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        x = x.reshape(-1, x.shape[-1])
+        if self.autogptq_cuda_available is True and (
+            self.kernel_switch_threshold is False or x.shape[0] < self.kernel_switch_threshold
+        ):
+            out = torch.zeros(x.shape[0], out_shape[-1], dtype=torch.float, device=x.device)
+            if self.use_cuda_fp16:
+                x = x.half()
+                if self.bits == 2:
+                    self.autogptq_cuda.vecquant2matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
+                elif self.bits == 3:
+                    self.autogptq_cuda.vecquant3matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
+                elif self.bits == 4:
+                    self.autogptq_cuda.vecquant4matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
+
+                else:
+                    raise NotImplementedError("Only 2,3,4 bits are supported.")
+            else:
+                x = x.float()
+                if self.bits == 2:
+                    self.autogptq_cuda.vecquant2matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
+                elif self.bits == 3:
+                    self.autogptq_cuda.vecquant3matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
+                elif self.bits == 4:
+                    self.autogptq_cuda.vecquant4matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
+                elif self.bits == 8:
+                    self.autogptq_cuda.vecquant8matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
+                else:
+                    raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        else:
+            if self.wf.device != self.qzeros.device:
+               self.wf = self.wf.to(self.qzeros.device)
+                
+            if self.bits in [2,4,8]:
+               zeros = torch.bitwise_right_shift(torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits), self.wf.unsqueeze(0)).to(torch.int16 if self.bits == 8 else torch.int8)
+               torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
+                   
+               zeros = zeros + 1
+               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
+   
+               scales = self.scales
+               scales = scales.reshape(-1, 1, scales.shape[-1])
+                
+               weight = torch.bitwise_right_shift(torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1), self.wf.unsqueeze(-1)).to(torch.int16 if self.bits == 8 else torch.int8)
+               torch.bitwise_and(weight,(2 ** self.bits) - 1, out=weight)
+               weight = weight.reshape(-1, self.group_size, weight.shape[2])
+            elif self.bits == 3:
+               zeros = self.qzeros.reshape(self.qzeros.shape[0], self.qzeros.shape[1]//3, 3, 1).expand(-1, -1, -1, 12)
+               zeros = (zeros >> self.wf.unsqueeze(0))
+               zeros[:,:,0,10] = (zeros[:,:,0,10]&0x3) | ((zeros[:,:,1,0] << 2)&0x4)
+               zeros[:,:,1,11] = (zeros[:,:,1,11]&0x1) | ((zeros[:,:,2,0] << 1)&0x6)
+               zeros = zeros & 0x7
+               zeros = torch.cat([zeros[:,:,0,:11], zeros[:,:,1,1:12], zeros[:,:,2,1:11]], dim=2)
+                
+               zeros = zeros + 1
+               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2]) 
+               
+               scales = self.scales
+               scales = scales.reshape(-1, 1, scales.shape[-1])
+                
+               weight = self.qweight.reshape(self.qweight.shape[0]//3, 3, 1, self.qweight.shape[1]).expand(-1, -1, 12, -1)
+               weight = (weight >> self.wf.unsqueeze(-1))&0x7
+               weight[:,0,10] = (weight[:,0,10]&0x3) | ((weight[:,1,0] << 2)&0x4)
+               weight[:,1,11] = (weight[:,1,11]&0x1) | ((weight[:,2,0] << 1)&0x6)
+               weight = weight & 0x7
+               weight = torch.cat([weight[:,0,:11], weight[:,1,1:12], weight[:,2,1:11]], dim=1)
+               weight = weight.reshape(-1, self.group_size, weight.shape[2])
+            else:
+               raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+            weight = (scales * (weight - zeros))
+            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
+
+            out = torch.matmul(x.half(), weight)
+        out = out.half().reshape(out_shape)
+        out = out + self.bias if self.bias is not None else out
+        return out
+
+
+__all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear_old.py` & `auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_cuda.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,254 +1,271 @@
-import math
-from logging import getLogger
-
-import numpy as np
-import torch
-import torch.nn as nn
-import transformers
-
-logger = getLogger(__name__)
-
-try:
-    import autogptq_cuda
-
-    _autogptq_cuda_available = True
-except ImportError:
-    logger.warning('CUDA extension not installed.')
-    _autogptq_cuda_available = False
-
-class QuantLinear(nn.Module):
-    def __init__(
-        self,
-        bits,
-        group_size,
-        infeatures,
-        outfeatures,
-        bias,
-        use_cuda_fp16=True,
-        kernel_switch_threshold=128
-    ):
-
-        super().__init__()
-        if bits not in [2, 3, 4, 8]:
-            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-        self.infeatures = infeatures
-        self.outfeatures = outfeatures
-        self.bits = bits
-        self.group_size = group_size if group_size != -1 else infeatures
-        self.maxq = 2 ** self.bits - 1
-
-        self.register_buffer(
-            'qweight',
-            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'qzeros',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'scales',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
-        )
-        self.register_buffer(
-            'g_idx',
-            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
-        )
-
-        if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
-        else:
-            self.bias = None
-        self.half_indim = self.infeatures // 2
-
-        self.use_cuda_fp16 = use_cuda_fp16 if bits != 8 else False
-        
-        # is performed by unpacking the weights and using torch.matmul
-        if self.bits in [2, 4, 8]:
-            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
-        elif self.bits == 3:
-            self.wf = torch.tensor(
-                [
-                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
-                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
-                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
-                ],
-                dtype=torch.int32
-            ).reshape(1, 3, 12)
-
-        self.kernel_switch_threshold = kernel_switch_threshold
-        self.autogptq_cuda_available = _autogptq_cuda_available
-        if infeatures % 256 != 0 or outfeatures % 256 != 0:
-            self.autogptq_cuda_available = False
-
-    def pack(self, linear, scales, zeros, g_idx):
-        scales = scales.t().contiguous()
-        zeros = zeros.t().contiguous()
-        scale_zeros = zeros * scales
-        self.scales = scales.clone().half()
-        if linear.bias is not None:
-            self.bias = linear.bias.clone().half()
-
-        intweight = []
-        for idx in range(self.infeatures):
-            g_idx = idx // self.group_size
-            intweight.append(
-                torch.round(
-                    (linear.weight.data[:, idx] + scale_zeros[g_idx]) / self.scales[g_idx]
-                ).to(torch.int)[:, None]
-            )
-        intweight = torch.cat(intweight, dim=1)
-        intweight = intweight.t().contiguous()
-        intweight = intweight.numpy().astype(np.uint32)
-
-        i = 0
-        row = 0
-        qweight = np.zeros(
-            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
-        )
-        while row < qweight.shape[0]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                row += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i))
-                i += 10
-                qweight[row] |= intweight[i] << 30
-                row += 1
-                qweight[row] |= (intweight[i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
-                i += 10
-                qweight[row] |= intweight[i] << 31
-                row += 1
-                qweight[row] |= (intweight[i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
-                i += 10
-                row += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight)
-
-        zeros -= 1
-        zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
-        i = 0
-        col = 0
-        while col < qzeros.shape[1]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                col += 1
-            elif self.bits == 3:
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 30
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
-                i += 10
-                qzeros[:, col] |= zeros[:, i] << 31
-                col += 1
-                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
-                i += 1
-                for j in range(i, i + 10):
-                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
-                i += 10
-                col += 1
-            else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
-        qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros)
-
-    def forward(self, x):
-        out_shape = x.shape[:-1] + (self.outfeatures,)
-        x = x.reshape(-1, x.shape[-1])
-        if self.autogptq_cuda_available is True and (
-            self.kernel_switch_threshold is False or x.shape[0] < self.kernel_switch_threshold
-        ):
-            out = torch.zeros(x.shape[0], out_shape[-1], dtype=torch.float, device=x.device)
-            if self.use_cuda_fp16:
-                x = x.half()
-                if self.bits == 2:
-                    autogptq_cuda.vecquant2matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
-                elif self.bits == 3:
-                    autogptq_cuda.vecquant3matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
-                elif self.bits == 4:
-                    autogptq_cuda.vecquant4matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
-
-                else:
-                    raise NotImplementedError("Only 2,3,4 bits are supported.")
-            else:
-                x = x.float()
-                if self.bits == 2:
-                    autogptq_cuda.vecquant2matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
-                elif self.bits == 3:
-                    autogptq_cuda.vecquant3matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
-                elif self.bits == 4:
-                    autogptq_cuda.vecquant4matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
-                elif self.bits == 8:
-                    autogptq_cuda.vecquant8matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
-                else:
-                    raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-        else:
-            if self.wf.device != self.qzeros.device:
-               self.wf = self.wf.to(self.qzeros.device)
-                
-            if self.bits in [2,4,8]:
-               zeros = torch.bitwise_right_shift(torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits), self.wf.unsqueeze(0)).to(torch.int16 if self.bits == 8 else torch.int8)
-               torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
-                   
-               zeros = zeros + 1
-               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
-   
-               scales = self.scales
-               scales = scales.reshape(-1, 1, scales.shape[-1])
-                
-               weight = torch.bitwise_right_shift(torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1), self.wf.unsqueeze(-1)).to(torch.int16 if self.bits == 8 else torch.int8)
-               torch.bitwise_and(weight,(2 ** self.bits) - 1, out=weight)
-               weight = weight.reshape(-1, self.group_size, weight.shape[2])
-            elif self.bits == 3:
-               zeros = self.qzeros.reshape(self.qzeros.shape[0], self.qzeros.shape[1]//3, 3, 1).expand(-1, -1, -1, 12)
-               zeros = (zeros >> self.wf.unsqueeze(0))
-               zeros[:,:,0,10] = (zeros[:,:,0,10]&0x3) | ((zeros[:,:,1,0] << 2)&0x4)
-               zeros[:,:,1,11] = (zeros[:,:,1,11]&0x1) | ((zeros[:,:,2,0] << 1)&0x6)
-               zeros = zeros & 0x7
-               zeros = torch.cat([zeros[:,:,0,:11], zeros[:,:,1,1:12], zeros[:,:,2,1:11]], dim=2)
-                
-               zeros = zeros + 1
-               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2]) 
-               
-               scales = self.scales
-               scales = scales.reshape(-1, 1, scales.shape[-1])
-                
-               weight = self.qweight.reshape(self.qweight.shape[0]//3, 3, 1, self.qweight.shape[1]).expand(-1, -1, 12, -1)
-               weight = (weight >> self.wf.unsqueeze(-1))&0x7
-               weight[:,0,10] = (weight[:,0,10]&0x3) | ((weight[:,1,0] << 2)&0x4)
-               weight[:,1,11] = (weight[:,1,11]&0x1) | ((weight[:,2,0] << 1)&0x6)
-               weight = weight & 0x7
-               weight = torch.cat([weight[:,0,:11], weight[:,1,1:12], weight[:,2,1:11]], dim=1)
-               weight = weight.reshape(-1, self.group_size, weight.shape[2])
-            else:
-               raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-            weight = (scales * (weight - zeros))
-            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
-
-            out = torch.matmul(x.half(), weight)
-        out = out.half().reshape(out_shape)
-        out = out + self.bias if self.bias is not None else out
-        return out
-
-
-__all__ = ["QuantLinear"]
+import math
+from logging import getLogger
+
+import numpy as np
+import torch
+import torch.nn as nn
+import transformers
+
+logger = getLogger(__name__)
+
+try:
+    import autogptq_cuda_256
+    import autogptq_cuda_64
+    _autogptq_cuda_available = True
+except ImportError:
+    logger.warning('CUDA extension not installed.')
+    _autogptq_cuda_available = False
+
+
+
+class QuantLinear(nn.Module):
+    def __init__(
+        self,
+        bits,
+        group_size,
+        infeatures,
+        outfeatures,
+        bias,
+        kernel_switch_threshold=128,
+        trainable=False
+    ):
+        super().__init__()
+        global _autogptq_cuda_available
+
+        if bits not in [2, 3, 4, 8]:
+            raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        if trainable:
+            _autogptq_cuda_available = False
+
+        self.infeatures = infeatures
+        self.outfeatures = outfeatures
+        self.bits = bits
+        self.group_size = group_size if group_size != -1 else infeatures
+        self.maxq = 2 ** self.bits - 1
+
+        self.register_buffer(
+            'qweight',
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'qzeros',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'scales',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
+        )
+        self.register_buffer(
+            'g_idx',
+            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
+        )
+        if bias:
+            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
+        else:
+            self.bias = None
+
+        # is performed by unpacking the weights and using torch.matmul
+        if self.bits in [2, 4, 8]:
+            self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
+        elif self.bits == 3:
+            self.wf = torch.tensor(
+                [
+                    [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
+                    [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
+                    [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
+                ],
+                dtype=torch.int32
+            ).reshape(1, 3, 12)
+
+        self.kernel_switch_threshold = kernel_switch_threshold
+        self.autogptq_cuda_available = _autogptq_cuda_available
+        
+        self.autogptq_cuda = autogptq_cuda_256
+        if infeatures % 256 != 0 or outfeatures % 256 != 0:
+            self.autogptq_cuda = autogptq_cuda_64
+        if infeatures % 64 != 0 or outfeatures % 64 != 0:
+            self.autogptq_cuda_available = False
+
+        self.trainable = trainable
+
+    def pack(self, linear, scales, zeros, g_idx=None):
+        W = linear.weight.data.clone()
+        if isinstance(linear, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(linear, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+
+        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
+
+        scales = scales.t().contiguous()
+        zeros = zeros.t().contiguous()
+        scale_zeros = zeros * scales
+        self.scales = scales.clone().half()
+        if linear.bias is not None:
+            self.bias = linear.bias.clone().half()
+
+        intweight = []
+        for idx in range(self.infeatures):
+            intweight.append(
+                torch.round(
+                    (
+                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
+        intweight = intweight.t().contiguous()
+        intweight = intweight.numpy().astype(np.uint32)
+
+        i = 0
+        row = 0
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
+        while row < qweight.shape[0]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qweight[row] |= intweight[j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                row += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i))
+                i += 10
+                qweight[row] |= intweight[i] << 30
+                row += 1
+                qweight[row] |= (intweight[i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 1)
+                i += 10
+                qweight[row] |= intweight[i] << 31
+                row += 1
+                qweight[row] |= (intweight[i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qweight[row] |= intweight[j] << (3 * (j - i) + 2)
+                i += 10
+                row += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qweight = qweight.astype(np.int32)
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
+        zeros = zeros.numpy().astype(np.uint32)
+        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        i = 0
+        col = 0
+        while col < qzeros.shape[1]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                col += 1
+            elif self.bits == 3:
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i))
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 30
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 2) & 1
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 1)
+                i += 10
+                qzeros[:, col] |= zeros[:, i] << 31
+                col += 1
+                qzeros[:, col] |= (zeros[:, i] >> 1) & 0x3
+                i += 1
+                for j in range(i, i + 10):
+                    qzeros[:, col] |= zeros[:, j] << (3 * (j - i) + 2)
+                i += 10
+                col += 1
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+        qzeros = qzeros.astype(np.int32)
+        self.qzeros = torch.from_numpy(qzeros)
+
+    def forward(self, x: torch.Tensor):
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        x = x.reshape(-1, x.shape[-1])
+        if self.autogptq_cuda_available and (
+            self.kernel_switch_threshold == 0 or x.shape[0] < self.kernel_switch_threshold
+        ):
+            out = torch.zeros((x.shape[0], self.outfeatures), device=x.device, dtype=torch.float32)
+            if self.bits == 2:
+                self.autogptq_cuda.vecquant2matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+            elif self.bits == 3:
+                self.autogptq_cuda.vecquant3matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+            elif self.bits == 4:
+                self.autogptq_cuda.vecquant4matmul(x.half(), self.qweight, out.half(), self.scales, self.qzeros, self.g_idx, self.infeatures // 2)
+            elif self.bits == 8:
+                self.autogptq_cuda.vecquant8matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+        else:
+            if self.wf.device != self.qzeros.device:
+                self.wf = self.wf.to(self.qzeros.device)
+
+            if self.bits in [2, 4, 8]:
+                zeros = torch.bitwise_right_shift(
+                    torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits),
+                    self.wf.unsqueeze(0)
+                ).to(torch.int16 if self.bits == 8 else torch.int8)
+                torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
+
+                zeros = zeros + 1
+                zeros = zeros.reshape(self.scales.shape)
+
+                weight = torch.bitwise_right_shift(
+                    torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1),
+                    self.wf.unsqueeze(-1)
+                ).to(torch.int16 if self.bits == 8 else torch.int8)
+                torch.bitwise_and(weight, (2 ** self.bits) - 1, out=weight)
+            elif self.bits == 3:
+                zeros = self.qzeros.reshape(
+                    self.qzeros.shape[0], self.qzeros.shape[1] // 3, 3, 1
+                ).expand(-1, -1, -1, 12)
+                zeros = (zeros >> self.wf.unsqueeze(0))
+                zeros[:, :, 0, 10] = (zeros[:, :, 0, 10] & 0x3) | ((zeros[:, :, 1, 0] << 2) & 0x4)
+                zeros[:, :, 1, 11] = (zeros[:, :, 1, 11] & 0x1) | ((zeros[:, :, 2, 0] << 1) & 0x6)
+                zeros = zeros & 0x7
+                zeros = torch.cat([zeros[:, :, 0, :11], zeros[:, :, 1, 1:12], zeros[:, :, 2, 1:11]], dim=2)
+
+                zeros = zeros + 1
+                zeros = zeros.reshape(self.scales.shape)
+
+                weight = self.qweight.reshape(
+                    self.qweight.shape[0] // 3, 3, 1, self.qweight.shape[1]
+                ).expand(-1, -1, 12, -1)
+                weight = (weight >> self.wf.unsqueeze(-1)) & 0x7
+                weight[:, 0, 10] = (weight[:, 0, 10] & 0x3) | ((weight[:, 1, 0] << 2) & 0x4)
+                weight[:, 1, 11] = (weight[:, 1, 11] & 0x1) | ((weight[:, 2, 0] << 1) & 0x6)
+                weight = weight & 0x7
+                weight = torch.cat([weight[:, 0, :11], weight[:, 1, 1:12], weight[:, 2, 1:11]], dim=1)
+            else:
+                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
+
+            weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
+            num_itr = self.g_idx.shape[0]//x.shape[-1]
+            if num_itr == 1:
+                weights = (self.scales[self.g_idx.long()] * (weight - zeros[self.g_idx.long()]))
+            else:
+                num_dim = self.g_idx.shape[0]//num_itr
+                weights = []
+                for i in range(num_itr):
+                    scale_i = self.scales[:,i*num_dim:(i+1)*num_dim]
+                    weight_i = weight[:,i*num_dim:(i+1)*num_dim]
+                    zeros_i = zeros[:,i*num_dim:(i+1)*num_dim]
+                    g_idx_i = self.g_idx[i*num_dim:(i+1)*num_dim]
+                    weights.append(scale_i[g_idx_i.long()] * (weight_i - zeros_i[g_idx_i.long()]))
+                weights = torch.cat(weights,dim=1)
+            out = torch.matmul(x.half(), weights)
+        out = out.half().reshape(out_shape)
+        out = out + self.bias if self.bias is not None else out
+        return out
+
+
+__all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/nn_modules/qlinear_triton.py` & `auto_gptq-0.3.0/auto_gptq/nn_modules/qlinear/qlinear_triton.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,171 +1,181 @@
-import math
-import numpy as np
-import torch
-import torch.nn as nn
-import transformers
-from torch.cuda.amp import custom_bwd, custom_fwd
-from logging import getLogger
-
-from .triton_utils.mixin import TritonModuleMixin
-
-logger = getLogger(__name__)
-
-try:
-    from .triton_utils.kernels import quant_matmul_248, transpose_quant_matmul_248, QuantLinearFunction
-except ImportError:
-    logger.error('triton not installed.')
-    raise
-
-
-class QuantLinear(nn.Module, TritonModuleMixin):
-    def __init__(
-        self,
-        bits,
-        group_size,
-        infeatures,
-        outfeatures,
-        bias
-    ):
-        super().__init__()
-        if bits not in [2, 4, 8]:
-            raise NotImplementedError("Only 2,4,8 bits are supported.")
-        if infeatures % 256 != 0 or outfeatures % 256 != 0:
-            raise NotImplementedError("in_feature or out_feature must be divisible by 256.")
-        self.infeatures = infeatures
-        self.outfeatures = outfeatures
-        self.bits = bits
-        self.group_size = group_size if group_size != -1 else infeatures
-        self.maxq = 2 ** self.bits - 1
-
-        self.register_buffer(
-            'qweight',
-            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'qzeros',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
-        )
-        self.register_buffer(
-            'scales',
-            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
-        )
-        self.register_buffer(
-            'g_idx',
-            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
-        )
-        if bias:
-            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
-        else:
-            self.bias = None
-
-    def pack(self, linear, scales, zeros, g_idx=None):
-        W = linear.weight.data.clone()
-        if isinstance(linear, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(linear, transformers.pytorch_utils.Conv1D):
-            W = W.t()
-    
-        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
-
-        scales = scales.t().contiguous()
-        zeros = zeros.t().contiguous()
-        scale_zeros = zeros * scales
-        self.scales = scales.clone().half()
-        if linear.bias is not None:
-            self.bias = linear.bias.clone().half()
-
-        intweight = []
-        for idx in range(self.infeatures):
-            intweight.append(
-                torch.round(
-                    (
-                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
-                ).to(torch.int)[:, None]
-            )
-        intweight = torch.cat(intweight, dim=1)
-        intweight = intweight.t().contiguous()
-        intweight = intweight.numpy().astype(np.uint32)
-
-        i = 0
-        row = 0
-        qweight = np.zeros(
-            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
-        )
-        while row < qweight.shape[0]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qweight[row] |= intweight[j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                row += 1
-            else:
-                raise NotImplementedError("Only 2,4,8 bits are supported.")
-
-        qweight = qweight.astype(np.int32)
-        self.qweight = torch.from_numpy(qweight)
-
-        zeros -= 1
-        zeros = zeros.numpy().astype(np.uint32)
-        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
-        i = 0
-        col = 0
-        while col < qzeros.shape[1]:
-            if self.bits in [2, 4, 8]:
-                for j in range(i, i + (32 // self.bits)):
-                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
-                i += 32 // self.bits
-                col += 1
-            else:
-                raise NotImplementedError("Only 2,4,8 bits are supported.")
-
-        qzeros = qzeros.astype(np.int32)
-        self.qzeros = torch.from_numpy(qzeros)
-
-    def forward(self, x):
-        out_shape = x.shape[:-1] + (self.outfeatures,)
-        out = QuantLinearFunction.apply(
-            x.reshape(-1, x.shape[-1]),
-            self.qweight,
-            self.scales,
-            self.qzeros,
-            self.g_idx,
-            self.bits,
-            self.maxq
-        )
-        out = out.half().reshape(out_shape)
-        out = out + self.bias if self.bias is not None else out
-        return out
-
-    @classmethod
-    def warmup(cls, model, transpose=False, seqlen=2048):
-        """
-        Pre-tunes the quantized kernel
-        """
-        from tqdm import tqdm
-
-        kn_values = {}
-
-        for _, m in model.named_modules():
-            if not isinstance(m, cls):
-                continue
-
-            k = m.infeatures
-            n = m.outfeatures
-
-            if (k, n) not in kn_values:
-                kn_values[(k, n)] = (m.qweight, m.scales, m.qzeros, m.g_idx, m.bits, m.maxq)
-
-        logger.info(f'Found {len(kn_values)} unique KN Linear values.')
-        logger.info('Warming up autotune cache ...')
-        with torch.no_grad():
-            for m in tqdm(range(0, math.ceil(math.log2(seqlen)) + 1)):
-                m = 2 ** m
-                for (k, n), (qweight, scales, qzeros, g_idx, bits, maxq) in kn_values.items():
-                    a = torch.randn(m, k, dtype=torch.float16, device=model.device)
-                    quant_matmul_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
-                    if transpose:
-                        a = torch.randn(m, n, dtype=torch.float16, device=model.device)
-                        transpose_quant_matmul_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
-        del kn_values
-
-
-__all__ = ["QuantLinear"]
+import math
+from logging import getLogger
+
+import numpy as np
+import torch
+import torch.nn as nn
+import transformers
+
+from ..triton_utils.mixin import TritonModuleMixin
+
+logger = getLogger(__name__)
+
+try:
+    from ..triton_utils.kernels import (
+        quant_matmul_248, transpose_quant_matmul_248, quant_matmul_inference_only_248,
+        QuantLinearFunction, QuantLinearInferenceOnlyFunction
+    )
+except ImportError:
+    logger.error('triton not installed.')
+    raise
+
+
+class QuantLinear(nn.Module, TritonModuleMixin):
+    def __init__(
+        self,
+        bits,
+        group_size,
+        infeatures,
+        outfeatures,
+        bias,
+        trainable=False
+    ):
+        super().__init__()
+        if bits not in [2, 4, 8]:
+            raise NotImplementedError("Only 2,4,8 bits are supported.")
+        if infeatures % 32 != 0 or outfeatures % 32 != 0:
+            raise NotImplementedError("in_feature and out_feature must be divisible by 32.")
+        self.infeatures = infeatures
+        self.outfeatures = outfeatures
+        self.bits = bits
+        self.group_size = group_size if group_size != -1 else infeatures
+        self.maxq = 2 ** self.bits - 1
+
+        self.register_buffer(
+            'qweight',
+            torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'qzeros',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
+        )
+        self.register_buffer(
+            'scales',
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
+        )
+        self.register_buffer(
+            'g_idx',
+            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
+        )
+        if bias:
+            self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
+        else:
+            self.bias = None
+
+        self.trainable = trainable
+
+    def pack(self, linear, scales, zeros, g_idx=None):
+        W = linear.weight.data.clone()
+        if isinstance(linear, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(linear, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+    
+        self.g_idx = g_idx.clone() if g_idx is not None else self.g_idx
+
+        scales = scales.t().contiguous()
+        zeros = zeros.t().contiguous()
+        scale_zeros = zeros * scales
+        self.scales = scales.clone().half()
+        if linear.bias is not None:
+            self.bias = linear.bias.clone().half()
+
+        intweight = []
+        for idx in range(self.infeatures):
+            intweight.append(
+                torch.round(
+                    (
+                        W[:, idx] + scale_zeros[self.g_idx[idx]]) / self.scales[self.g_idx[idx]]
+                ).to(torch.int)[:, None]
+            )
+        intweight = torch.cat(intweight, dim=1)
+        intweight = intweight.t().contiguous()
+        intweight = intweight.numpy().astype(np.uint32)
+
+        i = 0
+        row = 0
+        qweight = np.zeros(
+            (intweight.shape[0] // 32 * self.bits, intweight.shape[1]), dtype=np.uint32
+        )
+        while row < qweight.shape[0]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qweight[row] |= intweight[j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                row += 1
+            else:
+                raise NotImplementedError("Only 2,4,8 bits are supported.")
+
+        qweight = qweight.astype(np.int32)
+        self.qweight = torch.from_numpy(qweight)
+
+        zeros -= 1
+        zeros = zeros.numpy().astype(np.uint32)
+        qzeros = np.zeros((zeros.shape[0], zeros.shape[1] // 32 * self.bits), dtype=np.uint32)
+        i = 0
+        col = 0
+        while col < qzeros.shape[1]:
+            if self.bits in [2, 4, 8]:
+                for j in range(i, i + (32 // self.bits)):
+                    qzeros[:, col] |= zeros[:, j] << (self.bits * (j - i))
+                i += 32 // self.bits
+                col += 1
+            else:
+                raise NotImplementedError("Only 2,4,8 bits are supported.")
+
+        qzeros = qzeros.astype(np.int32)
+        self.qzeros = torch.from_numpy(qzeros)
+
+    def forward(self, x):
+        out_shape = x.shape[:-1] + (self.outfeatures,)
+        quant_linear_fn = QuantLinearFunction if self.trainable else QuantLinearInferenceOnlyFunction
+        out = quant_linear_fn.apply(
+            x.reshape(-1, x.shape[-1]),
+            self.qweight,
+            self.scales,
+            self.qzeros,
+            self.g_idx,
+            self.bits,
+            self.maxq
+        )
+        out = out.half().reshape(out_shape)
+        out = out + self.bias if self.bias is not None else out
+        return out
+
+    @classmethod
+    def warmup(cls, model, transpose=False, seqlen=2048):
+        """
+        Pre-tunes the quantized kernel
+        """
+        from tqdm import tqdm
+
+        kn_values = {}
+
+        for _, m in model.named_modules():
+            if not isinstance(m, cls):
+                continue
+
+            k = m.infeatures
+            n = m.outfeatures
+
+            if (k, n) not in kn_values:
+                kn_values[(k, n)] = (m.qweight, m.scales, m.qzeros, m.g_idx, m.bits, m.maxq)
+
+        logger.info(f'Found {len(kn_values)} unique KN Linear values.')
+        logger.info('Warming up autotune cache ...')
+        with torch.no_grad():
+            for m in tqdm(range(0, math.ceil(math.log2(seqlen)) + 1)):
+                m = 2 ** m
+                for (k, n), (qweight, scales, qzeros, g_idx, bits, maxq) in kn_values.items():
+                    if transpose:
+                        a = torch.randn(m, k, dtype=torch.float16, device=model.device)
+                        quant_matmul_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
+                        a = torch.randn(m, n, dtype=torch.float16, device=model.device)
+                        transpose_quant_matmul_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
+                    else:
+                        a = torch.randn(m, k, dtype=torch.float16, device=model.device)
+                        quant_matmul_inference_only_248(a, qweight, scales, qzeros, g_idx, bits, maxq)
+        del kn_values
+
+
+__all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/custom_autotune.py` & `auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-import builtins
-import math
-import time
-from typing import Dict
-
-import triton
-
-
-#  code based https://github.com/fpgaminer/GPTQ-triton
-"""
-Mostly the same as the autotuner in Triton, but with a few changes like using 40 runs instead of 100.
-"""
-
-
-class CustomizedTritonAutoTuner(triton.KernelInterface):
-    def __init__(
-        self,
-        fn,
-        arg_names,
-        configs,
-        key,
-        reset_to_zero,
-        prune_configs_by: Dict = None,
-        nearest_power_of_two: bool = False
-    ):
-        if not configs:
-            self.configs = [triton.Config({}, num_warps=4, num_stages=2)]
-        else:
-            self.configs = configs
-        self.key_idx = [arg_names.index(k) for k in key]
-        self.nearest_power_of_two = nearest_power_of_two
-        self.cache = {}
-        # hook to reset all required tensor to zeros before relaunching a kernel
-        self.hook = lambda args: 0
-        if reset_to_zero is not None:
-            self.reset_idx = [arg_names.index(k) for k in reset_to_zero]
-
-            def _hook(args):
-                for i in self.reset_idx:
-                    args[i].zero_()
-
-            self.hook = _hook
-        self.arg_names = arg_names
-        # prune configs
-        if prune_configs_by:
-            perf_model, top_k = prune_configs_by['perf_model'], prune_configs_by['top_k']
-            if 'early_config_prune' in prune_configs_by:
-                early_config_prune = prune_configs_by['early_config_prune']
-        else:
-            perf_model, top_k, early_config_prune = None, None, None
-        self.perf_model, self.configs_top_k = perf_model, top_k
-        self.early_config_prune = early_config_prune
-        self.fn = fn
-
-    def _bench(self, *args, config, **meta):
-        # check for conflicts, i.e. meta-parameters both provided
-        # as kwargs and by the autotuner
-        conflicts = meta.keys() & config.kwargs.keys()
-        if conflicts:
-            raise ValueError(f"Conflicting meta-parameters: {', '.join(conflicts)}."
-                             " Make sure that you don't re-define auto-tuned symbols.")
-        # augment meta-parameters with tunable ones
-        current = dict(meta, **config.kwargs)
-
-        def kernel_call():
-            if config.pre_hook:
-                config.pre_hook(self.nargs)
-            self.hook(args)
-            self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **current)
-
-        try:
-            # In testings using only 40 reps seems to be close enough and it appears to be what PyTorch uses
-            # PyTorch also sets fast_flush to True, but I didn't see any speedup so I'll leave the default
-            return triton.testing.do_bench(kernel_call, percentiles=(0.5, 0.2, 0.8), rep=40)
-        except triton.compiler.OutOfResources:
-            return (float('inf'), float('inf'), float('inf'))
-
-    def run(self, *args, **kwargs):
-        self.nargs = dict(zip(self.arg_names, args))
-        if len(self.configs) > 1:
-            key = tuple(args[i] for i in self.key_idx)
-
-            # This reduces the amount of autotuning by rounding the keys to the nearest power of two
-            # In my testing this gives decent results, and greatly reduces the amount of tuning required
-            if self.nearest_power_of_two:
-                key = tuple([2 ** int(math.log2(x) + 0.5) for x in key])
-
-            if key not in self.cache:
-                # prune configs
-                pruned_configs = self.prune_configs(kwargs)
-                bench_start = time.time()
-                timings = {config: self._bench(*args, config=config, **kwargs) for config in pruned_configs}
-                bench_end = time.time()
-                self.bench_time = bench_end - bench_start
-                self.cache[key] = builtins.min(timings, key=timings.get)
-                self.hook(args)
-                self.configs_timings = timings
-            config = self.cache[key]
-        else:
-            config = self.configs[0]
-        self.best_config = config
-        if config.pre_hook is not None:
-            config.pre_hook(self.nargs)
-        return self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **kwargs, **config.kwargs)
-
-    def prune_configs(self, kwargs):
-        pruned_configs = self.configs
-        if self.early_config_prune:
-            pruned_configs = self.early_config_prune(self.configs, self.nargs)
-        if self.perf_model:
-            top_k = self.configs_top_k
-            if isinstance(top_k, float) and top_k <= 1.0:
-                top_k = int(len(self.configs) * top_k)
-            if len(pruned_configs) > top_k:
-                est_timing = {
-                    config: self.perf_model(**self.nargs, **kwargs, **config.kwargs, num_stages=config.num_stages,
-                                            num_warps=config.num_warps) for config in pruned_configs}
-                pruned_configs = sorted(est_timing.keys(), key=lambda x: est_timing[x])[:top_k]
-        return pruned_configs
-
-    def warmup(self, *args, **kwargs):
-        self.nargs = dict(zip(self.arg_names, args))
-        for config in self.prune_configs(kwargs):
-            self.fn.warmup(
-                *args,
-                num_warps=config.num_warps,
-                num_stages=config.num_stages,
-                **kwargs,
-                **config.kwargs,
-            )
-        self.nargs = None
-
-
-def autotune(configs, key, prune_configs_by=None, reset_to_zero=None, nearest_power_of_two=False):
-    def decorator(fn):
-        return CustomizedTritonAutoTuner(
-            fn, fn.arg_names, configs, key, reset_to_zero, prune_configs_by, nearest_power_of_two
-        )
-
-    return decorator
-
-
-def matmul248_kernel_config_pruner(configs, nargs):
-    """
-    The main purpose of this function is to shrink BLOCK_SIZE_* when the corresponding dimension is smaller.
-    """
-    m = max(2 ** int(math.ceil(math.log2(nargs['M']))), 16)
-    n = max(2 ** int(math.ceil(math.log2(nargs['N']))), 16)
-    k = max(2 ** int(math.ceil(math.log2(nargs['K']))), 16)
-
-    used = set()
-    for config in configs:
-        block_size_m = min(m, config.kwargs['BLOCK_SIZE_M'])
-        block_size_n = min(n, config.kwargs['BLOCK_SIZE_N'])
-        block_size_k = min(k, config.kwargs['BLOCK_SIZE_K'])
-        group_size_m = config.kwargs['GROUP_SIZE_M']
-
-        if (block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps) in used:
-            continue
-
-        used.add((block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps))
-        yield triton.Config(
-            {
-                'BLOCK_SIZE_M': block_size_m,
-                'BLOCK_SIZE_N': block_size_n,
-                'BLOCK_SIZE_K': block_size_k,
-                'GROUP_SIZE_M': group_size_m
-            },
-            num_stages=config.num_stages,
-            num_warps=config.num_warps
-        )
-
-
-__all__ = ["autotune"]
+import builtins
+import math
+import time
+from typing import Dict
+
+import triton
+
+
+#  code based https://github.com/fpgaminer/GPTQ-triton
+"""
+Mostly the same as the autotuner in Triton, but with a few changes like using 40 runs instead of 100.
+"""
+
+
+class CustomizedTritonAutoTuner(triton.KernelInterface):
+    def __init__(
+        self,
+        fn,
+        arg_names,
+        configs,
+        key,
+        reset_to_zero,
+        prune_configs_by: Dict = None,
+        nearest_power_of_two: bool = False
+    ):
+        if not configs:
+            self.configs = [triton.Config({}, num_warps=4, num_stages=2)]
+        else:
+            self.configs = configs
+        self.key_idx = [arg_names.index(k) for k in key]
+        self.nearest_power_of_two = nearest_power_of_two
+        self.cache = {}
+        # hook to reset all required tensor to zeros before relaunching a kernel
+        self.hook = lambda args: 0
+        if reset_to_zero is not None:
+            self.reset_idx = [arg_names.index(k) for k in reset_to_zero]
+
+            def _hook(args):
+                for i in self.reset_idx:
+                    args[i].zero_()
+
+            self.hook = _hook
+        self.arg_names = arg_names
+        # prune configs
+        if prune_configs_by:
+            perf_model, top_k = prune_configs_by['perf_model'], prune_configs_by['top_k']
+            if 'early_config_prune' in prune_configs_by:
+                early_config_prune = prune_configs_by['early_config_prune']
+        else:
+            perf_model, top_k, early_config_prune = None, None, None
+        self.perf_model, self.configs_top_k = perf_model, top_k
+        self.early_config_prune = early_config_prune
+        self.fn = fn
+
+    def _bench(self, *args, config, **meta):
+        # check for conflicts, i.e. meta-parameters both provided
+        # as kwargs and by the autotuner
+        conflicts = meta.keys() & config.kwargs.keys()
+        if conflicts:
+            raise ValueError(f"Conflicting meta-parameters: {', '.join(conflicts)}."
+                             " Make sure that you don't re-define auto-tuned symbols.")
+        # augment meta-parameters with tunable ones
+        current = dict(meta, **config.kwargs)
+
+        def kernel_call():
+            if config.pre_hook:
+                config.pre_hook(self.nargs)
+            self.hook(args)
+            self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **current)
+
+        try:
+            # In testings using only 40 reps seems to be close enough and it appears to be what PyTorch uses
+            # PyTorch also sets fast_flush to True, but I didn't see any speedup so I'll leave the default
+            return triton.testing.do_bench(kernel_call, percentiles=(0.5, 0.2, 0.8), rep=40)
+        except triton.compiler.OutOfResources:
+            return (float('inf'), float('inf'), float('inf'))
+
+    def run(self, *args, **kwargs):
+        self.nargs = dict(zip(self.arg_names, args))
+        if len(self.configs) > 1:
+            key = tuple(args[i] for i in self.key_idx)
+
+            # This reduces the amount of autotuning by rounding the keys to the nearest power of two
+            # In my testing this gives decent results, and greatly reduces the amount of tuning required
+            if self.nearest_power_of_two:
+                key = tuple([2 ** int(math.log2(x) + 0.5) for x in key])
+
+            if key not in self.cache:
+                # prune configs
+                pruned_configs = self.prune_configs(kwargs)
+                bench_start = time.time()
+                timings = {config: self._bench(*args, config=config, **kwargs) for config in pruned_configs}
+                bench_end = time.time()
+                self.bench_time = bench_end - bench_start
+                self.cache[key] = builtins.min(timings, key=timings.get)
+                self.hook(args)
+                self.configs_timings = timings
+            config = self.cache[key]
+        else:
+            config = self.configs[0]
+        self.best_config = config
+        if config.pre_hook is not None:
+            config.pre_hook(self.nargs)
+        return self.fn.run(*args, num_warps=config.num_warps, num_stages=config.num_stages, **kwargs, **config.kwargs)
+
+    def prune_configs(self, kwargs):
+        pruned_configs = self.configs
+        if self.early_config_prune:
+            pruned_configs = self.early_config_prune(self.configs, self.nargs)
+        if self.perf_model:
+            top_k = self.configs_top_k
+            if isinstance(top_k, float) and top_k <= 1.0:
+                top_k = int(len(self.configs) * top_k)
+            if len(pruned_configs) > top_k:
+                est_timing = {
+                    config: self.perf_model(**self.nargs, **kwargs, **config.kwargs, num_stages=config.num_stages,
+                                            num_warps=config.num_warps) for config in pruned_configs}
+                pruned_configs = sorted(est_timing.keys(), key=lambda x: est_timing[x])[:top_k]
+        return pruned_configs
+
+    def warmup(self, *args, **kwargs):
+        self.nargs = dict(zip(self.arg_names, args))
+        for config in self.prune_configs(kwargs):
+            self.fn.warmup(
+                *args,
+                num_warps=config.num_warps,
+                num_stages=config.num_stages,
+                **kwargs,
+                **config.kwargs,
+            )
+        self.nargs = None
+
+
+def autotune(configs, key, prune_configs_by=None, reset_to_zero=None, nearest_power_of_two=False):
+    def decorator(fn):
+        return CustomizedTritonAutoTuner(
+            fn, fn.arg_names, configs, key, reset_to_zero, prune_configs_by, nearest_power_of_two
+        )
+
+    return decorator
+
+
+def matmul248_kernel_config_pruner(configs, nargs):
+    """
+    The main purpose of this function is to shrink BLOCK_SIZE_* when the corresponding dimension is smaller.
+    """
+    m = max(2 ** int(math.ceil(math.log2(nargs['M']))), 16)
+    n = max(2 ** int(math.ceil(math.log2(nargs['N']))), 16)
+    k = max(2 ** int(math.ceil(math.log2(nargs['K']))), 16)
+
+    used = set()
+    for config in configs:
+        block_size_m = min(m, config.kwargs['BLOCK_SIZE_M'])
+        block_size_n = min(n, config.kwargs['BLOCK_SIZE_N'])
+        block_size_k = min(k, config.kwargs['BLOCK_SIZE_K'])
+        group_size_m = config.kwargs['GROUP_SIZE_M']
+
+        if (block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps) in used:
+            continue
+
+        used.add((block_size_m, block_size_n, block_size_k, group_size_m, config.num_stages, config.num_warps))
+        yield triton.Config(
+            {
+                'BLOCK_SIZE_M': block_size_m,
+                'BLOCK_SIZE_N': block_size_n,
+                'BLOCK_SIZE_K': block_size_k,
+                'GROUP_SIZE_M': group_size_m
+            },
+            num_stages=config.num_stages,
+            num_warps=config.num_warps
+        )
+
+
+__all__ = ["autotune"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/nn_modules/triton_utils/kernels.py` & `auto_gptq-0.3.0/auto_gptq/nn_modules/triton_utils/kernels.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,416 +1,402 @@
-import torch
-from torch.cuda.amp import custom_bwd, custom_fwd
-from logging import getLogger
-
-import triton
-import triton.language as tl
-
-from . import custom_autotune
-
-logger = getLogger(__name__)
-
-
-# code based https://github.com/fpgaminer/GPTQ-triton
-
-@custom_autotune.autotune(
-    configs=[
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 256,
-                'BLOCK_SIZE_K': 32,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 128,
-                'BLOCK_SIZE_N': 128,
-                'BLOCK_SIZE_K': 32,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 128,
-                'BLOCK_SIZE_K': 32,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 128,
-                'BLOCK_SIZE_N': 32,
-                'BLOCK_SIZE_K': 32,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 64,
-                'BLOCK_SIZE_K': 32,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 128,
-                'BLOCK_SIZE_K': 32,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=2,
-            num_warps=8
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 64,
-                'BLOCK_SIZE_K': 64,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=3,
-            num_warps=8
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 32,
-                'BLOCK_SIZE_N': 32,
-                'BLOCK_SIZE_K': 128,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=2,
-            num_warps=4
-        ),
-    ],
-    key=['M', 'N', 'K'],
-    nearest_power_of_two=True,
-    prune_configs_by={
-        'early_config_prune': custom_autotune.matmul248_kernel_config_pruner,
-        'perf_model': None,
-        'top_k': None,
-    },
-)
-@triton.jit
-def quant_matmul_248_kernel(
-    a_ptr, b_ptr, c_ptr,
-    scales_ptr, zeros_ptr, g_ptr,
-    M, N, K,
-    bits, maxq,
-    stride_am, stride_ak,
-    stride_bk, stride_bn,
-    stride_cm, stride_cn,
-    stride_scales, stride_zeros,
-    BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
-    GROUP_SIZE_M: tl.constexpr
-):
-    """
-    Compute the matrix multiplication C = A x B.
-    A is of shape (M, K) float16
-    B is of shape (K//8, N) int32
-    C is of shape (M, N) float16
-    scales is of shape (G, N) float16
-    zeros is of shape (G, N) float16
-    g_ptr is of shape (K) int32
-    """
-    infearure_per_bits = 32 // bits
-
-    pid = tl.program_id(axis=0)
-    num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
-    num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
-    num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
-    num_pid_in_group = GROUP_SIZE_M * num_pid_n
-    group_id = pid // num_pid_in_group
-    first_pid_m = group_id * GROUP_SIZE_M
-    group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
-    pid_m = first_pid_m + (pid % group_size_m)
-    pid_n = (pid % num_pid_in_group) // group_size_m
-
-    offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
-    offs_bn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
-    offs_k = tl.arange(0, BLOCK_SIZE_K)
-    a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_k[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
-    a_mask = (offs_am[:, None] < M)
-    # b_ptrs is set up such that it repeats elements along the K axis 8 times
-    b_ptrs = b_ptr + (
-        (offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn
-    )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
-    g_ptrs = g_ptr + offs_k
-    # shifter is used to extract the N bits of each element in the 32-bit word from B
-    scales_ptrs = scales_ptr + offs_bn[None, :]
-    zeros_ptrs = zeros_ptr + (offs_bn[None, :] // infearure_per_bits)
-
-    shifter = (offs_k % infearure_per_bits) * bits
-    zeros_shifter = (offs_bn % infearure_per_bits) * bits
-    accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
-
-    for k in range(0, num_pid_k):
-        g_idx = tl.load(g_ptrs)
-
-        # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
-        scales = tl.load(scales_ptrs + g_idx[:, None] * stride_scales)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-        zeros = tl.load(zeros_ptrs + g_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-
-        zeros = (zeros >> zeros_shifter[None, :]) & maxq
-        zeros = (zeros + 1)
-
-        a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
-        b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
-
-        # Now we need to unpack b (which is N-bit values) into 32-bit values
-        b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
-        b = (b - zeros) * scales  # Scale and shift
-
-        accumulator += tl.dot(a, b)
-        a_ptrs += BLOCK_SIZE_K
-        b_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
-        g_ptrs += BLOCK_SIZE_K
-
-    c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bn[None, :]
-    c_mask = (offs_am[:, None] < M) & (offs_bn[None, :] < N)
-    tl.store(c_ptrs, accumulator, mask=c_mask)
-
-
-@custom_autotune.autotune(
-    configs=[
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 32,
-                'BLOCK_SIZE_K': 256,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 128,
-                'BLOCK_SIZE_N': 32,
-                'BLOCK_SIZE_K': 128,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 32,
-                'BLOCK_SIZE_K': 128,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 128,
-                'BLOCK_SIZE_N': 32,
-                'BLOCK_SIZE_K': 32,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 32,
-                'BLOCK_SIZE_K': 64,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=4,
-            num_warps=4
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 32,
-                'BLOCK_SIZE_K': 128,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=2,
-            num_warps=8
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 64,
-                'BLOCK_SIZE_N': 64,
-                'BLOCK_SIZE_K': 64,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=3,
-            num_warps=8
-        ),
-        triton.Config(
-            {
-                'BLOCK_SIZE_M': 32,
-                'BLOCK_SIZE_N': 128,
-                'BLOCK_SIZE_K': 32,
-                'GROUP_SIZE_M': 8
-            },
-            num_stages=2,
-            num_warps=4
-        ),
-    ],
-    key=['M', 'N', 'K'],
-    nearest_power_of_two=True
-)
-@triton.jit
-def transpose_quant_matmul_248_kernel(
-    a_ptr, b_ptr, c_ptr,
-    scales_ptr, zeros_ptr, g_ptr,
-    M, N, K,
-    bits, maxq,
-    stride_am, stride_ak,
-    stride_bk, stride_bn,
-    stride_cm, stride_cn,
-    stride_scales, stride_zeros,
-    BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
-    GROUP_SIZE_M: tl.constexpr
-):
-    """
-    Compute the matrix multiplication C = A x B.
-    A is of shape (M, N) float16
-    B is of shape (K//8, N) int32
-    C is of shape (M, K) float16
-    scales is of shape (G, N) float16
-    zeros is of shape (G, N) float16
-    g_ptr is of shape (K) int32
-    """
-    infearure_per_bits = 32 // bits
-
-    pid = tl.program_id(axis=0)
-    num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
-    num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
-    num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
-    num_pid_in_group = GROUP_SIZE_M * num_pid_k
-    group_id = pid // num_pid_in_group
-    first_pid_m = group_id * GROUP_SIZE_M
-    group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
-    pid_m = first_pid_m + (pid % group_size_m)
-    pid_k = (pid % num_pid_in_group) // group_size_m
-
-    offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
-    offs_bk = pid_k * BLOCK_SIZE_K + tl.arange(0, BLOCK_SIZE_K)
-    offs_n = tl.arange(0, BLOCK_SIZE_N)
-    a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_n[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
-    a_mask = (offs_am[:, None] < M)
-    # b_ptrs is set up such that it repeats elements along the K axis 8 times
-    b_ptrs = b_ptr + (
-        (offs_bk[:, None] // infearure_per_bits) * stride_bk + offs_n[None, :] * stride_bn
-    )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
-    g_ptrs = g_ptr + offs_bk
-    g_idx = tl.load(g_ptrs)
-
-    # shifter is used to extract the N bits of each element in the 32-bit word from B
-    scales_ptrs = scales_ptr + offs_n[None, :] + g_idx[:, None] * stride_scales
-    zeros_ptrs = zeros_ptr + (offs_n[None, :] // infearure_per_bits) + g_idx[:, None] * stride_zeros
-
-    shifter = (offs_bk % infearure_per_bits) * bits
-    zeros_shifter = (offs_n % infearure_per_bits) * bits
-    accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_K), dtype=tl.float32)
-
-    for k in range(0, num_pid_n):
-        # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
-        scales = tl.load(scales_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-        zeros = tl.load(zeros_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
-
-        zeros = (zeros >> zeros_shifter[None, :]) & maxq
-        zeros = (zeros + 1)
-
-        a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
-        b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
-
-        # Now we need to unpack b (which is N-bit values) into 32-bit values
-        b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
-        b = (b - zeros) * scales  # Scale and shift
-        b = tl.trans(b)
-
-        accumulator += tl.dot(a, b)
-        a_ptrs += BLOCK_SIZE_N
-        b_ptrs += BLOCK_SIZE_N
-        scales_ptrs += BLOCK_SIZE_N
-        zeros_ptrs += (BLOCK_SIZE_N // infearure_per_bits)
-
-    c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bk[None, :]
-    c_mask = (offs_am[:, None] < M) & (offs_bk[None, :] < K)
-    tl.store(c_ptrs, accumulator, mask=c_mask)
-
-
-@triton.jit
-def silu(x):
-    return x * tl.sigmoid(x)
-
-
-
-def quant_matmul_248(input, qweight, scales, qzeros, g_idx, bits, maxq):
-    with torch.cuda.device(input.device):
-        output = torch.empty((input.shape[0], qweight.shape[1]), device=input.device, dtype=input.dtype)
-        grid = lambda META: (
-            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(qweight.shape[1], META['BLOCK_SIZE_N']),
-        )
-        quant_matmul_248_kernel[grid](
-            input, qweight, output,
-            scales.to(input.dtype), qzeros, g_idx,
-            input.shape[0], qweight.shape[1], input.shape[1],
-            bits, maxq,
-            input.stride(0), input.stride(1),
-            qweight.stride(0), qweight.stride(1),
-            output.stride(0), output.stride(1),
-            scales.stride(0), qzeros.stride(0)
-        )
-        return output
-
-
-def transpose_quant_matmul_248(input, qweight, scales, qzeros, g_idx, bits, maxq):
-    with torch.cuda.device(input.device):
-        output_dim = (qweight.shape[0] * 32) // bits
-        output = torch.empty((input.shape[0], output_dim), device=input.device, dtype=input.dtype)
-        grid = lambda META: (
-            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(output_dim, META['BLOCK_SIZE_K']),)
-        transpose_quant_matmul_248_kernel[grid](
-            input, qweight, output,
-            scales.to(input.dtype), qzeros, g_idx,
-            input.shape[0], qweight.shape[1], output_dim,
-            bits, maxq,
-            input.stride(0), input.stride(1),
-            qweight.stride(0), qweight.stride(1),
-            output.stride(0), output.stride(1),
-            scales.stride(0), qzeros.stride(0)
-        )
-        return output
-
-
-class QuantLinearFunction(torch.autograd.Function):
-    @staticmethod
-    @custom_fwd
-    def forward(ctx, input, qweight, scales, qzeros, g_idx, bits, maxq):
-        output = quant_matmul_248(input, qweight, scales, qzeros, g_idx, bits, maxq)
-        ctx.save_for_backward(qweight, scales, qzeros, g_idx)
-        ctx.bits, ctx.maxq = bits, maxq
-        return output
-
-    @staticmethod
-    @custom_bwd
-    def backward(ctx, grad_output):
-        qweight, scales, qzeros, g_idx = ctx.saved_tensors
-        bits, maxq = ctx.bits, ctx.maxq
-        grad_input = None
-
-        if ctx.needs_input_grad[0]:
-            grad_input = transpose_quant_matmul_248(grad_output, qweight, scales, qzeros, g_idx, bits, maxq)
-        return grad_input, None, None, None, None, None, None
+import torch
+from torch.cuda.amp import custom_bwd, custom_fwd
+from logging import getLogger
+
+import triton
+import triton.language as tl
+
+from . import custom_autotune
+
+logger = getLogger(__name__)
+
+
+# code based https://github.com/fpgaminer/GPTQ-triton
+
+@custom_autotune.autotune(
+    configs=[
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 64,
+                'BLOCK_SIZE_N': 256,
+                'BLOCK_SIZE_K': 32,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 128,
+                'BLOCK_SIZE_N': 128,
+                'BLOCK_SIZE_K': 32,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 64,
+                'BLOCK_SIZE_N': 128,
+                'BLOCK_SIZE_K': 32,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 128,
+                'BLOCK_SIZE_N': 32,
+                'BLOCK_SIZE_K': 32,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 64,
+                'BLOCK_SIZE_N': 64,
+                'BLOCK_SIZE_K': 32,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 64,
+                'BLOCK_SIZE_N': 128,
+                'BLOCK_SIZE_K': 32,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=2,
+            num_warps=8
+        )
+    ],
+    key=['M', 'N', 'K'],
+    nearest_power_of_two=True,
+    prune_configs_by={
+        'early_config_prune': custom_autotune.matmul248_kernel_config_pruner,
+        'perf_model': None,
+        'top_k': None,
+    },
+)
+@triton.jit
+def quant_matmul_248_kernel(
+    a_ptr, b_ptr, c_ptr,
+    scales_ptr, zeros_ptr, g_ptr,
+    M, N, K,
+    bits, maxq,
+    stride_am, stride_ak,
+    stride_bk, stride_bn,
+    stride_cm, stride_cn,
+    stride_scales, stride_zeros,
+    BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
+    GROUP_SIZE_M: tl.constexpr
+):
+    """
+    Compute the matrix multiplication C = A x B.
+    A is of shape (M, K) float16
+    B is of shape (K//8, N) int32
+    C is of shape (M, N) float16
+    scales is of shape (G, N) float16
+    zeros is of shape (G, N) float16
+    g_ptr is of shape (K) int32
+    """
+    infearure_per_bits = 32 // bits
+
+    pid = tl.program_id(axis=0)
+    num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
+    num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
+    num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
+    num_pid_in_group = GROUP_SIZE_M * num_pid_n
+    group_id = pid // num_pid_in_group
+    first_pid_m = group_id * GROUP_SIZE_M
+    group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
+    pid_m = first_pid_m + (pid % group_size_m)
+    pid_n = (pid % num_pid_in_group) // group_size_m
+
+    offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
+    offs_bn = pid_n * BLOCK_SIZE_N + tl.arange(0, BLOCK_SIZE_N)
+    offs_k = tl.arange(0, BLOCK_SIZE_K)
+    a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_k[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
+    a_mask = (offs_am[:, None] < M)
+    # b_ptrs is set up such that it repeats elements along the K axis 8 times
+    b_ptrs = b_ptr + (
+        (offs_k[:, None] // infearure_per_bits) * stride_bk + offs_bn[None, :] * stride_bn
+    )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
+    g_ptrs = g_ptr + offs_k
+    # shifter is used to extract the N bits of each element in the 32-bit word from B
+    scales_ptrs = scales_ptr + offs_bn[None, :]
+    zeros_ptrs = zeros_ptr + (offs_bn[None, :] // infearure_per_bits)
+
+    shifter = (offs_k % infearure_per_bits) * bits
+    zeros_shifter = (offs_bn % infearure_per_bits) * bits
+    accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_N), dtype=tl.float32)
+
+    for k in range(0, num_pid_k):
+        g_idx = tl.load(g_ptrs)
+
+        # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
+        scales = tl.load(scales_ptrs + g_idx[:, None] * stride_scales)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+        zeros = tl.load(zeros_ptrs + g_idx[:, None] * stride_zeros)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+
+        zeros = (zeros >> zeros_shifter[None, :]) & maxq
+        zeros = (zeros + 1)
+
+        a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_K)
+        b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
+
+        # Now we need to unpack b (which is N-bit values) into 32-bit values
+        b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
+        b = (b - zeros) * scales  # Scale and shift
+
+        accumulator += tl.dot(a, b)
+        a_ptrs += BLOCK_SIZE_K
+        b_ptrs += (BLOCK_SIZE_K // infearure_per_bits) * stride_bk
+        g_ptrs += BLOCK_SIZE_K
+
+    c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bn[None, :]
+    c_mask = (offs_am[:, None] < M) & (offs_bn[None, :] < N)
+    tl.store(c_ptrs, accumulator, mask=c_mask)
+
+
+@custom_autotune.autotune(
+    configs=[
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 64,
+                'BLOCK_SIZE_N': 32,
+                'BLOCK_SIZE_K': 256,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 128,
+                'BLOCK_SIZE_N': 32,
+                'BLOCK_SIZE_K': 128,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 64,
+                'BLOCK_SIZE_N': 32,
+                'BLOCK_SIZE_K': 128,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 128,
+                'BLOCK_SIZE_N': 32,
+                'BLOCK_SIZE_K': 32,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 64,
+                'BLOCK_SIZE_N': 32,
+                'BLOCK_SIZE_K': 64,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=4,
+            num_warps=4
+        ),
+        triton.Config(
+            {
+                'BLOCK_SIZE_M': 64,
+                'BLOCK_SIZE_N': 32,
+                'BLOCK_SIZE_K': 128,
+                'GROUP_SIZE_M': 8
+            },
+            num_stages=2,
+            num_warps=8
+        )
+    ],
+    key=['M', 'N', 'K'],
+    nearest_power_of_two=True
+)
+@triton.jit
+def transpose_quant_matmul_248_kernel(
+    a_ptr, b_ptr, c_ptr,
+    scales_ptr, zeros_ptr, g_ptr,
+    M, N, K,
+    bits, maxq,
+    stride_am, stride_ak,
+    stride_bk, stride_bn,
+    stride_cm, stride_cn,
+    stride_scales, stride_zeros,
+    BLOCK_SIZE_M: tl.constexpr, BLOCK_SIZE_N: tl.constexpr, BLOCK_SIZE_K: tl.constexpr,
+    GROUP_SIZE_M: tl.constexpr
+):
+    """
+    Compute the matrix multiplication C = A x B.
+    A is of shape (M, N) float16
+    B is of shape (K//8, N) int32
+    C is of shape (M, K) float16
+    scales is of shape (G, N) float16
+    zeros is of shape (G, N) float16
+    g_ptr is of shape (K) int32
+    """
+    infearure_per_bits = 32 // bits
+
+    pid = tl.program_id(axis=0)
+    num_pid_m = tl.cdiv(M, BLOCK_SIZE_M)
+    num_pid_k = tl.cdiv(K, BLOCK_SIZE_K)
+    num_pid_n = tl.cdiv(N, BLOCK_SIZE_N)
+    num_pid_in_group = GROUP_SIZE_M * num_pid_k
+    group_id = pid // num_pid_in_group
+    first_pid_m = group_id * GROUP_SIZE_M
+    group_size_m = min(num_pid_m - first_pid_m, GROUP_SIZE_M)
+    pid_m = first_pid_m + (pid % group_size_m)
+    pid_k = (pid % num_pid_in_group) // group_size_m
+
+    offs_am = pid_m * BLOCK_SIZE_M + tl.arange(0, BLOCK_SIZE_M)
+    offs_bk = pid_k * BLOCK_SIZE_K + tl.arange(0, BLOCK_SIZE_K)
+    offs_n = tl.arange(0, BLOCK_SIZE_N)
+    a_ptrs = a_ptr + (offs_am[:, None] * stride_am + offs_n[None, :] * stride_ak)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
+    a_mask = (offs_am[:, None] < M)
+    # b_ptrs is set up such that it repeats elements along the K axis 8 times
+    b_ptrs = b_ptr + (
+        (offs_bk[:, None] // infearure_per_bits) * stride_bk + offs_n[None, :] * stride_bn
+    )  # (BLOCK_SIZE_K, BLOCK_SIZE_N)
+    g_ptrs = g_ptr + offs_bk
+    g_idx = tl.load(g_ptrs)
+
+    # shifter is used to extract the N bits of each element in the 32-bit word from B
+    scales_ptrs = scales_ptr + offs_n[None, :] + g_idx[:, None] * stride_scales
+    zeros_ptrs = zeros_ptr + (offs_n[None, :] // infearure_per_bits) + g_idx[:, None] * stride_zeros
+
+    shifter = (offs_bk % infearure_per_bits) * bits
+    zeros_shifter = (offs_n % infearure_per_bits) * bits
+    accumulator = tl.zeros((BLOCK_SIZE_M, BLOCK_SIZE_K), dtype=tl.float32)
+
+    for k in range(0, num_pid_n):
+        # Fetch scales and zeros; these are per-outfeature and thus reused in the inner loop
+        scales = tl.load(scales_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+        zeros = tl.load(zeros_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N,)
+
+        zeros = (zeros >> zeros_shifter[None, :]) & maxq
+        zeros = (zeros + 1)
+
+        a = tl.load(a_ptrs, mask=a_mask, other=0.)  # (BLOCK_SIZE_M, BLOCK_SIZE_N)
+        b = tl.load(b_ptrs)  # (BLOCK_SIZE_K, BLOCK_SIZE_N), but repeated
+
+        # Now we need to unpack b (which is N-bit values) into 32-bit values
+        b = (b >> shifter[:, None]) & maxq  # Extract the N-bit values
+        b = (b - zeros) * scales  # Scale and shift
+        b = tl.trans(b)
+
+        accumulator += tl.dot(a, b)
+        a_ptrs += BLOCK_SIZE_N
+        b_ptrs += BLOCK_SIZE_N
+        scales_ptrs += BLOCK_SIZE_N
+        zeros_ptrs += (BLOCK_SIZE_N // infearure_per_bits)
+
+    c_ptrs = c_ptr + stride_cm * offs_am[:, None] + stride_cn * offs_bk[None, :]
+    c_mask = (offs_am[:, None] < M) & (offs_bk[None, :] < K)
+    tl.store(c_ptrs, accumulator, mask=c_mask)
+
+
+@triton.jit
+def silu(x):
+    return x * tl.sigmoid(x)
+
+
+def quant_matmul_248(input, qweight, scales, qzeros, g_idx, bits, maxq):
+    with torch.cuda.device(input.device):
+        output = torch.empty((input.shape[0], qweight.shape[1]), device=input.device, dtype=input.dtype)
+        grid = lambda META: (
+            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(qweight.shape[1], META['BLOCK_SIZE_N']),
+        )
+        quant_matmul_248_kernel[grid](
+            input, qweight, output,
+            scales.to(input.dtype), qzeros, g_idx,
+            input.shape[0], qweight.shape[1], input.shape[1],
+            bits, maxq,
+            input.stride(0), input.stride(1),
+            qweight.stride(0), qweight.stride(1),
+            output.stride(0), output.stride(1),
+            scales.stride(0), qzeros.stride(0)
+        )
+        return output
+
+
+def transpose_quant_matmul_248(input, qweight, scales, qzeros, g_idx, bits, maxq):
+    with torch.cuda.device(input.device):
+        output_dim = (qweight.shape[0] * 32) // bits
+        output = torch.empty((input.shape[0], output_dim), device=input.device, dtype=input.dtype)
+        grid = lambda META: (
+            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(output_dim, META['BLOCK_SIZE_K']),)
+        transpose_quant_matmul_248_kernel[grid](
+            input, qweight, output,
+            scales.to(input.dtype), qzeros, g_idx,
+            input.shape[0], qweight.shape[1], output_dim,
+            bits, maxq,
+            input.stride(0), input.stride(1),
+            qweight.stride(0), qweight.stride(1),
+            output.stride(0), output.stride(1),
+            scales.stride(0), qzeros.stride(0)
+        )
+        return output
+
+
+class QuantLinearFunction(torch.autograd.Function):
+    @staticmethod
+    @custom_fwd
+    def forward(ctx, input, qweight, scales, qzeros, g_idx, bits, maxq):
+        output = quant_matmul_248(input, qweight, scales, qzeros, g_idx, bits, maxq)
+        ctx.save_for_backward(qweight, scales, qzeros, g_idx)
+        ctx.bits, ctx.maxq = bits, maxq
+        return output
+
+    @staticmethod
+    @custom_bwd
+    def backward(ctx, grad_output):
+        qweight, scales, qzeros, g_idx = ctx.saved_tensors
+        bits, maxq = ctx.bits, ctx.maxq
+        grad_input = None
+
+        if ctx.needs_input_grad[0]:
+            grad_input = transpose_quant_matmul_248(grad_output, qweight, scales, qzeros, g_idx, bits, maxq)
+        return grad_input, None, None, None, None, None, None
+
+
+def quant_matmul_inference_only_248(input, qweight, scales, qzeros, g_idx, bits, maxq):
+    with torch.cuda.device(input.device):
+        output = torch.empty((input.shape[0], qweight.shape[1]), device=input.device, dtype=torch.float16)
+        grid = lambda META: (
+            triton.cdiv(input.shape[0], META['BLOCK_SIZE_M']) * triton.cdiv(qweight.shape[1], META['BLOCK_SIZE_N']),
+        )
+        quant_matmul_248_kernel[grid](
+            input, qweight, output,
+            scales, qzeros, g_idx,
+            input.shape[0], qweight.shape[1], input.shape[1],
+            bits, maxq,
+            input.stride(0), input.stride(1),
+            qweight.stride(0), qweight.stride(1),
+            output.stride(0), output.stride(1),
+            scales.stride(0), qzeros.stride(0)
+        )
+        return output
+
+
+class QuantLinearInferenceOnlyFunction(torch.autograd.Function):
+    @staticmethod
+    @custom_fwd(cast_inputs=torch.float16)
+    def forward(ctx, input, qweight, scales, qzeros, g_idx, bits, maxq):
+        output = quant_matmul_248(input, qweight, scales, qzeros, g_idx, bits, maxq)
+        return output
```

### Comparing `auto_gptq-0.2.2/auto_gptq/quantization/gptq.py` & `auto_gptq-0.3.0/auto_gptq/quantization/gptq.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-import math
-import os
-import time
-from logging import getLogger
-
-import torch
-import torch.nn as nn
-import transformers
-
-from .quantizer import Quantizer
-
-
-logger = getLogger(__name__)
-
-torch.backends.cuda.matmul.allow_tf32 = False
-torch.backends.cudnn.allow_tf32 = False
-
-
-class GPTQ:
-    def __init__(self, layer):
-        self.layer = layer
-        self.dev = self.layer.weight.device
-        W = layer.weight.data.clone()
-        if isinstance(self.layer, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(self.layer, transformers.pytorch_utils.Conv1D):
-            W = W.t()
-        self.rows = W.shape[0]
-        self.columns = W.shape[1]
-        self.H = torch.zeros((self.columns, self.columns), device=self.dev)
-        self.nsamples = 0
-        self.quantizer = Quantizer()
-
-    def add_batch(self, inp, out):
-        if os.environ.get("DEBUG"):
-            self.inp1 = inp
-            self.out1 = out
-        if len(inp.shape) == 2:
-            inp = inp.unsqueeze(0)
-        tmp = inp.shape[0]
-        if isinstance(self.layer, nn.Linear) or isinstance(self.layer, transformers.Conv1D):
-            if len(inp.shape) == 3:
-                inp = inp.reshape((-1, inp.shape[-1]))
-            inp = inp.t()
-        if isinstance(self.layer, nn.Conv2d):
-            unfold = nn.Unfold(
-                self.layer.kernel_size,
-                dilation=self.layer.dilation,
-                padding=self.layer.padding,
-                stride=self.layer.stride
-            )
-            inp = unfold(inp)
-            inp = inp.permute([1, 0, 2])
-            inp = inp.flatten(1)
-        self.H *= self.nsamples / (self.nsamples + tmp)
-        self.nsamples += tmp
-        # inp = inp.float()
-        inp = math.sqrt(2 / self.nsamples) * inp.float()
-        # self.H += 2 / self.nsamples * inp.matmul(inp.t())
-        self.H += inp.matmul(inp.t())
-
-    def fasterquant(
-        self, blocksize=128, percdamp=.01, group_size=-1, actorder=False
-    ):
-        W = self.layer.weight.data.clone()
-        if isinstance(self.layer, nn.Conv2d):
-            W = W.flatten(1)
-        if isinstance(self.layer, transformers.Conv1D):
-            W = W.t()
-        W = W.float()
-
-        tick = time.time()
-
-        if not self.quantizer.ready():
-            self.quantizer.find_params(W, weight=True)
-
-        H = self.H
-        del self.H
-        dead = torch.diag(H) == 0
-        H[dead, dead] = 1
-        W[:, dead] = 0
-
-        if actorder:
-            perm = torch.argsort(torch.diag(H), descending=True)
-            W = W[:, perm]
-            H = H[perm][:, perm]
-
-        Losses = torch.zeros_like(W)
-        Q = torch.zeros_like(W)
-
-        damp = percdamp * torch.mean(torch.diag(H))
-        diag = torch.arange(self.columns, device=self.dev)
-        H[diag, diag] += damp
-        H = torch.linalg.cholesky(H)
-        H = torch.cholesky_inverse(H)
-        H = torch.linalg.cholesky(H, upper=True)
-        Hinv = H
-
-        g_idx = []
-        scale = []
-        zero = []
-        now_idx = 1
-
-        for i1 in range(0, self.columns, blocksize):
-            i2 = min(i1 + blocksize, self.columns)
-            count = i2 - i1
-
-            W1 = W[:, i1:i2].clone()
-            Q1 = torch.zeros_like(W1)
-            Err1 = torch.zeros_like(W1)
-            Losses1 = torch.zeros_like(W1)
-            Hinv1 = Hinv[i1:i2, i1:i2]
-
-            for i in range(count):
-                w = W1[:, i]
-                d = Hinv1[i, i]
-
-                if group_size != -1:
-                    if (i1 + i) % group_size == 0:
-                        self.quantizer.find_params(W[:, (i1 + i):(i1 + i + group_size)], weight=True)
-
-                    if ((i1 + i) // group_size) - now_idx == -1:
-                        scale.append(self.quantizer.scale)
-                        zero.append(self.quantizer.zero)
-                        now_idx += 1
-
-                q = self.quantizer.quantize(w.unsqueeze(1)).flatten()
-                Q1[:, i] = q
-                Losses1[:, i] = (w - q) ** 2 / d ** 2
-
-                err1 = (w - q) / d
-                W1[:, i:] -= err1.unsqueeze(1).matmul(Hinv1[i, i:].unsqueeze(0))
-                Err1[:, i] = err1
-
-            Q[:, i1:i2] = Q1
-            Losses[:, i1:i2] = Losses1 / 2
-
-            W[:, i2:] -= Err1.matmul(Hinv[i1:i2, i2:])
-
-            if os.environ.get("DEBUG"):
-                self.layer.weight.data[:, :i2] = Q[:, :i2]
-                self.layer.weight.data[:, i2:] = W[:, i2:]
-                logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
-                logger.debug(torch.sum(Losses))
-
-        torch.cuda.synchronize()
-        logger.info(f'duration: {(time.time() - tick)}')
-        logger.info(f'avg loss: {torch.sum(Losses).item() / self.nsamples}')
-
-        group_size = group_size if group_size != -1 else self.columns
-        g_idx = [i // group_size for i in range(self.columns)]
-        g_idx = torch.tensor(g_idx, dtype=torch.int32, device=Q.device)
-        if actorder:
-            invperm = torch.argsort(perm)
-            Q = Q[:, invperm]
-            g_idx = g_idx[invperm]
-
-        if isinstance(self.layer, transformers.Conv1D):
-            Q = Q.t()
-        self.layer.weight.data = Q.reshape(self.layer.weight.shape).type_as(self.layer.weight.data)
-        if os.environ.get("DEBUG"):
-            logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
-
-        if scale == []:
-            scale.append(self.quantizer.scale)
-            zero.append(self.quantizer.zero)
-        scale = torch.cat(scale, dim=1)
-        zero = torch.cat(zero, dim=1)
-        return scale, zero, g_idx
-
-    def free(self):
-        if os.environ.get("DEBUG"):
-            self.inp1 = None
-            self.out1 = None
-        self.H = None
-        self.Losses = None
-        self.Trace = None
-        torch.cuda.empty_cache()
-
-
-__all__ = ["GPTQ"]
+import math
+import os
+import time
+from logging import getLogger
+
+import torch
+import torch.nn as nn
+import transformers
+
+from .quantizer import Quantizer
+
+
+logger = getLogger(__name__)
+
+torch.backends.cuda.matmul.allow_tf32 = False
+torch.backends.cudnn.allow_tf32 = False
+
+
+class GPTQ:
+    def __init__(self, layer):
+        self.layer = layer
+        self.dev = self.layer.weight.device
+        W = layer.weight.data.clone()
+        if isinstance(self.layer, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(self.layer, transformers.pytorch_utils.Conv1D):
+            W = W.t()
+        self.rows = W.shape[0]
+        self.columns = W.shape[1]
+        self.H = torch.zeros((self.columns, self.columns), device=self.dev)
+        self.nsamples = 0
+        self.quantizer = Quantizer()
+
+    def add_batch(self, inp, out):
+        if os.environ.get("DEBUG"):
+            self.inp1 = inp
+            self.out1 = out
+        if len(inp.shape) == 2:
+            inp = inp.unsqueeze(0)
+        tmp = inp.shape[0]
+        if isinstance(self.layer, nn.Linear) or isinstance(self.layer, transformers.Conv1D):
+            if len(inp.shape) == 3:
+                inp = inp.reshape((-1, inp.shape[-1]))
+            inp = inp.t()
+        if isinstance(self.layer, nn.Conv2d):
+            unfold = nn.Unfold(
+                self.layer.kernel_size,
+                dilation=self.layer.dilation,
+                padding=self.layer.padding,
+                stride=self.layer.stride
+            )
+            inp = unfold(inp)
+            inp = inp.permute([1, 0, 2])
+            inp = inp.flatten(1)
+        self.H *= self.nsamples / (self.nsamples + tmp)
+        self.nsamples += tmp
+        # inp = inp.float()
+        inp = math.sqrt(2 / self.nsamples) * inp.float()
+        # self.H += 2 / self.nsamples * inp.matmul(inp.t())
+        self.H += inp.matmul(inp.t())
+
+    def fasterquant(
+        self, blocksize=128, percdamp=.01, group_size=-1, actorder=False
+    ):
+        W = self.layer.weight.data.clone()
+        if isinstance(self.layer, nn.Conv2d):
+            W = W.flatten(1)
+        if isinstance(self.layer, transformers.Conv1D):
+            W = W.t()
+        W = W.float()
+
+        tick = time.time()
+
+        if not self.quantizer.ready():
+            self.quantizer.find_params(W, weight=True)
+
+        H = self.H
+        del self.H
+        dead = torch.diag(H) == 0
+        H[dead, dead] = 1
+        W[:, dead] = 0
+
+        if actorder:
+            perm = torch.argsort(torch.diag(H), descending=True)
+            W = W[:, perm]
+            H = H[perm][:, perm]
+
+        Losses = torch.zeros_like(W)
+        Q = torch.zeros_like(W)
+
+        damp = percdamp * torch.mean(torch.diag(H))
+        diag = torch.arange(self.columns, device=self.dev)
+        H[diag, diag] += damp
+        H = torch.linalg.cholesky(H)
+        H = torch.cholesky_inverse(H)
+        H = torch.linalg.cholesky(H, upper=True)
+        Hinv = H
+
+        g_idx = []
+        scale = []
+        zero = []
+        now_idx = 1
+
+        for i1 in range(0, self.columns, blocksize):
+            i2 = min(i1 + blocksize, self.columns)
+            count = i2 - i1
+
+            W1 = W[:, i1:i2].clone()
+            Q1 = torch.zeros_like(W1)
+            Err1 = torch.zeros_like(W1)
+            Losses1 = torch.zeros_like(W1)
+            Hinv1 = Hinv[i1:i2, i1:i2]
+
+            for i in range(count):
+                w = W1[:, i]
+                d = Hinv1[i, i]
+
+                if group_size != -1:
+                    if (i1 + i) % group_size == 0:
+                        self.quantizer.find_params(W[:, (i1 + i):(i1 + i + group_size)], weight=True)
+
+                    if ((i1 + i) // group_size) - now_idx == -1:
+                        scale.append(self.quantizer.scale)
+                        zero.append(self.quantizer.zero)
+                        now_idx += 1
+
+                q = self.quantizer.quantize(w.unsqueeze(1)).flatten()
+                Q1[:, i] = q
+                Losses1[:, i] = (w - q) ** 2 / d ** 2
+
+                err1 = (w - q) / d
+                W1[:, i:] -= err1.unsqueeze(1).matmul(Hinv1[i, i:].unsqueeze(0))
+                Err1[:, i] = err1
+
+            Q[:, i1:i2] = Q1
+            Losses[:, i1:i2] = Losses1 / 2
+
+            W[:, i2:] -= Err1.matmul(Hinv[i1:i2, i2:])
+
+            if os.environ.get("DEBUG"):
+                self.layer.weight.data[:, :i2] = Q[:, :i2]
+                self.layer.weight.data[:, i2:] = W[:, i2:]
+                logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
+                logger.debug(torch.sum(Losses))
+
+        torch.cuda.synchronize()
+        logger.info(f'duration: {(time.time() - tick)}')
+        logger.info(f'avg loss: {torch.sum(Losses).item() / self.nsamples}')
+
+        group_size = group_size if group_size != -1 else self.columns
+        g_idx = [i // group_size for i in range(self.columns)]
+        g_idx = torch.tensor(g_idx, dtype=torch.int32, device=Q.device)
+        if actorder:
+            invperm = torch.argsort(perm)
+            Q = Q[:, invperm]
+            g_idx = g_idx[invperm]
+
+        if isinstance(self.layer, transformers.Conv1D):
+            Q = Q.t()
+        self.layer.weight.data = Q.reshape(self.layer.weight.shape).type_as(self.layer.weight.data)
+        if os.environ.get("DEBUG"):
+            logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
+
+        if scale == []:
+            scale.append(self.quantizer.scale)
+            zero.append(self.quantizer.zero)
+        scale = torch.cat(scale, dim=1)
+        zero = torch.cat(zero, dim=1)
+        return scale, zero, g_idx
+
+    def free(self):
+        if os.environ.get("DEBUG"):
+            self.inp1 = None
+            self.out1 = None
+        self.H = None
+        self.Losses = None
+        self.Trace = None
+        torch.cuda.empty_cache()
+
+
+__all__ = ["GPTQ"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/quantization/quantizer.py` & `auto_gptq-0.3.0/auto_gptq/quantization/quantizer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-from logging import getLogger
-
-import torch
-import torch.nn as nn
-
-
-logger = getLogger(__name__)
-
-
-def quantize(x, scale, zero, maxq):
-    if maxq < 0:
-        return (x > scale / 2).float() * scale + (x < zero / 2).float() * zero
-    q = torch.clamp(torch.round(x / scale) + zero, 0, maxq)
-    return scale * (q - zero)
-
-
-class Quantizer(nn.Module):
-
-    def __init__(self, shape=1):
-        super(Quantizer, self).__init__()
-        self.register_buffer('maxq', torch.tensor(0))
-        self.register_buffer('scale', torch.zeros(shape))
-        self.register_buffer('zero', torch.zeros(shape))
-
-    def configure(
-        self,
-        bits, perchannel=False, sym=True,
-        mse=False, norm=2.4, grid=100, maxshrink=.8,
-        trits=False
-    ):
-
-        self.maxq = torch.tensor(2 ** bits - 1)
-        self.perchannel = perchannel
-        self.sym = sym
-        self.mse = mse
-        self.norm = norm
-        self.grid = grid
-        self.maxshrink = maxshrink
-        if trits:
-            self.maxq = torch.tensor(-1)
-
-    def find_params(self, x, weight=False):
-        dev = x.device
-        self.maxq = self.maxq.to(dev)
-
-        shape = x.shape
-        if self.perchannel:
-            if weight:
-                x = x.flatten(1)
-            else:
-                if len(shape) == 4:
-                    x = x.permute([1, 0, 2, 3])
-                    x = x.flatten(1)
-                if len(shape) == 3:
-                    x = x.reshape((-1, shape[-1])).t()
-                if len(shape) == 2:
-                    x = x.t()
-        else:
-            x = x.flatten().unsqueeze(0)
-
-        tmp = torch.zeros(x.shape[0], device=dev)
-        xmin = torch.minimum(x.min(1)[0], tmp)
-        xmax = torch.maximum(x.max(1)[0], tmp)
-
-        if self.sym:
-            xmax = torch.maximum(torch.abs(xmin), xmax)
-            tmp = xmin < 0
-            if torch.any(tmp):
-                xmin[tmp] = -xmax[tmp]
-        tmp = (xmin == 0) & (xmax == 0)
-        xmin[tmp] = -1
-        xmax[tmp] = +1
-
-        if self.maxq < 0:
-            self.scale = xmax
-            self.zero = xmin
-        else:
-            self.scale = (xmax - xmin) / self.maxq
-            if self.sym:
-                self.zero = torch.full_like(self.scale, (self.maxq + 1) / 2)
-            else:
-                self.zero = torch.round(-xmin / self.scale)
-
-        if self.mse:
-            best = torch.full([x.shape[0]], float('inf'), device=dev)
-            for i in range(int(self.maxshrink * self.grid)):
-                p = 1 - i / self.grid
-                xmin1 = p * xmin
-                xmax1 = p * xmax
-                scale1 = (xmax1 - xmin1) / self.maxq
-                zero1 = torch.round(-xmin1 / scale1) if not self.sym else self.zero
-                q = quantize(x, scale1.unsqueeze(1), zero1.unsqueeze(1), self.maxq)
-                q -= x
-                q.abs_()
-                q.pow_(self.norm)
-                err = torch.sum(q, 1)
-                tmp = err < best
-                if torch.any(tmp):
-                    best[tmp] = err[tmp]
-                    self.scale[tmp] = scale1[tmp]
-                    self.zero[tmp] = zero1[tmp]
-        if not self.perchannel:
-            if weight:
-                tmp = shape[0]
-            else:
-                tmp = shape[1] if len(shape) != 3 else shape[2]
-            self.scale = self.scale.repeat(tmp)
-            self.zero = self.zero.repeat(tmp)
-
-        if weight:
-            shape = [-1] + [1] * (len(shape) - 1)
-            self.scale = self.scale.reshape(shape)
-            self.zero = self.zero.reshape(shape)
-            return
-        if len(shape) == 4:
-            self.scale = self.scale.reshape((1, -1, 1, 1))
-            self.zero = self.zero.reshape((1, -1, 1, 1))
-        if len(shape) == 3:
-            self.scale = self.scale.reshape((1, 1, -1))
-            self.zero = self.zero.reshape((1, 1, -1))
-        if len(shape) == 2:
-            self.scale = self.scale.unsqueeze(0)
-            self.zero = self.zero.unsqueeze(0)
-
-    def quantize(self, x):
-        if self.ready():
-            return quantize(x, self.scale, self.zero, self.maxq)
-        return x
-
-    def enabled(self):
-        return self.maxq > 0
-
-    def ready(self):
-        return torch.all(self.scale != 0)
-
-
-__all__ = ["Quantizer"]
+from logging import getLogger
+
+import torch
+import torch.nn as nn
+
+
+logger = getLogger(__name__)
+
+
+def quantize(x, scale, zero, maxq):
+    if maxq < 0:
+        return (x > scale / 2).float() * scale + (x < zero / 2).float() * zero
+    q = torch.clamp(torch.round(x / scale) + zero, 0, maxq)
+    return scale * (q - zero)
+
+
+class Quantizer(nn.Module):
+
+    def __init__(self, shape=1):
+        super(Quantizer, self).__init__()
+        self.register_buffer('maxq', torch.tensor(0))
+        self.register_buffer('scale', torch.zeros(shape))
+        self.register_buffer('zero', torch.zeros(shape))
+
+    def configure(
+        self,
+        bits, perchannel=False, sym=True,
+        mse=False, norm=2.4, grid=100, maxshrink=.8,
+        trits=False
+    ):
+
+        self.maxq = torch.tensor(2 ** bits - 1)
+        self.perchannel = perchannel
+        self.sym = sym
+        self.mse = mse
+        self.norm = norm
+        self.grid = grid
+        self.maxshrink = maxshrink
+        if trits:
+            self.maxq = torch.tensor(-1)
+
+    def find_params(self, x, weight=False):
+        dev = x.device
+        self.maxq = self.maxq.to(dev)
+
+        shape = x.shape
+        if self.perchannel:
+            if weight:
+                x = x.flatten(1)
+            else:
+                if len(shape) == 4:
+                    x = x.permute([1, 0, 2, 3])
+                    x = x.flatten(1)
+                if len(shape) == 3:
+                    x = x.reshape((-1, shape[-1])).t()
+                if len(shape) == 2:
+                    x = x.t()
+        else:
+            x = x.flatten().unsqueeze(0)
+
+        tmp = torch.zeros(x.shape[0], device=dev)
+        xmin = torch.minimum(x.min(1)[0], tmp)
+        xmax = torch.maximum(x.max(1)[0], tmp)
+
+        if self.sym:
+            xmax = torch.maximum(torch.abs(xmin), xmax)
+            tmp = xmin < 0
+            if torch.any(tmp):
+                xmin[tmp] = -xmax[tmp]
+        tmp = (xmin == 0) & (xmax == 0)
+        xmin[tmp] = -1
+        xmax[tmp] = +1
+
+        if self.maxq < 0:
+            self.scale = xmax
+            self.zero = xmin
+        else:
+            self.scale = (xmax - xmin) / self.maxq
+            if self.sym:
+                self.zero = torch.full_like(self.scale, (self.maxq + 1) / 2)
+            else:
+                self.zero = torch.round(-xmin / self.scale)
+
+        if self.mse:
+            best = torch.full([x.shape[0]], float('inf'), device=dev)
+            for i in range(int(self.maxshrink * self.grid)):
+                p = 1 - i / self.grid
+                xmin1 = p * xmin
+                xmax1 = p * xmax
+                scale1 = (xmax1 - xmin1) / self.maxq
+                zero1 = torch.round(-xmin1 / scale1) if not self.sym else self.zero
+                q = quantize(x, scale1.unsqueeze(1), zero1.unsqueeze(1), self.maxq)
+                q -= x
+                q.abs_()
+                q.pow_(self.norm)
+                err = torch.sum(q, 1)
+                tmp = err < best
+                if torch.any(tmp):
+                    best[tmp] = err[tmp]
+                    self.scale[tmp] = scale1[tmp]
+                    self.zero[tmp] = zero1[tmp]
+        if not self.perchannel:
+            if weight:
+                tmp = shape[0]
+            else:
+                tmp = shape[1] if len(shape) != 3 else shape[2]
+            self.scale = self.scale.repeat(tmp)
+            self.zero = self.zero.repeat(tmp)
+
+        if weight:
+            shape = [-1] + [1] * (len(shape) - 1)
+            self.scale = self.scale.reshape(shape)
+            self.zero = self.zero.reshape(shape)
+            return
+        if len(shape) == 4:
+            self.scale = self.scale.reshape((1, -1, 1, 1))
+            self.zero = self.zero.reshape((1, -1, 1, 1))
+        if len(shape) == 3:
+            self.scale = self.scale.reshape((1, 1, -1))
+            self.zero = self.zero.reshape((1, 1, -1))
+        if len(shape) == 2:
+            self.scale = self.scale.unsqueeze(0)
+            self.zero = self.zero.unsqueeze(0)
+
+    def quantize(self, x):
+        if self.ready():
+            return quantize(x, self.scale, self.zero, self.maxq)
+        return x
+
+    def enabled(self):
+        return self.maxq > 0
+
+    def ready(self):
+        return torch.all(self.scale != 0)
+
+
+__all__ = ["Quantizer"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq/utils/data_utils.py` & `auto_gptq-0.3.0/auto_gptq/utils/data_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-import copy
-import random
-from functools import partial
-from typing import Callable, Dict, List, Optional
-
-import torch
-from datasets import load_dataset, DatasetDict, IterableDatasetDict
-from torch import LongTensor
-from torch.utils.data import DataLoader
-from transformers import PreTrainedTokenizer
-
-
-def make_data_block(
-    samples: Dict[str, List[str]],
-    prompt_col_name: str,
-    label_col_name: str,
-    tokenizer: PreTrainedTokenizer,
-    preprocess_fn: Optional[Callable] = None,
-    sample_max_len: int = 1024,
-    block_max_len: int = 2048,
-    add_eos_token: bool = False,
-    truncate_prompt: bool = True,
-    merge_prompt_label: bool = False
-) -> Dict[str, List[LongTensor]]:
-    """A simple implementation of text generation oriented smart batching to maximize VRAM usage when evaluation
-
-    :param samples: Dict[str, List[str]], samples that used to make data blocks
-    :param prompt_col_name: str, name of the key in samples whose value stores prompt
-    :param label_col_name: str, name of the key in samples whose value stores label
-    :param tokenizer: transformers.PretrainedTokenizer, tokenizer that used to tokenize samples
-    :param preprocess_fn: Optional[Callable], optional function that used to preprocess samples such as
-        refactor the data structure of samples, note the output of this function must be a dict whose keys
-        at least contains `prompt_col_name` and `label_col_name`
-    :param sample_max_len: int, defaults to 1024, max tokens number of each sample (before padding)
-    :param block_max_len: int, defaults to 2048, max tokens number of each data block (after padding)
-    :param add_eos_token: bool, defaults to False, whether add eos_token or not to the label
-    :param truncate_prompt: bool, defaults to True, whether to truncate prompt if the sample's total tokens
-        number exceeds `sample_max_len`, if not, will truncate label and drop this sample when all tokens
-        in label are truncated
-    :param merge_prompt_label: bool, defaults to False, will merge label into prompt if set to True, usually
-        this only required when doing language modeling task
-    :return: Dict[str, List[torch.LongTensor]], a dict whose keys are `input_ids`, `attention_mask` and
-        `label` and values are a list of torch.LongTensor
-    """
-    if preprocess_fn:
-        samples = preprocess_fn(samples)
-
-    prompts = samples[prompt_col_name]
-    labels = samples[label_col_name]
-
-    # tokenize samples
-    tokenized_prompts = tokenizer(prompts, truncation=False)["input_ids"]
-    tokenized_labels = tokenizer(labels, truncation=False)["input_ids"]
-
-    # filter tokenized samples by length
-    dropped_indices = []
-    for idx, (tokenized_prompt, tokenized_label) in enumerate(zip(tokenized_prompts, tokenized_labels)):
-        if add_eos_token:
-            tokenized_label += [tokenizer.eos_token_id]
-        len_prompt = len(tokenized_prompt)
-        len_label = len(tokenized_label)
-        exceed_len = len_prompt + len_label - sample_max_len
-        if exceed_len > 0:
-            if truncate_prompt:
-                tokenized_prompt = tokenized_prompt[exceed_len:]
-            else:
-                tokenized_label = tokenized_label[: -exceed_len]
-        tokenized_prompts[idx] = tokenized_prompt
-        tokenized_labels[idx] = tokenized_label
-        if not tokenized_label:
-            dropped_indices.append(idx)
-
-    # make data blocks of samples
-    tokenized_samples = sorted(
-        [
-            (p, l) for idx, (p, l) in enumerate(zip(tokenized_prompts, tokenized_labels))
-            if idx not in dropped_indices
-        ],
-        key=lambda x: (len(x[0]) + len(x[1])) if merge_prompt_label else len(x[0])
-    )
-    sample_blocks = []
-    sample_block = []
-    blk_max_len = 0
-    blk_total_len = 0
-    for tokenized_sample in tokenized_samples:
-        prompt_ids, label_ids = tokenized_sample
-        ori_sample_len = len(prompt_ids)
-        if merge_prompt_label:
-            ori_sample_len += len(label_ids)
-        if ori_sample_len <= blk_max_len:
-            additional_len = blk_max_len
-            sample_len = blk_max_len
-        else:
-            additional_len = len(sample_block) * (ori_sample_len - blk_max_len) + ori_sample_len
-            sample_len = ori_sample_len
-
-        if blk_total_len + additional_len > block_max_len:
-            sample_blocks.append((copy.copy(sample_block), blk_max_len))
-            sample_block = []
-            blk_max_len = 0
-            blk_total_len = 0
-            sample_len = ori_sample_len
-            additional_len = ori_sample_len
-
-        sample_block.append(tokenized_sample)
-        blk_max_len = max(blk_max_len, sample_len)
-        blk_total_len += additional_len
-
-    if sample_block:
-        sample_blocks.append((copy.copy(sample_block), blk_max_len))
-    del sample_block
-    del blk_max_len
-    del blk_total_len
-
-    new_samples = {
-        "input_ids": [],
-        "attention_mask": [],
-        "labels": []
-    }
-    # padding each data block internally
-    for block, blk_max_len in sample_blocks:
-        input_ids = []
-        attention_mask = []
-        label_ids = []
-        label_max_len = max([len(sample[1]) for sample in block])
-
-        for sample in block:
-            tokenized_prompt, tokenized_label = sample
-            sample_len = len(tokenized_prompt)
-            if merge_prompt_label:
-                sample_len += len(tokenized_label)
-            pad_num = blk_max_len - sample_len
-            if merge_prompt_label:
-                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt + tokenized_label)
-                label_ids.append([-100] * (pad_num + len(tokenized_prompt)) + tokenized_label)
-            else:
-                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt)
-                label_ids.append([-100] * (label_max_len - len(tokenized_label)) + tokenized_label)
-            attention_mask.append([0] * pad_num + [1] * sample_len)
-
-        new_samples["input_ids"].append(input_ids)
-        new_samples["attention_mask"].append(attention_mask)
-        new_samples["labels"].append(label_ids)
-
-    return new_samples
-
-
-def collate_data(blocks: List[Dict[str, List[List[int]]]], pad_token_id: int) -> Dict[str, LongTensor]:
-    def pad_block(block, pads):
-        return torch.cat((pads.to(block.device), block), dim=-1)
-
-    input_ids_blocks = [LongTensor(block["input_ids"]) for block in blocks]
-    attention_mask_blocks = [LongTensor(block["attention_mask"]) for block in blocks]
-    label_blocks = [LongTensor(block["labels"]) for block in blocks]
-
-    bsz = len(blocks)
-    inp_max_len = max([block.size(-1) for block in input_ids_blocks])
-    label_max_len = max([block.size(-1) for block in label_blocks])
-
-    for i in range(bsz):
-        block_bsz, block_inp_len = input_ids_blocks[i].shape
-        block_label_len = label_blocks[i].shape[-1]
-        pad_num = inp_max_len - block_inp_len
-        if pad_num > 0:
-            input_ids_blocks[i] = pad_block(input_ids_blocks[i], torch.ones((block_bsz, pad_num)) * pad_token_id)
-            attention_mask_blocks[i] = pad_block(attention_mask_blocks[i], torch.zeros((block_bsz, pad_num)))
-        label_pad_num = label_max_len - block_label_len
-        if label_pad_num > 0:
-            label_blocks[i] = pad_block(label_blocks[i], torch.ones((block_bsz, label_pad_num)) * -100)
-
-    return {
-        "input_ids": torch.cat(input_ids_blocks, dim=0).long(),
-        "attention_mask": torch.cat(attention_mask_blocks, dim=0).long(),
-        "labels": torch.cat(label_blocks, dim=0).long()
-    }
-
-
-def get_dataloader(
-    data_path_or_name: str,
-    prompt_col_name: str,
-    label_col_name: str,
-    tokenizer: PreTrainedTokenizer,
-    load_fn: Optional[Callable] = None,
-    preprocess_fn: Optional[Callable] = None,
-    num_samples: int = 128,
-    sample_max_len: int = 1024,
-    block_max_len: int = 2048,
-    add_eos_token: bool = False,
-    truncate_prompt: bool = True,
-    merge_prompt_label: bool = False,
-    load_fn_kwargs: Optional[dict] = None,
-    preprocess_fn_kwargs: Optional[dict] = None,
-    **kwargs
-) -> DataLoader:
-    """load dataset and build dataloader
-
-    :param data_path_or_name: str, dataset name in hf-hub or local file path
-    :param prompt_col_name: str, see `make_data_block`
-    :param label_col_name: str, see `make_data_block`
-    :param tokenizer: str, see `make_data_block`
-    :param load_fn: Optional[Callable], defaults to None, function used to load dataset, if not specified,
-        use `datasets.load_dataset`
-    :param preprocess_fn: Optional[Callable], see `make_data_block`
-    :param num_samples: int, defaults to 128, total samples used to evaluation
-    :param sample_max_len: int, see `make_data_block`
-    :param block_max_len: int, see `make_data_block`
-    :param add_eos_token: bool, see `make_data_block`
-    :param truncate_prompt: bool, see `make_data_block`
-    :param merge_prompt_label: bool, see `make_data_block`
-    :param load_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
-        for `load_fn` or `datasets.load_dataset`
-    :param preprocess_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
-        for `preprocess_fn`
-    :param kwargs: additional keyword arguments will be passed to torch's `DataLoader` initialization,
-        note values of `batch_size`, `shuffle` and `collate_fn` will always be overridden to fixed value
-    :return: torch.utils.data.DataLoader
-    """
-
-    if not load_fn_kwargs:
-        load_fn_kwargs = dict()
-    if not preprocess_fn_kwargs:
-        preprocess_fn_kwargs = dict()
-
-    if load_fn:
-        ds = load_fn(data_path_or_name, **load_fn_kwargs)
-    else:
-        ds = load_dataset(data_path_or_name, **load_fn_kwargs)
-    if isinstance(ds, (DatasetDict, IterableDatasetDict)):
-        if "evaluation" in ds:
-            ds = ds["evaluation"]
-        elif "test" in ds:
-            ds = ds["test"]
-        else:
-            ds = ds["train"]
-
-    ds = ds.select(indices=random.sample(range(len(ds)), min(len(ds), num_samples)), keep_in_memory=True)
-    ds = ds.map(
-        make_data_block,
-        batched=True,
-        batch_size=len(ds),
-        num_proc=1,
-        remove_columns=ds.column_names,
-        keep_in_memory=True,
-        load_from_cache_file=False,
-        fn_kwargs={
-            "prompt_col_name": prompt_col_name,
-            "label_col_name": label_col_name,
-            "tokenizer": tokenizer,
-            "preprocess_fn": partial(preprocess_fn, **preprocess_fn_kwargs),
-            "sample_max_len": sample_max_len,
-            "block_max_len": block_max_len,
-            "add_eos_token": add_eos_token,
-            "truncate_prompt": truncate_prompt,
-            "merge_prompt_label": merge_prompt_label
-        }
-    )
-
-    # override some arguments' values in kwargs despite user specified
-    kwargs["batch_size"] = 1
-    kwargs["shuffle"] = False
-    kwargs["collate_fn"] = partial(collate_data, pad_token_id=tokenizer.pad_token_id)
-    dl = DataLoader(ds, **kwargs)
-
-    return dl
-
-
-__all__ = ["make_data_block", "collate_data", "get_dataloader"]
+import copy
+import random
+from functools import partial
+from typing import Callable, Dict, List, Optional
+
+import torch
+from datasets import load_dataset, DatasetDict, IterableDatasetDict
+from torch import LongTensor
+from torch.utils.data import DataLoader
+from transformers import PreTrainedTokenizer
+
+
+def make_data_block(
+    samples: Dict[str, List[str]],
+    prompt_col_name: str,
+    label_col_name: str,
+    tokenizer: PreTrainedTokenizer,
+    preprocess_fn: Optional[Callable] = None,
+    sample_max_len: int = 1024,
+    block_max_len: int = 2048,
+    add_eos_token: bool = False,
+    truncate_prompt: bool = True,
+    merge_prompt_label: bool = False
+) -> Dict[str, List[LongTensor]]:
+    """A simple implementation of text generation oriented smart batching to maximize VRAM usage when evaluation
+
+    :param samples: Dict[str, List[str]], samples that used to make data blocks
+    :param prompt_col_name: str, name of the key in samples whose value stores prompt
+    :param label_col_name: str, name of the key in samples whose value stores label
+    :param tokenizer: transformers.PretrainedTokenizer, tokenizer that used to tokenize samples
+    :param preprocess_fn: Optional[Callable], optional function that used to preprocess samples such as
+        refactor the data structure of samples, note the output of this function must be a dict whose keys
+        at least contains `prompt_col_name` and `label_col_name`
+    :param sample_max_len: int, defaults to 1024, max tokens number of each sample (before padding)
+    :param block_max_len: int, defaults to 2048, max tokens number of each data block (after padding)
+    :param add_eos_token: bool, defaults to False, whether add eos_token or not to the label
+    :param truncate_prompt: bool, defaults to True, whether to truncate prompt if the sample's total tokens
+        number exceeds `sample_max_len`, if not, will truncate label and drop this sample when all tokens
+        in label are truncated
+    :param merge_prompt_label: bool, defaults to False, will merge label into prompt if set to True, usually
+        this only required when doing language modeling task
+    :return: Dict[str, List[torch.LongTensor]], a dict whose keys are `input_ids`, `attention_mask` and
+        `label` and values are a list of torch.LongTensor
+    """
+    if preprocess_fn:
+        samples = preprocess_fn(samples)
+
+    prompts = samples[prompt_col_name]
+    labels = samples[label_col_name]
+
+    # tokenize samples
+    tokenized_prompts = tokenizer(prompts, truncation=False)["input_ids"]
+    tokenized_labels = tokenizer(labels, truncation=False)["input_ids"]
+
+    # filter tokenized samples by length
+    dropped_indices = []
+    for idx, (tokenized_prompt, tokenized_label) in enumerate(zip(tokenized_prompts, tokenized_labels)):
+        if add_eos_token:
+            tokenized_label += [tokenizer.eos_token_id]
+        len_prompt = len(tokenized_prompt)
+        len_label = len(tokenized_label)
+        exceed_len = len_prompt + len_label - sample_max_len
+        if exceed_len > 0:
+            if truncate_prompt:
+                tokenized_prompt = tokenized_prompt[exceed_len:]
+            else:
+                tokenized_label = tokenized_label[: -exceed_len]
+        tokenized_prompts[idx] = tokenized_prompt
+        tokenized_labels[idx] = tokenized_label
+        if not tokenized_label:
+            dropped_indices.append(idx)
+
+    # make data blocks of samples
+    tokenized_samples = sorted(
+        [
+            (p, l) for idx, (p, l) in enumerate(zip(tokenized_prompts, tokenized_labels))
+            if idx not in dropped_indices
+        ],
+        key=lambda x: (len(x[0]) + len(x[1])) if merge_prompt_label else len(x[0])
+    )
+    sample_blocks = []
+    sample_block = []
+    blk_max_len = 0
+    blk_total_len = 0
+    for tokenized_sample in tokenized_samples:
+        prompt_ids, label_ids = tokenized_sample
+        ori_sample_len = len(prompt_ids)
+        if merge_prompt_label:
+            ori_sample_len += len(label_ids)
+        if ori_sample_len <= blk_max_len:
+            additional_len = blk_max_len
+            sample_len = blk_max_len
+        else:
+            additional_len = len(sample_block) * (ori_sample_len - blk_max_len) + ori_sample_len
+            sample_len = ori_sample_len
+
+        if blk_total_len + additional_len > block_max_len:
+            sample_blocks.append((copy.copy(sample_block), blk_max_len))
+            sample_block = []
+            blk_max_len = 0
+            blk_total_len = 0
+            sample_len = ori_sample_len
+            additional_len = ori_sample_len
+
+        sample_block.append(tokenized_sample)
+        blk_max_len = max(blk_max_len, sample_len)
+        blk_total_len += additional_len
+
+    if sample_block:
+        sample_blocks.append((copy.copy(sample_block), blk_max_len))
+    del sample_block
+    del blk_max_len
+    del blk_total_len
+
+    new_samples = {
+        "input_ids": [],
+        "attention_mask": [],
+        "labels": []
+    }
+    # padding each data block internally
+    for block, blk_max_len in sample_blocks:
+        input_ids = []
+        attention_mask = []
+        label_ids = []
+        label_max_len = max([len(sample[1]) for sample in block])
+
+        for sample in block:
+            tokenized_prompt, tokenized_label = sample
+            sample_len = len(tokenized_prompt)
+            if merge_prompt_label:
+                sample_len += len(tokenized_label)
+            pad_num = blk_max_len - sample_len
+            if merge_prompt_label:
+                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt + tokenized_label)
+                label_ids.append([-100] * (pad_num + len(tokenized_prompt)) + tokenized_label)
+            else:
+                input_ids.append([tokenizer.pad_token_id] * pad_num + tokenized_prompt)
+                label_ids.append([-100] * (label_max_len - len(tokenized_label)) + tokenized_label)
+            attention_mask.append([0] * pad_num + [1] * sample_len)
+
+        new_samples["input_ids"].append(input_ids)
+        new_samples["attention_mask"].append(attention_mask)
+        new_samples["labels"].append(label_ids)
+
+    return new_samples
+
+
+def collate_data(blocks: List[Dict[str, List[List[int]]]], pad_token_id: int) -> Dict[str, LongTensor]:
+    def pad_block(block, pads):
+        return torch.cat((pads.to(block.device), block), dim=-1)
+
+    input_ids_blocks = [LongTensor(block["input_ids"]) for block in blocks]
+    attention_mask_blocks = [LongTensor(block["attention_mask"]) for block in blocks]
+    label_blocks = [LongTensor(block["labels"]) for block in blocks]
+
+    bsz = len(blocks)
+    inp_max_len = max([block.size(-1) for block in input_ids_blocks])
+    label_max_len = max([block.size(-1) for block in label_blocks])
+
+    for i in range(bsz):
+        block_bsz, block_inp_len = input_ids_blocks[i].shape
+        block_label_len = label_blocks[i].shape[-1]
+        pad_num = inp_max_len - block_inp_len
+        if pad_num > 0:
+            input_ids_blocks[i] = pad_block(input_ids_blocks[i], torch.ones((block_bsz, pad_num)) * pad_token_id)
+            attention_mask_blocks[i] = pad_block(attention_mask_blocks[i], torch.zeros((block_bsz, pad_num)))
+        label_pad_num = label_max_len - block_label_len
+        if label_pad_num > 0:
+            label_blocks[i] = pad_block(label_blocks[i], torch.ones((block_bsz, label_pad_num)) * -100)
+
+    return {
+        "input_ids": torch.cat(input_ids_blocks, dim=0).long(),
+        "attention_mask": torch.cat(attention_mask_blocks, dim=0).long(),
+        "labels": torch.cat(label_blocks, dim=0).long()
+    }
+
+
+def get_dataloader(
+    data_path_or_name: str,
+    prompt_col_name: str,
+    label_col_name: str,
+    tokenizer: PreTrainedTokenizer,
+    load_fn: Optional[Callable] = None,
+    preprocess_fn: Optional[Callable] = None,
+    num_samples: int = 128,
+    sample_max_len: int = 1024,
+    block_max_len: int = 2048,
+    add_eos_token: bool = False,
+    truncate_prompt: bool = True,
+    merge_prompt_label: bool = False,
+    load_fn_kwargs: Optional[dict] = None,
+    preprocess_fn_kwargs: Optional[dict] = None,
+    **kwargs
+) -> DataLoader:
+    """load dataset and build dataloader
+
+    :param data_path_or_name: str, dataset name in hf-hub or local file path
+    :param prompt_col_name: str, see `make_data_block`
+    :param label_col_name: str, see `make_data_block`
+    :param tokenizer: str, see `make_data_block`
+    :param load_fn: Optional[Callable], defaults to None, function used to load dataset, if not specified,
+        use `datasets.load_dataset`
+    :param preprocess_fn: Optional[Callable], see `make_data_block`
+    :param num_samples: int, defaults to 128, total samples used to evaluation
+    :param sample_max_len: int, see `make_data_block`
+    :param block_max_len: int, see `make_data_block`
+    :param add_eos_token: bool, see `make_data_block`
+    :param truncate_prompt: bool, see `make_data_block`
+    :param merge_prompt_label: bool, see `make_data_block`
+    :param load_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
+        for `load_fn` or `datasets.load_dataset`
+    :param preprocess_fn_kwargs: Optional[dict], defaults to None, keyword arguments used
+        for `preprocess_fn`
+    :param kwargs: additional keyword arguments will be passed to torch's `DataLoader` initialization,
+        note values of `batch_size`, `shuffle` and `collate_fn` will always be overridden to fixed value
+    :return: torch.utils.data.DataLoader
+    """
+
+    if not load_fn_kwargs:
+        load_fn_kwargs = dict()
+    if not preprocess_fn_kwargs:
+        preprocess_fn_kwargs = dict()
+
+    if load_fn:
+        ds = load_fn(data_path_or_name, **load_fn_kwargs)
+    else:
+        ds = load_dataset(data_path_or_name, **load_fn_kwargs)
+    if isinstance(ds, (DatasetDict, IterableDatasetDict)):
+        if "evaluation" in ds:
+            ds = ds["evaluation"]
+        elif "test" in ds:
+            ds = ds["test"]
+        else:
+            ds = ds["train"]
+
+    ds = ds.select(indices=random.sample(range(len(ds)), min(len(ds), num_samples)), keep_in_memory=True)
+    ds = ds.map(
+        make_data_block,
+        batched=True,
+        batch_size=len(ds),
+        num_proc=1,
+        remove_columns=ds.column_names,
+        keep_in_memory=True,
+        load_from_cache_file=False,
+        fn_kwargs={
+            "prompt_col_name": prompt_col_name,
+            "label_col_name": label_col_name,
+            "tokenizer": tokenizer,
+            "preprocess_fn": partial(preprocess_fn, **preprocess_fn_kwargs),
+            "sample_max_len": sample_max_len,
+            "block_max_len": block_max_len,
+            "add_eos_token": add_eos_token,
+            "truncate_prompt": truncate_prompt,
+            "merge_prompt_label": merge_prompt_label
+        }
+    )
+
+    # override some arguments' values in kwargs despite user specified
+    kwargs["batch_size"] = 1
+    kwargs["shuffle"] = False
+    kwargs["collate_fn"] = partial(collate_data, pad_token_id=tokenizer.pad_token_id)
+    dl = DataLoader(ds, **kwargs)
+
+    return dl
+
+
+__all__ = ["make_data_block", "collate_data", "get_dataloader"]
```

### Comparing `auto_gptq-0.2.2/auto_gptq.egg-info/PKG-INFO` & `auto_gptq-0.3.0/auto_gptq.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,352 +1,345 @@
-Metadata-Version: 2.1
-Name: auto-gptq
-Version: 0.2.2
-Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
-Home-page: https://github.com/PanQiWei/AutoGPTQ
-Author: PanQiWei
-Keywords: gptq,quantization,large-language-models,pytorch,transformers
-Platform: windows
-Platform: linux
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
-Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: C++
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-Provides-Extra: llama
-Provides-Extra: triton
-License-File: LICENSE
-
-<h1 align="center">AutoGPTQ</h1>
-<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
-<p align="center">
-    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
-        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
-    </a>
-    <a href="https://pypi.org/project/auto-gptq/">
-        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
-    </a>
-</p>
-<h4 align="center">
-    <p>
-        <b>English</b> |
-        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
-    <p>
-</h4>
-
-## News or Update
-
-**To experience adapter training using `auto_gptq` quantized model in advance, you can try [this branch](https://github.com/PanQiWei/AutoGPTQ/tree/peft_integration) and discuss [in here](https://github.com/PanQiWei/AutoGPTQ/issues/103), examples are [in here](https://github.com/PanQiWei/AutoGPTQ/tree/peft_integration/examples/peft).**
-
-- 2023-05-25 - (In Progress) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
-- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
-- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
-- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
-
-*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
-
-## Performance Comparison
-
-### Inference Speed
-> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
-> 
-> The quantized model is loaded using the setup that can gain the fastest inference speed.
-
-| model         | GPU           | num_beams | fp16  | gptq-int4 |
-|---------------|---------------|-----------|-------|-----------|
-| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
-| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
-| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
-| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
-| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
-| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
-| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
-| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
-
-
-### Perplexity
-For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
-
-## Installation
-
-### Quick Installation
-You can install the latest stable release of AutoGPTQ from pip:
-```shell
-pip install auto-gptq
-```
-Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
-```shell
-# firstly, cd the directory where the wheel saved, then execute command below
-pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
-```
-#### disable cuda extensions
-By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
-```shell
-BUILD_CUDA_EXT=0 pip install auto-gptq
-```
-And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
-```shell
-pip uninstall autogptq_cuda -y
-```
-#### to support LLaMa model
-For some people want to try LLaMa and whose `transformers` version not meet the newest one that supports it, using:
-```shell
-pip install auto-gptq[llama]
-```
-#### to support triton speedup
-To integrate with `triton`, using:
-> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
-
-```shell
-pip install auto-gptq[triton]
-```
-
-### Install from source
-<details>
-<summary>click to see details</summary>
-
-Clone the source code:
-```shell
-git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
-```
-Then, install from source:
-```shell
-pip install .
-```
-Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
-
-Use `.[llama]` if you want to try LLaMa model.
-
-Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
-
-</details>
-
-## Quick Tour
-
-### Quantization and Inference
-> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
-
-Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
-```python
-from transformers import AutoTokenizer, TextGenerationPipeline
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-import logging
-
-logging.basicConfig(
-    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
-)
-
-pretrained_model_dir = "facebook/opt-125m"
-quantized_model_dir = "opt-125m-4bit"
-
-tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
-examples = [
-    tokenizer(
-        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
-    )
-]
-
-quantize_config = BaseQuantizeConfig(
-    bits=4,  # quantize model to 4-bit
-    group_size=128,  # it is recommended to set the value to 128
-    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
-)
-
-# load un-quantized model, by default, the model will always be loaded into CPU memory
-model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
-
-# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
-model.quantize(examples)
-
-# save quantized model
-model.save_quantized(quantized_model_dir)
-
-# save quantized model using safetensors
-model.save_quantized(quantized_model_dir, use_safetensors=True)
-
-# push quantized model to Hugging Face Hub. 
-# to use use_auth_token=True, Login first via huggingface-cli login.
-# or pass explcit token with: use_auth_token="hf_xxxxxxx"
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
-
-# alternatively you can save and push at the same time
-# (uncomment the following three lines to enable this feature)
-# repo_id = f"YourUserName/{quantized_model_dir}"
-# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
-# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
-
-# load quantized model to the first GPU
-model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
-
-# download quantized model from Hugging Face Hub and load to the first GPU
-# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
-
-# inference with model.generate
-print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
-
-# or you can also use pipeline
-pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
-print(pipeline("auto-gptq is")[0]["generated_text"])
-```
-
-For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
-
-### Customize Model
-<details>
-
-<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
-
-```python
-from auto_gptq.modeling import BaseGPTQForCausalLM
-
-
-class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
-    # chained attribute name of transformer layer block
-    layers_block_name = "model.decoder.layers"
-    # chained attribute names of other nn modules that in the same level as the transformer layer block
-    outside_layer_modules = [
-        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
-        "model.decoder.project_in", "model.decoder.final_layer_norm"
-    ]
-    # chained attribute names of linear layers in transformer layer module
-    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
-    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
-    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
-    inside_layer_modules = [
-        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
-        ["self_attn.out_proj"],
-        ["fc1"],
-        ["fc2"]
-    ]
-```
-After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
-
-</details>
-
-### Evaluation on Downstream Tasks
-You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
-
-The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
-
-<details>
-
-<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
-
-```python
-from functools import partial
-
-import datasets
-from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
-
-from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
-from auto_gptq.eval_tasks import SequenceClassificationTask
-
-
-MODEL = "EleutherAI/gpt-j-6b"
-DATASET = "cardiffnlp/tweet_sentiment_multilingual"
-TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
-ID2LABEL = {
-    0: "negative",
-    1: "neutral",
-    2: "positive"
-}
-LABELS = list(ID2LABEL.values())
-
-
-def ds_refactor_fn(samples):
-    text_data = samples["text"]
-    label_data = samples["label"]
-
-    new_samples = {"prompt": [], "label": []}
-    for text, label in zip(text_data, label_data):
-        prompt = TEMPLATE.format(labels=LABELS, text=text)
-        new_samples["prompt"].append(prompt)
-        new_samples["label"].append(ID2LABEL[label])
-
-    return new_samples
-
-
-#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
-model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
-tokenizer = AutoTokenizer.from_pretrained(MODEL)
-
-task = SequenceClassificationTask(
-        model=model,
-        tokenizer=tokenizer,
-        classes=LABELS,
-        data_name_or_path=DATASET,
-        prompt_col_name="prompt",
-        label_col_name="label",
-        **{
-            "num_samples": 1000,  # how many samples will be sampled to evaluation
-            "sample_max_len": 1024,  # max tokens for each sample
-            "block_max_len": 2048,  # max tokens for each data block
-            # function to load dataset, one must only accept data_name_or_path as input 
-            # and return datasets.Dataset
-            "load_fn": partial(datasets.load_dataset, name="english"),  
-            # function to preprocess dataset, which is used for datasets.Dataset.map, 
-            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
-            "preprocess_fn": ds_refactor_fn,  
-            # truncate label when sample's length exceed sample_max_len
-            "truncate_prompt": False  
-        }
-    )
-
-# note that max_new_tokens will be automatically specified internally based on given classes
-print(task.run())
-
-# self-consistency
-print(
-    task.run(
-        generation_config=GenerationConfig(
-            num_beams=3,
-            num_return_sequences=3,
-            do_sample=True
-        )
-    )
-)
-```
-
-</details>
-
-## Learn More
-[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
-
-[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
-
-## Supported Models
-
-> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
-> 
-> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
-
-| model type                         | quantization | inference | peft-lora | peft-adaption_prompt |
-|------------------------------------|--------------|-----------|-----------|----------------------|
-| bloom                              | ✅            | ✅         |           |                      |
-| gpt2                               | ✅            | ✅         |           |                      |
-| gpt_neox                           | ✅            | ✅         |           |                      |
-| gptj                               | ✅            | ✅         |           |                      |
-| llama                              | ✅            | ✅         |           | ✅                    |
-| moss                               | ✅            | ✅         |           |                      |
-| opt                                | ✅            | ✅         |           |                      |
-| gpt_bigcode                        | ✅            | ✅         |           |                      |
-| codegen                            | ✅            | ✅         |           |                      |
-| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         |           |                      |
-
-## Supported Evaluation Tasks
-Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
-
-## Acknowledgement
-- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
-- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
-
-
-[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
+Metadata-Version: 2.1
+Name: auto-gptq
+Version: 0.3.0
+Summary: An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
+Home-page: https://github.com/PanQiWei/AutoGPTQ
+Author: PanQiWei
+Keywords: gptq,quantization,large-language-models,pytorch,transformers
+Platform: windows
+Platform: linux
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
+Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: C++
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+Provides-Extra: triton
+License-File: LICENSE
+
+<h1 align="center">AutoGPTQ</h1>
+<p align="center">An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.</p>
+<p align="center">
+    <a href="https://github.com/PanQiWei/AutoGPTQ/releases">
+        <img alt="GitHub release" src="https://img.shields.io/github/release/PanQiWei/AutoGPTQ.svg">
+    </a>
+    <a href="https://pypi.org/project/auto-gptq/">
+        <img alt="PyPI - Downloads" src="https://img.shields.io/pypi/dd/auto-gptq">
+    </a>
+</p>
+<h4 align="center">
+    <p>
+        <b>English</b> |
+        <a href="https://github.com/PanQiWei/AutoGPTQ/blob/main/README_zh.md">中文</a>
+    </p>
+</h4>
+
+*<center>📣 Long time no see! 👋 Architecture upgrade, performance optimization and more new features will come in July and August, stay tune! 🥂</center>*
+
+## News or Update
+
+- 2023-06-05 - (Update) - Integrate with 🤗 peft to use gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc.
+- 2023-05-30 - (Update) - Support download/upload quantized model from/to 🤗 Hub.
+- 2023-05-27 - (Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types.
+- 2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or group_size == -1`.
+
+*For more histories please turn to [here](docs/NEWS_OR_UPDATE.md)*
+
+## Performance Comparison
+
+### Inference Speed
+> The result is generated using [this script](examples/benchmark/generation_speed.py), batch size of input is 1, decode strategy is beam search and enforce the model to generate 512 tokens, speed metric is tokens/s (the larger, the better).
+> 
+> The quantized model is loaded using the setup that can gain the fastest inference speed.
+
+| model         | GPU           | num_beams | fp16  | gptq-int4 |
+|---------------|---------------|-----------|-------|-----------|
+| llama-7b      | 1xA100-40G    | 1         | 18.87 | 25.53     |
+| llama-7b      | 1xA100-40G    | 4         | 68.79 | 91.30     |
+| moss-moon 16b | 1xA100-40G    | 1         | 12.48 | 15.25     |
+| moss-moon 16b | 1xA100-40G    | 4         | OOM   | 42.67     |
+| moss-moon 16b | 2xA100-40G    | 1         | 06.83 | 06.78     |
+| moss-moon 16b | 2xA100-40G    | 4         | 13.10 | 10.80     |
+| gpt-j 6b      | 1xRTX3060-12G | 1         | OOM   | 29.55     |
+| gpt-j 6b      | 1xRTX3060-12G | 4         | OOM   | 47.36     |
+
+
+### Perplexity
+For perplexity comparison, you can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes)
+
+## Installation
+
+### Quick Installation
+You can install the latest stable release of AutoGPTQ from pip:
+```shell
+pip install auto-gptq
+```
+Start from v0.2.0, you can download pre-build wheel that satisfied your environment setup from each version's release assets and install it to skip building stage for the fastest installation speed. For example:
+```shell
+# firstly, cd the directory where the wheel saved, then execute command below
+pip install auto_gptq-0.2.0+cu118-cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for linux in an environment whose python=3.10 and cuda=11.8
+```
+#### disable cuda extensions
+By default, cuda extensions will be installed when `torch` and `cuda` is already installed in your machine, if you don't want to use them, using:
+```shell
+BUILD_CUDA_EXT=0 pip install auto-gptq
+```
+And to make sure `autogptq_cuda` is not ever in your virtual environment, run:
+```shell
+pip uninstall autogptq_cuda -y
+```
+
+#### to support triton speedup
+To integrate with `triton`, using:
+> warning: currently triton only supports linux; 3-bit quantization is not supported when using triton
+
+```shell
+pip install auto-gptq[triton]
+```
+
+### Install from source
+<details>
+<summary>click to see details</summary>
+
+Clone the source code:
+```shell
+git clone https://github.com/PanQiWei/AutoGPTQ.git && cd AutoGPTQ
+```
+Then, install from source:
+```shell
+pip install .
+```
+Like quick installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension building.
+
+Use `.[triton]` if you want to integrate with triton and it's available on your operating system.
+
+</details>
+
+## Quick Tour
+
+### Quantization and Inference
+> warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which uses only one sample to quantize a much small model, quality of quantized model using such little samples may not good.
+
+Below is an example for the simplest use of `auto_gptq` to quantize a model and inference after quantization: 
+```python
+from transformers import AutoTokenizer, TextGenerationPipeline
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+import logging
+
+logging.basicConfig(
+    format="%(asctime)s %(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S"
+)
+
+pretrained_model_dir = "facebook/opt-125m"
+quantized_model_dir = "opt-125m-4bit"
+
+tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True)
+examples = [
+    tokenizer(
+        "auto-gptq is an easy-to-use model quantization library with user-friendly apis, based on GPTQ algorithm."
+    )
+]
+
+quantize_config = BaseQuantizeConfig(
+    bits=4,  # quantize model to 4-bit
+    group_size=128,  # it is recommended to set the value to 128
+    desc_act=False,  # set to False can significantly speed up inference but the perplexity may slightly bad 
+)
+
+# load un-quantized model, by default, the model will always be loaded into CPU memory
+model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir, quantize_config)
+
+# quantize model, the examples should be list of dict whose keys can only be "input_ids" and "attention_mask"
+model.quantize(examples)
+
+# save quantized model
+model.save_quantized(quantized_model_dir)
+
+# save quantized model using safetensors
+model.save_quantized(quantized_model_dir, use_safetensors=True)
+
+# push quantized model to Hugging Face Hub. 
+# to use use_auth_token=True, Login first via huggingface-cli login.
+# or pass explcit token with: use_auth_token="hf_xxxxxxx"
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, commit_message=commit_message, use_auth_token=True)
+
+# alternatively you can save and push at the same time
+# (uncomment the following three lines to enable this feature)
+# repo_id = f"YourUserName/{quantized_model_dir}"
+# commit_message = f"AutoGPTQ model for {pretrained_model_dir}: {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act={quantize_config.desc_act}"
+# model.push_to_hub(repo_id, save_dir=quantized_model_dir, use_safetensors=True, commit_message=commit_message, use_auth_token=True)
+
+# load quantized model to the first GPU
+model = AutoGPTQForCausalLM.from_quantized(quantized_model_dir, device="cuda:0")
+
+# download quantized model from Hugging Face Hub and load to the first GPU
+# model = AutoGPTQForCausalLM.from_quantized(repo_id, device="cuda:0", use_safetensors=True, use_triton=False)
+
+# inference with model.generate
+print(tokenizer.decode(model.generate(**tokenizer("auto_gptq is", return_tensors="pt").to(model.device))[0]))
+
+# or you can also use pipeline
+pipeline = TextGenerationPipeline(model=model, tokenizer=tokenizer)
+print(pipeline("auto-gptq is")[0]["generated_text"])
+```
+
+For more advanced features of model quantization, please reference to [this script](examples/quantization/quant_with_alpaca.py)
+
+### Customize Model
+<details>
+
+<summary>Below is an example to extend `auto_gptq` to support `OPT` model, as you will see, it's very easy:</summary>
+
+```python
+from auto_gptq.modeling import BaseGPTQForCausalLM
+
+
+class OPTGPTQForCausalLM(BaseGPTQForCausalLM):
+    # chained attribute name of transformer layer block
+    layers_block_name = "model.decoder.layers"
+    # chained attribute names of other nn modules that in the same level as the transformer layer block
+    outside_layer_modules = [
+        "model.decoder.embed_tokens", "model.decoder.embed_positions", "model.decoder.project_out",
+        "model.decoder.project_in", "model.decoder.final_layer_norm"
+    ]
+    # chained attribute names of linear layers in transformer layer module
+    # normally, there are four sub lists, for each one the modules in it can be seen as one operation, 
+    # and the order should be the order when they are truly executed, in this case (and usually in most cases), 
+    # they are: attention q_k_v projection, attention output projection, MLP project input, MLP project output
+    inside_layer_modules = [
+        ["self_attn.k_proj", "self_attn.v_proj", "self_attn.q_proj"],
+        ["self_attn.out_proj"],
+        ["fc1"],
+        ["fc2"]
+    ]
+```
+After this, you can use `OPTGPTQForCausalLM.from_pretrained` and other methods as shown in Basic.
+
+</details>
+
+### Evaluation on Downstream Tasks
+You can use tasks defined in `auto_gptq.eval_tasks` to evaluate model's performance on specific down-stream task before and after quantization.
+
+The predefined tasks support all causal-language-models implemented in [🤗 transformers](https://github.com/huggingface/transformers) and in this project.
+
+<details>
+
+<summary>Below is an example to evaluate `EleutherAI/gpt-j-6b` on sequence-classification task using `cardiffnlp/tweet_sentiment_multilingual` dataset:</summary>
+
+```python
+from functools import partial
+
+import datasets
+from transformers import AutoTokenizer, AutoModelForCausalLM, GenerationConfig
+
+from auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig
+from auto_gptq.eval_tasks import SequenceClassificationTask
+
+
+MODEL = "EleutherAI/gpt-j-6b"
+DATASET = "cardiffnlp/tweet_sentiment_multilingual"
+TEMPLATE = "Question:What's the sentiment of the given text? Choices are {labels}.\nText: {text}\nAnswer:"
+ID2LABEL = {
+    0: "negative",
+    1: "neutral",
+    2: "positive"
+}
+LABELS = list(ID2LABEL.values())
+
+
+def ds_refactor_fn(samples):
+    text_data = samples["text"]
+    label_data = samples["label"]
+
+    new_samples = {"prompt": [], "label": []}
+    for text, label in zip(text_data, label_data):
+        prompt = TEMPLATE.format(labels=LABELS, text=text)
+        new_samples["prompt"].append(prompt)
+        new_samples["label"].append(ID2LABEL[label])
+
+    return new_samples
+
+
+#  model = AutoModelForCausalLM.from_pretrained(MODEL).eval().half().to("cuda:0")
+model = AutoGPTQForCausalLM.from_pretrained(MODEL, BaseQuantizeConfig())
+tokenizer = AutoTokenizer.from_pretrained(MODEL)
+
+task = SequenceClassificationTask(
+        model=model,
+        tokenizer=tokenizer,
+        classes=LABELS,
+        data_name_or_path=DATASET,
+        prompt_col_name="prompt",
+        label_col_name="label",
+        **{
+            "num_samples": 1000,  # how many samples will be sampled to evaluation
+            "sample_max_len": 1024,  # max tokens for each sample
+            "block_max_len": 2048,  # max tokens for each data block
+            # function to load dataset, one must only accept data_name_or_path as input 
+            # and return datasets.Dataset
+            "load_fn": partial(datasets.load_dataset, name="english"),  
+            # function to preprocess dataset, which is used for datasets.Dataset.map, 
+            # must return Dict[str, list] with only two keys: [prompt_col_name, label_col_name]
+            "preprocess_fn": ds_refactor_fn,  
+            # truncate label when sample's length exceed sample_max_len
+            "truncate_prompt": False  
+        }
+    )
+
+# note that max_new_tokens will be automatically specified internally based on given classes
+print(task.run())
+
+# self-consistency
+print(
+    task.run(
+        generation_config=GenerationConfig(
+            num_beams=3,
+            num_return_sequences=3,
+            do_sample=True
+        )
+    )
+)
+```
+
+</details>
+
+## Learn More
+[tutorials](docs/tutorial) provide step-by-step guidance to integrate `auto_gptq` with your own project and some best practice principles.
+
+[examples](examples/README.md) provide plenty of example scripts to use `auto_gptq` in different ways.
+
+## Supported Models
+
+> you can use `model.config.model_type` to compare with the table below to check whether the model you use is supported by `auto_gptq`.
+> 
+> for example, model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they are all supported by `auto_gptq`.
+
+| model type                         | quantization | inference | peft-lora | peft-ada-lora | peft-adaption_prompt                                                                            |
+|------------------------------------|--------------|-----------|-----------|---------------|-------------------------------------------------------------------------------------------------|
+| bloom                              | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt2                               | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_neox                           | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| gptj                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| llama                              | ✅            | ✅         | ✅         | ✅             | ✅                                                                                               |
+| moss                               | ✅            | ✅         | ✅         | ✅             | ✅[requires this peft branch](https://github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) |
+| opt                                | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| gpt_bigcode                        | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| codegen                            | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+| falcon(RefinedWebModel/RefinedWeb) | ✅            | ✅         | ✅         | ✅             |                                                                                                 |
+
+## Supported Evaluation Tasks
+Currently, `auto_gptq` supports: `LanguageModelingTask`, `SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come soon!
+
+## Acknowledgement
+- Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code](https://github.com/IST-DASLab/gptq).
+- Specially thanks **qwopqwop200**, for code in this project that relevant to quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda).
+
+
+[![Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
```

#### html2text {}

```diff
@@ -1,99 +1,95 @@
-Metadata-Version: 2.1 Name: auto-gptq Version: 0.2.2 Summary: An easy-to-use
+Metadata-Version: 2.1 Name: auto-gptq Version: 0.3.0 Summary: An easy-to-use
 LLMs quantization package with user-friendly apis, based on GPTQ algorithm.
 Home-page: https://github.com/PanQiWei/AutoGPTQ Author: PanQiWei Keywords:
 gptq,quantization,large-language-models,pytorch,transformers Platform: windows
 Platform: linux Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.7
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.8 Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: Chinese
 (Simplified) Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: C++ Requires-Python: >=3.8.0 Description-Content-Type: text/
-markdown Provides-Extra: llama Provides-Extra: triton License-File: LICENSE
+markdown Provides-Extra: triton License-File: LICENSE
                             ****** AutoGPTQ ******
 An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ
                                   algorithm.
                       [GitHub_release] [PyPI_-_Downloads]
                            *** English | ä¸­æ ***
-## News or Update **To experience adapter training using `auto_gptq` quantized
-model in advance, you can try [this branch](https://github.com/PanQiWei/
-AutoGPTQ/tree/peft_integration) and discuss [in here](https://github.com/
-PanQiWei/AutoGPTQ/issues/103), examples are [in here](https://github.com/
-PanQiWei/AutoGPTQ/tree/peft_integration/examples/peft).** - 2023-05-25 - (In
-Progress) - Integrate with ð¤ peft to use gptq quantized model to train
-adapters, support LoRA, AdaLoRA, AdaptionPrompt, etc. - 2023-05-30 - (Update) -
-Support download/upload quantized model from/to ð¤ Hub. - 2023-05-27 -
-(Update) - Support quantization and inference for `gpt_bigcode`, `codegen` and
-`RefineWeb/RefineWebModel`(falcon) model types. - 2023-05-04 - (Update) -
-Support using faster cuda kernel when `not desc_act or group_size == -1`. *For
-more histories please turn to [here](docs/NEWS_OR_UPDATE.md)* ## Performance
-Comparison ### Inference Speed > The result is generated using [this script]
-(examples/benchmark/generation_speed.py), batch size of input is 1, decode
-strategy is beam search and enforce the model to generate 512 tokens, speed
-metric is tokens/s (the larger, the better). > > The quantized model is loaded
-using the setup that can gain the fastest inference speed. | model | GPU |
-num_beams | fp16 | gptq-int4 | |---------------|---------------|-----------|---
-----|-----------| | llama-7b | 1xA100-40G | 1 | 18.87 | 25.53 | | llama-7b |
-1xA100-40G | 4 | 68.79 | 91.30 | | moss-moon 16b | 1xA100-40G | 1 | 12.48 |
-15.25 | | moss-moon 16b | 1xA100-40G | 4 | OOM | 42.67 | | moss-moon 16b |
-2xA100-40G | 1 | 06.83 | 06.78 | | moss-moon 16b | 2xA100-40G | 4 | 13.10 |
-10.80 | | gpt-j 6b | 1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b | 1xRTX3060-
-12G | 4 | OOM | 47.36 | ### Perplexity For perplexity comparison, you can turn
-to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and [here]
-(https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ##
+*
+ð£ Long time no see! ð Architecture upgrade, performance optimization and
+        more new features will come in July and August, stay tune! ð¥
+* ## News or Update - 2023-06-05 - (Update) - Integrate with ð¤ peft to use
+gptq quantized model to train adapters, support LoRA, AdaLoRA, AdaptionPrompt,
+etc. - 2023-05-30 - (Update) - Support download/upload quantized model from/to
+ð¤ Hub. - 2023-05-27 - (Update) - Support quantization and inference for
+`gpt_bigcode`, `codegen` and `RefineWeb/RefineWebModel`(falcon) model types. -
+2023-05-04 - (Update) - Support using faster cuda kernel when `not desc_act or
+group_size == -1`. *For more histories please turn to [here](docs/
+NEWS_OR_UPDATE.md)* ## Performance Comparison ### Inference Speed > The result
+is generated using [this script](examples/benchmark/generation_speed.py), batch
+size of input is 1, decode strategy is beam search and enforce the model to
+generate 512 tokens, speed metric is tokens/s (the larger, the better). > > The
+quantized model is loaded using the setup that can gain the fastest inference
+speed. | model | GPU | num_beams | fp16 | gptq-int4 | |---------------|--------
+-------|-----------|-------|-----------| | llama-7b | 1xA100-40G | 1 | 18.87 |
+25.53 | | llama-7b | 1xA100-40G | 4 | 68.79 | 91.30 | | moss-moon 16b | 1xA100-
+40G | 1 | 12.48 | 15.25 | | moss-moon 16b | 1xA100-40G | 4 | OOM | 42.67 | |
+moss-moon 16b | 2xA100-40G | 1 | 06.83 | 06.78 | | moss-moon 16b | 2xA100-40G |
+4 | 13.10 | 10.80 | | gpt-j 6b | 1xRTX3060-12G | 1 | OOM | 29.55 | | gpt-j 6b |
+1xRTX3060-12G | 4 | OOM | 47.36 | ### Perplexity For perplexity comparison, you
+can turn to [here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#result) and
+[here](https://github.com/qwopqwop200/GPTQ-for-LLaMa#gptq-vs-bitsandbytes) ##
 Installation ### Quick Installation You can install the latest stable release
 of AutoGPTQ from pip: ```shell pip install auto-gptq ``` Start from v0.2.0, you
 can download pre-build wheel that satisfied your environment setup from each
 version's release assets and install it to skip building stage for the fastest
 installation speed. For example: ```shell # firstly, cd the directory where the
 wheel saved, then execute command below pip install auto_gptq-0.2.0+cu118-
 cp310-cp310-linux_x86_64.whl # install v0.2.0 auto_gptq pre-build wheel for
 linux in an environment whose python=3.10 and cuda=11.8 ``` #### disable cuda
 extensions By default, cuda extensions will be installed when `torch` and
 `cuda` is already installed in your machine, if you don't want to use them,
 using: ```shell BUILD_CUDA_EXT=0 pip install auto-gptq ``` And to make sure
 `autogptq_cuda` is not ever in your virtual environment, run: ```shell pip
-uninstall autogptq_cuda -y ``` #### to support LLaMa model For some people want
-to try LLaMa and whose `transformers` version not meet the newest one that
-supports it, using: ```shell pip install auto-gptq[llama] ``` #### to support
-triton speedup To integrate with `triton`, using: > warning: currently triton
-only supports linux; 3-bit quantization is not supported when using triton
-```shell pip install auto-gptq[triton] ``` ### Install from source  click to
-see details Clone the source code: ```shell git clone https://github.com/
-PanQiWei/AutoGPTQ.git && cd AutoGPTQ ``` Then, install from source: ```shell
-pip install . ``` Like quick installation, you can also set `BUILD_CUDA_EXT=0`
-to disable pytorch extension building. Use `.[llama]` if you want to try LLaMa
-model. Use `.[triton]` if you want to integrate with triton and it's available
-on your operating system.  ## Quick Tour ### Quantization and Inference >
-warning: this is just a showcase of the usage of basic apis in AutoGPTQ, which
-uses only one sample to quantize a much small model, quality of quantized model
-using such little samples may not good. Below is an example for the simplest
-use of `auto_gptq` to quantize a model and inference after quantization:
-```python from transformers import AutoTokenizer, TextGenerationPipeline from
-auto_gptq import AutoGPTQForCausalLM, BaseQuantizeConfig import logging
-logging.basicConfig( format="%(asctime)s %(levelname)s [%(name)s] %(message)s",
-level=logging.INFO, datefmt="%Y-%m-%d %H:%M:%S" ) pretrained_model_dir =
-"facebook/opt-125m" quantized_model_dir = "opt-125m-4bit" tokenizer =
-AutoTokenizer.from_pretrained(pretrained_model_dir, use_fast=True) examples =
-[ tokenizer( "auto-gptq is an easy-to-use model quantization library with user-
-friendly apis, based on GPTQ algorithm." ) ] quantize_config =
-BaseQuantizeConfig( bits=4, # quantize model to 4-bit group_size=128, # it is
-recommended to set the value to 128 desc_act=False, # set to False can
-significantly speed up inference but the perplexity may slightly bad ) # load
-un-quantized model, by default, the model will always be loaded into CPU memory
-model = AutoGPTQForCausalLM.from_pretrained(pretrained_model_dir,
-quantize_config) # quantize model, the examples should be list of dict whose
-keys can only be "input_ids" and "attention_mask" model.quantize(examples) #
-save quantized model model.save_quantized(quantized_model_dir) # save quantized
-model using safetensors model.save_quantized(quantized_model_dir,
-use_safetensors=True) # push quantized model to Hugging Face Hub. # to use
-use_auth_token=True, Login first via huggingface-cli login. # or pass explcit
-token with: use_auth_token="hf_xxxxxxx" # (uncomment the following three lines
-to enable this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
+uninstall autogptq_cuda -y ``` #### to support triton speedup To integrate with
+`triton`, using: > warning: currently triton only supports linux; 3-bit
+quantization is not supported when using triton ```shell pip install auto-gptq
+[triton] ``` ### Install from source  click to see details Clone the source
+code: ```shell git clone https://github.com/PanQiWei/AutoGPTQ.git && cd
+AutoGPTQ ``` Then, install from source: ```shell pip install . ``` Like quick
+installation, you can also set `BUILD_CUDA_EXT=0` to disable pytorch extension
+building. Use `.[triton]` if you want to integrate with triton and it's
+available on your operating system.  ## Quick Tour ### Quantization and
+Inference > warning: this is just a showcase of the usage of basic apis in
+AutoGPTQ, which uses only one sample to quantize a much small model, quality of
+quantized model using such little samples may not good. Below is an example for
+the simplest use of `auto_gptq` to quantize a model and inference after
+quantization: ```python from transformers import AutoTokenizer,
+TextGenerationPipeline from auto_gptq import AutoGPTQForCausalLM,
+BaseQuantizeConfig import logging logging.basicConfig( format="%(asctime)s %
+(levelname)s [%(name)s] %(message)s", level=logging.INFO, datefmt="%Y-%m-%d %H:
+%M:%S" ) pretrained_model_dir = "facebook/opt-125m" quantized_model_dir = "opt-
+125m-4bit" tokenizer = AutoTokenizer.from_pretrained(pretrained_model_dir,
+use_fast=True) examples = [ tokenizer( "auto-gptq is an easy-to-use model
+quantization library with user-friendly apis, based on GPTQ algorithm." ) ]
+quantize_config = BaseQuantizeConfig( bits=4, # quantize model to 4-bit
+group_size=128, # it is recommended to set the value to 128 desc_act=False, #
+set to False can significantly speed up inference but the perplexity may
+slightly bad ) # load un-quantized model, by default, the model will always be
+loaded into CPU memory model = AutoGPTQForCausalLM.from_pretrained
+(pretrained_model_dir, quantize_config) # quantize model, the examples should
+be list of dict whose keys can only be "input_ids" and "attention_mask"
+model.quantize(examples) # save quantized model model.save_quantized
+(quantized_model_dir) # save quantized model using safetensors
+model.save_quantized(quantized_model_dir, use_safetensors=True) # push
+quantized model to Hugging Face Hub. # to use use_auth_token=True, Login first
+via huggingface-cli login. # or pass explcit token with:
+use_auth_token="hf_xxxxxxx" # (uncomment the following three lines to enable
+this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
 {quantize_config.bits}bits, gr{quantize_config.group_size}, desc_act=
 {quantize_config.desc_act}" # model.push_to_hub(repo_id,
 commit_message=commit_message, use_auth_token=True) # alternatively you can
 save and push at the same time # (uncomment the following three lines to enable
 this feature) # repo_id = f"YourUserName/{quantized_model_dir}" #
 commit_message = f"AutoGPTQ model for {pretrained_model_dir}:
@@ -165,23 +161,29 @@
 step-by-step guidance to integrate `auto_gptq` with your own project and some
 best practice principles. [examples](examples/README.md) provide plenty of
 example scripts to use `auto_gptq` in different ways. ## Supported Models > you
 can use `model.config.model_type` to compare with the table below to check
 whether the model you use is supported by `auto_gptq`. > > for example,
 model_type of `WizardLM`, `vicuna` and `gpt4all` are all `llama`, hence they
 are all supported by `auto_gptq`. | model type | quantization | inference |
-peft-lora | peft-adaption_prompt | |------------------------------------|------
---------|-----------|-----------|----------------------| | bloom | â | â |
-| | | gpt2 | â | â | | | | gpt_neox | â | â | | | | gptj | â | â |
-| | | llama | â | â | | â | | moss | â | â | | | | opt | â | â |
-| | | gpt_bigcode | â | â | | | | codegen | â | â | | | | falcon
-(RefinedWebModel/RefinedWeb) | â | â | | | ## Supported Evaluation Tasks
-Currently, `auto_gptq` supports: `LanguageModelingTask`,
-`SequenceClassificationTask` and `TextSummarizationTask`; more Tasks will come
-soon! ## Acknowledgement - Specially thanks **Elias Frantar**, **Saleh
-Ashkboos**, **Torsten Hoefler** and **Dan Alistarh** for proposing **GPTQ**
-algorithm and open source the [code](https://github.com/IST-DASLab/gptq). -
-Specially thanks **qwopqwop200**, for code in this project that relevant to
-quantization are mainly referenced from [GPTQ-for-LLaMa](https://github.com/
-qwopqwop200/GPTQ-for-LLaMa/tree/cuda). [![Star History Chart](https://api.star-
-history.com/svg?repos=PanQiwei/AutoGPTQ&type=Date)](https://star-history.com/
-#PanQiWei/AutoGPTQ&Date)
+peft-lora | peft-ada-lora | peft-adaption_prompt | |---------------------------
+---------|--------------|-----------|-----------|---------------|--------------
+-------------------------------------------------------------------------------
+----| | bloom | â | â | â | â | | | gpt2 | â | â | â | â | | |
+gpt_neox | â | â | â | â | â[requires this peft branch](https://
+github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) | | gptj | â | â
+| â | â | â[requires this peft branch](https://github.com/PanQiWei/peft/
+tree/multi_modal_adaption_prompt) | | llama | â | â | â | â | â | |
+moss | â | â | â | â | â[requires this peft branch](https://
+github.com/PanQiWei/peft/tree/multi_modal_adaption_prompt) | | opt | â | â
+| â | â | | | gpt_bigcode | â | â | â | â | | | codegen | â | â
+| â | â | | | falcon(RefinedWebModel/RefinedWeb) | â | â | â | â |
+| ## Supported Evaluation Tasks Currently, `auto_gptq` supports:
+`LanguageModelingTask`, `SequenceClassificationTask` and
+`TextSummarizationTask`; more Tasks will come soon! ## Acknowledgement -
+Specially thanks **Elias Frantar**, **Saleh Ashkboos**, **Torsten Hoefler** and
+**Dan Alistarh** for proposing **GPTQ** algorithm and open source the [code]
+(https://github.com/IST-DASLab/gptq). - Specially thanks **qwopqwop200**, for
+code in this project that relevant to quantization are mainly referenced from
+[GPTQ-for-LLaMa](https://github.com/qwopqwop200/GPTQ-for-LLaMa/tree/cuda). [!
+[Star History Chart](https://api.star-history.com/svg?repos=PanQiwei/
+AutoGPTQ&type=Date)](https://star-history.com/#PanQiWei/AutoGPTQ&Date)
```

### Comparing `auto_gptq-0.2.2/auto_gptq.egg-info/SOURCES.txt` & `auto_gptq-0.3.0/auto_gptq.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -16,37 +16,43 @@
 auto_gptq/eval_tasks/_utils/classification_utils.py
 auto_gptq/eval_tasks/_utils/generation_utils.py
 auto_gptq/modeling/__init__.py
 auto_gptq/modeling/_base.py
 auto_gptq/modeling/_const.py
 auto_gptq/modeling/_utils.py
 auto_gptq/modeling/auto.py
+auto_gptq/modeling/baichuan.py
 auto_gptq/modeling/bloom.py
 auto_gptq/modeling/codegen.py
 auto_gptq/modeling/gpt2.py
 auto_gptq/modeling/gpt_bigcode.py
 auto_gptq/modeling/gpt_neox.py
 auto_gptq/modeling/gptj.py
+auto_gptq/modeling/internlm.py
 auto_gptq/modeling/llama.py
 auto_gptq/modeling/moss.py
 auto_gptq/modeling/opt.py
 auto_gptq/modeling/rw.py
 auto_gptq/nn_modules/__init__.py
 auto_gptq/nn_modules/_fused_base.py
 auto_gptq/nn_modules/fused_gptj_attn.py
 auto_gptq/nn_modules/fused_llama_attn.py
 auto_gptq/nn_modules/fused_llama_mlp.py
-auto_gptq/nn_modules/qlinear.py
-auto_gptq/nn_modules/qlinear_old.py
-auto_gptq/nn_modules/qlinear_triton.py
+auto_gptq/nn_modules/qlinear/__init__.py
+auto_gptq/nn_modules/qlinear/qlinear_cuda.py
+auto_gptq/nn_modules/qlinear/qlinear_cuda_old.py
+auto_gptq/nn_modules/qlinear/qlinear_triton.py
 auto_gptq/nn_modules/triton_utils/__init__.py
 auto_gptq/nn_modules/triton_utils/custom_autotune.py
 auto_gptq/nn_modules/triton_utils/kernels.py
 auto_gptq/nn_modules/triton_utils/mixin.py
 auto_gptq/quantization/__init__.py
 auto_gptq/quantization/gptq.py
 auto_gptq/quantization/quantizer.py
 auto_gptq/utils/__init__.py
 auto_gptq/utils/data_utils.py
 auto_gptq/utils/import_utils.py
-autogptq_cuda/autogptq_cuda.cpp
-autogptq_cuda/autogptq_cuda_kernel.cu
+auto_gptq/utils/peft_utils.py
+autogptq_cuda/autogptq_cuda_256.cpp
+autogptq_cuda/autogptq_cuda_64.cpp
+autogptq_cuda/autogptq_cuda_kernel_256.cu
+autogptq_cuda/autogptq_cuda_kernel_64.cu
```

### Comparing `auto_gptq-0.2.2/autogptq_cuda/autogptq_cuda.cpp` & `auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_256.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,187 +1,202 @@
-#include <torch/all.h>
-#include <torch/python.h>
-#include <c10/cuda/CUDAGuard.h>
-
-void vecquant2matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant2matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-void vecquant3matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant3matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-void vecquant4matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant4matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-void vecquant8matmul_cuda(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-);
-
-void vecquant8matmul(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant8matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
-}
-
-
-// old
-
-void vecquant2matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant2matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_cuda_old(vec, mat, mul, scales, zeros,groupsize);
-}
-
-void vecquant3matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant3matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant4matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant4matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant8matmul_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-); 
-
-void vecquant8matmul_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant8matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
-}
-
-void vecquant2matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant2matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant2matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-void vecquant3matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant3matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant3matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-void vecquant4matmul_faster_cuda_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-); 
-
-void vecquant4matmul_faster_old(
-  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
-  torch::Tensor scales, torch::Tensor zeros,
-  int groupsize, int vec_height
-) {
-  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
-  vecquant4matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
-}
-
-
-PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
-  m.def("vecquant2matmul", &vecquant2matmul, "Vector 2-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant3matmul", &vecquant3matmul, "Vector 3-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant4matmul", &vecquant4matmul, "Vector 4-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant8matmul", &vecquant8matmul, "Vector 8-bit Quantized Matrix Multiplication (CUDA)");
-  
-  m.def("vecquant2matmul_old", &vecquant2matmul_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant3matmul_old", &vecquant3matmul_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant4matmul_old", &vecquant4matmul_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant8matmul_old", &vecquant8matmul_old, "Vector 8-bit Quantized Matrix Multiplication (CUDA)");
-  m.def("vecquant2matmul_faster_old", &vecquant2matmul_faster_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA), faster version");
-  m.def("vecquant3matmul_faster_old", &vecquant3matmul_faster_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA), faster version");
-  m.def("vecquant4matmul_faster_old", &vecquant4matmul_faster_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA), faster version");
-}
+#include <torch/all.h>
+#include <torch/python.h>
+#include <c10/cuda/CUDAGuard.h>
+
+void vecquant2matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant2matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+void vecquant3matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant3matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+void vecquant4matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx, int vec_height
+);
+
+void vecquant4matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx, vec_height);
+}
+
+//void vecquant4matmul_cuda(
+//  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+//  torch::Tensor scales, torch::Tensor zeros,
+//  torch::Tensor g_idx
+//);
+//
+//void vecquant4matmul(
+//  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+//  torch::Tensor scales, torch::Tensor zeros,
+//  torch::Tensor g_idx
+//) {
+//  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+//  vecquant4matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+//}
+
+void vecquant8matmul_cuda(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+);
+
+void vecquant8matmul(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant8matmul_cuda(vec, mat, mul, scales, zeros, g_idx);
+}
+
+
+// old
+
+void vecquant2matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant2matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_cuda_old(vec, mat, mul, scales, zeros,groupsize);
+}
+
+void vecquant3matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant3matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant4matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant4matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant8matmul_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+); 
+
+void vecquant8matmul_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant8matmul_cuda_old(vec, mat, mul, scales, zeros, groupsize);
+}
+
+void vecquant2matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant2matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant2matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+void vecquant3matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant3matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant3matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+void vecquant4matmul_faster_cuda_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+); 
+
+void vecquant4matmul_faster_old(
+  torch::Tensor vec, torch::Tensor mat, torch::Tensor mul,
+  torch::Tensor scales, torch::Tensor zeros,
+  int groupsize, int vec_height
+) {
+  const at::cuda::OptionalCUDAGuard device_guard(device_of(vec));
+  vecquant4matmul_faster_cuda_old(vec, mat, mul, scales, zeros, groupsize, vec_height);
+}
+
+
+PYBIND11_MODULE(TORCH_EXTENSION_NAME, m) {
+  m.def("vecquant2matmul", &vecquant2matmul, "Vector 2-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant3matmul", &vecquant3matmul, "Vector 3-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant4matmul", &vecquant4matmul, "Vector 4-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  m.def("vecquant8matmul", &vecquant8matmul, "Vector 8-bit Quantized Matrix Multiplication (CUDA) (desc_act)");
+  
+  m.def("vecquant2matmul_old", &vecquant2matmul_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant3matmul_old", &vecquant3matmul_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant4matmul_old", &vecquant4matmul_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant8matmul_old", &vecquant8matmul_old, "Vector 8-bit Quantized Matrix Multiplication (CUDA)");
+  m.def("vecquant2matmul_faster_old", &vecquant2matmul_faster_old, "Vector 2-bit Quantized Matrix Multiplication (CUDA), faster version");
+  m.def("vecquant3matmul_faster_old", &vecquant3matmul_faster_old, "Vector 3-bit Quantized Matrix Multiplication (CUDA), faster version");
+  m.def("vecquant4matmul_faster_old", &vecquant4matmul_faster_old, "Vector 4-bit Quantized Matrix Multiplication (CUDA), faster version");
+}
```

### Comparing `auto_gptq-0.2.2/autogptq_cuda/autogptq_cuda_kernel.cu` & `auto_gptq-0.3.0/autogptq_cuda/autogptq_cuda_kernel_64.cu`

 * *Files 20% similar despite different names*

```diff
@@ -1,1390 +1,1560 @@
-#include <torch/all.h>
-#include <torch/python.h>
-#include <cuda.h>
-#include <cuda_runtime.h>
-#include <cuda_fp16.h>
-
-// atomicAdd for double-precision floating-point numbers on hardware with
-// compute capability < 6.0 from:
-// https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#atomic-functions
-#if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 600
-__device__ double atomicAdd(
-    double* address,
-    double val
-) {
-  unsigned long long int* address_as_ull = (unsigned long long int*)address;
-  unsigned long long int old = *address_as_ull, assumed;
-
-  do {
-    assumed = old;
-    old = atomicCAS(
-      address_as_ull,
-      assumed,
-      __double_as_longlong(val + __longlong_as_double(assumed))
-    );
-
-  // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
-  } while (assumed != old);
-
-  return __longlong_as_double(old);
-}
-#endif
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-	const  	    int* __restrict__ g_idx,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-	int zero_width
-);
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant2MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant3MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-__global__ void VecQuant4MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const    int* __restrict__ zeros,
-    int batch,
-    int vec_height, 	
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-);
-
-
-const int BLOCKWIDTH  = 256;
-const int BLOCKHEIGHT2 =  16;
-const int BLOCKHEIGHT3 =  24;
-const int BLOCKHEIGHT4 =  32;
-const int BLOCKHEIGHT8 =  64;
-
-__device__ inline unsigned int as_unsigned(int i) {
-  return *reinterpret_cast<unsigned int*>(&i);
-}
-
-__device__ inline int as_int(int i) {
-  return *reinterpret_cast<int*>(&i);
-}
-
-
-void vecquant2matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant2matmul_cuda", ([&] {
-      VecQuant2MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  		int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 16); 
-	int k_bit = (k % 16) * 2;
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
-	
-    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x3);
-    
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-void vecquant3matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant3matmul_cuda", ([&] {
-      VecQuant3MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = (w / 32) * 3; 
-  int z_mod = w % 32;
-  int z_bit;
-  unsigned int z_tmp;
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 32) * 3; 
-	int k_mod = k % 32;
-	int k_bit;
-	  
-	if (k_mod != 10){
-	  if (k_mod != 21){
-        k_bit = k_mod;
-        if (k_bit > 21){
-		  k_bit -= 22;
-		  k_bit *= 3;
-		  k_bit += 2;
-		  k_w += 2;
-        } else if (k_bit > 10){
-		  k_bit -= 11;
-		  k_bit *= 3;
-		  k_bit += 1;
-		  k_w += 1;
-        } else {
-		  k_bit *= 3;
-        }
-	  } else {
-        k_w += 1;
-	  }
-	}
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = scalar_t((z_tmp) + 1);
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = scalar_t((z_tmp) + 1);
-    } else {
-      zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
-    }
-	
-    if (k_mod == 10) {
-      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 30) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 2) & 0x4);
-    } else if (k_mod == 21){
-      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 31) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 1) & 0x6);
-    } else {
-      w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x7);
-    }
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-void vecquant4matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant4matmul_cuda", ([&] {
-      VecQuant4MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-
-  int z_w = w / 8; 
-  int z_mod = (w % 8) * 4;
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 8); 
-	int k_bit = (k % 8) * 4;
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
-	
-    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xF);
-    
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-void vecquant8matmul_cuda(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  torch::Tensor g_idx
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant8matmul_cuda", ([&] {
-      VecQuant8MatMulKernel<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
-        batch, vec_height, height, width, zero_width
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    const   	int* __restrict__ g_idx,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-	int zero_width
-) {
-  int h = BLOCKHEIGHT8 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-  
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  int i = width * h + w;
-  int g_h = h * 4;
-  int k;
-  unsigned int g;
-  scalar_t w_tmp;
-  
-  int z_w = w / 4; 
-  int z_mod = (w % 4) * 8;
-  
-  float weight[BLOCKWIDTH];
-  
-  for (k = 0; k <  BLOCKWIDTH; ++k){	
-	int k_w = (k / 4); 
-	int k_bit = (k % 4) * 8;
-	
-    g = as_int(g_idx[g_h + k]);
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
-	
-    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xFF);
-    
-	weight[k] = scale * (w_tmp - zero);
-  }
-
-  scalar_t res;
-  for (int b = 0; b < batch; ++b){	
-	res = 0;
-	
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-    __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){	
-	  res += weight[k] * blockvec[k];
-    }
-    atomicAdd(&mul[b * width + w], res);
-    __syncthreads();
-  }
-}
-
-
-void vecquant2matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant2matmul_cuda_old", ([&] {
-      VecQuant2MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant2MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k = 0;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0x3) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 2) & 0x3) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 4) & 0x3) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 6) & 0x3) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp >> 8) & 0x3) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp >> 10) & 0x3) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp >> 12) & 0x3) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp >> 14) & 0x3) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp >> 16) & 0x3) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp >> 18) & 0x3) - zero) * blockvec[k + 9];
-    res += (scale * scalar_t((tmp >> 20) & 0x3) - zero) * blockvec[k + 10];
-    res += (scale * scalar_t((tmp >> 22) & 0x3) - zero) * blockvec[k + 11];
-    res += (scale * scalar_t((tmp >> 24) & 0x3) - zero) * blockvec[k + 12];
-    res += (scale * scalar_t((tmp >> 26) & 0x3) - zero) * blockvec[k + 13];
-    res += (scale * scalar_t((tmp >> 28) & 0x3) - zero) * blockvec[k + 14];
-    res += (scale * scalar_t((tmp >> 30) & 0x3) - zero) * blockvec[k + 15];
-	
-    i += width;
-    k += 16;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant3matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant3matmul_cuda_old", ([&] {
-      VecQuant3MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant3MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k = 0;
-  
-  int z_w = (w / 32) * 3; 
-  int z_mod = w % 32;
-  int z_bit;
-  
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
- 
-  unsigned int tmp1;
-  unsigned int tmp2;
-  unsigned int tmp;
-  unsigned int z_tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp1 = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = scale * scalar_t((z_tmp) + 1);
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = scale * scalar_t((z_tmp) + 1);
-    } else {
-      zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
-    }
-	
-    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    tmp2 = as_unsigned(mat[i]);
-    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x4);
-    tmp2 >>= 1;
-    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
-    k += 11;
-	
-    res += (scale * scalar_t((tmp2 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp2 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp2 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp2 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp2 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp2 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp2 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp2 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp2 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp2 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    tmp1 = as_unsigned(mat[i]);
-    tmp = (tmp2 >> 30) | ((tmp1 << 1) & 0x6);
-    tmp1 >>= 2;
-    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
-    k += 11;
-	
-    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
-    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
-    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
-	
-    i += width;
-    k += 10;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant4matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant4matmul_cuda_old", ([&] {
-      VecQuant4MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant4MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const       int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k = 0;
-
-  int z_w = w / 8; 
-  int z_mod = (w % 8) * 4;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) {
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0xF) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 4) & 0xF) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 8) & 0xF) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 12) & 0xF) - zero) * blockvec[k + 3];
-    res += (scale * scalar_t((tmp >> 16) & 0xF) - zero) * blockvec[k + 4];
-    res += (scale * scalar_t((tmp >> 20) & 0xF) - zero) * blockvec[k + 5];
-    res += (scale * scalar_t((tmp >> 24) & 0xF) - zero) * blockvec[k + 6];
-    res += (scale * scalar_t((tmp >> 28) & 0xF) - zero) * blockvec[k + 7];
-	
-    i += width;
-    k += 8;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant8matmul_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize
-) {
-  int batch = vec.size(0);
-  int vec_height = vec.size(1);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-
-  dim3 blocks(
-    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  AT_DISPATCH_FLOATING_TYPES(
-    vec.type(), "vecquant8matmul_cuda_old", ([&] {
-      VecQuant8MatMulKernel_old<<<blocks, threads>>>(
-        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(),
-        batch, vec_height, height, width, zero_width, groupsize
-      );
-    })
-  );
-}
-
-template <typename scalar_t>
-__global__ void VecQuant8MatMulKernel_old(
-    const  scalar_t* __restrict__ vec,
-    const       int* __restrict__ mat,
-           scalar_t* __restrict__ mul,
-    const  scalar_t* __restrict__ scales,
-    const  	int* __restrict__ zeros,
-    int batch,
-    int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT8 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ scalar_t blockvec[BLOCKWIDTH];
-  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
-  __syncthreads();
-
-  scalar_t res = 0;
-  int i = width * h + w;
-  int g_h = h * 4;
-  int k = 0;
-  
-  int z_w = w / 4; 
-  int z_mod = (w % 4) * 8;
-
-  unsigned int tmp;
-
-  while (k < BLOCKWIDTH) { 
-    tmp = as_unsigned(mat[i]);
-	
-    int g = (g_h + k) / groupsize;
-    scalar_t scale = scales[g * width + w];
-    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
-	
-    res += (scale * scalar_t((tmp >> 0) & 0xFF) - zero) * blockvec[k + 0];
-    res += (scale * scalar_t((tmp >> 8) & 0xFF) - zero) * blockvec[k + 1];
-    res += (scale * scalar_t((tmp >> 16) & 0xFF) - zero) * blockvec[k + 2];
-    res += (scale * scalar_t((tmp >> 24) & 0xFF) - zero) * blockvec[k + 3];
-	
-    i += width;
-    k += 4;
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-
-void vecquant2matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant2MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant2MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT2 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[16][16];
-  int val = threadIdx.x / 16;
-  int off = threadIdx.x % 16;
-  for (; val < 16; val += BLOCKWIDTH / 16) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0x3), __int2half_rn(val >> 2)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = h * 16;
-  int k = 0;
-  
-  int z_w = w / 16; 
-  int z_mod = (w % 16) * 2;
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0x3) + 1)));
-	
-    res2 = {};
-    tmp = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xf][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  4) & 0xf][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xf][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 12) & 0xf][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xf][off], scale, zero), blockvec[k + 4], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 20) & 0xf][off], scale, zero), blockvec[k + 5], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xf][off], scale, zero), blockvec[k + 6], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 28) & 0xf][off], scale, zero), blockvec[k + 7], res2);
-	i += width;
-    k += 8;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant3matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant3MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant3MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT3 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[64][32];
-  int val = threadIdx.x / 32;
-  int off = threadIdx.x % 32;
-  for (; val < 64; val += BLOCKWIDTH / 32) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0x7), __int2half_rn(val >> 3)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = (h / 3) * 32;
-  int k = 0;
-  
-  int z_w = (w / 32) * 3;
-  int z_mod = w % 32;
-  int z_bit;
-  
-  if (z_mod != 10){
-    if (z_mod != 21){
-      z_bit = z_mod;
-      if (z_bit > 21){
-        z_bit -= 22;
-        z_bit *= 3;
-        z_bit += 2;
-        z_w += 2;
-      } else if (z_bit > 10){
-        z_bit -= 11;
-        z_bit *= 3;
-        z_bit += 1;
-        z_w += 1;
-      } else {
-        z_bit *= 3;
-      }
-    } else {
-      z_w += 1;
-    }
-  }
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp1;
-  unsigned int tmp2;
-  unsigned int tmp;
-  unsigned int z_tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero;
-    if (z_mod == 10) {
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
-      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
-    } else if (z_mod == 21){
-      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
-      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
-    } else {
-      zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1)));
-    }
-	
-    res2 = {};
-    tmp1 = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
-    i += width;
-    tmp2 = as_unsigned(mat[i]);
-    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x3c);
-    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 5], res2);
-    tmp2 >>= 4;
-    k += 6;
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    i += width;
-    tmp1 = as_unsigned(mat[i]);
-    tmp = (tmp2 >> 24) | ((tmp1 << 4) & 0x30);
-    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 4], res2);
-    tmp1 >>= 2;
-    k += 5;
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
-    i += width;
-    k += 5;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
-
-void vecquant4matmul_faster_cuda_old(
-  torch::Tensor vec,
-  torch::Tensor mat,
-  torch::Tensor mul,
-  torch::Tensor scales,
-  torch::Tensor zeros,
-  int groupsize,
-  int vec_height
-) {
-  int batch = vec.size(0);
-  int height = mat.size(0);
-  int width = mat.size(1);
-  int zero_width = zeros.size(1);
-  
-  dim3 blocks(
-    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
-    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
-    batch
-  );
-  dim3 threads(BLOCKWIDTH);
-
-  VecQuant4MatMulKernelFaster_old<<<blocks, threads>>>(
-    (half2*) vec.data_ptr(),
-    mat.data_ptr<int>(),
-    mul.data_ptr<float>(),
-    scales.data_ptr<float>(),
-    zeros.data_ptr<int>(),
-    batch, vec_height, height, width, zero_width, groupsize
-  );
-}
-
-__global__ void VecQuant4MatMulKernelFaster_old(
-    const  half2* __restrict__ vec,
-    const    int* __restrict__ mat,
-           float* __restrict__ mul,
-    const  float* __restrict__ scales,
-    const  	 int* __restrict__ zeros,
-	int batch,
-	int vec_height,
-    int height,
-    int width,
-    int zero_width,
-    int groupsize
-) {
-  const int blockwidth2 = BLOCKWIDTH / 2;
-  int b = blockIdx.z;
-  int h = BLOCKHEIGHT4 * blockIdx.x;
-  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
-  __shared__ half2 blockvec[blockwidth2];
-  if (threadIdx.x < blockwidth2)
-    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
-
-  __shared__ half2 deq2[256][8];
-  int val = threadIdx.x / 8;
-  int off = threadIdx.x % 8;
-  for (; val < 256; val += BLOCKWIDTH / 8) {
-    deq2[val][off] = __halves2half2(
-       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
-    );
-  }
-
-  int i = width * h + w;
-  int g_h = h * 8;
-  int k = 0;
-
-  int z_w = w / 8; 
-  int z_mod = (w % 8) * 4;
-
-  float res = 0;
-  half2 res2;
-
-  unsigned int tmp;
-
-  __syncthreads();
-
-  while (k < blockwidth2) {
-    int g = (g_h + (k * 2)) / groupsize;
-	float scale_f = scales[g * width + w];
-    half2 scale = __float2half2_rn(scale_f);
-    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)));
-	
-    res2 = {};
-    tmp = as_unsigned(mat[i]);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scale, zero), blockvec[k + 0], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scale, zero), blockvec[k + 1], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scale, zero), blockvec[k + 2], res2);
-    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scale, zero), blockvec[k + 3], res2);
-	i += width;
-    k += 4;
-    res += __half2float(res2.x) + __half2float(res2.y);
-  }
-
-  atomicAdd(&mul[b * width + w], res);
-}
+#include <torch/all.h>
+#include <torch/python.h>
+#include <cuda.h>
+#include <cuda_runtime.h>
+#include <cuda_fp16.h>
+
+// atomicAdd for double-precision floating-point numbers on hardware with
+// compute capability < 6.0 from:
+// https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#atomic-functions
+// #if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 600
+// __device__ double atomicAdd(
+//     double* address,
+//     double val
+// ) {
+//   unsigned long long int* address_as_ull = (unsigned long long int*)address;
+//   unsigned long long int old = *address_as_ull, assumed;
+//
+//   do {
+//     assumed = old;
+//     old = atomicCAS(
+//       address_as_ull,
+//       assumed,
+//       __double_as_longlong(val + __longlong_as_double(assumed))
+//     );
+//
+//   // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
+//   } while (assumed != old);
+//
+//   return __longlong_as_double(old);
+// }
+// #endif
+
+#if defined(__CUDA_ARCH__) && __CUDA_ARCH__ < 700
+// adapted from https://github.com/torch/cutorch/blob/master/lib/THC/THCAtomics.cuh
+__device__ __forceinline__ void atomicAdd(c10::Half* address, c10::Half val) {
+    unsigned int *address_as_ui = reinterpret_cast<unsigned int *>(reinterpret_cast<char *>(address) - (reinterpret_cast<size_t>(address) & 2));
+    unsigned int old = *address_as_ui;
+    unsigned int assumed;
+
+    do {
+        assumed = old;
+        unsigned short hsum = reinterpret_cast<size_t>(address) & 2 ? (old >> 16) : (old & 0xffff);
+        hsum += val;
+        old = reinterpret_cast<size_t>(address) & 2
+                 ? (old & 0xffff) | (hsum << 16)
+                 : (old & 0xffff0000) | hsum;
+        old = atomicCAS(address_as_ui, assumed, old);
+
+    // Note: uses integer comparison to avoid hang in case of NaN (since NaN != NaN)
+    } while (assumed != old);
+}
+__device__ __forceinline__ void atomicAdd(__half* address, c10::Half val) {
+    unsigned int * address_as_ui = (unsigned int *) ((char *)address - ((size_t)address & 2));
+    unsigned int old = *address_as_ui;
+    unsigned int assumed;
+
+    do {
+        assumed = old;
+        __half_raw hsum;
+        hsum.x = (size_t)address & 2 ? (old >> 16) : (old & 0xffff);
+        half tmpres = __hadd(hsum, val);
+        hsum = __half_raw(tmpres);
+        old = (size_t)address & 2 ? (old & 0xffff) | (hsum.x << 16) : (old & 0xffff0000) | hsum.x;
+        old = atomicCAS(address_as_ui, assumed, old);
+    } while (assumed != old);
+}
+#endif
+
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+// template <typename scalar_t>
+// __global__ void VecQuant4MatMulKernel(
+//     const  scalar_t* __restrict__ vec,
+//     const       int* __restrict__ mat,
+//            scalar_t* __restrict__ mul,
+//     const  scalar_t* __restrict__ scales,
+//     const  		int* __restrict__ zeros,
+// 	const  	    int* __restrict__ g_idx,
+//     int batch,
+//     int vec_height,
+//     int height,
+//     int width,
+// 	int zero_width
+// );
+
+// referenced from https://github.com/iwalton3/GPTQ-for-LLaMa/commit/209d16b0187f149bf13318360925cc4f679cb2ea
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    const    int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+	const  	    int* __restrict__ g_idx,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+	int zero_width
+);
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant2MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant3MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+__global__ void VecQuant4MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const    int* __restrict__ zeros,
+    int batch,
+    int vec_height, 	
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+);
+
+
+const int BLOCKWIDTH  = 64;
+const int BLOCKHEIGHT2 =  4;
+const int BLOCKHEIGHT3 =  6;
+const int BLOCKHEIGHT4 =  8;
+const int BLOCKHEIGHT8 =  16;
+
+__device__ inline unsigned int as_unsigned(int i) {
+  return *reinterpret_cast<unsigned int*>(&i);
+}
+
+__device__ inline int as_int(int i) {
+  return *reinterpret_cast<int*>(&i);
+}
+
+
+void vecquant2matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant2matmul_cuda", ([&] {
+      VecQuant2MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  		int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 16); 
+	int k_bit = (k % 16) * 2;
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
+	
+    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x3);
+    
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+void vecquant3matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant3matmul_cuda", ([&] {
+      VecQuant3MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = (w / 32) * 3; 
+  int z_mod = w % 32;
+  int z_bit;
+  unsigned int z_tmp;
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 32) * 3; 
+	int k_mod = k % 32;
+	int k_bit;
+	  
+	if (k_mod != 10){
+	  if (k_mod != 21){
+        k_bit = k_mod;
+        if (k_bit > 21){
+		  k_bit -= 22;
+		  k_bit *= 3;
+		  k_bit += 2;
+		  k_w += 2;
+        } else if (k_bit > 10){
+		  k_bit -= 11;
+		  k_bit *= 3;
+		  k_bit += 1;
+		  k_w += 1;
+        } else {
+		  k_bit *= 3;
+        }
+	  } else {
+        k_w += 1;
+	  }
+	}
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = scalar_t((z_tmp) + 1);
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = scalar_t((z_tmp) + 1);
+    } else {
+      zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
+    }
+	
+    if (k_mod == 10) {
+      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 30) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 2) & 0x4);
+    } else if (k_mod == 21){
+      w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 31) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 1) & 0x6);
+    } else {
+      w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x7);
+    }
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+void vecquant4matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_SWITCH(vec.type(), "vecquant4matmul_cuda",
+    AT_DISPATCH_CASE(at::ScalarType::Half, ([&] {
+      VecQuant4MatMulKernel<<<blocks, threads>>>(
+        (half2*) vec.data_ptr<scalar_t>(),
+        mat.data_ptr<int>(),
+        mul.data_ptr<scalar_t>(),
+        scales.data_ptr<scalar_t>(),
+        zeros.data_ptr<int>(),
+        g_idx.data_ptr<int>(),
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  ));
+}
+
+// void vecquant4matmul_cuda(
+//   torch::Tensor vec,
+//   torch::Tensor mat,
+//   torch::Tensor mul,
+//   torch::Tensor scales,
+//   torch::Tensor zeros,
+//   torch::Tensor g_idx
+// ) {
+//   int batch = vec.size(0);
+//   int vec_height = vec.size(1);
+//   int height = mat.size(0);
+//   int width = mat.size(1);
+//   int zero_width = zeros.size(1);
+//
+//   dim3 blocks(
+//     (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+//     (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+//   );
+//   dim3 threads(BLOCKWIDTH);
+//
+//   AT_DISPATCH_FLOATING_TYPES(
+//     vec.type(), "vecquant4matmul_cuda", ([&] {
+//       VecQuant4MatMulKernel<<<blocks, threads>>>(
+//         vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+//         scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(),
+//         batch, vec_height, height, width, zero_width
+//       );
+//     })
+//   );
+// }
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel(
+    const     half2* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	    int* __restrict__ zeros,
+    const       int* __restrict__ g_idx,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[256][8];
+  int val = threadIdx.x / 8;
+  int off = threadIdx.x % 8;
+  for (; val < 256; val += BLOCKWIDTH / 8) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k = 0;
+
+  int z_w = w / 8;
+  int z_mod = (w % 8) * 4;
+
+  scalar_t res = 0;
+  half2 res2;
+
+  unsigned int tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    res2 = {};
+    tmp = as_unsigned(mat[i]);
+
+    int tmp_k = 0;
+    half2 scales_tmp[4];
+    half2 zeros_tmp[4];
+    while (tmp_k < 4) {
+      int g = as_int(g_idx[g_h + (k + tmp_k) * 2]);
+      int g2 = as_int(g_idx[g_h + (k + tmp_k) * 2 + 1]);
+      scalar_t scale_f = scales[g * width + w];
+      scalar_t scale_f2 = scales[g2 * width + w];
+      half2 scale = __halves2half2(scale_f, scale_f2);
+      half2 zero = __halves2half2(
+        __hmul(-scale_f, __int2half_rn(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)),
+        __hmul(-scale_f2, __int2half_rn(((as_unsigned(zeros[g2 * zero_width + z_w]) >> z_mod) & 0xF) + 1))
+      );
+      scales_tmp[tmp_k] = scale;
+      zeros_tmp[tmp_k] = zero;
+      tmp_k += 1;
+    }
+
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scales_tmp[0], zeros_tmp[0]), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scales_tmp[1], zeros_tmp[1]), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scales_tmp[2], zeros_tmp[2]), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scales_tmp[3], zeros_tmp[3]), blockvec[k + 3], res2);
+	i += width;
+    k += 4;
+    res = __hadd(res, __hadd(res2.x, res2.y));;
+  }
+
+  __half* mul2 = (__half*)mul;
+  atomicAdd(&mul2[b * width + w], res);
+}
+
+// template <typename scalar_t>
+// __global__ void VecQuant4MatMulKernel(
+//     const  scalar_t* __restrict__ vec,
+//     const       int* __restrict__ mat,
+//            scalar_t* __restrict__ mul,
+//     const  scalar_t* __restrict__ scales,
+//     const       int* __restrict__ zeros,
+//     const   	int* __restrict__ g_idx,
+//     int batch,
+//     int vec_height,
+//     int height,
+//     int width,
+// 	int zero_width
+// ) {
+//   int h = BLOCKHEIGHT4 * blockIdx.x;
+//   int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+//
+//   __shared__ scalar_t blockvec[BLOCKWIDTH];
+//   int i = width * h + w;
+//   int g_h = h * 8;
+//   int k;
+//   unsigned int g;
+//   scalar_t w_tmp;
+//
+//
+//   int z_w = w / 8;
+//   int z_mod = (w % 8) * 4;
+//
+//   float weight[BLOCKWIDTH];
+//
+//   for (k = 0; k <  BLOCKWIDTH; ++k){
+// 	int k_w = (k / 8);
+// 	int k_bit = (k % 8) * 4;
+//
+//     g = as_int(g_idx[g_h + k]);
+//     scalar_t scale = scales[g * width + w];
+//     scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
+//
+//     w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xF);
+//
+// 	weight[k] = scale * (w_tmp - zero);
+//   }
+//
+//   scalar_t res;
+//   for (int b = 0; b < batch; ++b){
+// 	res = 0;
+//
+//     blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+//     __syncthreads();
+// 	for (k = 0; k <  BLOCKWIDTH; ++k){
+// 	  res += weight[k] * blockvec[k];
+//     }
+//     atomicAdd(&mul[b * width + w], res);
+//     __syncthreads();
+//   }
+// }
+
+void vecquant8matmul_cuda(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  torch::Tensor g_idx
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant8matmul_cuda", ([&] {
+      VecQuant8MatMulKernel<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
+        batch, vec_height, height, width, zero_width
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    const   	int* __restrict__ g_idx,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+	int zero_width
+) {
+  int h = BLOCKHEIGHT8 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+  
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  int i = width * h + w;
+  int g_h = h * 4;
+  int k;
+  unsigned int g;
+  scalar_t w_tmp;
+  
+  int z_w = w / 4; 
+  int z_mod = (w % 4) * 8;
+  
+  float weight[BLOCKWIDTH];
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 4); 
+	int k_bit = (k % 4) * 8;
+	
+    g = as_int(g_idx[g_h + k]);
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
+	
+    w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xFF);
+    
+	weight[k] = scale * (w_tmp - zero);
+  }
+
+  scalar_t res;
+  for (int b = 0; b < batch; ++b){	
+	res = 0;
+	
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+    __syncthreads();
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
+	  res += weight[k] * blockvec[k];
+    }
+    atomicAdd(&mul[b * width + w], res);
+    __syncthreads();
+  }
+}
+
+
+void vecquant2matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant2matmul_cuda_old", ([&] {
+      VecQuant2MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant2MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k = 0;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0x3) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 2) & 0x3) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 4) & 0x3) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 6) & 0x3) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp >> 8) & 0x3) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp >> 10) & 0x3) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp >> 12) & 0x3) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp >> 14) & 0x3) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp >> 16) & 0x3) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp >> 18) & 0x3) - zero) * blockvec[k + 9];
+    res += (scale * scalar_t((tmp >> 20) & 0x3) - zero) * blockvec[k + 10];
+    res += (scale * scalar_t((tmp >> 22) & 0x3) - zero) * blockvec[k + 11];
+    res += (scale * scalar_t((tmp >> 24) & 0x3) - zero) * blockvec[k + 12];
+    res += (scale * scalar_t((tmp >> 26) & 0x3) - zero) * blockvec[k + 13];
+    res += (scale * scalar_t((tmp >> 28) & 0x3) - zero) * blockvec[k + 14];
+    res += (scale * scalar_t((tmp >> 30) & 0x3) - zero) * blockvec[k + 15];
+	
+    i += width;
+    k += 16;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant3matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant3matmul_cuda_old", ([&] {
+      VecQuant3MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant3MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k = 0;
+  
+  int z_w = (w / 32) * 3; 
+  int z_mod = w % 32;
+  int z_bit;
+  
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+ 
+  unsigned int tmp1;
+  unsigned int tmp2;
+  unsigned int tmp;
+  unsigned int z_tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp1 = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = scale * scalar_t((z_tmp) + 1);
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = scale * scalar_t((z_tmp) + 1);
+    } else {
+      zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
+    }
+	
+    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    tmp2 = as_unsigned(mat[i]);
+    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x4);
+    tmp2 >>= 1;
+    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
+    k += 11;
+	
+    res += (scale * scalar_t((tmp2 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp2 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp2 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp2 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp2 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp2 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp2 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp2 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp2 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp2 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    tmp1 = as_unsigned(mat[i]);
+    tmp = (tmp2 >> 30) | ((tmp1 << 1) & 0x6);
+    tmp1 >>= 2;
+    res += (scale * scalar_t(tmp) - zero) * blockvec[k + 10];
+    k += 11;
+	
+    res += (scale * scalar_t((tmp1 >>  0) & 0x7) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp1 >>  3) & 0x7) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp1 >>  6) & 0x7) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp1 >>  9) & 0x7) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp1 >> 12) & 0x7) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp1 >> 15) & 0x7) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp1 >> 18) & 0x7) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp1 >> 21) & 0x7) - zero) * blockvec[k + 7];
+    res += (scale * scalar_t((tmp1 >> 24) & 0x7) - zero) * blockvec[k + 8];
+    res += (scale * scalar_t((tmp1 >> 27) & 0x7) - zero) * blockvec[k + 9];
+	
+    i += width;
+    k += 10;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant4matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant4matmul_cuda_old", ([&] {
+      VecQuant4MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant4MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const       int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k = 0;
+
+  int z_w = w / 8; 
+  int z_mod = (w % 8) * 4;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) {
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0xF) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 4) & 0xF) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 8) & 0xF) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 12) & 0xF) - zero) * blockvec[k + 3];
+    res += (scale * scalar_t((tmp >> 16) & 0xF) - zero) * blockvec[k + 4];
+    res += (scale * scalar_t((tmp >> 20) & 0xF) - zero) * blockvec[k + 5];
+    res += (scale * scalar_t((tmp >> 24) & 0xF) - zero) * blockvec[k + 6];
+    res += (scale * scalar_t((tmp >> 28) & 0xF) - zero) * blockvec[k + 7];
+	
+    i += width;
+    k += 8;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant8matmul_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize
+) {
+  int batch = vec.size(0);
+  int vec_height = vec.size(1);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+
+  dim3 blocks(
+    (height + BLOCKHEIGHT8 - 1) / BLOCKHEIGHT8,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  AT_DISPATCH_FLOATING_TYPES(
+    vec.type(), "vecquant8matmul_cuda_old", ([&] {
+      VecQuant8MatMulKernel_old<<<blocks, threads>>>(
+        vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
+        scales.data<scalar_t>(), zeros.data<int>(),
+        batch, vec_height, height, width, zero_width, groupsize
+      );
+    })
+  );
+}
+
+template <typename scalar_t>
+__global__ void VecQuant8MatMulKernel_old(
+    const  scalar_t* __restrict__ vec,
+    const       int* __restrict__ mat,
+           scalar_t* __restrict__ mul,
+    const  scalar_t* __restrict__ scales,
+    const  	int* __restrict__ zeros,
+    int batch,
+    int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT8 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ scalar_t blockvec[BLOCKWIDTH];
+  blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
+  __syncthreads();
+
+  scalar_t res = 0;
+  int i = width * h + w;
+  int g_h = h * 4;
+  int k = 0;
+  
+  int z_w = w / 4; 
+  int z_mod = (w % 4) * 8;
+
+  unsigned int tmp;
+
+  while (k < BLOCKWIDTH) { 
+    tmp = as_unsigned(mat[i]);
+	
+    int g = (g_h + k) / groupsize;
+    scalar_t scale = scales[g * width + w];
+    scalar_t zero = scale * scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
+	
+    res += (scale * scalar_t((tmp >> 0) & 0xFF) - zero) * blockvec[k + 0];
+    res += (scale * scalar_t((tmp >> 8) & 0xFF) - zero) * blockvec[k + 1];
+    res += (scale * scalar_t((tmp >> 16) & 0xFF) - zero) * blockvec[k + 2];
+    res += (scale * scalar_t((tmp >> 24) & 0xFF) - zero) * blockvec[k + 3];
+	
+    i += width;
+    k += 4;
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+
+void vecquant2matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT2 - 1) / BLOCKHEIGHT2,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant2MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant2MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT2 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[16][16];
+  int val = threadIdx.x / 16;
+  int off = threadIdx.x % 16;
+  for (; val < 16; val += BLOCKWIDTH / 16) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0x3), __int2half_rn(val >> 2)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = h * 16;
+  int k = 0;
+  
+  int z_w = w / 16; 
+  int z_mod = (w % 16) * 2;
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0x3) + 1)));
+	
+    res2 = {};
+    tmp = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xf][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  4) & 0xf][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xf][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 12) & 0xf][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xf][off], scale, zero), blockvec[k + 4], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 20) & 0xf][off], scale, zero), blockvec[k + 5], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xf][off], scale, zero), blockvec[k + 6], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 28) & 0xf][off], scale, zero), blockvec[k + 7], res2);
+	i += width;
+    k += 8;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant3matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT3 - 1) / BLOCKHEIGHT3,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant3MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant3MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT3 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[64][32];
+  int val = threadIdx.x / 32;
+  int off = threadIdx.x % 32;
+  for (; val < 64; val += BLOCKWIDTH / 32) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0x7), __int2half_rn(val >> 3)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = (h / 3) * 32;
+  int k = 0;
+  
+  int z_w = (w / 32) * 3;
+  int z_mod = w % 32;
+  int z_bit;
+  
+  if (z_mod != 10){
+    if (z_mod != 21){
+      z_bit = z_mod;
+      if (z_bit > 21){
+        z_bit -= 22;
+        z_bit *= 3;
+        z_bit += 2;
+        z_w += 2;
+      } else if (z_bit > 10){
+        z_bit -= 11;
+        z_bit *= 3;
+        z_bit += 1;
+        z_w += 1;
+      } else {
+        z_bit *= 3;
+      }
+    } else {
+      z_w += 1;
+    }
+  }
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp1;
+  unsigned int tmp2;
+  unsigned int tmp;
+  unsigned int z_tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero;
+    if (z_mod == 10) {
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
+      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
+    } else if (z_mod == 21){
+      z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
+      zero = __float2half2_rn(-(scale_f * ((z_tmp) + 1)));
+    } else {
+      zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1)));
+    }
+	
+    res2 = {};
+    tmp1 = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
+    i += width;
+    tmp2 = as_unsigned(mat[i]);
+    tmp = (tmp1 >> 30) | ((tmp2 << 2) & 0x3c);
+    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 5], res2);
+    tmp2 >>= 4;
+    k += 6;
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp2 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    i += width;
+    tmp1 = as_unsigned(mat[i]);
+    tmp = (tmp2 >> 24) | ((tmp1 << 4) & 0x30);
+    res2 = __hfma2(__hfma2(deq2[tmp][off], scale, zero), blockvec[k + 4], res2);
+    tmp1 >>= 2;
+    k += 5;
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  0) & 0x3f][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >>  6) & 0x3f][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 12) & 0x3f][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 18) & 0x3f][off], scale, zero), blockvec[k + 3], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp1 >> 24) & 0x3f][off], scale, zero), blockvec[k + 4], res2);
+    i += width;
+    k += 5;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
+
+void vecquant4matmul_faster_cuda_old(
+  torch::Tensor vec,
+  torch::Tensor mat,
+  torch::Tensor mul,
+  torch::Tensor scales,
+  torch::Tensor zeros,
+  int groupsize,
+  int vec_height
+) {
+  int batch = vec.size(0);
+  int height = mat.size(0);
+  int width = mat.size(1);
+  int zero_width = zeros.size(1);
+  
+  dim3 blocks(
+    (height + BLOCKHEIGHT4 - 1) / BLOCKHEIGHT4,
+    (width + BLOCKWIDTH - 1) / BLOCKWIDTH,
+    batch
+  );
+  dim3 threads(BLOCKWIDTH);
+
+  VecQuant4MatMulKernelFaster_old<<<blocks, threads>>>(
+    (half2*) vec.data_ptr(),
+    mat.data_ptr<int>(),
+    mul.data_ptr<float>(),
+    scales.data_ptr<float>(),
+    zeros.data_ptr<int>(),
+    batch, vec_height, height, width, zero_width, groupsize
+  );
+}
+
+__global__ void VecQuant4MatMulKernelFaster_old(
+    const  half2* __restrict__ vec,
+    const    int* __restrict__ mat,
+           float* __restrict__ mul,
+    const  float* __restrict__ scales,
+    const  	 int* __restrict__ zeros,
+	int batch,
+	int vec_height,
+    int height,
+    int width,
+    int zero_width,
+    int groupsize
+) {
+  const int blockwidth2 = BLOCKWIDTH / 2;
+  int b = blockIdx.z;
+  int h = BLOCKHEIGHT4 * blockIdx.x;
+  int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
+
+  __shared__ half2 blockvec[blockwidth2];
+  if (threadIdx.x < blockwidth2)
+    blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * blockwidth2 + threadIdx.x];
+
+  __shared__ half2 deq2[256][8];
+  int val = threadIdx.x / 8;
+  int off = threadIdx.x % 8;
+  for (; val < 256; val += BLOCKWIDTH / 8) {
+    deq2[val][off] = __halves2half2(
+       __int2half_rn(val & 0xF), __int2half_rn(val >> 4)
+    );
+  }
+
+  int i = width * h + w;
+  int g_h = h * 8;
+  int k = 0;
+
+  int z_w = w / 8; 
+  int z_mod = (w % 8) * 4;
+
+  float res = 0;
+  half2 res2;
+
+  unsigned int tmp;
+
+  __syncthreads();
+
+  while (k < blockwidth2) {
+    int g = (g_h + (k * 2)) / groupsize;
+	float scale_f = scales[g * width + w];
+    half2 scale = __float2half2_rn(scale_f);
+    half2 zero = __float2half2_rn(-(scale_f * (((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1)));
+	
+    res2 = {};
+    tmp = as_unsigned(mat[i]);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  0) & 0xff][off], scale, zero), blockvec[k + 0], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >>  8) & 0xff][off], scale, zero), blockvec[k + 1], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 16) & 0xff][off], scale, zero), blockvec[k + 2], res2);
+    res2 = __hfma2(__hfma2(deq2[(tmp >> 24) & 0xff][off], scale, zero), blockvec[k + 3], res2);
+	i += width;
+    k += 4;
+    res += __half2float(res2.x) + __half2float(res2.y);
+  }
+
+  atomicAdd(&mul[b * width + w], res);
+}
```

### Comparing `auto_gptq-0.2.2/setup.py` & `auto_gptq-0.3.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,112 @@
-import os
-import platform
-import sys
-from pathlib import Path
-from setuptools import setup, find_packages
-
-try:
-    import torch
-    TORCH_AVAILABLE = True
-except ImportError:
-    TORCH_AVAILABLE = False
-
-IN_GITHUB_ACTIONS = os.environ.get("GITHUB_ACTIONS", "false") == "true"
-
-python_min_version = (3, 8, 0)
-python_min_version_str = '.'.join(map(str, python_min_version))
-if sys.version_info < python_min_version:
-    print(f"You are using Python {platform.python_version()}. Python >={python_min_version_str} is required.")
-    sys.exit(-1)
-
-CUDA_VERSION = "".join(os.environ.get("CUDA_VERSION", "").split("."))
-
-version = "0.2.2" + (f"+cu{CUDA_VERSION}" if CUDA_VERSION and IN_GITHUB_ACTIONS else "")
-common_setup_kwargs = {
-    "version": version,
-    "name": "auto_gptq",
-    "author": "PanQiWei",
-    "description": "An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.",
-    "long_description": (Path(__file__).parent / "README.md").read_text(encoding="UTF-8"),
-    "long_description_content_type": "text/markdown",
-    "url": "https://github.com/PanQiWei/AutoGPTQ",
-    "keywords": ["gptq", "quantization", "large-language-models", "pytorch", "transformers"],
-    "platforms": ["windows", "linux"],
-    "classifiers": [
-        "Environment :: GPU :: NVIDIA CUDA :: 11.7",
-        "Environment :: GPU :: NVIDIA CUDA :: 11.8",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: Chinese (Simplified)",
-        "Natural Language :: English",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: C++",
-    ],
-    "python_requires": f">={python_min_version_str}"
-}
-
-requirements = [
-    "accelerate>=0.19.0",
-    "datasets",
-    "numpy",
-    "rouge",
-    "torch>=1.13.0",
-    "safetensors",
-    "transformers>=4.26.1"
-]
-
-extras_require = {
-    "llama": ["transformers>=4.28.0"],
-    "triton": ["triton>=2.0.0"]
-}
-
-include_dirs = ["autogptq_cuda"]
-
-if TORCH_AVAILABLE:
-    BUILD_CUDA_EXT = int(os.environ.get('BUILD_CUDA_EXT', '1')) == 1
-    
-    additional_setup_kwargs = dict()
-    if BUILD_CUDA_EXT and (torch.cuda.is_available() or IN_GITHUB_ACTIONS):
-        from torch.utils import cpp_extension
-        from distutils.sysconfig import get_python_lib
-        conda_cuda_include_dir=os.path.join(get_python_lib(),"nvidia/cuda_runtime/include")
-        if os.path.isdir(conda_cuda_include_dir):
-            include_dirs.append(conda_cuda_include_dir)
-            print(f"appending conda cuda include dir {conda_cuda_include_dir}")
-        extensions = [
-            cpp_extension.CUDAExtension(
-                "autogptq_cuda",
-                [
-                    "autogptq_cuda/autogptq_cuda.cpp",
-                    "autogptq_cuda/autogptq_cuda_kernel.cu"
-                ]
-            )
-        ]
-
-        additional_setup_kwargs = {
-            "ext_modules": extensions,
-            "cmdclass": {'build_ext': cpp_extension.BuildExtension}
-        }
-    common_setup_kwargs.update(additional_setup_kwargs)
-    print(f"include dirs are: {include_dirs}")
-    setup(
-        packages=find_packages(),
-        install_requires=requirements,
-        extras_require=extras_require,
-        include_dirs=include_dirs,
-        **common_setup_kwargs
-    )
-else:
-    print(f"include dirs are: {include_dirs}")
-    for each in include_dirs:
-        assert os.path.isdir(each)
-    setup(
-        packages=find_packages(),
-        install_requires=requirements,
-        extras_require=extras_require,
-        include_dirs=include_dirs,
-        **common_setup_kwargs
-    )
+import os
+import platform
+import sys
+from pathlib import Path
+from setuptools import setup, find_packages
+
+try:
+    import torch
+    TORCH_AVAILABLE = True
+except ImportError:
+    TORCH_AVAILABLE = False
+
+IN_GITHUB_ACTIONS = os.environ.get("GITHUB_ACTIONS", "false") == "true"
+
+python_min_version = (3, 8, 0)
+python_min_version_str = '.'.join(map(str, python_min_version))
+if sys.version_info < python_min_version:
+    print(f"You are using Python {platform.python_version()}. Python >={python_min_version_str} is required.")
+    sys.exit(-1)
+
+CUDA_VERSION = "".join(os.environ.get("CUDA_VERSION", "").split("."))
+
+version = "0.3.0" + (f"+cu{CUDA_VERSION}" if CUDA_VERSION and IN_GITHUB_ACTIONS else "")
+common_setup_kwargs = {
+    "version": version,
+    "name": "auto_gptq",
+    "author": "PanQiWei",
+    "description": "An easy-to-use LLMs quantization package with user-friendly apis, based on GPTQ algorithm.",
+    "long_description": (Path(__file__).parent / "README.md").read_text(encoding="UTF-8"),
+    "long_description_content_type": "text/markdown",
+    "url": "https://github.com/PanQiWei/AutoGPTQ",
+    "keywords": ["gptq", "quantization", "large-language-models", "pytorch", "transformers"],
+    "platforms": ["windows", "linux"],
+    "classifiers": [
+        "Environment :: GPU :: NVIDIA CUDA :: 11.7",
+        "Environment :: GPU :: NVIDIA CUDA :: 11.8",
+        "License :: OSI Approved :: MIT License",
+        "Natural Language :: Chinese (Simplified)",
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: C++",
+    ],
+    "python_requires": f">={python_min_version_str}"
+}
+
+requirements = [
+    "accelerate>=0.19.0",
+    "datasets",
+    "numpy",
+    "rouge",
+    "torch>=1.13.0",
+    "safetensors",
+    "transformers>=4.29.0",
+    "peft"
+]
+
+extras_require = {
+    "triton": ["triton>=2.0.0"]
+}
+
+include_dirs = ["autogptq_cuda"]
+
+if TORCH_AVAILABLE:
+    BUILD_CUDA_EXT = int(os.environ.get('BUILD_CUDA_EXT', '1')) == 1
+    
+    additional_setup_kwargs = dict()
+    if BUILD_CUDA_EXT and (torch.cuda.is_available() or IN_GITHUB_ACTIONS):
+        from torch.utils import cpp_extension
+        from distutils.sysconfig import get_python_lib
+        conda_cuda_include_dir = os.path.join(get_python_lib(), "nvidia/cuda_runtime/include")
+        if os.path.isdir(conda_cuda_include_dir):
+            include_dirs.append(conda_cuda_include_dir)
+            print(f"appending conda cuda include dir {conda_cuda_include_dir}")
+        extensions = [
+            cpp_extension.CUDAExtension(
+                "autogptq_cuda_64",
+                [
+                    "autogptq_cuda/autogptq_cuda_64.cpp",
+                    "autogptq_cuda/autogptq_cuda_kernel_64.cu"
+                ]
+            ),
+            cpp_extension.CUDAExtension(
+                "autogptq_cuda_256",
+                [
+                    "autogptq_cuda/autogptq_cuda_256.cpp",
+                    "autogptq_cuda/autogptq_cuda_kernel_256.cu"
+                ]
+            )
+        ]
+
+        additional_setup_kwargs = {
+            "ext_modules": extensions,
+            "cmdclass": {'build_ext': cpp_extension.BuildExtension}
+        }
+    common_setup_kwargs.update(additional_setup_kwargs)
+    setup(
+        packages=find_packages(),
+        install_requires=requirements,
+        extras_require=extras_require,
+        include_dirs=include_dirs,
+        **common_setup_kwargs
+    )
+else:
+    setup(
+        packages=find_packages(),
+        install_requires=requirements,
+        extras_require=extras_require,
+        include_dirs=include_dirs,
+        **common_setup_kwargs
+    )
```

