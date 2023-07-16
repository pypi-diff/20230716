# Comparing `tmp/llama_index-0.7.8.tar.gz` & `tmp/llama_index-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index-0.7.8.tar", last modified: Fri Jul 14 02:40:30 2023, max compression
+gzip compressed data, was "llama_index-0.7.9.tar", last modified: Sun Jul 16 04:38:32 2023, max compression
```

## Comparing `llama_index-0.7.8.tar` & `llama_index-0.7.9.tar`

### file list

```diff
@@ -1,672 +1,676 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.018167 llama_index-0.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-14 02:40:11.000000 llama_index-0.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-14 02:40:11.000000 llama_index-0.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-14 02:40:30.018167 llama_index-0.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-14 02:40:11.000000 llama_index-0.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.914166 llama_index-0.7.8/llama_index/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.914166 llama_index-0.7.8/llama_index/agent/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/context_retriever_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/openai_agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.914166 llama_index-0.7.8/llama_index/agent/react/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/react/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/react/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/react/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/react/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/react/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/react/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/retriever_openai_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/agent/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/async_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.918166 llama_index-0.7.8/llama_index/bridge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/bridge/langchain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.918166 llama_index-0.7.8/llama_index/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/callbacks/aim.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/callbacks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/callbacks/llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/callbacks/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/callbacks/token_counting.py
--rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/callbacks/wandb_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.918166 llama_index-0.7.8/llama_index/chat_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/chat_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/chat_engine/condense_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/chat_engine/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/chat_engine/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/chat_engine/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.918166 llama_index-0.7.8/llama_index/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/composability/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/composability/joint_qa_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.918166 llama_index-0.7.8/llama_index/data_structs/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/data_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/data_structs/data_structs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/data_structs/document_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/data_structs/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/data_structs/struct_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/data_structs/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.922166 llama_index-0.7.8/llama_index/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/embeddings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/embeddings/google.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/embeddings/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/embeddings/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/embeddings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.922166 llama_index-0.7.8/llama_index/evaluation/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/evaluation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/evaluation/dataset_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/evaluation/guideline_eval.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.922166 llama_index-0.7.8/llama_index/graph_stores/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/graph_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19697 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/graph_stores/nebulagraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/graph_stores/registery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/graph_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/graph_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/img_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.922166 llama_index-0.7.8/llama_index/indices/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/base_retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.926166 llama_index-0.7.8/llama_index/indices/common/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.926166 llama_index-0.7.8/llama_index/indices/common/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/common/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/common/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/common/struct_store/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/common/struct_store/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.926166 llama_index-0.7.8/llama_index/indices/common_tree/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/common_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/common_tree/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.926166 llama_index-0.7.8/llama_index/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/composability/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.926166 llama_index-0.7.8/llama_index/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/document_summary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/document_summary/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.926166 llama_index-0.7.8/llama_index/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/empty/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/empty/retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.926166 llama_index-0.7.8/llama_index/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/keyword_table/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/keyword_table/rake_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/keyword_table/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/keyword_table/simple_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/keyword_table/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.930166 llama_index-0.7.8/llama_index/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/knowledge_graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/knowledge_graph/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.930166 llama_index-0.7.8/llama_index/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/list/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/list/retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.930166 llama_index-0.7.8/llama_index/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/postprocessor/cohere_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/postprocessor/llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/postprocessor/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/postprocessor/node_recency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/postprocessor/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/postprocessor/pii.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/postprocessor/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/prompt_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.930166 llama_index-0.7.8/llama_index/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/query/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/query/embedding_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.934167 llama_index-0.7.8/llama_index/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/query/query_transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/query/query_transform/feedback_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/query/query_transform/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8973 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/service_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.934167 llama_index-0.7.8/llama_index/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/struct_store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/struct_store/container_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/struct_store/json_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/struct_store/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/struct_store/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/struct_store/sql_query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.934167 llama_index-0.7.8/llama_index/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/tree/all_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/tree/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/tree/inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/tree/select_leaf_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/tree/select_leaf_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/tree/tree_root_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/tree/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.934167 llama_index-0.7.8/llama_index/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/vector_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/vector_store/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.934167 llama_index-0.7.8/llama_index/indices/vector_store/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/vector_store/retrievers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.938166 llama_index-0.7.8/llama_index/indices/vector_store/retrievers/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/indices/vector_store/retrievers/retriever.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.938166 llama_index-0.7.8/llama_index/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.938166 llama_index-0.7.8/llama_index/langchain_helpers/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/agents/agents.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/agents/toolkits.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/agents/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/memory_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/sql_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/langchain_helpers/text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.938166 llama_index-0.7.8/llama_index/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/structured.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.942166 llama_index-0.7.8/llama_index/llm_predictor/vellum/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/vellum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/vellum/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/vellum/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/vellum/prompt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/vellum/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llm_predictor/vellum/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.942166 llama_index-0.7.8/llama_index/llms/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/anthropic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/azure_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/generic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/langchain_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/palm.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/llms/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.942166 llama_index-0.7.8/llama_index/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/logger/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.942166 llama_index-0.7.8/llama_index/memory/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/memory/chat_memory_buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/memory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.946166 llama_index-0.7.8/llama_index/node_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/node_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.946166 llama_index-0.7.8/llama_index/node_parser/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/node_parser/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/node_parser/extractors/metadata_extractors.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/node_parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/node_parser/node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/node_parser/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.946166 llama_index-0.7.8/llama_index/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/objects/base_node_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/objects/table_node_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/objects/tool_node_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.946166 llama_index-0.7.8/llama_index/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/output_parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/output_parsers/guardrails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/output_parsers/langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/output_parsers/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/output_parsers/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/output_parsers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.946166 llama_index-0.7.8/llama_index/playground/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/playground/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.950167 llama_index-0.7.8/llama_index/program/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/base_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/guidance_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/llm_program.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/llm_prompt_program.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/openai_program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.950167 llama_index-0.7.8/llama_index/program/predefined/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/predefined/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/predefined/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.950167 llama_index-0.7.8/llama_index/program/predefined/evaporate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/predefined/evaporate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/predefined/evaporate/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/predefined/evaporate/extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/program/predefined/evaporate/prompts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.950167 llama_index-0.7.8/llama_index/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/chat_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/choice_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/default_prompt_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/default_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/guidance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/prompt_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/prompt_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.954167 llama_index-0.7.8/llama_index/query_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/citation_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.954167 llama_index-0.7.8/llama_index/query_engine/flare/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/flare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/flare/answer_inserter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/flare/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/flare/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/flare/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/knowledge_graph_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/multistep_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/pandas_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/retriever_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/retry_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/retry_source_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/router_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/sql_join_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/sql_vector_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/sub_question_query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/query_engine/transform_query_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.958166 llama_index-0.7.8/llama_index/question_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/question_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/question_gen/guidance_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/question_gen/llm_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/question_gen/output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/question_gen/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/question_gen/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/chatgpt_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/chatgpt_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/chatgpt_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/deeplake.py
--rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/discord_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/faiss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/file/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/docs_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/epub_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/image_caption_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/image_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/image_vision_llm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/ipynb_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/markdown_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/mbox_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/slides_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/tabular_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/file/video_audio_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/github_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/github_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/github_readers/github_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/github_readers/github_repository_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/github_readers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/google_readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/google_readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/google_readers/gdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/google_readers/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/make_com/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/make_com/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/make_com/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/mbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/notion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/obsidian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/psychic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/qdrant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/redis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/schema/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/steamship/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/steamship/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/steamship/file_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/string_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/twitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/readers/weaviate/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/weaviate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/weaviate/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/web.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/wikipedia.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/readers/youtube_transcript.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.966167 llama_index-0.7.8/llama_index/response/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response/notebook_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response/pprint_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.970167 llama_index-0.7.8/llama_index/response_synthesizers/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/accumulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/compact_and_accumulate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/compact_and_refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/no_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/refine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/simple_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/tree_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/response_synthesizers/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.970167 llama_index-0.7.8/llama_index/retrievers/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/retrievers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/retrievers/recursive_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/retrievers/transform_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.970167 llama_index-0.7.8/llama_index/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/selectors/llm_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/selectors/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/selectors/pydantic_selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/selectors/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.970167 llama_index-0.7.8/llama_index/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.974167 llama_index-0.7.8/llama_index/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/dynamodb_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/keyval_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/redis_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/docstore/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.974167 llama_index-0.7.8/llama_index/storage/index_store/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/index_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/index_store/dynamodb_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/index_store/keyval_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/index_store/mongo_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/index_store/redis_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/index_store/simple_index_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/index_store/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/index_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.974167 llama_index-0.7.8/llama_index/storage/kvstore/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/kvstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/kvstore/dynamodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/kvstore/mongodb_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/kvstore/redis_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/kvstore/s3_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/kvstore/simple_kvstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/kvstore/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/storage/storage_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.974167 llama_index-0.7.8/llama_index/token_counter/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/token_counter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/token_counter/mock_embed_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/token_counter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.978167 llama_index-0.7.8/llama_index/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/function_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/ondemand_loader_tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/query_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/query_plan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.978167 llama_index-0.7.8/llama_index/tools/tool_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/tool_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/tool_spec/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.978167 llama_index-0.7.8/llama_index/tools/tool_spec/load_and_search/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/tool_spec/load_and_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/tool_spec/load_and_search/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.978167 llama_index-0.7.8/llama_index/tools/tool_spec/notion/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/tool_spec/notion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/tool_spec/notion/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.978167 llama_index-0.7.8/llama_index/tools/tool_spec/slack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/tool_spec/slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/tool_spec/slack/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.978167 llama_index-0.7.8/llama_index/tts/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tts/bark.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/tts/elevenlabs.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.982167 llama_index-0.7.8/llama_index/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/chatgpt_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/deeplake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.982167 llama_index-0.7.8/llama_index/vector_stores/docarray/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/docarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/docarray/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/docarray/hnsw.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/docarray/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/lancedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/milvus.py
--rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/mongodb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/opensearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/supabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/tair.py
--rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/typesense.py
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/weaviate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-14 02:40:11.000000 llama_index-0.7.8/llama_index/vector_stores/weaviate_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.914166 llama_index-0.7.8/llama_index.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-14 02:40:29.000000 llama_index-0.7.8/llama_index.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-07-14 02:40:29.000000 llama_index-0.7.8/llama_index.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 02:40:29.000000 llama_index-0.7.8/llama_index.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-14 02:40:29.000000 llama_index-0.7.8/llama_index.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 02:40:29.000000 llama_index-0.7.8/llama_index.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-14 02:40:11.000000 llama_index-0.7.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 02:40:30.018167 llama_index-0.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-14 02:40:11.000000 llama_index-0.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.986167 llama_index-0.7.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.986167 llama_index-0.7.8/tests/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/callbacks/test_llama_debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/callbacks/test_token_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.986167 llama_index-0.7.8/tests/chat_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/chat_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/chat_engine/test_condense_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/chat_engine/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.986167 llama_index-0.7.8/tests/embeddings/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/embeddings/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.986167 llama_index-0.7.8/tests/indices/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.986167 llama_index-0.7.8/tests/indices/composability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/composability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/composability/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.986167 llama_index-0.7.8/tests/indices/document_summary/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/document_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/document_summary/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/document_summary/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.990167 llama_index-0.7.8/tests/indices/empty/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/empty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/empty/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.990167 llama_index-0.7.8/tests/indices/keyword_table/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/keyword_table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/keyword_table/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/keyword_table/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/keyword_table/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.990167 llama_index-0.7.8/tests/indices/knowledge_graph/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/knowledge_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/knowledge_graph/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/knowledge_graph/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/knowledge_graph/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.990167 llama_index-0.7.8/tests/indices/list/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/list/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/list/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/list/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.990167 llama_index-0.7.8/tests/indices/postprocessor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/postprocessor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/postprocessor/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/postprocessor/test_llm_rerank.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/postprocessor/test_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.990167 llama_index-0.7.8/tests/indices/query/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.994167 llama_index-0.7.8/tests/indices/query/query_transform/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/query_transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/query_transform/mock_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/query_transform/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/test_compose.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/test_compose_vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/test_embedding_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/query/test_query_bundle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.994167 llama_index-0.7.8/tests/indices/struct_store/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/struct_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/struct_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/struct_store/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/struct_store/test_json_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/struct_store/test_sql_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/test_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/test_loading_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/test_node_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/test_prompt_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.994167 llama_index-0.7.8/tests/indices/tree/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/tree/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/tree/test_embedding_retriever.py
--rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/tree/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/tree/test_retrievers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.998167 llama_index-0.7.8/tests/indices/vector_store/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.998167 llama_index-0.7.8/tests/indices/vector_store/auto_retriever/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/auto_retriever/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/auto_retriever/test_output_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/mock_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/mock_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/test_faiss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/test_myscale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/test_pinecone.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/test_retrievers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/test_simple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/indices/vector_store/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.998167 llama_index-0.7.8/tests/langchain_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/langchain_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/langchain_helpers/test_text_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:29.998167 llama_index-0.7.8/tests/llm_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llm_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llm_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.002167 llama_index-0.7.8/tests/llm_predictor/vellum/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llm_predictor/vellum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llm_predictor/vellum/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llm_predictor/vellum/test_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llm_predictor/vellum/test_prompt_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llm_predictor/vellum/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.002167 llama_index-0.7.8/tests/llms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llms/test_anthropic.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llms/test_anthropic_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llms/test_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llms/test_langchain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llms/test_openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llms/test_openai_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/llms/test_palm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.002167 llama_index-0.7.8/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/logger/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.006167 llama_index-0.7.8/tests/mock_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/mock_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/mock_utils/mock_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/mock_utils/mock_prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/mock_utils/mock_text_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/mock_utils/mock_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.006167 llama_index-0.7.8/tests/objects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/objects/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/objects/test_node_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.006167 llama_index-0.7.8/tests/output_parsers/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/output_parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/output_parsers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/output_parsers/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/output_parsers/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/output_parsers/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.006167 llama_index-0.7.8/tests/playground/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/playground/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/playground/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.006167 llama_index-0.7.8/tests/program/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/program/test_guidance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/program/test_llm_program.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.010167 llama_index-0.7.8/tests/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/prompts/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/prompts/test_guidance_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.010167 llama_index-0.7.8/tests/question_gen/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/question_gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/question_gen/test_guidance_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/question_gen/test_llm_generators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.010167 llama_index-0.7.8/tests/readers/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/readers/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/readers/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/readers/test_mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/readers/test_string_iterable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.010167 llama_index-0.7.8/tests/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/selectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/selectors/test_llm_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.010167 llama_index-0.7.8/tests/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/storage/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.014167 llama_index-0.7.8/tests/storage/docstore/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/storage/docstore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/storage/docstore/test_dynamodb_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/storage/docstore/test_mongo_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/storage/docstore/test_redis_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/storage/docstore/test_simple_docstore.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/storage/test_storage_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.014167 llama_index-0.7.8/tests/token_predictor/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/token_predictor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/token_predictor/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.014167 llama_index-0.7.8/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/tools/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/tools/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/tools/test_ondemand_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/tools/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.014167 llama_index-0.7.8/tests/tools/tool_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/tools/tool_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/tools/tool_spec/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:30.018167 llama_index-0.7.8/tests/vector_stores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/vector_stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/vector_stores/test_docarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/vector_stores/test_postgres.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/vector_stores/test_qdrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/vector_stores/test_tair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-14 02:40:11.000000 llama_index-0.7.8/tests/vector_stores/test_weaviate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.775222 llama_index-0.7.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-07-16 04:38:18.000000 llama_index-0.7.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-16 04:38:18.000000 llama_index-0.7.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-16 04:38:32.775222 llama_index-0.7.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-16 04:38:18.000000 llama_index-0.7.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.695221 llama_index-0.7.9/llama_index/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.699221 llama_index-0.7.9/llama_index/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/context_retriever_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18519 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/openai_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.699221 llama_index-0.7.9/llama_index/agent/react/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/react/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/react/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/react/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/react/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/react/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/react/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/retriever_openai_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/agent/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/async_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.699221 llama_index-0.7.9/llama_index/bridge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/bridge/langchain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.703221 llama_index-0.7.9/llama_index/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/callbacks/aim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/callbacks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/callbacks/llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/callbacks/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/callbacks/token_counting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20607 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/callbacks/wandb_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.703221 llama_index-0.7.9/llama_index/chat_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/chat_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/chat_engine/condense_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/chat_engine/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/chat_engine/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/chat_engine/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.703221 llama_index-0.7.9/llama_index/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/composability/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/composability/joint_qa_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.707221 llama_index-0.7.9/llama_index/data_structs/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/data_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/data_structs/data_structs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/data_structs/document_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/data_structs/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/data_structs/struct_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/data_structs/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.707221 llama_index-0.7.9/llama_index/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/embeddings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/embeddings/google.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/embeddings/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/embeddings/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/embeddings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.711221 llama_index-0.7.9/llama_index/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/evaluation/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.711221 llama_index-0.7.9/llama_index/evaluation/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/evaluation/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/evaluation/benchmarks/beir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/evaluation/dataset_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/evaluation/guideline_eval.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.711221 llama_index-0.7.9/llama_index/graph_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/graph_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19697 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/graph_stores/nebulagraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/graph_stores/registery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/graph_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/graph_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/img_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.715221 llama_index-0.7.9/llama_index/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15477 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/base_retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.715221 llama_index-0.7.9/llama_index/indices/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.715221 llama_index-0.7.9/llama_index/indices/common/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/common/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/common/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/common/struct_store/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/common/struct_store/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.719221 llama_index-0.7.9/llama_index/indices/common_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/common_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/common_tree/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.719221 llama_index-0.7.9/llama_index/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/composability/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.719221 llama_index-0.7.9/llama_index/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/document_summary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7056 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/document_summary/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.719221 llama_index-0.7.9/llama_index/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/empty/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/empty/retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.719221 llama_index-0.7.9/llama_index/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/keyword_table/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/keyword_table/rake_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/keyword_table/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/keyword_table/simple_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/keyword_table/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.719221 llama_index-0.7.9/llama_index/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/knowledge_graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/knowledge_graph/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.723221 llama_index-0.7.9/llama_index/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/list/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/list/retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.723221 llama_index-0.7.9/llama_index/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/postprocessor/cohere_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/postprocessor/llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12587 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/postprocessor/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8653 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/postprocessor/node_recency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/postprocessor/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5388 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/postprocessor/pii.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/postprocessor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/prompt_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.723221 llama_index-0.7.9/llama_index/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/query/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/query/embedding_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.723221 llama_index-0.7.9/llama_index/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8829 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/query/query_transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/query/query_transform/feedback_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/query/query_transform/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/service_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.723221 llama_index-0.7.9/llama_index/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/struct_store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5796 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/struct_store/container_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/struct_store/json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/struct_store/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/struct_store/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/struct_store/sql_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.723221 llama_index-0.7.9/llama_index/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/tree/all_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/tree/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/tree/inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/tree/select_leaf_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15368 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/tree/select_leaf_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/tree/tree_root_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/tree/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.723221 llama_index-0.7.9/llama_index/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/vector_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/vector_store/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.727221 llama_index-0.7.9/llama_index/indices/vector_store/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/vector_store/retrievers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.727221 llama_index-0.7.9/llama_index/indices/vector_store/retrievers/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/vector_store/retrievers/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/indices/vector_store/retrievers/retriever.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.727221 llama_index-0.7.9/llama_index/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.727221 llama_index-0.7.9/llama_index/langchain_helpers/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2924 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/agents/agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/agents/toolkits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/agents/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/memory_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/sql_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19862 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/langchain_helpers/text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.727221 llama_index-0.7.9/llama_index/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6604 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.727221 llama_index-0.7.9/llama_index/llm_predictor/vellum/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/vellum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/vellum/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/vellum/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/vellum/prompt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/vellum/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llm_predictor/vellum/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.731221 llama_index-0.7.9/llama_index/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/anthropic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/azure_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8920 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/generic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/langchain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14661 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/palm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/llms/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.731221 llama_index-0.7.9/llama_index/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/logger/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.731221 llama_index-0.7.9/llama_index/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/memory/chat_memory_buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/memory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.731221 llama_index-0.7.9/llama_index/node_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/node_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.731221 llama_index-0.7.9/llama_index/node_parser/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/node_parser/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12569 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/node_parser/extractors/metadata_extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/node_parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/node_parser/node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/node_parser/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.731221 llama_index-0.7.9/llama_index/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/objects/base_node_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/objects/table_node_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/objects/tool_node_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.731221 llama_index-0.7.9/llama_index/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/output_parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/output_parsers/guardrails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/output_parsers/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/output_parsers/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/output_parsers/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/output_parsers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.731221 llama_index-0.7.9/llama_index/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6877 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/playground/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.735221 llama_index-0.7.9/llama_index/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/base_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/guidance_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/llm_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/llm_prompt_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/openai_program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.735221 llama_index-0.7.9/llama_index/program/predefined/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/predefined/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/predefined/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.735221 llama_index-0.7.9/llama_index/program/predefined/evaporate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/predefined/evaporate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9960 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/predefined/evaporate/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/predefined/evaporate/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/program/predefined/evaporate/prompts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.735221 llama_index-0.7.9/llama_index/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6349 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/chat_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/choice_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/default_prompt_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/default_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/guidance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/prompt_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/prompt_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.735221 llama_index-0.7.9/llama_index/query_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12295 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/citation_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.739221 llama_index-0.7.9/llama_index/query_engine/flare/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/flare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/flare/answer_inserter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/flare/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/flare/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/flare/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10514 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/knowledge_graph_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/multistep_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/pandas_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/retriever_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/retry_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/retry_source_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/router_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/sql_join_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/sql_vector_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/sub_question_query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/query_engine/transform_query_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.739221 llama_index-0.7.9/llama_index/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/question_gen/guidance_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/question_gen/llm_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/question_gen/output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/question_gen/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/question_gen/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/chatgpt_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/chatgpt_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/chatgpt_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/discord_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/faiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/file/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/docs_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/epub_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/image_caption_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/image_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/image_vision_llm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/ipynb_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/markdown_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/mbox_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/slides_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/tabular_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/file/video_audio_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/github_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/github_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/github_readers/github_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15684 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/github_readers/github_repository_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/github_readers/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/google_readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/google_readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/google_readers/gdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4979 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/google_readers/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/make_com/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/make_com/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/make_com/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/mbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/notion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/obsidian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/psychic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/qdrant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/schema/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.743221 llama_index-0.7.9/llama_index/readers/steamship/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/steamship/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/steamship/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/string_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/twitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.747221 llama_index-0.7.9/llama_index/readers/weaviate/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/weaviate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/weaviate/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/wikipedia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/readers/youtube_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.747221 llama_index-0.7.9/llama_index/response/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response/notebook_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response/pprint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.747221 llama_index-0.7.9/llama_index/response_synthesizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/compact_and_accumulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/compact_and_refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/no_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9181 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/refine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/simple_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5508 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/tree_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/response_synthesizers/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.747221 llama_index-0.7.9/llama_index/retrievers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/retrievers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/retrievers/recursive_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/retrievers/transform_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.747221 llama_index-0.7.9/llama_index/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/selectors/llm_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/selectors/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/selectors/pydantic_selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/selectors/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.747221 llama_index-0.7.9/llama_index/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.751221 llama_index-0.7.9/llama_index/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/dynamodb_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/keyval_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/redis_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/docstore/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.751221 llama_index-0.7.9/llama_index/storage/index_store/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/index_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/index_store/dynamodb_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/index_store/keyval_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/index_store/mongo_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/index_store/redis_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/index_store/simple_index_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/index_store/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/index_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.751221 llama_index-0.7.9/llama_index/storage/kvstore/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/kvstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/kvstore/dynamodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/kvstore/mongodb_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/kvstore/redis_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3862 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/kvstore/s3_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/kvstore/simple_kvstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/kvstore/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/storage/storage_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.751221 llama_index-0.7.9/llama_index/token_counter/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/token_counter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/token_counter/mock_embed_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/token_counter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.751221 llama_index-0.7.9/llama_index/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/function_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/ondemand_loader_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/query_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/query_plan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.751221 llama_index-0.7.9/llama_index/tools/tool_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/tool_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/tool_spec/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.751221 llama_index-0.7.9/llama_index/tools/tool_spec/load_and_search/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/tool_spec/load_and_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/tool_spec/load_and_search/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.751221 llama_index-0.7.9/llama_index/tools/tool_spec/notion/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/tool_spec/notion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/tool_spec/notion/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.755221 llama_index-0.7.9/llama_index/tools/tool_spec/slack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/tool_spec/slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/tool_spec/slack/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.755221 llama_index-0.7.9/llama_index/tts/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tts/bark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/tts/elevenlabs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.755221 llama_index-0.7.9/llama_index/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/chatgpt_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5492 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/deeplake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/llama_index/vector_stores/docarray/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/docarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/docarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/docarray/hnsw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/docarray/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5668 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/lancedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18160 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/milvus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6729 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9039 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8820 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/opensearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10278 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16884 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5071 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/supabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8975 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/tair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4085 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/typesense.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/weaviate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4885 2023-07-16 04:38:18.000000 llama_index-0.7.9/llama_index/vector_stores/weaviate_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.695221 llama_index-0.7.9/llama_index.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-07-16 04:38:32.000000 llama_index-0.7.9/llama_index.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21566 2023-07-16 04:38:32.000000 llama_index-0.7.9/llama_index.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:38:32.000000 llama_index-0.7.9/llama_index.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-16 04:38:32.000000 llama_index-0.7.9/llama_index.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-16 04:38:32.000000 llama_index-0.7.9/llama_index.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-16 04:38:18.000000 llama_index-0.7.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 04:38:32.775222 llama_index-0.7.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-07-16 04:38:18.000000 llama_index-0.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/callbacks/test_llama_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/callbacks/test_token_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/chat_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/chat_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/chat_engine/test_condense_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/chat_engine/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/embeddings/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/indices/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/indices/composability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/composability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/composability/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/indices/document_summary/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/document_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/document_summary/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/document_summary/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/indices/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/empty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/empty/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/indices/keyword_table/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/keyword_table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/keyword_table/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/keyword_table/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/keyword_table/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.759221 llama_index-0.7.9/tests/indices/knowledge_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/knowledge_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/knowledge_graph/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/knowledge_graph/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/knowledge_graph/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.763221 llama_index-0.7.9/tests/indices/list/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/list/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/list/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/list/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.763221 llama_index-0.7.9/tests/indices/postprocessor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/postprocessor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12320 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/postprocessor/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/postprocessor/test_llm_rerank.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/postprocessor/test_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.763221 llama_index-0.7.9/tests/indices/query/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.763221 llama_index-0.7.9/tests/indices/query/query_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/query_transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/query_transform/mock_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/query_transform/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6579 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/test_compose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/test_compose_vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/test_embedding_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/query/test_query_bundle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.763221 llama_index-0.7.9/tests/indices/struct_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/struct_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/struct_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11906 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/struct_store/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/struct_store/test_json_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/struct_store/test_sql_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/test_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/test_loading_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/test_node_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/test_prompt_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.763221 llama_index-0.7.9/tests/indices/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/tree/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/tree/test_embedding_retriever.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8219 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/tree/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/tree/test_retrievers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/indices/vector_store/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/indices/vector_store/auto_retriever/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/auto_retriever/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/auto_retriever/test_output_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/mock_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/mock_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/test_deeplake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/test_faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/test_myscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/test_pinecone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/test_retrievers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7416 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/test_simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/indices/vector_store/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/langchain_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/langchain_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/langchain_helpers/test_text_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/llm_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llm_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llm_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/llm_predictor/vellum/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llm_predictor/vellum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llm_predictor/vellum/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llm_predictor/vellum/test_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llm_predictor/vellum/test_prompt_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llm_predictor/vellum/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/llms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llms/test_anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llms/test_anthropic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llms/test_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llms/test_langchain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7356 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llms/test_openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llms/test_openai_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/llms/test_palm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/logger/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/mock_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/mock_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/mock_utils/mock_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/mock_utils/mock_prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/mock_utils/mock_text_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/mock_utils/mock_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.767222 llama_index-0.7.9/tests/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/objects/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/objects/test_node_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/output_parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/output_parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/output_parsers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/output_parsers/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/output_parsers/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/output_parsers/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/playground/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/playground/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/playground/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/program/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/program/test_guidance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/program/test_llm_program.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/prompts/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/prompts/test_guidance_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/question_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/question_gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/question_gen/test_guidance_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/question_gen/test_llm_generators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/readers/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/readers/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/readers/test_mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/readers/test_string_iterable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/selectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/selectors/test_llm_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/storage/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/storage/docstore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/storage/docstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/storage/docstore/test_dynamodb_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/storage/docstore/test_mongo_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/storage/docstore/test_redis_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/storage/docstore/test_simple_docstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/storage/test_storage_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.771221 llama_index-0.7.9/tests/token_predictor/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/token_predictor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/token_predictor/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.775222 llama_index-0.7.9/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/tools/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/tools/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/tools/test_ondemand_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/tools/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.775222 llama_index-0.7.9/tests/tools/tool_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/tools/tool_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/tools/tool_spec/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:32.775222 llama_index-0.7.9/tests/vector_stores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/vector_stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/vector_stores/test_docarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/vector_stores/test_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/vector_stores/test_qdrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/vector_stores/test_tair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-16 04:38:18.000000 llama_index-0.7.9/tests/vector_stores/test_weaviate.py
```

### Comparing `llama_index-0.7.8/LICENSE` & `llama_index-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/PKG-INFO` & `llama_index-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama_index
-Version: 0.7.8
+Version: 0.7.9
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 Author: Jerry Liu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llama_index-0.7.8/README.md` & `llama_index-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/__init__.py` & `llama_index-0.7.9/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/context_retriever_agent.py` & `llama_index-0.7.9/llama_index/agent/context_retriever_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/openai_agent.py` & `llama_index-0.7.9/llama_index/agent/openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/react/base.py` & `llama_index-0.7.9/llama_index/agent/react/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/react/formatter.py` & `llama_index-0.7.9/llama_index/agent/react/formatter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/react/output_parser.py` & `llama_index-0.7.9/llama_index/agent/react/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/react/prompts.py` & `llama_index-0.7.9/llama_index/agent/react/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/react/types.py` & `llama_index-0.7.9/llama_index/agent/react/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/retriever_openai_agent.py` & `llama_index-0.7.9/llama_index/agent/retriever_openai_agent.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/agent/types.py` & `llama_index-0.7.9/llama_index/agent/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/bridge/langchain.py` & `llama_index-0.7.9/llama_index/bridge/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/callbacks/aim.py` & `llama_index-0.7.9/llama_index/callbacks/aim.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/callbacks/base.py` & `llama_index-0.7.9/llama_index/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/callbacks/llama_debug.py` & `llama_index-0.7.9/llama_index/callbacks/llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/callbacks/schema.py` & `llama_index-0.7.9/llama_index/callbacks/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/callbacks/token_counting.py` & `llama_index-0.7.9/llama_index/callbacks/token_counting.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/callbacks/wandb_callback.py` & `llama_index-0.7.9/llama_index/callbacks/wandb_callback.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/chat_engine/condense_question.py` & `llama_index-0.7.9/llama_index/query_engine/knowledge_graph_query_engine.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,273 +1,294 @@
+""" Knowledge Graph Query Engine"""
+
 import logging
-from typing import Any, List, Type, Optional
+from typing import Any, Optional, Sequence
 
-from llama_index.chat_engine.types import (
-    BaseChatEngine,
-    AgentChatResponse,
-    StreamingAgentChatResponse,
+from llama_index.bridge.langchain import print_text
+from llama_index.callbacks.schema import CBEventType, EventPayload
+from llama_index.graph_stores.registery import (
+    GRAPH_STORE_CLASS_TO_GRAPH_STORE_TYPE,
+    GraphStoreType,
 )
-from llama_index.chat_engine.utils import response_gen_with_chat_history
 from llama_index.indices.query.base import BaseQueryEngine
+from llama_index.indices.query.schema import QueryBundle
 from llama_index.indices.service_context import ServiceContext
-from llama_index.llms.base import ChatMessage, MessageRole
-from llama_index.llms.generic_utils import messages_to_history_str
-from llama_index.memory import BaseMemory, ChatMemoryBuffer
-from llama_index.prompts.base import Prompt
-from llama_index.response.schema import StreamingResponse, RESPONSE_TYPE
-from llama_index.tools import ToolOutput
+from llama_index.prompts.base import Prompt, PromptType
+from llama_index.response.schema import RESPONSE_TYPE
+from llama_index.response_synthesizers import BaseSynthesizer, get_response_synthesizer
+from llama_index.schema import NodeWithScore, TextNode
+from llama_index.storage.storage_context import StorageContext
 
 logger = logging.getLogger(__name__)
 
+# Prompt
+DEFAULT_NEBULAGRAPH_NL2CYPHER_PROMPT_TMPL = """
+Generate NebulaGraph query from natural language.
+Use only the provided relationship types and properties in the schema.
+Do not use any other relationship types or properties that are not provided.
+Schema:
+---
+{schema}
+---
+Note: NebulaGraph speaks a dialect of Cypher, comparing to standard Cypher:
+
+1. it uses double equals sign for comparison: `==` rather than `=`
+2. it needs explicit label specification when referring to node properties, i.e.
+v is a variable of a node, and we know its label is Foo, v.`foo`.name is correct
+while v.name is not.
+
+For example, see this diff between standard and NebulaGraph Cypher dialect:
+```diff
+< MATCH (p:person)-[:directed]->(m:movie) WHERE m.name = 'The Godfather'
+< RETURN p.name;
+---
+> MATCH (p:`person`)-[:directed]->(m:`movie`) WHERE m.`movie`.`name` == 'The Godfather'
+> RETURN p.`person`.`name`;
+```
 
-DEFAULT_TEMPLATE = """\
-Given a conversation (between Human and Assistant) and a follow up message from Human, \
-rewrite the message to be a standalone question that captures all relevant context \
-from the conversation.
-
-<Chat History> 
-{chat_history}
+Question: {query_str}
 
-<Follow Up Message>
-{question}
+NebulaGraph Cypher dialect query:
+"""
+DEFAULT_NEBULAGRAPH_NL2CYPHER_PROMPT = Prompt(
+    DEFAULT_NEBULAGRAPH_NL2CYPHER_PROMPT_TMPL,
+    prompt_type=PromptType.TEXT_TO_GRAPH_QUERY,
+)
 
-<Standalone question>
+DEFAULT_NL2GRAPH_PROMPT_MAP = {
+    GraphStoreType.NEBULA: DEFAULT_NEBULAGRAPH_NL2CYPHER_PROMPT,
+}
+
+DEFAULT_KG_RESPONSE_ANSWER_PROMPT_TMPL = """
+The original question is given below.
+This question has been translated into a Graph Database query.
+Both the Graph query and the response are given below.
+Given the Graph Query response, synthesise a response to the original question.
+
+Original question: {query_str}
+Graph query: {kg_query_str}
+Graph response: {kg_response_str}
+Response: 
 """
 
-DEFAULT_PROMPT = Prompt(DEFAULT_TEMPLATE)
+DEFAULT_KG_RESPONSE_ANSWER_PROMPT = Prompt(
+    DEFAULT_KG_RESPONSE_ANSWER_PROMPT_TMPL,
+    prompt_type=PromptType.QUESTION_ANSWER,
+)
+
 
+class KnowledgeGraphQueryEngine(BaseQueryEngine):
+    """Knowledge graph query engine.
 
-class CondenseQuestionChatEngine(BaseChatEngine):
-    """Condense Question Chat Engine.
+    Query engine to call a knowledge graph.
+
+    Args:
+        service_context (Optional[ServiceContext]): A service context to use.
+        storage_context (Optional[StorageContext]): A storage context to use.
+        refresh_schema (bool): Whether to refresh the schema.
+        verbose (bool): Whether to print intermediate results.
+        response_synthesizer (Optional[BaseSynthesizer]):
+            A BaseSynthesizer object.
+        **kwargs: Additional keyword arguments.
 
-    First generate a standalone question from conversation context and last message,
-    then query the query engine for a response.
     """
 
     def __init__(
         self,
-        query_engine: BaseQueryEngine,
-        condense_question_prompt: Prompt,
-        memory: BaseMemory,
-        service_context: ServiceContext,
-        verbose: bool = False,
-    ) -> None:
-        self._query_engine = query_engine
-        self._condense_question_prompt = condense_question_prompt
-        self._memory = memory
-        self._service_context = service_context
-        self._verbose = verbose
-
-    @classmethod
-    def from_defaults(
-        cls,
-        query_engine: BaseQueryEngine,
-        condense_question_prompt: Optional[Prompt] = None,
-        chat_history: Optional[List[ChatMessage]] = None,
-        memory: Optional[BaseMemory] = None,
-        memory_cls: Type[BaseMemory] = ChatMemoryBuffer,
         service_context: Optional[ServiceContext] = None,
+        storage_context: Optional[StorageContext] = None,
+        graph_query_synthesis_prompt: Optional[Prompt] = None,
+        graph_response_answer_prompt: Optional[Prompt] = None,
+        refresh_schema: bool = False,
         verbose: bool = False,
-        system_prompt: Optional[str] = None,
-        prefix_messages: Optional[List[ChatMessage]] = None,
+        response_synthesizer: Optional[BaseSynthesizer] = None,
         **kwargs: Any,
-    ) -> "CondenseQuestionChatEngine":
-        """Initialize a CondenseQuestionChatEngine from default parameters."""
-        condense_question_prompt = condense_question_prompt or DEFAULT_PROMPT
-        chat_history = chat_history or []
-        memory = memory or memory_cls.from_defaults(chat_history=chat_history)
-        service_context = service_context or ServiceContext.from_defaults()
-
-        if system_prompt is not None:
-            raise NotImplementedError(
-                "system_prompt is not supported for CondenseQuestionChatEngine."
-            )
-        if prefix_messages is not None:
-            raise NotImplementedError(
-                "prefix_messages is not supported for CondenseQuestionChatEngine."
-            )
+    ):
+        # Ensure that we have a graph store
+        assert storage_context is not None, "Must provide a storage context."
+        assert (
+            storage_context.graph_store is not None
+        ), "Must provide a graph store in the storage context."
+        self._storage_context = storage_context
+        self.graph_store = storage_context.graph_store
+
+        self._service_context = service_context or ServiceContext.from_defaults()
+
+        # Get Graph Store Type
+        self._graph_store_type = GRAPH_STORE_CLASS_TO_GRAPH_STORE_TYPE[
+            self.graph_store.__class__
+        ]
+
+        # Get Graph schema
+        self._graph_schema = self.graph_store.get_schema(refresh=refresh_schema)
+
+        # Get graph store query synthesis prompt
+        self._graph_query_synthesis_prompt = (
+            graph_query_synthesis_prompt
+            or DEFAULT_NL2GRAPH_PROMPT_MAP[self._graph_store_type]
+        )
 
-        return cls(
-            query_engine,
-            condense_question_prompt,
-            memory,
-            service_context,
-            verbose=verbose,
-        )
-
-    def _condense_question(
-        self, chat_history: List[ChatMessage], last_message: str
-    ) -> str:
-        """
-        Generate standalone question from conversation context and last message.
-        """
-
-        chat_history_str = messages_to_history_str(chat_history)
-        logger.debug(chat_history_str)
-
-        response = self._service_context.llm_predictor.predict(
-            self._condense_question_prompt,
-            question=last_message,
-            chat_history=chat_history_str,
+        self._graph_response_answer_prompt = (
+            graph_response_answer_prompt or DEFAULT_KG_RESPONSE_ANSWER_PROMPT
         )
-        return response
+        self._verbose = verbose
+        self._response_synthesizer = response_synthesizer or get_response_synthesizer(
+            callback_manager=self._service_context.callback_manager,
+            service_context=self._service_context,
+        )
+
+        super().__init__(self._service_context.callback_manager)
 
-    async def _acondense_question(
-        self, chat_history: List[ChatMessage], last_message: str
-    ) -> str:
-        """
-        Generate standalone question from conversation context and last message.
-        """
-
-        chat_history_str = messages_to_history_str(chat_history)
-        logger.debug(chat_history_str)
-
-        response = await self._service_context.llm_predictor.apredict(
-            self._condense_question_prompt,
-            question=last_message,
-            chat_history=chat_history_str,
+    def generate_query(self, query_str: str) -> str:
+        """Generate a Graph Store Query from a query bundle."""
+        # Get the query engine query string
+
+        graph_store_query: str = self._service_context.llm_predictor.predict(
+            self._graph_query_synthesis_prompt,
+            query_str=query_str,
+            schema=self._graph_schema,
         )
-        return response
 
-    def _get_tool_output_from_response(
-        self, query: str, response: RESPONSE_TYPE
-    ) -> ToolOutput:
-        return ToolOutput(
-            content=str(response),
-            tool_name="query_engine",
-            raw_input={"query": query},
-            raw_output=response,
-        )
-
-    def chat(
-        self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> AgentChatResponse:
-        chat_history = chat_history or self._memory.get()
+        return graph_store_query
 
-        # Generate standalone question from conversation context and last message
-        condensed_question = self._condense_question(chat_history, message)
+    async def agenerate_query(self, query_str: str) -> str:
+        """Generate a Graph Store Query from a query bundle."""
+        # Get the query engine query string
+
+        graph_store_query: str = await self._service_context.llm_predictor.apredict(
+            self._graph_query_synthesis_prompt,
+            query_str=query_str,
+            schema=self._graph_schema,
+        )
 
-        log_str = f"Querying with: {condensed_question}"
-        logger.info(log_str)
-        if self._verbose:
-            print(log_str)
+        return graph_store_query
 
-        # Query with standalone question
-        query_response = self._query_engine.query(condensed_question)
-        tool_output = self._get_tool_output_from_response(
-            condensed_question, query_response
+    def _query(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
+        """Query the graph store."""
+        query_id = self.callback_manager.on_event_start(
+            CBEventType.QUERY, payload={EventPayload.QUERY_STR: query_bundle.query_str}
         )
 
-        # Record response
-        self._memory.put(ChatMessage(role=MessageRole.USER, content=message))
-        self._memory.put(
-            ChatMessage(role=MessageRole.ASSISTANT, content=str(query_response))
+        graph_store_query = self.generate_query(query_bundle.query_str)
+        if self._verbose:
+            print_text(f"Graph Store Query: {graph_store_query}\n", color="yellow")
+        logger.info(f"Graph Store Query: {graph_store_query}")
+        retrieve_id = self.callback_manager.on_event_start(
+            CBEventType.RETRIEVE,
+            payload={
+                EventPayload.QUERY_STR: graph_store_query,
+            },
         )
+        # Get the graph store response
+        graph_store_response = self.graph_store.query(query=graph_store_query)
+        if self._verbose:
+            print_text(
+                f"Graph Store Response: {graph_store_response}\n", color="yellow"
+            )
+        logger.info(f"Graph Store Response: {graph_store_response}")
 
-        return AgentChatResponse(response=str(query_response), sources=[tool_output])
+        self.callback_manager.on_event_end(
+            CBEventType.RETRIEVE,
+            payload={EventPayload.RESPONSE: graph_store_response},
+            event_id=retrieve_id,
+        )
+
+        prompt_string: Sequence = self._graph_response_answer_prompt.format(
+            query_str=query_bundle.query_str,
+            kg_query_str=graph_store_query,
+            kg_response_str=graph_store_response,
+        )
 
-    def stream_chat(
-        self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> StreamingAgentChatResponse:
-        chat_history = chat_history or self._memory.get()
+        node = NodeWithScore(
+            node=TextNode(
+                text=prompt_string,
+                score=1.0,
+                metadata={
+                    "query_str": query_bundle.query_str,
+                    "graph_store_query": graph_store_query,
+                    "graph_store_response": graph_store_response,
+                    "graph_schema": self._graph_schema,
+                },
+            )
+        )
 
-        # Generate standalone question from conversation context and last message
-        condensed_question = self._condense_question(chat_history, message)
+        response = self._response_synthesizer.synthesize(
+            query=query_bundle,
+            nodes=[node],
+        )
 
-        log_str = f"Querying with: {condensed_question}"
-        logger.info(log_str)
         if self._verbose:
-            print(log_str)
+            print_text(f"Final Response: {response}\n", color="green")
 
-        # Query with standalone question
-        query_response = self._query_engine.query(condensed_question)
-        tool_output = self._get_tool_output_from_response(
-            condensed_question, query_response
-        )
-
-        # Record response
-        if (
-            isinstance(query_response, StreamingResponse)
-            and query_response.response_gen is not None
-        ):
-            # override the generator to include writing to chat history
-            response = StreamingAgentChatResponse(
-                chat_stream=response_gen_with_chat_history(
-                    message, self._memory, query_response.response_gen
-                ),
-                sources=[tool_output],
-            )
-        else:
-            raise ValueError("Streaming is not enabled. Please use chat() instead.")
-        return response
+        self.callback_manager.on_event_end(
+            CBEventType.QUERY,
+            payload={EventPayload.RESPONSE: response},
+            event_id=query_id,
+        )
 
-    async def achat(
-        self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> AgentChatResponse:
-        chat_history = chat_history or self._memory.get()
+        return response
 
-        # Generate standalone question from conversation context and last message
-        condensed_question = await self._acondense_question(chat_history, message)
+    async def _aquery(self, query_bundle: QueryBundle) -> RESPONSE_TYPE:
+        """Query the graph store."""
+        query_id = self.callback_manager.on_event_start(
+            CBEventType.QUERY, payload={EventPayload.QUERY_STR: query_bundle.query_str}
+        )
 
-        log_str = f"Querying with: {condensed_question}"
-        logger.info(log_str)
+        graph_store_query = await self.agenerate_query(query_bundle.query_str)
         if self._verbose:
-            print(log_str)
-
-        # Query with standalone question
-        query_response = await self._query_engine.aquery(condensed_question)
-        tool_output = self._get_tool_output_from_response(
-            condensed_question, query_response
+            print_text(f"Graph Store Query: {graph_store_query}\n", color="yellow")
+        logger.info(f"Graph Store Query: {graph_store_query}")
+        retrieve_id = self.callback_manager.on_event_start(
+            CBEventType.RETRIEVE,
+            payload={
+                EventPayload.QUERY_STR: graph_store_query,
+            },
         )
+        # Get the graph store response
+        # TBD: This is a blocking call. We need to make it async.
+        graph_store_response = self.graph_store.query(query=graph_store_query)
+        if self._verbose:
+            print_text(
+                f"Graph Store Response: {graph_store_response}\n", color="yellow"
+            )
+        logger.info(f"Graph Store Response: {graph_store_response}")
 
-        # Record response
-        self._memory.put(ChatMessage(role=MessageRole.USER, content=message))
-        self._memory.put(
-            ChatMessage(role=MessageRole.ASSISTANT, content=str(query_response))
+        self.callback_manager.on_event_end(
+            CBEventType.RETRIEVE,
+            payload={EventPayload.RESPONSE: graph_store_response},
+            event_id=retrieve_id,
         )
 
-        return AgentChatResponse(response=str(query_response), sources=[tool_output])
+        prompt_string: Sequence = self._graph_response_answer_prompt.format(
+            query_str=query_bundle.query_str,
+            kg_query_str=graph_store_query,
+            kg_response_str=graph_store_response,
+        )
 
-    async def astream_chat(
-        self, message: str, chat_history: Optional[List[ChatMessage]] = None
-    ) -> StreamingAgentChatResponse:
-        chat_history = chat_history or self._memory.get()
+        node = NodeWithScore(
+            node=TextNode(
+                text=prompt_string,
+                score=1.0,
+                metadata={
+                    "query_str": query_bundle.query_str,
+                    "graph_store_query": graph_store_query,
+                    "graph_store_response": graph_store_response,
+                    "graph_schema": self._graph_schema,
+                },
+            )
+        )
 
-        # Generate standalone question from conversation context and last message
-        condensed_question = await self._acondense_question(chat_history, message)
+        response = await self._response_synthesizer.asynthesize(
+            query=query_bundle,
+            nodes=[node],
+        )
 
-        log_str = f"Querying with: {condensed_question}"
-        logger.info(log_str)
         if self._verbose:
-            print(log_str)
+            print_text(f"Final Response: {response}\n", color="green")
 
-        # Query with standalone question
-        query_response = await self._query_engine.aquery(condensed_question)
-        tool_output = self._get_tool_output_from_response(
-            condensed_question, query_response
-        )
-
-        # Record response
-        if (
-            isinstance(query_response, StreamingResponse)
-            and query_response.response_gen is not None
-        ):
-            # override the generator to include writing to chat history
-            # TODO: query engine does not support async generator yet
-            response = StreamingAgentChatResponse(
-                chat_stream=response_gen_with_chat_history(
-                    message, self._memory, query_response.response_gen
-                ),
-                sources=[tool_output],
-            )
-        else:
-            raise ValueError("Streaming is not enabled. Please use achat() instead.")
-        return response
+        self.callback_manager.on_event_end(
+            CBEventType.QUERY,
+            payload={EventPayload.RESPONSE: response},
+            event_id=query_id,
+        )
 
-    def reset(self) -> None:
-        # Clear chat history
-        self._memory.reset()
-
-    @property
-    def chat_history(self) -> List[ChatMessage]:
-        """Get chat history."""
-        return self._memory.get_all()
+        return response
```

### Comparing `llama_index-0.7.8/llama_index/chat_engine/simple.py` & `llama_index-0.7.9/llama_index/chat_engine/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/chat_engine/types.py` & `llama_index-0.7.9/llama_index/chat_engine/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/chat_engine/utils.py` & `llama_index-0.7.9/llama_index/chat_engine/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/composability/joint_qa_summary.py` & `llama_index-0.7.9/llama_index/composability/joint_qa_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/data_structs/data_structs.py` & `llama_index-0.7.9/llama_index/data_structs/data_structs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/data_structs/document_summary.py` & `llama_index-0.7.9/llama_index/data_structs/document_summary.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/data_structs/registry.py` & `llama_index-0.7.9/llama_index/data_structs/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/data_structs/struct_type.py` & `llama_index-0.7.9/llama_index/data_structs/struct_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/data_structs/table.py` & `llama_index-0.7.9/llama_index/data_structs/table.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/embeddings/base.py` & `llama_index-0.7.9/llama_index/embeddings/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/embeddings/google.py` & `llama_index-0.7.9/llama_index/embeddings/google.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/embeddings/langchain.py` & `llama_index-0.7.9/llama_index/embeddings/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/embeddings/openai.py` & `llama_index-0.7.9/llama_index/embeddings/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/embeddings/utils.py` & `llama_index-0.7.9/llama_index/embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/evaluation/base.py` & `llama_index-0.7.9/llama_index/evaluation/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/evaluation/dataset_generation.py` & `llama_index-0.7.9/llama_index/evaluation/dataset_generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/evaluation/guideline_eval.py` & `llama_index-0.7.9/llama_index/evaluation/guideline_eval.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/graph_stores/nebulagraph.py` & `llama_index-0.7.9/llama_index/graph_stores/nebulagraph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/graph_stores/registery.py` & `llama_index-0.7.9/llama_index/graph_stores/registery.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/graph_stores/simple.py` & `llama_index-0.7.9/llama_index/graph_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/graph_stores/types.py` & `llama_index-0.7.9/llama_index/graph_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/img_utils.py` & `llama_index-0.7.9/llama_index/img_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/__init__.py` & `llama_index-0.7.9/llama_index/indices/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/base.py` & `llama_index-0.7.9/llama_index/indices/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/base_retriever.py` & `llama_index-0.7.9/llama_index/indices/base_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/common/struct_store/base.py` & `llama_index-0.7.9/llama_index/indices/common/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/common/struct_store/schema.py` & `llama_index-0.7.9/llama_index/indices/common/struct_store/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/common/struct_store/sql.py` & `llama_index-0.7.9/llama_index/indices/common/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/common_tree/base.py` & `llama_index-0.7.9/llama_index/indices/common_tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/composability/graph.py` & `llama_index-0.7.9/llama_index/indices/composability/graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/document_summary/base.py` & `llama_index-0.7.9/llama_index/indices/document_summary/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/document_summary/retrievers.py` & `llama_index-0.7.9/llama_index/indices/document_summary/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/empty/base.py` & `llama_index-0.7.9/llama_index/indices/empty/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/empty/retrievers.py` & `llama_index-0.7.9/llama_index/indices/empty/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/keyword_table/__init__.py` & `llama_index-0.7.9/llama_index/indices/keyword_table/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/keyword_table/base.py` & `llama_index-0.7.9/llama_index/indices/keyword_table/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/keyword_table/rake_base.py` & `llama_index-0.7.9/llama_index/indices/keyword_table/rake_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/keyword_table/retrievers.py` & `llama_index-0.7.9/llama_index/indices/keyword_table/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/keyword_table/simple_base.py` & `llama_index-0.7.9/llama_index/indices/keyword_table/simple_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/keyword_table/utils.py` & `llama_index-0.7.9/llama_index/indices/keyword_table/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/knowledge_graph/base.py` & `llama_index-0.7.9/llama_index/indices/knowledge_graph/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/knowledge_graph/retriever.py` & `llama_index-0.7.9/llama_index/indices/knowledge_graph/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/list/base.py` & `llama_index-0.7.9/llama_index/indices/list/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/list/retrievers.py` & `llama_index-0.7.9/llama_index/indices/list/retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/loading.py` & `llama_index-0.7.9/llama_index/indices/loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/postprocessor/__init__.py` & `llama_index-0.7.9/llama_index/indices/postprocessor/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/postprocessor/cohere_rerank.py` & `llama_index-0.7.9/llama_index/indices/postprocessor/cohere_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/postprocessor/llm_rerank.py` & `llama_index-0.7.9/llama_index/indices/postprocessor/llm_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/postprocessor/node.py` & `llama_index-0.7.9/llama_index/indices/postprocessor/node.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/postprocessor/node_recency.py` & `llama_index-0.7.9/llama_index/indices/postprocessor/node_recency.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/postprocessor/optimizer.py` & `llama_index-0.7.9/llama_index/indices/postprocessor/optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/postprocessor/pii.py` & `llama_index-0.7.9/llama_index/indices/postprocessor/pii.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/prompt_helper.py` & `llama_index-0.7.9/llama_index/indices/prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/query/base.py` & `llama_index-0.7.9/llama_index/indices/query/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/query/embedding_utils.py` & `llama_index-0.7.9/llama_index/indices/query/embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/query/query_transform/base.py` & `llama_index-0.7.9/llama_index/indices/query/query_transform/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/query/query_transform/feedback_transform.py` & `llama_index-0.7.9/llama_index/indices/query/query_transform/feedback_transform.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/query/query_transform/prompts.py` & `llama_index-0.7.9/llama_index/indices/query/query_transform/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/query/schema.py` & `llama_index-0.7.9/llama_index/indices/query/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/registry.py` & `llama_index-0.7.9/llama_index/indices/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/service_context.py` & `llama_index-0.7.9/llama_index/indices/service_context.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import logging
 from dataclasses import dataclass
-from typing import Optional
+from typing import Optional, Union
 
 import llama_index
 from llama_index.callbacks.base import CallbackManager
 from llama_index.embeddings.base import BaseEmbedding
 from llama_index.embeddings.openai import OpenAIEmbedding
 from llama_index.indices.prompt_helper import PromptHelper
 from llama_index.llm_predictor import LLMPredictor
 from llama_index.llm_predictor.base import BaseLLMPredictor, LLMMetadata
 from llama_index.llms.base import LLM
 from llama_index.llms.utils import LLMType
 from llama_index.logger import LlamaLogger
 from llama_index.node_parser.interface import NodeParser
 from llama_index.node_parser.simple import SimpleNodeParser
+from llama_index.embeddings import (
+    DEFAULT_HUGGINGFACE_EMBEDDING_MODEL,
+    LangchainEmbedding,
+)
 
 logger = logging.getLogger(__name__)
 
 
 def _get_default_node_parser(
     chunk_size: Optional[int] = None,
     chunk_overlap: Optional[int] = None,
@@ -68,15 +72,15 @@
 
     @classmethod
     def from_defaults(
         cls,
         llm_predictor: Optional[BaseLLMPredictor] = None,
         llm: Optional[LLMType] = None,
         prompt_helper: Optional[PromptHelper] = None,
-        embed_model: Optional[BaseEmbedding] = None,
+        embed_model: Optional[Union[BaseEmbedding, str]] = None,
         node_parser: Optional[NodeParser] = None,
         llama_logger: Optional[LlamaLogger] = None,
         callback_manager: Optional[CallbackManager] = None,
         # node parser kwargs
         chunk_size: Optional[int] = None,
         chunk_overlap: Optional[int] = None,
         # prompt helper kwargs
@@ -92,14 +96,15 @@
         You can change the base defaults by setting llama_index.global_service_context
         to a ServiceContext object with your desired settings.
 
         Args:
             llm_predictor (Optional[BaseLLMPredictor]): LLMPredictor
             prompt_helper (Optional[PromptHelper]): PromptHelper
             embed_model (Optional[BaseEmbedding]): BaseEmbedding
+                or "local" (use local model)
             node_parser (Optional[NodeParser]): NodeParser
             llama_logger (Optional[LlamaLogger]): LlamaLogger (deprecated)
             chunk_size (Optional[int]): chunk_size
             callback_manager (Optional[CallbackManager]): CallbackManager
 
         Deprecated Args:
             chunk_size_limit (Optional[int]): renamed to chunk_size
@@ -107,14 +112,36 @@
         """
         if chunk_size_limit is not None and chunk_size is None:
             logger.warning(
                 "chunk_size_limit is deprecated, please specify chunk_size instead"
             )
             chunk_size = chunk_size_limit
 
+        if isinstance(embed_model, str):
+            splits = embed_model.split(":", 1)
+            is_local = splits[0]
+            model_name = splits[1] if len(splits) > 1 else None
+            if is_local != "local":
+                raise ValueError(
+                    "embed_model must start with str 'local' or of type BaseEmbedding"
+                )
+            try:
+                from langchain.embeddings import HuggingFaceEmbeddings
+            except ImportError as exc:
+                raise ImportError(
+                    "Could not import sentence_transformers or langchain package. "
+                    "Please install with `pip install sentence-transformers langchain`."
+                ) from exc
+
+            embed_model = LangchainEmbedding(
+                HuggingFaceEmbeddings(
+                    model_name=model_name or DEFAULT_HUGGINGFACE_EMBEDDING_MODEL
+                )
+            )
+
         if llama_index.global_service_context is not None:
             return cls.from_service_context(
                 llama_index.global_service_context,
                 llm_predictor=llm_predictor,
                 prompt_helper=prompt_helper,
                 embed_model=embed_model,
                 node_parser=node_parser,
```

### Comparing `llama_index-0.7.8/llama_index/indices/struct_store/__init__.py` & `llama_index-0.7.9/llama_index/indices/struct_store/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/struct_store/base.py` & `llama_index-0.7.9/llama_index/indices/struct_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/struct_store/container_builder.py` & `llama_index-0.7.9/llama_index/indices/struct_store/container_builder.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/struct_store/json_query.py` & `llama_index-0.7.9/llama_index/indices/struct_store/json_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/struct_store/pandas.py` & `llama_index-0.7.9/llama_index/indices/struct_store/pandas.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/struct_store/sql.py` & `llama_index-0.7.9/llama_index/indices/struct_store/sql.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/struct_store/sql_query.py` & `llama_index-0.7.9/llama_index/indices/struct_store/sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/tree/__init__.py` & `llama_index-0.7.9/llama_index/indices/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/tree/all_leaf_retriever.py` & `llama_index-0.7.9/llama_index/indices/tree/all_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/tree/base.py` & `llama_index-0.7.9/llama_index/indices/tree/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/tree/inserter.py` & `llama_index-0.7.9/llama_index/indices/tree/inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/tree/select_leaf_embedding_retriever.py` & `llama_index-0.7.9/llama_index/indices/tree/select_leaf_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/tree/select_leaf_retriever.py` & `llama_index-0.7.9/llama_index/indices/tree/select_leaf_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/tree/tree_root_retriever.py` & `llama_index-0.7.9/llama_index/indices/tree/tree_root_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/tree/utils.py` & `llama_index-0.7.9/llama_index/indices/tree/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/utils.py` & `llama_index-0.7.9/llama_index/indices/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/vector_store/base.py` & `llama_index-0.7.9/llama_index/indices/vector_store/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py` & `llama_index-0.7.9/llama_index/indices/vector_store/retrievers/auto_retriever/auto_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py` & `llama_index-0.7.9/llama_index/indices/vector_store/retrievers/auto_retriever/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py` & `llama_index-0.7.9/llama_index/indices/vector_store/retrievers/auto_retriever/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/indices/vector_store/retrievers/retriever.py` & `llama_index-0.7.9/llama_index/indices/vector_store/retrievers/retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/langchain_helpers/agents/__init__.py` & `llama_index-0.7.9/llama_index/langchain_helpers/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/langchain_helpers/agents/agents.py` & `llama_index-0.7.9/llama_index/langchain_helpers/agents/agents.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/langchain_helpers/agents/toolkits.py` & `llama_index-0.7.9/llama_index/langchain_helpers/agents/toolkits.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/langchain_helpers/agents/tools.py` & `llama_index-0.7.9/llama_index/langchain_helpers/agents/tools.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/langchain_helpers/memory_wrapper.py` & `llama_index-0.7.9/llama_index/langchain_helpers/memory_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/langchain_helpers/sql_wrapper.py` & `llama_index-0.7.9/llama_index/langchain_helpers/sql_wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/langchain_helpers/streaming.py` & `llama_index-0.7.9/llama_index/langchain_helpers/streaming.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/langchain_helpers/text_splitter.py` & `llama_index-0.7.9/llama_index/langchain_helpers/text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llm_predictor/base.py` & `llama_index-0.7.9/llama_index/llm_predictor/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llm_predictor/mock.py` & `llama_index-0.7.9/llama_index/llm_predictor/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llm_predictor/structured.py` & `llama_index-0.7.9/llama_index/llm_predictor/structured.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llm_predictor/utils.py` & `llama_index-0.7.9/llama_index/llm_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llm_predictor/vellum/predictor.py` & `llama_index-0.7.9/llama_index/llm_predictor/vellum/predictor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llm_predictor/vellum/prompt_registry.py` & `llama_index-0.7.9/llama_index/llm_predictor/vellum/prompt_registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llm_predictor/vellum/types.py` & `llama_index-0.7.9/llama_index/llm_predictor/vellum/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/__init__.py` & `llama_index-0.7.9/llama_index/llms/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/anthropic.py` & `llama_index-0.7.9/llama_index/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/anthropic_utils.py` & `llama_index-0.7.9/llama_index/llms/anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/azure_openai.py` & `llama_index-0.7.9/llama_index/llms/azure_openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/base.py` & `llama_index-0.7.9/llama_index/llms/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/custom.py` & `llama_index-0.7.9/llama_index/llms/custom.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/generic_utils.py` & `llama_index-0.7.9/llama_index/llms/generic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/huggingface.py` & `llama_index-0.7.9/llama_index/llms/huggingface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/langchain.py` & `llama_index-0.7.9/llama_index/llms/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/langchain_utils.py` & `llama_index-0.7.9/llama_index/llms/langchain_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/mock.py` & `llama_index-0.7.9/llama_index/llms/mock.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/openai.py` & `llama_index-0.7.9/llama_index/llms/openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/openai_utils.py` & `llama_index-0.7.9/llama_index/llms/openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/llms/palm.py` & `llama_index-0.7.9/llama_index/llms/palm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/logger/base.py` & `llama_index-0.7.9/llama_index/logger/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/memory/chat_memory_buffer.py` & `llama_index-0.7.9/llama_index/memory/chat_memory_buffer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/memory/types.py` & `llama_index-0.7.9/llama_index/memory/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/node_parser/extractors/metadata_extractors.py` & `llama_index-0.7.9/llama_index/node_parser/extractors/metadata_extractors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/node_parser/interface.py` & `llama_index-0.7.9/llama_index/node_parser/interface.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/node_parser/node_utils.py` & `llama_index-0.7.9/llama_index/node_parser/node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/node_parser/simple.py` & `llama_index-0.7.9/llama_index/node_parser/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/objects/__init__.py` & `llama_index-0.7.9/llama_index/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/objects/base.py` & `llama_index-0.7.9/llama_index/objects/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/objects/base_node_mapping.py` & `llama_index-0.7.9/llama_index/objects/base_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/objects/table_node_mapping.py` & `llama_index-0.7.9/llama_index/objects/table_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/objects/tool_node_mapping.py` & `llama_index-0.7.9/llama_index/objects/tool_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/output_parsers/guardrails.py` & `llama_index-0.7.9/llama_index/output_parsers/guardrails.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/output_parsers/langchain.py` & `llama_index-0.7.9/llama_index/output_parsers/langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/output_parsers/pydantic.py` & `llama_index-0.7.9/llama_index/output_parsers/pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/output_parsers/selection.py` & `llama_index-0.7.9/llama_index/output_parsers/selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/output_parsers/utils.py` & `llama_index-0.7.9/llama_index/output_parsers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/playground/base.py` & `llama_index-0.7.9/llama_index/playground/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/program/__init__.py` & `llama_index-0.7.9/llama_index/program/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/program/guidance_program.py` & `llama_index-0.7.9/llama_index/program/guidance_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/program/llm_program.py` & `llama_index-0.7.9/llama_index/program/llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/program/llm_prompt_program.py` & `llama_index-0.7.9/llama_index/program/llm_prompt_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/program/openai_program.py` & `llama_index-0.7.9/llama_index/program/openai_program.py`

 * *Files 18% similar despite different names*

```diff
@@ -98,7 +98,37 @@
         if self._verbose:
             name = function_call["name"]
             arguments_str = function_call["arguments"]
             print(f"Function call: {name} with args: {arguments_str}")
 
         output = self.output_cls.parse_raw(function_call["arguments"])
         return output
+
+    async def acall(
+        self,
+        *args: Any,
+        **kwargs: Any,
+    ) -> BaseModel:
+        formatted_prompt = self._prompt.format(**kwargs)
+
+        openai_fn_spec = to_openai_function(self._output_cls)
+
+        chat_response = await self._llm.achat(
+            messages=[ChatMessage(role=MessageRole.USER, content=formatted_prompt)],
+            functions=[openai_fn_spec],
+            function_call=self._function_call,
+        )
+        message = chat_response.message
+        if "function_call" not in message.additional_kwargs:
+            raise ValueError(
+                "Expected function call in ai_message.additional_kwargs, "
+                "but none found."
+            )
+
+        function_call = message.additional_kwargs["function_call"]
+        if self._verbose:
+            name = function_call["name"]
+            arguments_str = function_call["arguments"]
+            print(f"Function call: {name} with args: {arguments_str}")
+
+        output = self.output_cls.parse_raw(function_call["arguments"])
+        return output
```

### Comparing `llama_index-0.7.8/llama_index/program/predefined/df.py` & `llama_index-0.7.9/llama_index/program/predefined/df.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/program/predefined/evaporate/base.py` & `llama_index-0.7.9/llama_index/program/predefined/evaporate/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/program/predefined/evaporate/extractor.py` & `llama_index-0.7.9/llama_index/program/predefined/evaporate/extractor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/program/predefined/evaporate/prompts.py` & `llama_index-0.7.9/llama_index/program/predefined/evaporate/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/base.py` & `llama_index-0.7.9/llama_index/prompts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/chat_prompts.py` & `llama_index-0.7.9/llama_index/prompts/chat_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/choice_select.py` & `llama_index-0.7.9/llama_index/prompts/choice_select.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/default_prompt_selectors.py` & `llama_index-0.7.9/llama_index/prompts/default_prompt_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/default_prompts.py` & `llama_index-0.7.9/llama_index/prompts/default_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/guidance_utils.py` & `llama_index-0.7.9/llama_index/prompts/guidance_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/prompt_selector.py` & `llama_index-0.7.9/llama_index/prompts/prompt_selector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/prompt_type.py` & `llama_index-0.7.9/llama_index/prompts/prompt_type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/prompts.py` & `llama_index-0.7.9/llama_index/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/system.py` & `llama_index-0.7.9/llama_index/prompts/system.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/prompts/utils.py` & `llama_index-0.7.9/llama_index/prompts/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/__init__.py` & `llama_index-0.7.9/llama_index/query_engine/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/citation_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/citation_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/flare/answer_inserter.py` & `llama_index-0.7.9/llama_index/query_engine/flare/answer_inserter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/flare/base.py` & `llama_index-0.7.9/llama_index/query_engine/flare/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/flare/output_parser.py` & `llama_index-0.7.9/llama_index/query_engine/flare/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/graph_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/graph_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/multistep_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/multistep_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/pandas_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/pandas_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/retriever_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/retriever_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/retry_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/retry_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/retry_source_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/retry_source_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/router_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/router_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/sql_join_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/sql_join_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/sql_vector_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/sql_vector_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/sub_question_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/sub_question_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/query_engine/transform_query_engine.py` & `llama_index-0.7.9/llama_index/query_engine/transform_query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/question_gen/guidance_generator.py` & `llama_index-0.7.9/llama_index/question_gen/guidance_generator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/question_gen/llm_generators.py` & `llama_index-0.7.9/llama_index/question_gen/llm_generators.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/question_gen/output_parser.py` & `llama_index-0.7.9/llama_index/question_gen/output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/question_gen/prompts.py` & `llama_index-0.7.9/llama_index/question_gen/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/question_gen/types.py` & `llama_index-0.7.9/llama_index/question_gen/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/__init__.py` & `llama_index-0.7.9/llama_index/readers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/base.py` & `llama_index-0.7.9/llama_index/readers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/chatgpt_plugin/base.py` & `llama_index-0.7.9/llama_index/readers/chatgpt_plugin/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/chroma.py` & `llama_index-0.7.9/llama_index/readers/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/database.py` & `llama_index-0.7.9/llama_index/readers/database.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/deeplake.py` & `llama_index-0.7.9/llama_index/readers/deeplake.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/discord_reader.py` & `llama_index-0.7.9/llama_index/readers/discord_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/download.py` & `llama_index-0.7.9/llama_index/readers/download.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/elasticsearch.py` & `llama_index-0.7.9/llama_index/readers/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/faiss.py` & `llama_index-0.7.9/llama_index/readers/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/base.py` & `llama_index-0.7.9/llama_index/readers/file/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Simple reader that reads files of different formats from a directory."""
 import logging
+import os
 from pathlib import Path
 from typing import Callable, Dict, Generator, List, Optional, Type
-import os
 
 from llama_index.readers.base import BaseReader
 from llama_index.readers.file.docs_reader import DocxReader, PDFReader
 from llama_index.readers.file.epub_reader import EpubReader
 from llama_index.readers.file.image_reader import ImageReader
 from llama_index.readers.file.ipynb_reader import IPYNBReader
 from llama_index.readers.file.markdown_reader import MarkdownReader
@@ -34,27 +34,31 @@
 
 logger = logging.getLogger(__name__)
 
 
 class SimpleDirectoryReader(BaseReader):
     """Simple directory reader.
 
-    Can read files into separate documents, or concatenates
-    files into one document text.
+    Load files from file directory.
+    Automatically select the best file reader given file extensions.
 
     Args:
         input_dir (str): Path to the directory.
         input_files (List): List of file paths to read
             (Optional; overrides input_dir, exclude)
         exclude (List): glob of python file paths to exclude (Optional)
         exclude_hidden (bool): Whether to exclude hidden files (dotfiles).
+        encoding (str): Encoding of the files.
+            Default is utf-8.
         errors (str): how encoding and decoding errors are to be handled,
               see https://docs.python.org/3/library/functions.html#open
         recursive (bool): Whether to recursively search in subdirectories.
             False by default.
+        filename_as_id (bool): Whether to use the filename as the document id.
+            False by default.
         required_exts (Optional[List[str]]): List of required extensions.
             Default is None.
         file_extractor (Optional[Dict[str, BaseReader]]): A mapping of file
             extension to a BaseReader class that specifies how to convert that file
             to text. If not specified, use default from DEFAULT_FILE_READER_CLS.
         num_files_limit (Optional[int]): Maximum number of files to read.
             Default is None.
@@ -67,27 +71,29 @@
         self,
         input_dir: Optional[str] = None,
         input_files: Optional[List] = None,
         exclude: Optional[List] = None,
         exclude_hidden: bool = True,
         errors: str = "ignore",
         recursive: bool = False,
+        encoding: str = "utf-8",
         filename_as_id: bool = False,
         required_exts: Optional[List[str]] = None,
         file_extractor: Optional[Dict[str, BaseReader]] = None,
         num_files_limit: Optional[int] = None,
         file_metadata: Optional[Callable[[str], Dict]] = None,
     ) -> None:
         """Initialize with parameters."""
         super().__init__()
 
         if not input_dir and not input_files:
             raise ValueError("Must provide either `input_dir` or `input_files`.")
 
         self.errors = errors
+        self.encoding = encoding
 
         self.exclude = exclude
         self.recursive = recursive
         self.exclude_hidden = exclude_hidden
         self.required_exts = required_exts
         self.num_files_limit = num_files_limit
 
@@ -170,22 +176,16 @@
         )
 
         return new_input_files
 
     def load_data(self) -> List[Document]:
         """Load data from the input directory.
 
-        Args:
-            concatenate (bool): whether to concatenate all text docs into a single doc.
-                If set to True, file metadata is ignored. False by default.
-                This setting does not apply to image docs (always one doc per image).
-
         Returns:
             List[Document]: A list of documents.
-
         """
         documents = []
         for input_file in self.input_files:
             metadata: Optional[dict] = None
             if self.file_metadata is not None:
                 metadata = self.file_metadata(str(input_file))
 
@@ -206,15 +206,17 @@
                 if self.filename_as_id:
                     for i, doc in enumerate(docs):
                         doc.id_ = f"{str(input_file)}_part_{i}"
 
                 documents.extend(docs)
             else:
                 # do standard read
-                with open(input_file, "r", errors=self.errors, encoding="utf8") as f:
+                with open(
+                    input_file, "r", errors=self.errors, encoding=self.encoding
+                ) as f:
                     data = f.read()
 
                 doc = Document(text=data, metadata=metadata or {})
                 if self.filename_as_id:
                     doc.id_ = str(input_file)
 
                 documents.append(doc)
```

### Comparing `llama_index-0.7.8/llama_index/readers/file/docs_reader.py` & `llama_index-0.7.9/llama_index/readers/file/docs_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/epub_reader.py` & `llama_index-0.7.9/llama_index/readers/file/epub_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/image_caption_reader.py` & `llama_index-0.7.9/llama_index/readers/file/image_caption_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/image_reader.py` & `llama_index-0.7.9/llama_index/readers/file/image_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/image_vision_llm_reader.py` & `llama_index-0.7.9/llama_index/readers/file/image_vision_llm_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/ipynb_reader.py` & `llama_index-0.7.9/llama_index/readers/file/ipynb_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/markdown_reader.py` & `llama_index-0.7.9/llama_index/readers/file/markdown_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/mbox_reader.py` & `llama_index-0.7.9/llama_index/readers/file/mbox_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/slides_reader.py` & `llama_index-0.7.9/llama_index/readers/file/slides_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/tabular_reader.py` & `llama_index-0.7.9/llama_index/readers/file/tabular_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/file/video_audio_reader.py` & `llama_index-0.7.9/llama_index/readers/file/video_audio_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/github_readers/github_api_client.py` & `llama_index-0.7.9/llama_index/readers/github_readers/github_api_client.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/github_readers/github_repository_reader.py` & `llama_index-0.7.9/llama_index/readers/github_readers/github_repository_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/github_readers/utils.py` & `llama_index-0.7.9/llama_index/readers/github_readers/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/google_readers/gdocs.py` & `llama_index-0.7.9/llama_index/readers/google_readers/gdocs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/google_readers/gsheets.py` & `llama_index-0.7.9/llama_index/readers/google_readers/gsheets.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/json.py` & `llama_index-0.7.9/llama_index/readers/json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/make_com/wrapper.py` & `llama_index-0.7.9/llama_index/readers/make_com/wrapper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/mbox.py` & `llama_index-0.7.9/llama_index/readers/mbox.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/metal.py` & `llama_index-0.7.9/llama_index/readers/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/milvus.py` & `llama_index-0.7.9/llama_index/readers/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/mongo.py` & `llama_index-0.7.9/llama_index/readers/mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/myscale.py` & `llama_index-0.7.9/llama_index/readers/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/notion.py` & `llama_index-0.7.9/llama_index/readers/notion.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/obsidian.py` & `llama_index-0.7.9/llama_index/readers/obsidian.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/pinecone.py` & `llama_index-0.7.9/llama_index/readers/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/psychic.py` & `llama_index-0.7.9/llama_index/readers/psychic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/qdrant.py` & `llama_index-0.7.9/llama_index/readers/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/redis/utils.py` & `llama_index-0.7.9/llama_index/readers/redis/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/slack.py` & `llama_index-0.7.9/llama_index/readers/slack.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/steamship/file_reader.py` & `llama_index-0.7.9/llama_index/readers/steamship/file_reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/string_iterable.py` & `llama_index-0.7.9/llama_index/readers/string_iterable.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/twitter.py` & `llama_index-0.7.9/llama_index/readers/twitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/weaviate/reader.py` & `llama_index-0.7.9/llama_index/readers/weaviate/reader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/web.py` & `llama_index-0.7.9/llama_index/readers/web.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/wikipedia.py` & `llama_index-0.7.9/llama_index/readers/wikipedia.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/readers/youtube_transcript.py` & `llama_index-0.7.9/llama_index/readers/youtube_transcript.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response/notebook_utils.py` & `llama_index-0.7.9/llama_index/response/notebook_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response/pprint_utils.py` & `llama_index-0.7.9/llama_index/response/pprint_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response/schema.py` & `llama_index-0.7.9/llama_index/response/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/__init__.py` & `llama_index-0.7.9/llama_index/response_synthesizers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/accumulate.py` & `llama_index-0.7.9/llama_index/response_synthesizers/accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/base.py` & `llama_index-0.7.9/llama_index/response_synthesizers/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/compact_and_accumulate.py` & `llama_index-0.7.9/llama_index/response_synthesizers/compact_and_accumulate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/compact_and_refine.py` & `llama_index-0.7.9/llama_index/response_synthesizers/compact_and_refine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/factory.py` & `llama_index-0.7.9/llama_index/response_synthesizers/factory.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/generation.py` & `llama_index-0.7.9/llama_index/response_synthesizers/generation.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/no_text.py` & `llama_index-0.7.9/llama_index/response_synthesizers/no_text.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/refine.py` & `llama_index-0.7.9/llama_index/response_synthesizers/refine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/simple_summarize.py` & `llama_index-0.7.9/llama_index/response_synthesizers/simple_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/tree_summarize.py` & `llama_index-0.7.9/llama_index/response_synthesizers/tree_summarize.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/response_synthesizers/type.py` & `llama_index-0.7.9/llama_index/response_synthesizers/type.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/retrievers/__init__.py` & `llama_index-0.7.9/llama_index/retrievers/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/retrievers/recursive_retriever.py` & `llama_index-0.7.9/llama_index/retrievers/recursive_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/retrievers/transform_retriever.py` & `llama_index-0.7.9/llama_index/retrievers/transform_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/schema.py` & `llama_index-0.7.9/llama_index/schema.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/selectors/llm_selectors.py` & `llama_index-0.7.9/llama_index/selectors/llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/selectors/prompts.py` & `llama_index-0.7.9/llama_index/selectors/prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/selectors/pydantic_selectors.py` & `llama_index-0.7.9/llama_index/selectors/pydantic_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/selectors/types.py` & `llama_index-0.7.9/llama_index/selectors/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/__init__.py` & `llama_index-0.7.9/llama_index/storage/docstore/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/dynamodb_docstore.py` & `llama_index-0.7.9/llama_index/storage/docstore/dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/keyval_docstore.py` & `llama_index-0.7.9/llama_index/storage/docstore/keyval_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/mongo_docstore.py` & `llama_index-0.7.9/llama_index/storage/docstore/mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/redis_docstore.py` & `llama_index-0.7.9/llama_index/storage/docstore/redis_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/registry.py` & `llama_index-0.7.9/llama_index/storage/docstore/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/simple_docstore.py` & `llama_index-0.7.9/llama_index/storage/docstore/simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/types.py` & `llama_index-0.7.9/llama_index/storage/docstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/docstore/utils.py` & `llama_index-0.7.9/llama_index/storage/docstore/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/index_store/dynamodb_index_store.py` & `llama_index-0.7.9/llama_index/storage/index_store/dynamodb_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/index_store/keyval_index_store.py` & `llama_index-0.7.9/llama_index/storage/index_store/keyval_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/index_store/mongo_index_store.py` & `llama_index-0.7.9/llama_index/storage/index_store/mongo_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/index_store/redis_index_store.py` & `llama_index-0.7.9/llama_index/storage/index_store/redis_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/index_store/simple_index_store.py` & `llama_index-0.7.9/llama_index/storage/index_store/simple_index_store.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/index_store/types.py` & `llama_index-0.7.9/llama_index/storage/index_store/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/index_store/utils.py` & `llama_index-0.7.9/llama_index/storage/index_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/kvstore/dynamodb_kvstore.py` & `llama_index-0.7.9/llama_index/storage/kvstore/dynamodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/kvstore/mongodb_kvstore.py` & `llama_index-0.7.9/llama_index/storage/kvstore/mongodb_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/kvstore/redis_kvstore.py` & `llama_index-0.7.9/llama_index/storage/kvstore/redis_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/kvstore/s3_kvstore.py` & `llama_index-0.7.9/llama_index/storage/kvstore/s3_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/kvstore/simple_kvstore.py` & `llama_index-0.7.9/llama_index/storage/kvstore/simple_kvstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/kvstore/types.py` & `llama_index-0.7.9/llama_index/storage/kvstore/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/storage/storage_context.py` & `llama_index-0.7.9/llama_index/storage/storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/token_counter/mock_embed_model.py` & `llama_index-0.7.9/llama_index/token_counter/mock_embed_model.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/token_counter/utils.py` & `llama_index-0.7.9/llama_index/token_counter/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/function_tool.py` & `llama_index-0.7.9/llama_index/tools/function_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/ondemand_loader_tool.py` & `llama_index-0.7.9/llama_index/tools/ondemand_loader_tool.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/query_engine.py` & `llama_index-0.7.9/llama_index/tools/query_engine.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/query_plan.py` & `llama_index-0.7.9/llama_index/tools/query_plan.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/tool_spec/base.py` & `llama_index-0.7.9/llama_index/tools/tool_spec/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/tool_spec/load_and_search/base.py` & `llama_index-0.7.9/llama_index/tools/tool_spec/load_and_search/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/tool_spec/notion/base.py` & `llama_index-0.7.9/llama_index/tools/tool_spec/notion/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/tool_spec/slack/base.py` & `llama_index-0.7.9/llama_index/tools/tool_spec/slack/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/types.py` & `llama_index-0.7.9/llama_index/tools/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tools/utils.py` & `llama_index-0.7.9/llama_index/tools/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tts/bark.py` & `llama_index-0.7.9/llama_index/tts/bark.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tts/base.py` & `llama_index-0.7.9/llama_index/tts/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/tts/elevenlabs.py` & `llama_index-0.7.9/llama_index/tts/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/types.py` & `llama_index-0.7.9/llama_index/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/utils.py` & `llama_index-0.7.9/llama_index/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 """General utils functions."""
 
+import os
 import random
 import sys
 import time
 import traceback
 import uuid
 from contextlib import contextmanager
 from dataclasses import dataclass
+from functools import partial
 from itertools import islice
+from pathlib import Path
 from typing import (
     Any,
     Callable,
     Generator,
+    Iterable,
     List,
     Optional,
     Set,
     Type,
-    cast,
     Union,
-    Iterable,
+    cast,
 )
-import os
 
 
 class GlobalsHelper:
     """Helper to retrieve globals.
 
     Helpful for global caching of certain variables that can be expensive to load.
     (e.g. tokenization)
@@ -43,15 +45,16 @@
             )
             try:
                 import tiktoken
             except ImportError:
                 raise ImportError(tiktoken_import_err)
             enc = tiktoken.get_encoding("gpt2")
             self._tokenizer = cast(Callable[[str], List], enc.encode)
-        return self._tokenizer
+            self._tokenizer = partial(self._tokenizer, allowed_special="all")
+        return self._tokenizer  # type: ignore
 
     @property
     def stopwords(self) -> List[str]:
         """Get stopwords."""
         if self._stopwords is None:
             try:
                 import nltk
@@ -232,14 +235,40 @@
         raise ValueError(
             "`transformers` package not found, please run `pip install transformers`"
         )
     tokenizer = AutoTokenizer.from_pretrained(model_name)
     return tokenizer.tokenize
 
 
+def get_cache_dir() -> Path:
+    """Locate a platform-appropriate cache directory for llama_index,
+    and create it if it doesn't yet exist
+    """
+    # Linux, Unix, AIX, etc.
+    if os.name == "posix" and sys.platform != "darwin":
+        # use ~/.cache if empty OR not set
+        base = os.path.expanduser("~/.cache")
+        path = Path(base, "llama_index")
+
+    # Mac OS
+    elif sys.platform == "darwin":
+        path = Path(os.path.expanduser("~"), "Library/Caches/llama_index")
+
+    # Windows (hopefully)
+    else:
+        local = os.environ.get("LOCALAPPDATA", None) or os.path.expanduser(
+            "~\\AppData\\Local"
+        )
+        path = Path(local, "llama_index")
+
+    if not os.path.exists(path):
+        os.makedirs(path)
+    return path
+
+
 # Sample text from llama_index's readme
 SAMPLE_TEXT = """
 Context
 LLMs are a phenomenonal piece of technology for knowledge generation and reasoning. 
 They are pre-trained on large amounts of publicly available data.
 How do we best augment LLMs with our own private data?
 We need a comprehensive toolkit to help perform this data augmentation for LLMs.
```

### Comparing `llama_index-0.7.8/llama_index/vector_stores/__init__.py` & `llama_index-0.7.9/llama_index/vector_stores/__init__.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/chatgpt_plugin.py` & `llama_index-0.7.9/llama_index/vector_stores/chatgpt_plugin.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/chroma.py` & `llama_index-0.7.9/llama_index/vector_stores/chroma.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/deeplake.py` & `llama_index-0.7.9/llama_index/vector_stores/deeplake.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,248 +1,202 @@
 """DeepLake vector store index.
 
 An index that is built within DeepLake.
 
 """
 import logging
-from typing import Any, Dict, List, Optional, cast
-
-import numpy as np
+from typing import Any, List, Optional, cast
 
 from llama_index.schema import MetadataMode
-from llama_index.indices.query.embedding_utils import get_top_k_embeddings
 from llama_index.vector_stores.types import (
     NodeWithEmbedding,
-    VectorStore,
     VectorStoreQuery,
     VectorStoreQueryResult,
 )
+from llama_index.vector_stores.types import VectorStore as VectorStoreBase
+from llama_index.vector_stores.utils import (
+    metadata_dict_to_node,
+    node_to_metadata_dict,
+)
 
-logger = logging.getLogger(__name__)
+try:
+    from deeplake.core.vectorstore import VectorStore
 
+    DEEPLAKE_INSTALLED = True
+except ImportError:
+    DEEPLAKE_INSTALLED = False
 
-def dp_filter(x: dict, filter: Dict[str, str]) -> bool:
-    """Filter helper function for Deep Lake"""
-    metadata = x["metadata"].data()["value"]
-    return all(k in metadata and v == metadata[k] for k, v in filter.items())
+logger = logging.getLogger(__name__)
 
 
-class DeepLakeVectorStore(VectorStore):
+class DeepLakeVectorStore(VectorStoreBase):
     """The DeepLake Vector Store.
 
     In this vector store we store the text, its embedding and
     a few pieces of its metadata in a deeplake dataset. This implemnetation
     allows the use of an already existing deeplake dataset if it is one that was created
     this vector store. It also supports creating a new one if the dataset doesnt
     exist or if `overwrite` is set to True.
-
-    Args:
-        deeplake_path (str, optional): Path to the deeplake dataset, where data will be
-        stored. Defaults to "llama_index".
-        overwrite (bool, optional): Whether to overwrite existing dataset with same
-            name. Defaults to False.
-        token (str, optional): the deeplake token that allows you to access the dataset
-            with proper access. Defaults to None.
-        read_only (bool, optional): Whether to open the dataset with read only mode.
-        ingestion_batch_size (bool, 1024): used for controlling batched data
-            injestion to deeplake dataset. Defaults to 1024.
-        injestion_num_workers (int, 1): number of workers to use during data injestion.
-            Defaults to 4.
-        overwrite (bool, optional): Whether to overwrite existing dataset with the
-            new dataset with the same name.
-
-    Raises:
-        ImportError: Unable to import `deeplake`.
-        UserNotLoggedinException: When user is not logged in with credentials
-            or token.
-        TokenPermissionError: When dataset does not exist or user doesn't have
-            enough permissions to modify the dataset.
-        InvalidTokenException: If the specified token is invalid
-
-
-    Returns:
-        DeepLakeVectorstore: Vectorstore that supports add, delete, and query.
     """
 
-    stores_text: bool = False
-    flat_metadata: bool = False
+    stores_text: bool = True
+    flat_metadata: bool = True
 
     def __init__(
         self,
         dataset_path: str = "llama_index",
         token: Optional[str] = None,
         read_only: Optional[bool] = False,
         ingestion_batch_size: int = 1024,
         ingestion_num_workers: int = 4,
         overwrite: bool = False,
+        exec_option: str = "python",
+        verbose: bool = True,
+        **kwargs: Any,
     ):
-        """Initialize with Deep Lake client."""
+        """
+        Args:
+            dataset_path (str): Path to the deeplake dataset, where data will be
+            stored. Defaults to "llama_index".
+            overwrite (bool, optional): Whether to overwrite existing dataset with same
+                name. Defaults to False.
+            token (str, optional): the deeplake token that allows you to access the
+                dataset with proper access. Defaults to None.
+            read_only (bool, optional): Whether to open the dataset with read only mode.
+            ingestion_batch_size (int): used for controlling batched data
+                injestion to deeplake dataset. Defaults to 1024.
+            ingestion_num_workers (int): number of workers to use during data injestion.
+                Defaults to 4.
+            overwrite (bool): Whether to overwrite existing dataset with the
+                new dataset with the same name.
+            exec_option (str): Default method for search execution. It could be either
+                It could be either ``"python"``, ``"compute_engine"`` or
+                ``"tensor_db"``. Defaults to ``"python"``.
+                - ``python`` - Pure-python implementation that runs on the client and
+                    can be used for data stored anywhere. WARNING: using this option
+                    with big datasets is discouraged because it can lead to memory
+                    issues.
+                - ``compute_engine`` - Performant C++ implementation of the Deep Lake
+                    Compute Engine that runs on the client and can be used for any data
+                    stored in or connected to Deep Lake. It cannot be used with
+                    in-memory or local datasets.
+                - ``tensor_db`` - Performant and fully-hosted Managed Tensor Database
+                    that is responsible for storage and query execution. Only available
+                    for data stored in the Deep Lake Managed Database. Store datasets in
+                    this database by specifying runtime = {"tensor_db": True} during
+                    dataset creation.
+            verbose (bool): Specify if verbose output is enabled. Default is True.
+            **kwargs (Any): Additional keyword arguments.
+
+        Raises:
+            ImportError: Unable to import `deeplake`.
+        """
         self.ingestion_batch_size = ingestion_batch_size
         self.num_workers = ingestion_num_workers
         self.token = token
         self.read_only = read_only
         self.dataset_path = dataset_path
 
-        try:
-            import deeplake
-            from deeplake.constants import MB
-        except ImportError:
-            raise ValueError(
+        if not DEEPLAKE_INSTALLED:
+            raise ImportError(
                 "Could not import deeplake python package. "
                 "Please install it with `pip install deeplake`."
             )
-        self._deeplake = deeplake
 
-        if deeplake.exists(dataset_path, token=token) and not overwrite:
-            self.ds = deeplake.load(dataset_path, token=token, read_only=read_only)
-            logger.warning(
-                f"Deep Lake Dataset in {dataset_path} already exists, "
-                f"loading from the storage"
-            )
-            self.ds.summary()
-        else:
-            self.ds = deeplake.empty(dataset_path, token=token, overwrite=True)
-
-            with self.ds:
-                self.ds.create_tensor(
-                    "text",
-                    htype="text",
-                    create_id_tensor=False,
-                    create_sample_info_tensor=False,
-                    create_shape_tensor=False,
-                    chunk_compression="lz4",
-                )
-                self.ds.create_tensor(
-                    "metadata",
-                    htype="json",
-                    create_id_tensor=False,
-                    create_sample_info_tensor=False,
-                    create_shape_tensor=False,
-                    chunk_compression="lz4",
-                )
-                self.ds.create_tensor(
-                    "embedding",
-                    htype="generic",
-                    dtype=np.float64,
-                    create_id_tensor=False,
-                    create_sample_info_tensor=False,
-                    max_chunk_size=64 * MB,
-                    create_shape_tensor=True,
-                )
-                self.ds.create_tensor(
-                    "ids",
-                    htype="text",
-                    create_id_tensor=False,
-                    create_sample_info_tensor=False,
-                    create_shape_tensor=False,
-                    chunk_compression="lz4",
-                )
+        self.vectorstore = VectorStore(
+            path=dataset_path,
+            ingestion_batch_size=ingestion_batch_size,
+            num_workers=ingestion_num_workers,
+            token=token,
+            read_only=read_only,
+            exec_option=exec_option,
+            overwrite=overwrite,
+            verbose=verbose,
+            **kwargs,
+        )
+        self._id_tensor_name = "ids" if "ids" in self.vectorstore.tensors() else "id"
 
     @property
-    def client(self) -> None:
-        """Get client."""
-        return self.ds
+    def client(self) -> Any:
+        """Get client.
+
+        Returns:
+            Any: DeepLake vectorstore dataset.
+        """
+        return self.vectorstore.dataset
 
     def add(self, embedding_results: List[NodeWithEmbedding]) -> List[str]:
         """Add the embeddings and their nodes into DeepLake.
 
         Args:
             embedding_results (List[NodeWithEmbedding]): The embeddings and their data
                 to insert.
 
-        Raises:
-            UserNotLoggedinException: When user is not logged in with credentials
-                or token.
-            TokenPermissionError: When dataset does not exist or user doesn't have
-                enough permissions to modify the dataset.
-            InvalidTokenException: If the specified token is invalid
-
         Returns:
             List[str]: List of ids inserted.
         """
-        data_to_injest = []
-        ids = []
+        embedding = []
+        metadata = []
+        id_ = []
+        text = []
 
         for result in embedding_results:
-            embedding = result.embedding
-            metadata = result.node.metadata or {}
-            metadata = {**metadata, **{"document_id": result.ref_doc_id}}
-            id = result.id
-            text = result.node.get_content(metadata_mode=MetadataMode.NONE)
-
-            data_to_injest.append(
-                {
-                    "text": text,
-                    "metadata": metadata,
-                    "ids": id,
-                    "embedding": embedding,
-                }
+            embedding.append(result.embedding)
+            metadata.append(
+                node_to_metadata_dict(
+                    result.node, remove_text=False, flat_metadata=self.flat_metadata
+                )
             )
-            ids.append(id)
+            id_.append(result.id)
+            text.append(result.node.get_content(metadata_mode=MetadataMode.NONE))
 
-        @self._deeplake.compute
-        def ingest(sample_in: List[Dict], sample_out: Any) -> None:
-            for item in sample_in:
-                sample_out.text.append(item["text"])
-                sample_out.metadata.append(item["metadata"])
-                sample_out.embedding.append(item["embedding"])
-                sample_out.ids.append(item["ids"])
-
-        batch_size = min(self.ingestion_batch_size, len(data_to_injest))
-        batched = [
-            data_to_injest[i : i + batch_size]
-            for i in range(0, len(data_to_injest), batch_size)
-        ]
-
-        ingest().eval(
-            batched,
-            self.ds,
-            num_workers=min(self.num_workers, len(batched) // self.num_workers),
+        kwargs = {
+            "embedding": embedding,
+            "metadata": metadata,
+            self._id_tensor_name: id_,
+            "text": text,
+        }
+
+        return self.vectorstore.add(
+            return_ids=True,
+            **kwargs,
         )
 
-        self.ds.commit(allow_empty=True)
-        self.ds.summary()
-        return ids
-
     def delete(self, ref_doc_id: str, **delete_kwargs: Any) -> None:
         """
         Delete nodes using with ref_doc_id.
 
         Args:
             ref_doc_id (str): The doc_id of the document to delete.
 
         """
-        view = None
-        if ref_doc_id:
-            view = self.ds.filter(lambda x: x["ids"].numpy().tolist() == [ref_doc_id])
-            ids = list(view.sample_indices)
-
-        with self.ds:
-            for id in sorted(ids)[::-1]:
-                self.ds.pop(id)
-
-            self.ds.commit(f"deleted {len(ids)} samples", allow_empty=True)
-            self.ds.summary()
+        self.vectorstore.delete(filter={"metadata": {"doc_id": ref_doc_id}})
 
     def query(self, query: VectorStoreQuery, **kwargs: Any) -> VectorStoreQueryResult:
         """Query index for top k most similar nodes.
 
         Args:
-            query_embedding (List[float]): query embedding
-            similarity_top_k (int): top k most similar nodes
-        """
-        if query.filters is not None:
-            raise ValueError("Metadata filters not implemented for DeepLake yet.")
+            query (VectorStoreQuery): VectorStoreQuery class input, it has
+                the following attributes:
+                1. query_embedding (List[float]): query embedding
+                2. similarity_top_k (int): top k most similar nodes
 
+        Returns:
+            VectorStoreQueryResult
+        """
         query_embedding = cast(List[float], query.query_embedding)
-        embeddings = self.ds.embedding.numpy(fetch_chunks=True)
-        embedding_ids = self.ds.ids.numpy(fetch_chunks=True)
-        embedding_ids = [str(embedding_id[0]) for embedding_id in embedding_ids]
-
-        top_similarities, top_ids = get_top_k_embeddings(
-            query_embedding,
-            embeddings,
-            similarity_top_k=query.similarity_top_k,
-            embedding_ids=embedding_ids,
+        exec_option = kwargs.get("exec_option", "python")
+        data = self.vectorstore.search(
+            embedding=query_embedding,
+            exec_option=exec_option,
+            k=query.similarity_top_k,
+            filter=query.filters,
         )
 
-        return VectorStoreQueryResult(similarities=top_similarities, ids=top_ids)
+        similarities = data["score"]
+        ids = data[self._id_tensor_name]
+        metadatas = data["metadata"]
+        nodes = []
+        for metadata in metadatas:
+            nodes.append(metadata_dict_to_node(metadata))
+
+        return VectorStoreQueryResult(nodes=nodes, similarities=similarities, ids=ids)
```

### Comparing `llama_index-0.7.8/llama_index/vector_stores/docarray/base.py` & `llama_index-0.7.9/llama_index/vector_stores/docarray/base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/docarray/hnsw.py` & `llama_index-0.7.9/llama_index/vector_stores/docarray/hnsw.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/docarray/in_memory.py` & `llama_index-0.7.9/llama_index/vector_stores/docarray/in_memory.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/dynamodb.py` & `llama_index-0.7.9/llama_index/vector_stores/dynamodb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/faiss.py` & `llama_index-0.7.9/llama_index/vector_stores/faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/lancedb.py` & `llama_index-0.7.9/llama_index/vector_stores/lancedb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/metal.py` & `llama_index-0.7.9/llama_index/vector_stores/metal.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/milvus.py` & `llama_index-0.7.9/llama_index/vector_stores/milvus.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/mongodb.py` & `llama_index-0.7.9/llama_index/vector_stores/mongodb.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/myscale.py` & `llama_index-0.7.9/llama_index/vector_stores/myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/opensearch.py` & `llama_index-0.7.9/llama_index/vector_stores/opensearch.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/pinecone.py` & `llama_index-0.7.9/llama_index/vector_stores/pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/postgres.py` & `llama_index-0.7.9/llama_index/vector_stores/postgres.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/qdrant.py` & `llama_index-0.7.9/llama_index/vector_stores/qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/redis.py` & `llama_index-0.7.9/llama_index/vector_stores/redis.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/registry.py` & `llama_index-0.7.9/llama_index/vector_stores/registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/simple.py` & `llama_index-0.7.9/llama_index/vector_stores/simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/supabase.py` & `llama_index-0.7.9/llama_index/vector_stores/supabase.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/tair.py` & `llama_index-0.7.9/llama_index/vector_stores/tair.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/types.py` & `llama_index-0.7.9/llama_index/vector_stores/types.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/typesense.py` & `llama_index-0.7.9/llama_index/vector_stores/typesense.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/utils.py` & `llama_index-0.7.9/llama_index/vector_stores/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,15 +65,18 @@
 
 # TODO: Deprecated conversion functions
 def legacy_metadata_dict_to_node(
     metadata: dict, text_key: str = DEFAULT_TEXT_KEY
 ) -> Tuple[dict, dict, dict]:
     """Common logic for loading Node data from metadata dict."""
     # make a copy first
-    metadata = metadata.copy()
+    if metadata is None:
+        metadata = {}
+    else:
+        metadata = metadata.copy()
 
     # load node_info from json string
     node_info_str = metadata.pop("node_info", "")
     if node_info_str == "":
         node_info = {}
     else:
         node_info = json.loads(node_info_str)
```

### Comparing `llama_index-0.7.8/llama_index/vector_stores/weaviate.py` & `llama_index-0.7.9/llama_index/vector_stores/weaviate.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index/vector_stores/weaviate_utils.py` & `llama_index-0.7.9/llama_index/vector_stores/weaviate_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/llama_index.egg-info/PKG-INFO` & `llama_index-0.7.9/llama_index.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llama-index
-Version: 0.7.8
+Version: 0.7.9
 Summary: Interface between LLMs and your data
 Home-page: https://github.com/jerryjliu/llama_index
 Author: Jerry Liu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `llama_index-0.7.8/llama_index.egg-info/SOURCES.txt` & `llama_index-0.7.9/llama_index.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,16 @@
 llama_index/embeddings/langchain.py
 llama_index/embeddings/openai.py
 llama_index/embeddings/utils.py
 llama_index/evaluation/__init__.py
 llama_index/evaluation/base.py
 llama_index/evaluation/dataset_generation.py
 llama_index/evaluation/guideline_eval.py
+llama_index/evaluation/benchmarks/__init__.py
+llama_index/evaluation/benchmarks/beir.py
 llama_index/graph_stores/__init__.py
 llama_index/graph_stores/nebulagraph.py
 llama_index/graph_stores/registery.py
 llama_index/graph_stores/simple.py
 llama_index/graph_stores/types.py
 llama_index/indices/__init__.py
 llama_index/indices/base.py
@@ -468,14 +470,15 @@
 tests/indices/tree/test_embedding_retriever.py
 tests/indices/tree/test_index.py
 tests/indices/tree/test_retrievers.py
 tests/indices/vector_store/__init__.py
 tests/indices/vector_store/conftest.py
 tests/indices/vector_store/mock_faiss.py
 tests/indices/vector_store/mock_services.py
+tests/indices/vector_store/test_deeplake.py
 tests/indices/vector_store/test_faiss.py
 tests/indices/vector_store/test_myscale.py
 tests/indices/vector_store/test_pinecone.py
 tests/indices/vector_store/test_retrievers.py
 tests/indices/vector_store/test_simple.py
 tests/indices/vector_store/utils.py
 tests/indices/vector_store/auto_retriever/__init__.py
```

### Comparing `llama_index-0.7.8/setup.py` & `llama_index-0.7.9/setup.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/callbacks/test_llama_debug.py` & `llama_index-0.7.9/tests/callbacks/test_llama_debug.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/callbacks/test_token_counter.py` & `llama_index-0.7.9/tests/callbacks/test_token_counter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/chat_engine/test_condense_question.py` & `llama_index-0.7.9/tests/chat_engine/test_condense_question.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/chat_engine/test_simple.py` & `llama_index-0.7.9/tests/chat_engine/test_simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/conftest.py` & `llama_index-0.7.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/embeddings/test_base.py` & `llama_index-0.7.9/tests/embeddings/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/composability/test_utils.py` & `llama_index-0.7.9/tests/indices/composability/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/conftest.py` & `llama_index-0.7.9/tests/indices/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/document_summary/test_index.py` & `llama_index-0.7.9/tests/indices/document_summary/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/empty/test_base.py` & `llama_index-0.7.9/tests/indices/empty/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/keyword_table/test_base.py` & `llama_index-0.7.9/tests/indices/keyword_table/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/keyword_table/test_retrievers.py` & `llama_index-0.7.9/tests/indices/keyword_table/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/keyword_table/test_utils.py` & `llama_index-0.7.9/tests/indices/keyword_table/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/knowledge_graph/test_base.py` & `llama_index-0.7.9/tests/indices/knowledge_graph/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/knowledge_graph/test_retrievers.py` & `llama_index-0.7.9/tests/indices/knowledge_graph/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/list/test_index.py` & `llama_index-0.7.9/tests/indices/list/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/list/test_retrievers.py` & `llama_index-0.7.9/tests/indices/list/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/postprocessor/test_base.py` & `llama_index-0.7.9/tests/indices/postprocessor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/postprocessor/test_llm_rerank.py` & `llama_index-0.7.9/tests/indices/postprocessor/test_llm_rerank.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/postprocessor/test_optimizer.py` & `llama_index-0.7.9/tests/indices/postprocessor/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/query/conftest.py` & `llama_index-0.7.9/tests/indices/query/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/query/query_transform/test_base.py` & `llama_index-0.7.9/tests/indices/query/query_transform/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/query/test_compose.py` & `llama_index-0.7.9/tests/indices/query/test_compose.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/query/test_compose_vector.py` & `llama_index-0.7.9/tests/indices/query/test_compose_vector.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/query/test_embedding_utils.py` & `llama_index-0.7.9/tests/indices/query/test_embedding_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/query/test_query_bundle.py` & `llama_index-0.7.9/tests/indices/query/test_query_bundle.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/struct_store/conftest.py` & `llama_index-0.7.9/tests/indices/struct_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/struct_store/test_base.py` & `llama_index-0.7.9/tests/indices/struct_store/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/struct_store/test_json_query.py` & `llama_index-0.7.9/tests/indices/struct_store/test_json_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/struct_store/test_sql_query.py` & `llama_index-0.7.9/tests/indices/struct_store/test_sql_query.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/test_loading.py` & `llama_index-0.7.9/tests/indices/test_loading.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/test_loading_graph.py` & `llama_index-0.7.9/tests/indices/test_loading_graph.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/test_node_utils.py` & `llama_index-0.7.9/tests/indices/test_node_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/test_prompt_helper.py` & `llama_index-0.7.9/tests/indices/test_prompt_helper.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/tree/conftest.py` & `llama_index-0.7.9/tests/indices/tree/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/tree/test_embedding_retriever.py` & `llama_index-0.7.9/tests/indices/tree/test_embedding_retriever.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/tree/test_index.py` & `llama_index-0.7.9/tests/indices/tree/test_index.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/tree/test_retrievers.py` & `llama_index-0.7.9/tests/indices/tree/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/auto_retriever/test_output_parser.py` & `llama_index-0.7.9/tests/indices/vector_store/auto_retriever/test_output_parser.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/conftest.py` & `llama_index-0.7.9/tests/indices/vector_store/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/mock_faiss.py` & `llama_index-0.7.9/tests/indices/vector_store/mock_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/mock_services.py` & `llama_index-0.7.9/tests/indices/vector_store/mock_services.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/test_faiss.py` & `llama_index-0.7.9/tests/indices/vector_store/test_faiss.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/test_myscale.py` & `llama_index-0.7.9/tests/indices/vector_store/test_myscale.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/test_pinecone.py` & `llama_index-0.7.9/tests/indices/vector_store/test_pinecone.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/test_retrievers.py` & `llama_index-0.7.9/tests/indices/vector_store/test_retrievers.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/test_simple.py` & `llama_index-0.7.9/tests/indices/vector_store/test_simple.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/indices/vector_store/utils.py` & `llama_index-0.7.9/tests/indices/vector_store/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/langchain_helpers/test_text_splitter.py` & `llama_index-0.7.9/tests/langchain_helpers/test_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llm_predictor/test_base.py` & `llama_index-0.7.9/tests/llm_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llm_predictor/vellum/conftest.py` & `llama_index-0.7.9/tests/llm_predictor/vellum/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llm_predictor/vellum/test_predictor.py` & `llama_index-0.7.9/tests/llm_predictor/vellum/test_predictor.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llm_predictor/vellum/test_prompt_registry.py` & `llama_index-0.7.9/tests/llm_predictor/vellum/test_prompt_registry.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llms/test_anthropic.py` & `llama_index-0.7.9/tests/llms/test_anthropic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llms/test_anthropic_utils.py` & `llama_index-0.7.9/tests/llms/test_anthropic_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llms/test_custom.py` & `llama_index-0.7.9/tests/llms/test_custom.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llms/test_langchain.py` & `llama_index-0.7.9/tests/llms/test_langchain.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llms/test_openai.py` & `llama_index-0.7.9/tests/llms/test_openai.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llms/test_openai_utils.py` & `llama_index-0.7.9/tests/llms/test_openai_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/llms/test_palm.py` & `llama_index-0.7.9/tests/llms/test_palm.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/logger/test_base.py` & `llama_index-0.7.9/tests/logger/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/mock_utils/mock_predict.py` & `llama_index-0.7.9/tests/mock_utils/mock_predict.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/mock_utils/mock_prompts.py` & `llama_index-0.7.9/tests/mock_utils/mock_prompts.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/mock_utils/mock_text_splitter.py` & `llama_index-0.7.9/tests/mock_utils/mock_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/mock_utils/mock_utils.py` & `llama_index-0.7.9/tests/mock_utils/mock_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/objects/test_base.py` & `llama_index-0.7.9/tests/objects/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/objects/test_node_mapping.py` & `llama_index-0.7.9/tests/objects/test_node_mapping.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/output_parsers/test_base.py` & `llama_index-0.7.9/tests/output_parsers/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/output_parsers/test_pydantic.py` & `llama_index-0.7.9/tests/output_parsers/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/output_parsers/test_selection.py` & `llama_index-0.7.9/tests/output_parsers/test_selection.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/playground/test_base.py` & `llama_index-0.7.9/tests/playground/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/program/test_guidance.py` & `llama_index-0.7.9/tests/program/test_guidance.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/program/test_llm_program.py` & `llama_index-0.7.9/tests/program/test_llm_program.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/prompts/test_base.py` & `llama_index-0.7.9/tests/prompts/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/prompts/test_guidance_utils.py` & `llama_index-0.7.9/tests/prompts/test_guidance_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/question_gen/test_guidance_generator.py` & `llama_index-0.7.9/tests/question_gen/test_guidance_generator.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/question_gen/test_llm_generators.py` & `llama_index-0.7.9/tests/question_gen/test_llm_generators.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/readers/test_file.py` & `llama_index-0.7.9/tests/readers/test_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Test file reader."""
 
 from tempfile import TemporaryDirectory
 from typing import Any, Dict
+
 import pytest
 
 from llama_index.readers.file.base import SimpleDirectoryReader
 
 
 def test_recursive() -> None:
     """Test simple directory reader in recursive mode."""
@@ -303,14 +304,45 @@
         ]
 
         # check paths. Split handles path_part_X doc_ids from md and json files
         for doc in documents:
             assert str(doc.node_id).split("_part")[0] in doc_paths
 
 
+def test_specifying_encoding() -> None:
+    """Test if file metadata is added to Document."""
+    # test file_metadata
+    with TemporaryDirectory() as tmp_dir:
+        with open(f"{tmp_dir}/test1.txt", "w", encoding="latin-1") as f:
+            f.write("test1á")
+        with open(f"{tmp_dir}/test2.txt", "w", encoding="latin-1") as f:
+            f.write("test2â")
+        with open(f"{tmp_dir}/test3.txt", "w", encoding="latin-1") as f:
+            f.write("test3ã")
+        with open(f"{tmp_dir}/test4.json", "w", encoding="latin-1") as f:
+            f.write('{"test_1á": {"test_2ã": ["â"]}}')
+
+        reader = SimpleDirectoryReader(
+            tmp_dir, filename_as_id=True, errors="strict", encoding="latin-1"
+        )
+
+        documents = reader.load_data()
+
+        doc_paths = [
+            f"{tmp_dir}/test1.txt",
+            f"{tmp_dir}/test2.txt",
+            f"{tmp_dir}/test3.txt",
+            f"{tmp_dir}/test4.json",
+        ]
+
+        # check paths. Split handles path_part_X doc_ids from md and json files
+        for doc in documents:
+            assert str(doc.node_id).split("_part")[0] in doc_paths
+
+
 def test_error_if_not_dir_or_file() -> None:
     with pytest.raises(ValueError, match="Directory"):
         SimpleDirectoryReader("not_a_dir")
     with pytest.raises(ValueError, match="File"):
         SimpleDirectoryReader(input_files=["not_a_file"])
     with TemporaryDirectory() as tmp_dir:
         with pytest.raises(ValueError, match="No files"):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `llama_index-0.7.8/tests/readers/test_json.py` & `llama_index-0.7.9/tests/readers/test_json.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/readers/test_mongo.py` & `llama_index-0.7.9/tests/readers/test_mongo.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/selectors/test_llm_selectors.py` & `llama_index-0.7.9/tests/selectors/test_llm_selectors.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/storage/conftest.py` & `llama_index-0.7.9/tests/storage/conftest.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/storage/docstore/test_dynamodb_docstore.py` & `llama_index-0.7.9/tests/storage/docstore/test_dynamodb_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/storage/docstore/test_mongo_docstore.py` & `llama_index-0.7.9/tests/storage/docstore/test_mongo_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/storage/docstore/test_redis_docstore.py` & `llama_index-0.7.9/tests/storage/docstore/test_redis_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/storage/docstore/test_simple_docstore.py` & `llama_index-0.7.9/tests/storage/docstore/test_simple_docstore.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/storage/test_storage_context.py` & `llama_index-0.7.9/tests/storage/test_storage_context.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/test_utils.py` & `llama_index-0.7.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/token_predictor/test_base.py` & `llama_index-0.7.9/tests/token_predictor/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/tools/test_base.py` & `llama_index-0.7.9/tests/tools/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/tools/test_ondemand_loader.py` & `llama_index-0.7.9/tests/tools/test_ondemand_loader.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/tools/test_utils.py` & `llama_index-0.7.9/tests/tools/test_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/tools/tool_spec/test_base.py` & `llama_index-0.7.9/tests/tools/tool_spec/test_base.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/vector_stores/test_docarray.py` & `llama_index-0.7.9/tests/vector_stores/test_docarray.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/vector_stores/test_postgres.py` & `llama_index-0.7.9/tests/vector_stores/test_postgres.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/vector_stores/test_qdrant.py` & `llama_index-0.7.9/tests/vector_stores/test_qdrant.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/vector_stores/test_tair.py` & `llama_index-0.7.9/tests/vector_stores/test_tair.py`

 * *Files identical despite different names*

### Comparing `llama_index-0.7.8/tests/vector_stores/test_weaviate.py` & `llama_index-0.7.9/tests/vector_stores/test_weaviate.py`

 * *Files identical despite different names*

