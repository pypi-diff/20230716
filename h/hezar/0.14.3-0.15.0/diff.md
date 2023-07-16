# Comparing `tmp/hezar-0.14.3.tar.gz` & `tmp/hezar-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hezar-0.14.3.tar", max compression
+gzip compressed data, was "hezar-0.15.0.tar", max compression
```

## Comparing `hezar-0.14.3.tar` & `hezar-0.15.0.tar`

### file list

```diff
@@ -1,77 +1,87 @@
--rw-r--r--   0        0        0     1065 2023-07-08 10:19:37.426862 hezar-0.14.3/LICENSE
--rw-r--r--   0        0        0     4427 2023-07-08 10:19:37.426862 hezar-0.14.3/README.md
--rw-r--r--   0        0        0      238 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/__init__.py
--rw-r--r--   0        0        0     4471 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/builders.py
--rw-r--r--   0        0        0    10536 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/configs.py
--rw-r--r--   0        0        0     1216 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/constants.py
--rw-r--r--   0        0        0       75 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/data/__init__.py
--rw-r--r--   0        0        0     6333 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/data/data_collators.py
--rw-r--r--   0        0        0      223 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/data/datasets/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/data/datasets/dataset.py
--rw-r--r--   0        0        0     4576 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/data/datasets/sequence_labeling_dataset.py
--rw-r--r--   0        0        0     3701 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/data/datasets/text_classification_dataset.py
--rw-r--r--   0        0        0       26 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/data/utils/__init__.py
--rw-r--r--   0        0        0     1856 2023-07-08 10:19:37.426862 hezar-0.14.3/hezar/data/utils/data_utils.py
--rw-r--r--   0        0        0      127 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/embeddings/__init__.py
--rw-r--r--   0        0        0     4124 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/embeddings/embedding.py
--rw-r--r--   0        0        0     3122 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/embeddings/fasttext.py
--rw-r--r--   0        0        0     3081 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/embeddings/word2vec.py
--rw-r--r--   0        0        0      282 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/audio_classification/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/image2text/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/image2text/crnn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/image2text/trocr/__init__.py
--rw-r--r--   0        0        0      144 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/__init__.py
--rw-r--r--   0        0        0       69 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/bert/__init__.py
--rw-r--r--   0        0        0     1136 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/bert/bert_lm.py
--rw-r--r--   0        0        0      762 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/bert/bert_lm_config.py
--rw-r--r--   0        0        0       93 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/distilbert/__init__.py
--rw-r--r--   0        0        0     1208 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/distilbert/distilbert_lm.py
--rw-r--r--   0        0        0      628 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
--rw-r--r--   0        0        0       81 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/roberta/__init__.py
--rw-r--r--   0        0        0     1172 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/roberta/roberta_lm.py
--rw-r--r--   0        0        0      822 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/language_modeling/roberta/roberta_lm_config.py
--rw-r--r--   0        0        0     9544 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/model.py
--rw-r--r--   0        0        0       67 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/sequence_labeling/__init__.py
--rw-r--r--   0        0        0      127 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/sequence_labeling/bert/__init__.py
--rw-r--r--   0        0        0     2853 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
--rw-r--r--   0        0        0      936 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/speech_recognition/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/speech_recognition/wav2vec/__init__.py
--rw-r--r--   0        0        0      240 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/__init__.py
--rw-r--r--   0        0        0      135 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/bert/__init__.py
--rw-r--r--   0        0        0     2679 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/bert/bert_text_classification.py
--rw-r--r--   0        0        0      850 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/bert/bert_text_classification_config.py
--rw-r--r--   0        0        0      159 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/distilbert/__init__.py
--rw-r--r--   0        0        0     2813 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py
--rw-r--r--   0        0        0      753 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
--rw-r--r--   0        0        0      147 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/roberta/__init__.py
--rw-r--r--   0        0        0     2943 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/roberta/roberta_text_classification.py
--rw-r--r--   0        0        0      947 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_detection/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_detection/ctpn/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_detection/dbnet/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/models/text_summarization/__init__.py
--rw-r--r--   0        0        0      104 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/normalizers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/normalizers/nfkc.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/normalizers/nfkd.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/normalizers/normalizer.py
--rw-r--r--   0        0        0     2218 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/preprocessor.py
--rw-r--r--   0        0        0      298 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/tokenizers/__init__.py
--rw-r--r--   0        0        0     4833 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/tokenizers/bpe.py
--rw-r--r--   0        0        0     5407 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
--rw-r--r--   0        0        0    18892 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/tokenizers/tokenizer.py
--rw-r--r--   0        0        0     4461 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/preprocessors/tokenizers/wordpiece.py
--rw-r--r--   0        0        0     7771 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/registry.py
--rw-r--r--   0        0        0       29 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/trainers/__init__.py
--rw-r--r--   0        0        0    14619 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/trainers/trainer.py
--rw-r--r--   0        0        0     1773 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/trainers/trainer_utils.py
--rw-r--r--   0        0        0      135 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/utils/__init__.py
--rw-r--r--   0        0        0     3468 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/utils/config_utils.py
--rw-r--r--   0        0        0      482 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/utils/context_managers.py
--rw-r--r--   0        0        0     2773 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/utils/hub_utils.py
--rw-r--r--   0        0        0      374 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/utils/logging.py
--rw-r--r--   0        0        0        0 2023-07-08 10:19:37.430863 hezar-0.14.3/hezar/utils/model_utils.py
--rw-r--r--   0        0        0     1579 2023-07-08 10:19:37.430863 hezar-0.14.3/pyproject.toml
--rw-r--r--   0        0        0     6804 1970-01-01 00:00:00.000000 hezar-0.14.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-16 06:43:10.952388 hezar-0.15.0/LICENSE
+-rw-r--r--   0        0        0     4427 2023-07-16 06:43:10.952388 hezar-0.15.0/README.md
+-rw-r--r--   0        0        0      261 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/__init__.py
+-rw-r--r--   0        0        0     5396 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/builders.py
+-rw-r--r--   0        0        0    10800 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/configs.py
+-rw-r--r--   0        0        0     1735 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/constants.py
+-rw-r--r--   0        0        0       75 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/__init__.py
+-rw-r--r--   0        0        0     6333 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/data_collators.py
+-rw-r--r--   0        0        0      223 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/datasets/__init__.py
+-rw-r--r--   0        0        0     1709 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/datasets/dataset.py
+-rw-r--r--   0        0        0     4576 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/datasets/sequence_labeling_dataset.py
+-rw-r--r--   0        0        0     3701 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/datasets/text_classification_dataset.py
+-rw-r--r--   0        0        0       26 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/utils/__init__.py
+-rw-r--r--   0        0        0     1856 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/data/utils/data_utils.py
+-rw-r--r--   0        0        0      127 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/embeddings/__init__.py
+-rw-r--r--   0        0        0     4124 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/embeddings/embedding.py
+-rw-r--r--   0        0        0     3122 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/embeddings/fasttext.py
+-rw-r--r--   0        0        0     3081 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/embeddings/word2vec.py
+-rw-r--r--   0        0        0      141 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/__init__.py
+-rw-r--r--   0        0        0     1184 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/f1.py
+-rw-r--r--   0        0        0      983 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/metric.py
+-rw-r--r--   0        0        0     1295 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/recall.py
+-rw-r--r--   0        0        0     2090 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/metrics/seqeval.py
+-rw-r--r--   0        0        0      282 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/audio_classification/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/image2text/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/image2text/crnn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/image2text/trocr/__init__.py
+-rw-r--r--   0        0        0      144 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/__init__.py
+-rw-r--r--   0        0        0       69 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/bert/__init__.py
+-rw-r--r--   0        0        0     1136 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/bert/bert_lm.py
+-rw-r--r--   0        0        0      762 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/bert/bert_lm_config.py
+-rw-r--r--   0        0        0       93 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/distilbert/__init__.py
+-rw-r--r--   0        0        0     1208 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/distilbert/distilbert_lm.py
+-rw-r--r--   0        0        0      628 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py
+-rw-r--r--   0        0        0       81 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/roberta/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/roberta/roberta_lm.py
+-rw-r--r--   0        0        0      822 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/language_modeling/roberta/roberta_lm_config.py
+-rw-r--r--   0        0        0     9544 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/model.py
+-rw-r--r--   0        0        0       67 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0      127 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/sequence_labeling/bert/__init__.py
+-rw-r--r--   0        0        0     3354 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py
+-rw-r--r--   0        0        0      936 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/speech_recognition/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/speech_recognition/wav2vec/__init__.py
+-rw-r--r--   0        0        0      240 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/__init__.py
+-rw-r--r--   0        0        0      135 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/bert/__init__.py
+-rw-r--r--   0        0        0     3082 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/bert/bert_text_classification.py
+-rw-r--r--   0        0        0      850 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/bert/bert_text_classification_config.py
+-rw-r--r--   0        0        0      159 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/distilbert/__init__.py
+-rw-r--r--   0        0        0     3217 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py
+-rw-r--r--   0        0        0      753 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py
+-rw-r--r--   0        0        0      147 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/roberta/__init__.py
+-rw-r--r--   0        0        0     3347 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/roberta/roberta_text_classification.py
+-rw-r--r--   0        0        0      947 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_detection/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_detection/ctpn/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_detection/dbnet/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/models/text_summarization/__init__.py
+-rw-r--r--   0        0        0      104 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/normalizers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/normalizers/nfkc.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/normalizers/nfkd.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/normalizers/normalizer.py
+-rw-r--r--   0        0        0     2218 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/preprocessor.py
+-rw-r--r--   0        0        0      231 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/__init__.py
+-rw-r--r--   0        0        0     4556 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/bpe.py
+-rw-r--r--   0        0        0     5045 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py
+-rw-r--r--   0        0        0    18797 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     4132 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/preprocessors/tokenizers/wordpiece.py
+-rw-r--r--   0        0        0     8898 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/registry.py
+-rw-r--r--   0        0        0      143 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/sequence_labeling/__init__.py
+-rw-r--r--   0        0        0     2538 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/sequence_labeling/sequence_labeling_trainer.py
+-rw-r--r--   0        0        0       67 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/text_classification/__init__.py
+-rw-r--r--   0        0        0     2177 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/text_classification/text_classification_trainer.py
+-rw-r--r--   0        0        0    17120 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/trainer.py
+-rw-r--r--   0        0        0     1626 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/trainers/trainer_utils.py
+-rw-r--r--   0        0        0      163 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/__init__.py
+-rw-r--r--   0        0        0      611 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/common_utils.py
+-rw-r--r--   0        0        0     3782 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/config_utils.py
+-rw-r--r--   0        0        0      482 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/context_managers.py
+-rw-r--r--   0        0        0     2773 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/hub_utils.py
+-rw-r--r--   0        0        0      374 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/logging.py
+-rw-r--r--   0        0        0        0 2023-07-16 06:43:10.956388 hezar-0.15.0/hezar/utils/model_utils.py
+-rw-r--r--   0        0        0     1626 2023-07-16 06:43:10.956388 hezar-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0     6874 1970-01-01 00:00:00.000000 hezar-0.15.0/PKG-INFO
```

### Comparing `hezar-0.14.3/LICENSE` & `hezar-0.15.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/README.md` & `hezar-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/builders.py` & `hezar-0.15.0/hezar/builders.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,38 @@
     >>> from hezar.builders import build_model
     >>> model = build_model('distilbert_text_classification', id2label={0: 'negative', 1: 'positive'})
     >>> print(model)
 
 """
 from typing import Optional
 
-from .constants import SplitType
 from .configs import (
     DatasetConfig,
     EmbeddingConfig,
+    MetricConfig,
     ModelConfig,
     PreprocessorConfig,
 )
+from .constants import SplitType
 from .registry import (  # noqa
     datasets_registry,  # noqa
     embeddings_registry,  # noqa
+    metrics_registry,  # noqa
     models_registry,  # noqa
     preprocessors_registry,  # noqa
 )
+from .utils.config_utils import snake_case
 
 
 __all__ = [
     "build_model",
     "build_dataset",
     "build_preprocessor",
     "build_embedding",
+    "build_metric"
 ]
 
 
 def build_model(name: str, config: Optional[ModelConfig] = None, **kwargs):
     """
     Build the model using its registry name. If config is None then the model is built using the default config. Notice
     that this function only builds the model and does not perform any weights loading/initialization unless these
@@ -115,7 +119,29 @@
     """
     if name not in embeddings_registry:
         raise ValueError(f"Unknown embedding name: `{name}`!\n"
                          f"Available embedding names: {list(embeddings_registry.keys())}")
     config = config or embeddings_registry[name].config_class()
     embedding = embeddings_registry[name].module_class(config, **kwargs)
     return embedding
+
+
+def build_metric(name: str, config: Optional[MetricConfig] = None, **kwargs):
+    """
+    Build the metric using its registry name. If config is None then the metric is built using the
+    default config.
+
+    Args:
+        name (str): Name of the metric in the metrics' registry
+        config (MetricConfig): A MetricConfig instance
+        **kwargs: Extra config parameters that are loaded to the metric
+
+    Returns:
+        A Dataset instance
+    """
+    if name not in metrics_registry:
+        raise ValueError(f"Unknown metric name: `{name}`!\n"
+                         f"Available metric names: {list(metrics_registry.keys())}")
+    name = snake_case(name)
+    config = config or metrics_registry[name].config_class()
+    metric = metrics_registry[name].module_class(config, **kwargs)
+    return metric
```

### Comparing `hezar-0.14.3/hezar/constants.py` & `hezar-0.15.0/hezar/constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,23 +20,49 @@
 DEFAULT_EMBEDDING_FILE = "embedding.bin"
 DEFAULT_EMBEDDING_CONFIG_FILE = "embedding_config.yaml"
 DEFAULT_EMBEDDING_SUBFOLDER = "embedding"
 
 TQDM_BAR_FORMAT = "{desc:<16}{percentage:3.0f}%|{bar:70}{r_bar}"
 
 
-class TaskType(Enum):
+class TaskType(str, Enum):
     AUDIO_CLASSIFICATION = "audio_classification"
     IMAGE2TEXT = "image2text"
     LANGUAGE_MODELING = "language_modeling"
     SEQUENCE_LABELING = "sequence_labeling"
     SPEECH_RECOGNITION = "speech_recognition"
     TEXT_CLASSIFICATION = "text_classification"
     TEXT_DETECTION = "text_detection"
     SEQ2SEQ = "seq2seq"
 
 
-class SplitType(Enum):
+class ConfigType(str, Enum):
+    BASE = "base"
+    MODEL = "model"
+    DATASET = "dataset"
+    PREPROCESSOR = "preprocessor"
+    EMBEDDING = "embedding"
+    TRAINER = "trainer"
+    OPTIMIZER = "optimizer"
+    CRITERION = "criterion"
+    LR_SCHEDULER = "lr_scheduler"
+    METRIC = "metric"
+
+
+class SplitType(str, Enum):
     TRAIN = "train"
     EVAL = "eval"
     VALID = "validation"
     TEST = "test"
+
+
+class MetricType(str, Enum):
+    ACCURACY = "accuracy"
+    F1 = "f1"
+    RECALL = "recall"
+    PRECISION = "precision"
+    SEQEVAL = "seqeval"
+
+
+class RepoType(str, Enum):
+    DATASET = "dataset"
+    MODEL = "model"
```

### Comparing `hezar-0.14.3/hezar/data/data_collators.py` & `hezar-0.15.0/hezar/data/data_collators.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/data/datasets/dataset.py` & `hezar-0.15.0/hezar/data/datasets/dataset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from typing import Optional, Union
 
 from torch.utils.data import Dataset as TorchDataset
 
 from ...configs import DatasetConfig
-from ...constants import DEFAULT_DATASET_CONFIG_FILE, SplitType
+from ...constants import DEFAULT_DATASET_CONFIG_FILE, ConfigType, RepoType, SplitType
 from ...utils import get_module_class
 
 
 class Dataset(TorchDataset):
     """
     Base class for all datasets in Hezar.
 
@@ -47,12 +47,12 @@
             **kwargs: Config parameters as keyword arguments
 
         Returns:
 
         """
         split = split or "train"
         config_filename = config_filename or cls.config_filename
-        dataset_config = DatasetConfig.load(hub_path, filename=config_filename, repo_type="dataset", **kwargs)
-        dataset_class = get_module_class(dataset_config.name, module_type="dataset")
+        dataset_config = DatasetConfig.load(hub_path, filename=config_filename, repo_type=RepoType.DATASET, **kwargs)
+        dataset_class = get_module_class(dataset_config.name, module_type=ConfigType.DATASET)
         dataset_config.path = hub_path
         dataset = dataset_class(dataset_config, split=split)
         return dataset
```

### Comparing `hezar-0.14.3/hezar/data/datasets/sequence_labeling_dataset.py` & `hezar-0.15.0/hezar/data/datasets/sequence_labeling_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/data/datasets/text_classification_dataset.py` & `hezar-0.15.0/hezar/data/datasets/text_classification_dataset.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/data/utils/data_utils.py` & `hezar-0.15.0/hezar/data/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/embeddings/embedding.py` & `hezar-0.15.0/hezar/embeddings/embedding.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/embeddings/fasttext.py` & `hezar-0.15.0/hezar/embeddings/fasttext.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/embeddings/word2vec.py` & `hezar-0.15.0/hezar/embeddings/word2vec.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/language_modeling/bert/bert_lm.py` & `hezar-0.15.0/hezar/models/language_modeling/bert/bert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/language_modeling/bert/bert_lm_config.py` & `hezar-0.15.0/hezar/models/language_modeling/bert/bert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/language_modeling/distilbert/distilbert_lm.py` & `hezar-0.15.0/hezar/models/language_modeling/distilbert/distilbert_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/language_modeling/distilbert/distilbert_lm_config.py` & `hezar-0.15.0/hezar/models/language_modeling/distilbert/distilbert_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/language_modeling/roberta/roberta_lm.py` & `hezar-0.15.0/hezar/models/language_modeling/roberta/roberta_lm.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/language_modeling/roberta/roberta_lm_config.py` & `hezar-0.15.0/hezar/models/language_modeling/roberta/roberta_lm_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/model.py` & `hezar-0.15.0/hezar/models/model.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling.py` & `hezar-0.15.0/hezar/models/text_classification/distilbert/distilbert_text_classification.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,78 @@
 """
-A BERT model for sequence labeling built using HuggingFace Transformers
+A DistilBERT model for text classification built using HuggingFace Transformers
 """
 from typing import Dict
 
 from torch import nn
-from transformers import BertConfig, BertModel
+from transformers import DistilBertConfig, DistilBertModel
 
 from ....models import Model
 from ....registry import register_model
-from .bert_sequence_labeling_config import BertSequenceLabelingConfig
+from .distilbert_text_classification_config import DistilBertTextClassificationConfig
 
 
-@register_model("bert_sequence_labeling", BertSequenceLabelingConfig)
-class BertSequenceLabeling(Model):
-    def __init__(self, config: BertSequenceLabelingConfig, **kwargs):
+@register_model(model_name="distilbert_text_classification", config_class=DistilBertTextClassificationConfig)
+class DistilBertTextClassification(Model):
+    """
+    A standard 🤗Transformers DistilBert model for text classification
+
+    Args:
+        config: The whole model config including arguments needed for the inner 🤗Transformers model.
+    """
+
+    def __init__(self, config: DistilBertTextClassificationConfig, **kwargs):
         super().__init__(config, **kwargs)
-        self.bert = BertModel(self._build_inner_config())
-        classifier_dropout = (
-            config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
-        )
-        self.dropout = nn.Dropout(classifier_dropout)
-        self.classifier = nn.Linear(config.hidden_size, config.num_labels)
+        self.distilbert = DistilBertModel(self._build_inner_config())
+        self.pre_classifier = nn.Linear(self.config.dim, self.config.dim)
+        self.classifier = nn.Linear(self.config.dim, self.config.num_labels)
+        self.dropout = nn.Dropout(self.config.seq_classif_dropout)
 
     def _build_inner_config(self):
         if self.config.num_labels is None and self.config.id2label is None:
             raise ValueError("Both `num_labels` and `id2label` are None. Please provide at least one of them!")
         if self.config.id2label and self.config.num_labels is None:
             self.config.num_labels = len(self.config.id2label)
-        bert_config = BertConfig(**self.config)
+        bert_config = DistilBertConfig(**self.config)
         return bert_config
 
     def forward(self, inputs, **kwargs) -> Dict:
         input_ids = inputs.get("token_ids")
-        labels = inputs.get("labels")
-
-        lm_outputs = self.bert(input_ids=input_ids, **kwargs)
-        sequence_output = lm_outputs[0]
-
-        sequence_output = self.dropout(sequence_output)
-        logits = self.classifier(sequence_output)
-
-        loss = None
-        if labels is not None:
-            criterion = nn.CrossEntropyLoss()
-            loss = criterion(logits.view(-1, self.config.num_labels), labels.view(-1))
+        attention_mask = inputs.get("attention_mask", None)
+        head_mask = inputs.get("head_mask", None)
+        inputs_embeds = inputs.get("inputs_embeds", None)
+        output_attentions = inputs.get("output_attentions", None)
+        output_hidden_states = inputs.get("output_hidden_states", None)
+
+        lm_outputs = self.distilbert(
+            input_ids,
+            attention_mask=attention_mask,
+            head_mask=head_mask,
+            inputs_embeds=inputs_embeds,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            **kwargs,
+        )
+        hidden_state = lm_outputs[0]
+        pooled_output = hidden_state[:, 0]
+        pooled_output = self.pre_classifier(pooled_output)
+        pooled_output = nn.ReLU()(pooled_output)
+        pooled_output = self.dropout(pooled_output)
+        logits = self.classifier(pooled_output)
 
         outputs = {
-            "loss": loss,
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
-            **inputs
         }
         return outputs
 
-    def post_process(self, inputs, **kwargs):
-        # TODO sequence labeling outputs should consider rejoining split words into single words with proper tag
+    def post_process(self, inputs, **kwargs) -> Dict:
         logits = inputs["logits"]
-        tokens = inputs["tokens"]
-        word_ids = inputs["word_ids"]  # noqa
-        predictions = logits.argmax(2).cpu()
-        predictions = [[self.config.id2label[p.item()] for p in prediction] for prediction in predictions]
-        outputs = []
-        for tokens_list, prediction in zip(tokens, predictions):
-            results = []
-            for token, tag in zip(tokens_list, prediction):
-                if token not in self.config.prediction_skip_tokens:
-                    results.append({"token": token, "tag": tag})
-            outputs.append(results)
+        predictions = logits.argmax(1)
+        predictions_probs = logits.softmax(1).max(1)
+        outputs = {"labels": [], "probs": []}
+        for prediction, prob in zip(predictions, predictions_probs):
+            label = self.config.id2label[prediction.item()]
+            outputs["labels"].append(label)
+            outputs["probs"].append(prob.item())
         return outputs
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hezar-0.14.3/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py` & `hezar-0.15.0/hezar/models/sequence_labeling/bert/bert_sequence_labeling_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/text_classification/bert/bert_text_classification.py` & `hezar-0.15.0/hezar/models/text_classification/bert/bert_text_classification.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,23 +36,33 @@
         if self.config.id2label and self.config.num_labels is None:
             self.config.num_labels = len(self.config.id2label)
         bert_config = BertConfig(**self.config)
         return bert_config
 
     def forward(self, inputs, **kwargs) -> Dict:
         input_ids = inputs.get("token_ids")
-        labels = inputs.get("labels")
+        attention_mask = inputs.get("attention_mask", None)
+        head_mask = inputs.get("head_mask", None)
+        inputs_embeds = inputs.get("inputs_embeds", None)
+        output_attentions = inputs.get("output_attentions", None)
+        output_hidden_states = inputs.get("output_hidden_states", None)
 
-        lm_outputs = self.bert(input_ids=input_ids, **kwargs)
+        lm_outputs = self.bert(
+            input_ids,
+            attention_mask=attention_mask,
+            head_mask=head_mask,
+            inputs_embeds=inputs_embeds,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            **kwargs,
+        )
         pooled_output = lm_outputs[1]
         pooled_output = self.dropout(pooled_output)
         logits = self.classifier(pooled_output)
-        loss = nn.CrossEntropyLoss()(logits, labels) if labels is not None else None
         outputs = {
-            "loss": loss,
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
         }
         return outputs
 
     def post_process(self, inputs, **kwargs) -> Dict:
```

### Comparing `hezar-0.14.3/hezar/models/text_classification/bert/bert_text_classification_config.py` & `hezar-0.15.0/hezar/models/text_classification/bert/bert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/text_classification/distilbert/distilbert_text_classification.py` & `hezar-0.15.0/hezar/models/text_classification/roberta/roberta_text_classification.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,85 @@
 """
-A DistilBERT model for text classification built using HuggingFace Transformers
+A RoBERTa Language Model (HuggingFace Transformers) wrapped by a Hezar Model class
 """
-from typing import Dict
-
-from torch import nn
-from transformers import DistilBertConfig, DistilBertModel
+from torch import nn, tanh
+from transformers import RobertaConfig, RobertaModel
 
 from ....models import Model
 from ....registry import register_model
-from .distilbert_text_classification_config import DistilBertTextClassificationConfig
+from .roberta_text_classification_config import RobertaTextClassificationConfig
 
 
-@register_model(model_name="distilbert_text_classification", config_class=DistilBertTextClassificationConfig)
-class DistilBertTextClassification(Model):
-    """
-    A standard 🤗Transformers DistilBert model for text classification
-
-    Args:
-        config: The whole model config including arguments needed for the inner 🤗Transformers model.
-    """
-
-    def __init__(self, config: DistilBertTextClassificationConfig, **kwargs):
-        super().__init__(config, **kwargs)
-        self.distilbert = DistilBertModel(self._build_inner_config())
-        self.pre_classifier = nn.Linear(self.config.dim, self.config.dim)
-        self.classifier = nn.Linear(self.config.dim, self.config.num_labels)
-        self.dropout = nn.Dropout(self.config.seq_classif_dropout)
+@register_model("roberta_text_classification", config_class=RobertaTextClassificationConfig)
+class RobertaTextClassification(Model):
+    def __init__(self, config, **kwargs):
+        super().__init__(config=config, **kwargs)
+        self.roberta = RobertaModel(self._build_inner_config(), add_pooling_layer=False)
+        self.classifier = RobertaClassificationHead(self.config)
 
     def _build_inner_config(self):
         if self.config.num_labels is None and self.config.id2label is None:
             raise ValueError("Both `num_labels` and `id2label` are None. Please provide at least one of them!")
         if self.config.id2label and self.config.num_labels is None:
             self.config.num_labels = len(self.config.id2label)
-        bert_config = DistilBertConfig(**self.config)
+        bert_config = RobertaConfig(**self.config)
         return bert_config
 
-    def forward(self, inputs, **kwargs) -> Dict:
+    def forward(self, inputs, **kwargs):
         input_ids = inputs.get("token_ids")
-        labels = inputs.get("labels")
+        attention_mask = inputs.get("attention_mask", None)
+        head_mask = inputs.get("head_mask", None)
+        inputs_embeds = inputs.get("inputs_embeds", None)
+        output_attentions = inputs.get("output_attentions", None)
+        output_hidden_states = inputs.get("output_hidden_states", None)
+
+        lm_outputs = self.roberta(
+            input_ids,
+            attention_mask=attention_mask,
+            head_mask=head_mask,
+            inputs_embeds=inputs_embeds,
+            output_attentions=output_attentions,
+            output_hidden_states=output_hidden_states,
+            **kwargs,
+        )
+        sequence_output = lm_outputs[0]
+        logits = self.classifier(sequence_output)
 
-        lm_outputs = self.distilbert(input_ids=input_ids, **kwargs)
-        hidden_state = lm_outputs[0]
-        pooled_output = hidden_state[:, 0]
-        pooled_output = self.pre_classifier(pooled_output)
-        pooled_output = nn.ReLU()(pooled_output)
-        pooled_output = self.dropout(pooled_output)
-        logits = self.classifier(pooled_output)
-        loss = nn.CrossEntropyLoss()(logits, labels) if labels is not None else None
         outputs = {
-            "loss": loss,
             "logits": logits,
             "hidden_states": lm_outputs.hidden_states,
             "attentions": lm_outputs.attentions,
         }
         return outputs
 
-    def post_process(self, inputs, **kwargs) -> Dict:
+    def post_process(self, inputs, **kwargs):
         logits = inputs["logits"]
         predictions = logits.argmax(1)
         predictions_probs = logits.softmax(1).max(1)
         outputs = {"labels": [], "probs": []}
         for prediction, prob in zip(predictions, predictions_probs):
             label = self.config.id2label[prediction.item()]
             outputs["labels"].append(label)
             outputs["probs"].append(prob.item())
         return outputs
+
+
+class RobertaClassificationHead(nn.Module):
+    """Head for sentence-level classification tasks."""
+
+    def __init__(self, config):
+        super().__init__()
+        self.dense = nn.Linear(config.hidden_size, config.hidden_size)
+        classifier_dropout = (
+            config.classifier_dropout if config.classifier_dropout is not None else config.hidden_dropout_prob
+        )
+        self.dropout = nn.Dropout(classifier_dropout)
+        self.out_proj = nn.Linear(config.hidden_size, config.num_labels)
+
+    def forward(self, inputs, **kwargs):
+        x = inputs[:, 0, :]  # take <s> token (equiv. to [CLS])
+        x = self.dropout(x)
+        x = self.dense(x)
+        x = tanh(x)
+        x = self.dropout(x)
+        x = self.out_proj(x)
+        return x
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hezar-0.14.3/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py` & `hezar-0.15.0/hezar/models/text_classification/distilbert/distilbert_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/models/text_classification/roberta/roberta_text_classification_config.py` & `hezar-0.15.0/hezar/models/text_classification/roberta/roberta_text_classification_config.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/preprocessors/preprocessor.py` & `hezar-0.15.0/hezar/preprocessors/preprocessor.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/hezar/preprocessors/tokenizers/bpe.py` & `hezar-0.15.0/hezar/preprocessors/tokenizers/sentencepiece_bpe.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 import os
 from dataclasses import dataclass, field
 from typing import List
 
 from huggingface_hub import hf_hub_download
 from tokenizers import Tokenizer as HFTokenizer
-from tokenizers import decoders, models, pre_tokenizers, trainers
+from tokenizers import decoders, models, normalizers, pre_tokenizers, trainers
 
 from ...constants import DEFAULT_TOKENIZER_CONFIG_FILE, DEFAULT_TOKENIZER_FILE, HEZAR_CACHE_DIR
 from ...registry import register_preprocessor
-from .tokenizer import Tokenizer, TokenizerConfig, TokenizerTrainConfig
+from .tokenizer import Tokenizer, TokenizerConfig
 
 
 @dataclass
-class BPETrainConfig(TokenizerTrainConfig):
-    name: str = "bpe_tokenizer"
-    vocab_size: int = 30000
-    min_frequency: int = 2
-    limit_alphabet: int = 1000
-    initial_alphabet: list = field(default_factory=list)
-    show_progress: bool = True
-
-
-@dataclass
-class BPEConfig(TokenizerConfig):
-    name: str = "bpe_tokenizer"
+class SentencePieceBPEConfig(TokenizerConfig):
+    name: str = "sentencepiece_bpe_tokenizer"
     max_length: int = 512
     truncation_strategy: str = "longest_first"
     truncation_direction: str = "right"
     stride: int = 0
     padding_strategy: str = "longest"
     padding_direction: str = "right"
     special_tokens: List[str] = field(
@@ -48,23 +38,29 @@
     unk_token: str = "<unk>"
     pad_token_id: int = 0
     pad_token_type_id: int = 0
     pad_token: str = "<pad>"
     pad_to_multiple_of: int = 0
     dropout: float = None
     continuing_subword_prefix: str = ""
+    replacement: str = "_"
+    add_prefix_space: bool = True
     end_of_word_suffix: str = ""
     fuse_unk: bool = False
-    train_config: BPETrainConfig = None
+    vocab_size: int = 30000
+    min_frequency: int = 2
+    limit_alphabet: int = 1000
+    initial_alphabet: list = field(default_factory=list)
+    show_progress: bool = True
 
 
-@register_preprocessor("bpe_tokenizer", config_class=BPEConfig)
-class BPETokenizer(Tokenizer):
+@register_preprocessor("sentencepiece_bpe_tokenizer", config_class=SentencePieceBPEConfig)
+class SentencePieceBPETokenizer(Tokenizer):
     """
-    A standard Byte-level BPE tokenizer using 🤗HuggingFace Tokenizers
+    A standard SentencePiece BPE tokenizer using 🤗HuggingFace Tokenizers
 
     Args:
         config: Preprocessor config for the tokenizer
         **kwargs: Extra/manual config parameters
     """
 
     tokenizer_filename = DEFAULT_TOKENIZER_FILE
@@ -99,40 +95,44 @@
                     unk_token=self.config.unk_token,
                     continuing_subword_prefix=self.config.continuing_subword_prefix,
                     end_of_word_suffix=self.config.end_of_word_suffix,
                     fuse_unk=self.config.fuse_unk,
                 )
             )
             tokenizer.add_special_tokens(self.config.special_tokens)
-            tokenizer.decoder = decoders.ByteLevel()  # noqa
+            tokenizer.normalizer = normalizers.NFKC()  # noqa
+            tokenizer.pre_tokenizer = pre_tokenizers.Metaspace(  # noqa
+                replacement=self.config.replacement, add_prefix_space=self.config.add_prefix_space
+            )
+            tokenizer.decoder = decoders.Metaspace(  # noqa
+                replacement=self.config.replacement, add_prefix_space=self.config.add_prefix_space
+            )
 
         return tokenizer
 
     def train(self, files: List[str], **train_kwargs):
         """Train the model using the given files"""
-        train_config = self.config.train_config or BPETrainConfig()
-        train_config.update(train_kwargs)
+        self.config.update(train_kwargs)
 
         trainer = trainers.BpeTrainer(
-            vocab_size=config.vocab_size,  # noqa
-            min_frequency=config.min_frequency,  # noqa
-            show_progress=config.show_progress,  # noqa
+            vocab_size=self.config.vocab_size,  # noqa
+            min_frequency=self.config.min_frequency,  # noqa
+            show_progress=self.config.show_progress,  # noqa
             special_tokens=self.config.special_tokens,  # noqa
-            initial_alphabet=pre_tokenizers.ByteLevel.alphabet(),  # noqa
+            initial_alphabet=self.config.initial_alphabet,  # noqa
         )
         if isinstance(files, str):
             files = [files]
         self._tokenizer.train(files, trainer=trainer)
 
     def train_from_iterator(self, dataset: List[str], **train_kwargs):
         """Train the model using the given files"""
-        train_config = self.config.train_config or BPETrainConfig()
-        train_config.update(train_kwargs)
+        self.config.update(train_kwargs)
 
         trainer = trainers.BpeTrainer(
-            vocab_size=train_config.vocab_size,  # noqa
-            min_frequency=train_config.min_frequency,  # noqa
-            show_progress=train_config.show_progress,  # noqa
+            vocab_size=self.config.vocab_size,  # noqa
+            min_frequency=self.config.min_frequency,  # noqa
+            show_progress=self.config.show_progress,  # noqa
             special_tokens=self.config.special_tokens,  # noqa
-            initial_alphabet=pre_tokenizers.ByteLevel.alphabet(),  # noqa
+            initial_alphabet=self.config.initial_alphabet,  # noqa
         )
         self._tokenizer.train_from_iterator(dataset, trainer=trainer, length=len(dataset))
```

### Comparing `hezar-0.14.3/hezar/preprocessors/tokenizers/sentencepiece_bpe.py` & `hezar-0.15.0/hezar/preprocessors/tokenizers/bpe.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 import os
 from dataclasses import dataclass, field
 from typing import List
 
 from huggingface_hub import hf_hub_download
 from tokenizers import Tokenizer as HFTokenizer
-from tokenizers import decoders, models, normalizers, pre_tokenizers, trainers
+from tokenizers import decoders, models, pre_tokenizers, trainers
 
 from ...constants import DEFAULT_TOKENIZER_CONFIG_FILE, DEFAULT_TOKENIZER_FILE, HEZAR_CACHE_DIR
 from ...registry import register_preprocessor
-from .tokenizer import Tokenizer, TokenizerConfig, TokenizerTrainConfig
+from .tokenizer import Tokenizer, TokenizerConfig
 
 
 @dataclass
-class SentencePieceBPETrainConfig(TokenizerTrainConfig):
-    name: str = "sentencepiece_bpe_tokenizer"
-    vocab_size: int = 30000
-    min_frequency: int = 2
-    limit_alphabet: int = 1000
-    initial_alphabet: list = field(default_factory=list)
-    show_progress: bool = True
-
-
-@dataclass
-class SentencePieceBPEConfig(TokenizerConfig):
-    name: str = "sentencepiece_bpe_tokenizer"
+class BPEConfig(TokenizerConfig):
+    name: str = "bpe_tokenizer"
     max_length: int = 512
     truncation_strategy: str = "longest_first"
     truncation_direction: str = "right"
     stride: int = 0
     padding_strategy: str = "longest"
     padding_direction: str = "right"
     special_tokens: List[str] = field(
@@ -48,25 +38,27 @@
     unk_token: str = "<unk>"
     pad_token_id: int = 0
     pad_token_type_id: int = 0
     pad_token: str = "<pad>"
     pad_to_multiple_of: int = 0
     dropout: float = None
     continuing_subword_prefix: str = ""
-    replacement: str = "_"
-    add_prefix_space: bool = True
     end_of_word_suffix: str = ""
     fuse_unk: bool = False
-    train_config: SentencePieceBPETrainConfig = None
+    vocab_size: int = 30000
+    min_frequency: int = 2
+    limit_alphabet: int = 1000
+    initial_alphabet: list = field(default_factory=list)
+    show_progress: bool = True
 
 
-@register_preprocessor("sentencepiece_bpe_tokenizer", config_class=SentencePieceBPEConfig)
-class SentencePieceBPETokenizer(Tokenizer):
+@register_preprocessor("bpe_tokenizer", config_class=BPEConfig)
+class BPETokenizer(Tokenizer):
     """
-    A standard SentencePiece BPE tokenizer using 🤗HuggingFace Tokenizers
+    A standard Byte-level BPE tokenizer using 🤗HuggingFace Tokenizers
 
     Args:
         config: Preprocessor config for the tokenizer
         **kwargs: Extra/manual config parameters
     """
 
     tokenizer_filename = DEFAULT_TOKENIZER_FILE
@@ -101,46 +93,38 @@
                     unk_token=self.config.unk_token,
                     continuing_subword_prefix=self.config.continuing_subword_prefix,
                     end_of_word_suffix=self.config.end_of_word_suffix,
                     fuse_unk=self.config.fuse_unk,
                 )
             )
             tokenizer.add_special_tokens(self.config.special_tokens)
-            tokenizer.normalizer = normalizers.NFKC()  # noqa
-            tokenizer.pre_tokenizer = pre_tokenizers.Metaspace(  # noqa
-                replacement=self.config.replacement, add_prefix_space=self.config.add_prefix_space
-            )
-            tokenizer.decoder = decoders.Metaspace(  # noqa
-                replacement=self.config.replacement, add_prefix_space=self.config.add_prefix_space
-            )
+            tokenizer.decoder = decoders.ByteLevel()  # noqa
 
         return tokenizer
 
     def train(self, files: List[str], **train_kwargs):
         """Train the model using the given files"""
-        train_config = self.config.train_config or SentencePieceBPETrainConfig()
-        train_config.update(train_kwargs)
+        self.config.update(train_kwargs)
 
         trainer = trainers.BpeTrainer(
-            vocab_size=train_config.vocab_size,  # noqa
-            min_frequency=train_config.min_frequency,  # noqa
-            show_progress=train_config.show_progress,  # noqa
+            vocab_size=self.config.vocab_size,  # noqa
+            min_frequency=self.config.min_frequency,  # noqa
+            show_progress=self.config.show_progress,  # noqa
             special_tokens=self.config.special_tokens,  # noqa
-            initial_alphabet=self.config.initial_alphabet,  # noqa
+            initial_alphabet=pre_tokenizers.ByteLevel.alphabet(),  # noqa
         )
         if isinstance(files, str):
             files = [files]
         self._tokenizer.train(files, trainer=trainer)
 
     def train_from_iterator(self, dataset: List[str], **train_kwargs):
         """Train the model using the given files"""
-        train_config = self.config.train_config or SentencePieceBPETrainConfig()
-        train_config.update(train_kwargs)
+        self.config.update(train_kwargs)
 
         trainer = trainers.BpeTrainer(
-            vocab_size=train_config.vocab_size,  # noqa
-            min_frequency=train_config.min_frequency,  # noqa
-            show_progress=train_config.show_progress,  # noqa
+            vocab_size=self.config.vocab_size,  # noqa
+            min_frequency=self.config.min_frequency,  # noqa
+            show_progress=self.config.show_progress,  # noqa
             special_tokens=self.config.special_tokens,  # noqa
-            initial_alphabet=train_config.initial_alphabet,  # noqa
+            initial_alphabet=pre_tokenizers.ByteLevel.alphabet(),  # noqa
         )
         self._tokenizer.train_from_iterator(dataset, trainer=trainer, length=len(dataset))
```

### Comparing `hezar-0.14.3/hezar/preprocessors/tokenizers/tokenizer.py` & `hezar-0.15.0/hezar/preprocessors/tokenizers/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import torch
 from huggingface_hub import create_repo, upload_file
 from tokenizers import Tokenizer as HFTokenizer
 from tokenizers.decoders import Decoder
 from tokenizers.models import Model
 
 from ...builders import build_preprocessor
-from ...configs import Config, PreprocessorConfig
+from ...configs import PreprocessorConfig
 from ...constants import DEFAULT_TOKENIZER_CONFIG_FILE, DEFAULT_TOKENIZER_FILE
 from ...data.utils import convert_batch_dict_dtype
 from ...utils import get_logger
 from ..preprocessor import Preprocessor
 
 
 logger = get_logger(__name__)
@@ -34,19 +34,14 @@
     pad_to_multiple_of: int = None
     pad_token_id: int = None
     pad_token: str = None
     pad_token_type_id: int = None
     unk_token: str = None
 
 
-@dataclass
-class TokenizerTrainConfig(Config):
-    config_type: str = "preprocessor"
-
-
 class Tokenizer(Preprocessor):
     """
     Base tokenizer class. Mostly copied from :class: ~tokenizers.implementations.BaseTokenizer
 
     Args:
         config: A TokenizerConfig instance
         **kwargs: Extra config parameters that merge into the main config
```

### Comparing `hezar-0.14.3/hezar/preprocessors/tokenizers/wordpiece.py` & `hezar-0.15.0/hezar/preprocessors/tokenizers/wordpiece.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,25 +4,15 @@
 
 from huggingface_hub import hf_hub_download
 from tokenizers import Tokenizer as HFTokenizer
 from tokenizers import decoders, models, trainers
 
 from ...constants import DEFAULT_TOKENIZER_CONFIG_FILE, DEFAULT_TOKENIZER_FILE, HEZAR_CACHE_DIR
 from ...registry import register_preprocessor
-from .tokenizer import Tokenizer, TokenizerConfig, TokenizerTrainConfig
-
-
-@dataclass
-class WordPieceTrainConfig(TokenizerTrainConfig):
-    name: str = "wordpiece_tokenizer"
-    vocab_size: int = 30000
-    min_frequency: int = 2
-    limit_alphabet: int = 1000
-    initial_alphabet: list = field(default_factory=list)
-    show_progress: bool = True
+from .tokenizer import Tokenizer, TokenizerConfig
 
 
 @dataclass
 class WordPieceConfig(TokenizerConfig):
     name: str = "wordpiece_tokenizer"
     max_length: int = 512
     truncation_strategy: str = "longest_first"
@@ -33,15 +23,19 @@
     pad_to_multiple_of: int = 0
     pad_token_id: int = 0
     pad_token: str = "[PAD]"
     pad_token_type_id: int = 0
     special_tokens: List[str] = field(default_factory=lambda: ["[UNK]", "[SEP]", "[CLS]", "[PAD]", "[MASK]"])
     unk_token: str = "[UNK]"
     wordpieces_prefix: str = "##"
-    train_config: WordPieceTrainConfig = None
+    vocab_size: int = 30000
+    min_frequency: int = 2
+    limit_alphabet: int = 1000
+    initial_alphabet: list = field(default_factory=list)
+    show_progress: bool = True
 
 
 @register_preprocessor("wordpiece_tokenizer", config_class=WordPieceConfig)
 class WordPieceTokenizer(Tokenizer):
     """
     A standard WordPiece tokenizer using 🤗HuggingFace Tokenizers
 
@@ -80,38 +74,36 @@
             tokenizer.add_special_tokens(self.config.special_tokens)
             tokenizer.decoder = decoders.WordPiece(self.config.wordpieces_prefix)  # noqa
 
         return tokenizer
 
     def train(self, files: List[str], **train_kwargs):
         """Train the model using the given files"""
-        train_config = self.config.train_config or WordPieceTrainConfig()
-        train_config.update(train_kwargs)
+        self.config.update(train_kwargs)
 
         trainer = trainers.WordPieceTrainer(
-            vocab_size=train_config.vocab_size,
-            min_frequency=train_config.min_frequency,
-            limit_alphabet=train_config.limit_alphabet,
-            initial_alphabet=train_config.initial_alphabet,
+            vocab_size=self.config.vocab_size,
+            min_frequency=self.config.min_frequency,
+            limit_alphabet=self.config.limit_alphabet,
+            initial_alphabet=self.config.initial_alphabet,
             special_tokens=self.config.special_tokens,
-            show_progress=train_config.show_progress,
+            show_progress=self.config.show_progress,
             continuing_subword_prefix=self.config.wordpieces_prefix,
         )
         if isinstance(files, str):
             files = [files]
         self._tokenizer.train(files, trainer=trainer)
 
     def train_from_iterator(self, dataset: List[str], **train_kwargs):
         """Train the model using the given files"""
-        train_config = self.config.train_config or WordPieceTrainConfig()
-        train_config.update(train_kwargs)
+        self.config.update(train_kwargs)
 
         trainer = trainers.WordPieceTrainer(
-            vocab_size=train_config.vocab_size,
-            min_frequency=train_config.min_frequency,
-            limit_alphabet=train_config.limit_alphabet,
-            initial_alphabet=train_config.initial_alphabet,
+            vocab_size=self.config.vocab_size,
+            min_frequency=self.config.min_frequency,
+            limit_alphabet=self.config.limit_alphabet,
+            initial_alphabet=self.config.initial_alphabet,
             special_tokens=self.config.special_tokens,
-            show_progress=train_config.show_progress,
+            show_progress=self.config.show_progress,
             continuing_subword_prefix=self.config.wordpieces_prefix,
         )
         self._tokenizer.train_from_iterator(dataset, trainer=trainer, length=len(dataset))
```

### Comparing `hezar-0.14.3/hezar/registry.py` & `hezar-0.15.0/hezar/registry.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,41 +21,44 @@
 Keep in mind that registries usually don't need to be used directly. There is a bunch of functions to build modules
 using a module's registry name in `hezar.builders` module. See the file `builders.py` for more info.
 
 Note: In case of adding a new registry container, make sure to add to `__all__` below!
 """
 
 from dataclasses import dataclass
-from typing import Dict, Type
+from typing import Dict, Optional, Type
 
-from .configs import DatasetConfig, EmbeddingConfig, ModelConfig, PreprocessorConfig, TrainConfig
+from .configs import DatasetConfig, EmbeddingConfig, MetricConfig, ModelConfig, PreprocessorConfig, TrainerConfig
 from .utils import get_logger
 
 
 __all__ = [
     "register_model",
     "register_preprocessor",
     "register_dataset",
     "register_embedding",
+    "register_metric",
+    "register_trainer",
 ]
 
 logger = get_logger(__name__)
 
 
 @dataclass
 class Registry:
     module_class: type
-    config_class: type
-    doc: str = None
+    config_class: type = None
+    doc: Optional[str] = None
 
 
 models_registry: Dict[str, Registry] = {}
 preprocessors_registry: Dict[str, Registry] = {}
 datasets_registry: Dict[str, Registry] = {}
 embeddings_registry: Dict[str, Registry] = {}
+metrics_registry: Dict[str, Registry] = {}
 trainers_registry: Dict[str, Registry] = {}
 
 
 def register_model(model_name: str, config_class: Type[ModelConfig]):
     """
     A class decorator that adds the model class and the config class to the `models_registry`
 
@@ -63,14 +66,15 @@
         model_name: Model's registry name e.g, `bert_sequence_labeling`
         config_class: Model's config class e.g, `BertSequenceLabelingConfig`. This parameter must be the config class
             itself not a config instance!
 
     Returns:
          The class itself
     """
+
     def register(cls):
         if model_name in models_registry:
             logger.warning(f"Model `{model_name}` is already registered. Overwriting...")
 
         if config_class.name != model_name:
             raise ValueError(f"`model_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"model_name: {model_name}\n"
@@ -95,14 +99,15 @@
         dataset_name: Dataset's registry name e.g, `text_classification`.
         config_class: Dataset's config class e.g, `TextClassificationDatasetConfig`. This parameter must be the config
             class itself not a config instance!
 
     Returns:
          The class itself
     """
+
     def register(cls):
         if dataset_name in datasets_registry:
             logger.warning(f"Dataset `{dataset_name}` is already registered. Overwriting...")
 
         if config_class.name != dataset_name:
             raise ValueError(f"`dataset_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"dataset_name: {dataset_name}\n"
@@ -127,14 +132,15 @@
         preprocessor_name: Preprocessor's registry name e.g, `bpe_tokenizer`.
         config_class: Preprocessor's config class e.g, BPEConfig. This parameter must be the config
             class itself not a config instance!
 
     Returns:
          The class itself
     """
+
     def register(cls):
         if preprocessor_name in preprocessors_registry:
             logger.warning(f"Preprocessor `{preprocessor_name}` is already registered. Overwriting...")
 
         if config_class.name != preprocessor_name:
             raise ValueError(f"`preprocessor_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"preprocessor_name: {preprocessor_name}\n"
@@ -159,14 +165,15 @@
         embedding_name: Embedding's registry name e.g, `word2vec_cbow`.
         config_class: Embedding's config class e.g, Word2VecCBOWConfig. This parameter must be the config
             class itself not a config instance!
 
     Returns:
          The class itself
     """
+
     def register(cls):
         if embedding_name in embeddings_registry:
             logger.warning(f"Embedding `{embedding_name}` is already registered. Overwriting...")
 
         if config_class.name != embedding_name:
             raise ValueError(f"`embedding_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"embedding_name: {embedding_name}\n"
@@ -179,26 +186,27 @@
         )
 
         return cls
 
     return register
 
 
-def register_trainer(trainer_name: str, config_class: Type[TrainConfig]):
+def register_trainer(trainer_name: str, config_class: Type[TrainerConfig]):
     """
     A class decorator that adds the Trainer class and the config class to the `trainers_registry`
 
     Args:
         trainer_name: Trainer's registry name e.g, `text_classification_trainer`
         config_class: Trainer's config class e.g, `TextClassificationTrainerConfig`.
             This parameter must be the config class itself not a config instance!
 
     Returns:
          The class itself
     """
+
     def register(cls):
         if trainer_name in trainers_registry:
             logger.warning(f"Trainer `{trainer_name}` is already registered. Overwriting...")
 
         if config_class.name != trainer_name:
             raise ValueError(f"`trainer_name` and `config.name` are not compatible for `{cls.__name__}`\n"
                              f"trainer_name: {trainer_name}\n"
@@ -209,7 +217,39 @@
             config_class=config_class,
             doc=cls.__doc__
         )
 
         return cls
 
     return register
+
+
+def register_metric(metric_name: str, config_class: Type[MetricConfig]):
+    """
+    A class decorator that adds the metric class and the config class to the `metrics_registry`
+
+    Args:
+        metric_name: Metric registry name e.g, `f1`
+        config_class: Metric config class
+
+    Returns:
+         The class itself
+    """
+
+    def register(cls):
+        if metric_name in metrics_registry:
+            logger.warning(f"Metric `{metric_name}` is already registered. Overwriting...")
+        if config_class.name != metric_name:
+            raise ValueError(f"`metric_name` and `config.name` are not compatible for `{cls.__name__}`\n"
+                             f"metric_name: {metric_name}\n"
+                             f"{config_class.__name__}.name: {config_class.name}")
+
+        metrics_registry[metric_name] = Registry(
+            module_class=cls,
+            config_class=config_class,
+            doc=cls.__doc__
+        )
+
+        return cls
+
+    return register
+
```

### Comparing `hezar-0.14.3/hezar/trainers/trainer.py` & `hezar-0.15.0/hezar/trainers/trainer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,36 @@
 import os
 import random
 import tempfile
-from typing import Dict, Optional, Union
+from typing import Any, Dict, Tuple
 
 import numpy as np
-from huggingface_hub import create_repo, hf_hub_download, upload_folder
 import torch
+from huggingface_hub import create_repo, hf_hub_download, upload_folder
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
-from torchmetrics import Accuracy, F1Score, Precision
 from tqdm import tqdm
 
-from ..configs import LRSchedulerConfig, OptimizerConfig, TrainConfig
+from ..builders import build_metric
+from ..configs import LRSchedulerConfig, MetricConfig, OptimizerConfig, TrainerConfig
 from ..constants import (
     DEFAULT_DATASET_CONFIG_FILE,
     DEFAULT_TRAINER_CONFIG_FILE,
     DEFAULT_TRAINER_SUBFOLDER,
     HEZAR_CACHE_DIR,
     TQDM_BAR_FORMAT,
 )
 from ..data.datasets import Dataset
 from ..models import Model
 from ..utils import get_logger
-from .trainer_utils import MetricsManager, write_to_tensorboard
+from .trainer_utils import MetricsTracker
 
 
 logger = get_logger(__name__)
 
-METRICS_MAP = {
-    "accuracy": Accuracy,
-    "f1": F1Score,
-    "precision": Precision,
-}
 
 optimizers = {
     "adam": torch.optim.Adam,
     "adamw": torch.optim.AdamW,
     "sgd": torch.optim.SGD,
 }
 lr_schedulers = {
@@ -46,37 +41,41 @@
 
 class Trainer:
     """
     A general but fully featured model trainer/evaluator for Hezar models.
 
     Args:
         model ([`Model`] or `torch.nn.Module`): The main model to train and evaluate
-        config (TrainConfig): Training configuration and parameters
+        config (TrainerConfig): Training configuration and parameters
         train_dataset (Dataset): Train dataset
         eval_dataset (Dataset): Evaluation dataset
         data_collator: Collate function, usually included in the dataset object itself
         optimizer (optim.Optimizer): Model optimizer
-        lr_scheduler: Optional scheduler
+        lr_scheduler: Optional learning-rate scheduler
 
     """
 
     trainer_subfolder = DEFAULT_TRAINER_SUBFOLDER
     trainer_config_file = DEFAULT_TRAINER_CONFIG_FILE
     dataset_config_file = DEFAULT_DATASET_CONFIG_FILE
+    AVAILABLE_METRICS = []
 
     def __init__(
         self,
         model: Model = None,
-        config: TrainConfig = None,
+        config: TrainerConfig = None,
         train_dataset: Dataset = None,
         eval_dataset: Dataset = None,
         data_collator=None,
         optimizer: torch.optim.Optimizer = None,
         lr_scheduler=None,
+        compute_metrics=None,
+        **kwargs,
     ):
+
         self.config = config
 
         self.device, self.device_type = self._prepare_device_and_type()
         self.autocast_dtype = torch.bfloat16 if self.device_type == "cpu" else torch.float16
         self.scaler = torch.cuda.amp.GradScaler(enabled=self.config.use_amp and self.device_type == "cuda")
 
         self._set_seed(self.config.seed)
@@ -86,30 +85,37 @@
         self.train_dataset = train_dataset
         self.eval_dataset = eval_dataset
         self.data_collator = data_collator or self.train_dataset.data_collator
         self.train_dataloader, self.eval_dataloader = self._prepare_dataloaders()
 
         self.optimizer, self.lr_scheduler = self._prepare_optimizers(optimizer, lr_scheduler)
 
-        self.metrics_manager = self._setup_metrics_manager(self.config.metrics)
+        self.metrics = self.setup_metrics()
+        self.metrics_tracker = MetricsTracker(list(self.metrics.keys()))
 
         self.tensorboard = SummaryWriter(log_dir=self.config.log_dir)
 
-    def _prepare_device_and_type(self):
+    def _prepare_device_and_type(self) -> Tuple[str, str]:
         device = self.config.device if "cuda" in self.config.device and torch.cuda.is_available() else "cpu"
         device_type = "cuda" if "cuda" in device else "cpu"
         return device, device_type
 
     @staticmethod
-    def _set_seed(seed):
+    def _set_seed(seed) -> None:
         torch.manual_seed(seed)
         np.random.seed(seed)
         random.seed(seed)
 
-    def _prepare_model(self, model: Model):
+    def _prepare_model(self, model: Model) -> Model:
+        """
+        Download the model from HuggingFace Hub if `init_weights_from` is given in the config. Load the model to the
+        device and return it.
+        :param model:
+        :return:
+        """
         if model is None:
             raise ValueError("`model` must be given to the Trainer!")
         hub_path = self.config.init_weights_from
         if hub_path is not None:
             local_path = hf_hub_download(hub_path, filename=model.model_filename, cache_dir=HEZAR_CACHE_DIR)
             model.load_state_dict(torch.load(local_path, map_location="cpu"))
         model.to(self.device)
@@ -124,24 +130,26 @@
         """
         if self.train_dataset is not None:
             train_dataloader = DataLoader(
                 dataset=self.train_dataset,
                 batch_size=self.config.batch_size,
                 collate_fn=self.data_collator,
                 num_workers=self.config.num_dataloader_workers,
+                drop_last=True,
                 shuffle=True,
             )
         else:
             raise ValueError("Cannot create train dataloader because `train_dataset` is not given!")
         if self.eval_dataset is not None:
             eval_dataloader = DataLoader(
                 dataset=self.eval_dataset,
                 batch_size=self.config.batch_size,
                 collate_fn=self.data_collator,
                 num_workers=self.config.num_dataloader_workers,
+                drop_last=True,
                 shuffle=True,
             )
         else:
             logger.warning("Cannot create eval dataloader because `eval_dataset` is not given to the Trainer!")
             eval_dataloader = None
 
         return train_dataloader, eval_dataloader
@@ -174,142 +182,210 @@
                 if isinstance(scheduler_config, LRSchedulerConfig):
                     scheduler_config = scheduler_config.dict()
                 scheduler_name = scheduler_config.pop("name")
                 scheduler_config.pop("config_type", None)
                 lr_scheduler = lr_schedulers[scheduler_name](optimizer, **scheduler_config)
         return optimizer, lr_scheduler
 
-    def _setup_metrics_manager(self, metrics: Dict[str, Dict]) -> MetricsManager:
+    def setup_metrics(self):
+        metrics_dict = {}
+        for metric in self.config.metrics:
+            if isinstance(metric, str):
+                if metric not in self.AVAILABLE_METRICS:
+                    raise ValueError(f"Invalid metric `{metric}`! Available metrics: {self.AVAILABLE_METRICS}")
+                metrics_dict[metric] = build_metric(metric)
+            elif isinstance(metric, MetricConfig):
+                metrics_dict[metric] = build_metric(metric.name, config=metric)
+            else:
+                raise ValueError(f"Invalid metric type `{type(metric)}`! Available metrics: {self.AVAILABLE_METRICS}")
+        return metrics_dict
+
+    def prepare_input_batch(self, input_batch):
+        """
+        Every operation required to prepare the inputs for model forward like moving to device, permutations, etc.
+        Args:
+            input_batch: Raw input batch from the dataloader
+
+        Returns:
+            The proper input batch required by model forward
+        """
+        # cast to device
+        input_batch = {k: v.to(self.device) for k, v in input_batch.items() if isinstance(v, torch.Tensor)}
+        return input_batch
+
+    def amp_context_manager(self):
+        """
+        A smart context manager for mixed precision.
+
+        Returns:
+            A torch autocast context manager
         """
-        Set up metrics manager to track and update metrics like loss, accuracy, f1, etc.
+        return torch.autocast(device_type=self.device_type, dtype=self.autocast_dtype, enabled=self.config.use_amp)
+
+    def forward(self, input_batch):
+        """
+        Perform model forward on the input batch
+
+        In special cases, one can override this method in their desired trainer.
 
         Args:
-            metrics: A dict of metrics names and their kwargs {metric_name: **kwargs}
+            input_batch: Input batch
 
         Returns:
-             A MetricsManager instance
+            Model outputs
         """
-        metrics_dict = {"loss": None}
-        for name, kwargs in metrics.items():
-            metrics_dict[name] = METRICS_MAP[name](num_classes=self.train_dataset.config.num_labels, **kwargs)
-        metrics_manager = MetricsManager(metrics_dict)
-        return metrics_manager
+        outputs = self.model(input_batch)
+        return outputs
 
-    def training_step(self, input_batch: Dict[str, torch.Tensor]):
+    def compute_loss(self, logits: torch.Tensor, labels: torch.Tensor, **kwargs) -> torch.Tensor:
         """
-        Train one batch of data and return metrics outputs
+        Perform model forward and compute loss.
+
+        This method must be implemented in other trainers.
 
         Args:
-            input_batch: A batch of inputs to train
+            logits: Logits from model outputs
+            labels: Ground truth labels
 
         Returns:
-            The metrics results
+            The loss tensor
         """
-        input_batch = {k: v.to(self.device) for k, v in input_batch.items() if isinstance(v, torch.Tensor)}
+        raise NotImplementedError
+
+    def compute_metrics(self, predictions, labels, **kwargs):
+        """
+        Compute metric values on the predictions and labels
 
-        with torch.autocast(device_type=self.device_type, dtype=self.autocast_dtype, enabled=self.config.use_amp):
-            outputs = self.model(input_batch)
-            if "loss" not in outputs:
-                raise ValueError("Model outputs must contain `loss`!")
-            loss: torch.Tensor = outputs["loss"]
+        Args:
+            predictions: A list of all predictions
+            labels: A list of all labels
+
+        Returns:
+            A dictionary of the results for every metric specified by the trainer
+        """
+        return {}
+
+    def training_step(self, input_batch: Dict[str, torch.Tensor]) -> Dict[str, Any]:
+        """
+        Train one batch of data and return loss and model outputs
+
+        Args:
+            input_batch: A batch of inputs to train
+
+        Returns:
+            Train step outputs including loss, logits, etc.
+        """
+        with self.amp_context_manager():
+            outputs = self.forward(input_batch)
+            loss = self.compute_loss(outputs["logits"], input_batch["labels"])
 
         self.scaler.scale(loss).backward()
         self.scaler.step(self.optimizer)
         self.scaler.update()
         self.optimizer.zero_grad()
 
-        results = self.metrics_manager.compute(outputs["logits"].detach().cpu(), input_batch["labels"].detach().cpu())
-        results["loss"] = loss.item()
+        outputs["loss"] = loss.item() if isinstance(loss, torch.Tensor) else loss
 
-        return results
+        return outputs
 
-    def evaluation_step(self, input_batch: Dict[str, torch.Tensor]):
+    def evaluation_step(self, input_batch: Dict[str, torch.Tensor]) -> Dict[str, Any]:
         """
-        Evaluate one batch of data and return metrics outputs
+        Evaluate one batch of data and return loss and model outputs
 
         Args:
-            input_batch: A batch of inputs to train
+            input_batch: A batch of inputs to evaluate
 
         Returns:
-            The metrics results
+            Evaluation step outputs including loss, logits, etc.
         """
-        input_batch = {k: v.to(self.device) for k, v in input_batch.items() if isinstance(v, torch.Tensor)}
-
-        with torch.autocast(device_type=self.device_type, dtype=self.autocast_dtype, enabled=self.config.use_amp):
-            outputs = self.model(input_batch)
-            if "loss" not in outputs:
-                raise ValueError("Model outputs must contain `loss`!")
-            loss: torch.Tensor = outputs["loss"]
+        with self.amp_context_manager():
+            outputs = self.forward(input_batch)
+            loss = self.compute_loss(outputs["logits"], input_batch["labels"])
 
-        results = self.metrics_manager.compute(outputs["logits"].detach().cpu(), input_batch["labels"].detach().cpu())
-        results["loss"] = loss.item()
+        outputs["loss"] = loss.item() if isinstance(loss, torch.Tensor) else loss
 
-        return results
+        return outputs
 
     def inner_training_loop(self, epoch_num: int):
         """
         Train the model for one epoch on the whole train dataset and verbose live metric values in the progress bar
 
         Args:
             epoch_num: Number of the current epoch
 
         Returns:
             Metrics averages through the full iteration
         """
-        self.metrics_manager.reset()
+        self.metrics_tracker.reset()
         self.model.train()
         with tqdm(
             self.train_dataloader,
             unit="batch",
             desc=f"Epoch: {epoch_num}/{self.config.num_epochs} ",
             bar_format=TQDM_BAR_FORMAT,
             ascii=" #",
         ) as iterator:
-            for input_batch in iterator:
-                results = self.training_step(input_batch)
-                self.metrics_manager.update(results)
-                iterator.set_postfix(**self.metrics_manager.avg())
-        return self.metrics_manager.avg()
+            for step, input_batch in enumerate(iterator):
+                input_batch = self.prepare_input_batch(input_batch)
+                # Training on one batch
+                outputs = self.training_step(input_batch)
+                # Compute metrics
+                training_results = self.compute_metrics(
+                    outputs["logits"].detach().cpu().numpy(),
+                    input_batch["labels"].detach().cpu().numpy(),
+                )
+                training_results["loss"] = outputs["loss"]
+                # Gather outputs for metrics
+                self.metrics_tracker.update(training_results)
+                iterator.set_postfix(**self.metrics_tracker.avg())
+
+        return self.metrics_tracker.avg()
 
     def evaluate(self):
         """
         Evaluates the model on the whole eval dataset and verbose live metric values in the progress bar
 
         Returns:
-            Metrics averages through the full iteration
+            Evaluation results
         """
-        self.metrics_manager.reset()
+        self.metrics_tracker.reset()
         self.model.eval()
         with tqdm(
             self.eval_dataloader,
             unit="batch",
             desc="Evaluating... ",
             bar_format=TQDM_BAR_FORMAT,
             ascii=" #",
         ) as iterator:
             with torch.inference_mode():
-                for input_batch in iterator:
-                    results = self.evaluation_step(input_batch)
-                    self.metrics_manager.update(results)
-                    iterator.set_postfix(**self.metrics_manager.avg())
-        return self.metrics_manager.avg()
+                for step, input_batch in enumerate(iterator):
+                    input_batch = self.prepare_input_batch(input_batch)
+                    # Evaluation on one batch
+                    outputs = self.evaluation_step(input_batch)
+                    # Compute metrics
+                    evaluation_results = self.compute_metrics(
+                        outputs["logits"].detach().cpu().numpy(),
+                        input_batch["labels"].detach().cpu().numpy(),
+                )
+                    evaluation_results["loss"] = outputs["loss"]
+                    # Gather outputs for metrics
+                    self.metrics_tracker.update(evaluation_results)
+                    iterator.set_postfix(**self.metrics_tracker.avg())
+
+        return self.metrics_tracker.avg()
 
     def train(self):
         """
         The full training process like training, evaluation, logging and saving model checkpoints.
         """
         for epoch in range(1, self.config.num_epochs + 1):
             print()
-            train_results = self.inner_training_loop(epoch)
-            eval_results = self.evaluate()
-            self.lr_scheduler.step(eval_results["loss"])
-
-            # tensorboard
-            write_to_tensorboard(self.tensorboard, train_results, "train", epoch)
-            write_to_tensorboard(self.tensorboard, eval_results, "val", epoch)
+            self.inner_training_loop(epoch)
+            evaluation_results = self.evaluate()
+            self.lr_scheduler.step(evaluation_results["loss"])
 
             # maybe save checkpoint
             if epoch % self.config.save_freq == 0:
                 ckpt_save_path = os.path.join(self.config.checkpoints_dir, str(epoch))
                 self.save(ckpt_save_path)
 
     def save(
```

### Comparing `hezar-0.14.3/hezar/trainers/trainer_utils.py` & `hezar-0.15.0/hezar/trainers/trainer_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from typing import List
+
 from torch.utils.tensorboard import SummaryWriter
 
 
-class AverageMeter(object):
-    """Computes and stores the average and current value"""
+class AverageMeter:
+    """Compute and store the average and current value"""
 
     def __init__(self, name, fmt=":f"):
         self.name = name
         self.fmt = fmt
         self.val = 0
         self.avg = 0
         self.sum = 0
@@ -26,39 +28,33 @@
         self.avg = self.sum / self.count
 
     def __str__(self):
         fmtstr = "{name} {val" + self.fmt + "} ({avg" + self.fmt + "})"
         return fmtstr.format(**self.__dict__)
 
 
-class MetricsManager:
-    def __init__(self, metrics_dict):
-        self.metrics_dict = metrics_dict
-        self.trackers = {m: AverageMeter(m) for m in self.metrics_dict.keys()}
-
-    def compute(self, preds, labels):
-        results = {}
-        for metric_name, metric in self.metrics_dict.items():
-            if metric is not None:
-                results[metric_name] = metric(preds, labels).item()
-
-        return results
+class MetricsTracker:
+    def __init__(self, metrics: List[str]):
+        self.metrics = metrics
+        self.trackers = {m: AverageMeter(m) for m in self.metrics}
+        if "loss" not in self.trackers:
+            self.trackers["loss"] = AverageMeter("loss")
 
     def update(self, results):
-        for metric_name, metric in self.trackers.items():
-            metric.update(results[metric_name])
+        for metric_name, tracker in self.trackers.items():
+            tracker.update(results[metric_name])
 
     def reset(self):
-        for metric in self.trackers.values():
-            metric.reset()
+        for tracker in self.trackers.values():
+            tracker.reset()
 
     def avg(self):
         avg_results = {}
-        for metric_name, metric in self.trackers.items():
-            avg_results[metric_name] = metric.avg
+        for metric_name, tracker in self.trackers.items():
+            avg_results[metric_name] = tracker.avg
 
         return avg_results
 
 
 def write_to_tensorboard(writer: SummaryWriter, logs: dict, mode: str, step: int):
     for metric_name, value in logs.items():
         writer.add_scalar(f"{mode}/{metric_name}", value, step)
```

### Comparing `hezar-0.14.3/hezar/utils/config_utils.py` & `hezar-0.15.0/hezar/utils/config_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 import os
 from typing import Dict, Union
 
 import omegaconf
 from omegaconf import DictConfig
 
+from ..constants import ConfigType
+from .common_utils import snake_case
 from .logging import get_logger
 
 
 __all__ = [
     "flatten_dict",
     "load_yaml_config",
     "load_json_config",
@@ -78,62 +80,65 @@
     Args:
         name (str): Model's registry name
         config_type (str): Registry type
 
     Returns:
         A class of type :class:`hezar.Config`
     """
-    if config_type == "model":
+    if config_type == ConfigType.MODEL:
         from ..registry import models_registry  # noqa
 
         registry = models_registry
-    elif config_type == "preprocessor":
+    elif config_type == ConfigType.PREPROCESSOR:
         from ..registry import preprocessors_registry  # noqa
 
         registry = preprocessors_registry
-    elif config_type == "dataset":
+    elif config_type == ConfigType.DATASET:
         from ..registry import datasets_registry  # noqa
 
         registry = datasets_registry
-    elif config_type == "embedding":
+    elif config_type == ConfigType.EMBEDDING:
         from ..registry import embeddings_registry  # noqa
         registry = embeddings_registry
 
     else:
         raise ValueError(f"Invalid `config_type`: {config_type}!")
 
     config_cls = registry[name].config_class
     return config_cls
 
 
-def get_module_class(name: str, module_type: str):
+def get_module_class(name: str, module_type: str) -> type:
     """
     Get module class based on registry name
 
     Args:
         name: Module's key name in its registry
         module_type: Type of the module e.g, model, dataset, preprocessor, embedding, etc
 
     Returns:
         A class corresponding to the given module
     """
-    if module_type == "model":
+    if module_type == ConfigType.MODEL:
         from ..registry import models_registry  # noqa
 
         registry = models_registry
-    elif module_type == "preprocessor":
+    elif module_type == ConfigType.PREPROCESSOR:
         from ..registry import preprocessors_registry  # noqa
 
         registry = preprocessors_registry
-    elif module_type == "dataset":
+    elif module_type == ConfigType.DATASET:
         from ..registry import datasets_registry  # noqa
 
         registry = datasets_registry
-    elif module_type == "embedding":
+    elif module_type == ConfigType.EMBEDDING:
         from ..registry import embeddings_registry  # noqa
         registry = embeddings_registry
+    elif module_type == ConfigType.METRIC:
+        from ..registry import metrics_registry  # noqa
+        registry = metrics_registry
 
     else:
-        raise ValueError(f"Invalid `config_type`: {module_type}!")
-
+        raise ValueError(f"Invalid `module_type`: {module_type}!")
+    name = snake_case(name)
     module_cls = registry[name].module_class
     return module_cls
```

### Comparing `hezar-0.14.3/hezar/utils/hub_utils.py` & `hezar-0.15.0/hezar/utils/hub_utils.py`

 * *Files identical despite different names*

### Comparing `hezar-0.14.3/pyproject.toml` & `hezar-0.15.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "hezar"
-version = "0.14.3"
+version = "0.15.0"
 packages = [{ include = "hezar" }]
 description = "Hezar: A seamless AI framework & library for Persian"
 license = "MIT"
 authors = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 maintainers = ["Aryan Shekarlaban <arxyzan@gmail.com>"]
 repository = "https://github.com/hezarai/hezar"
 homepage = "https://github.com/hezarai"
@@ -33,14 +33,17 @@
 python = ">=3.8"
 torch = ">=1.10.0"
 omegaconf = ">=2.3.0"
 transformers = ">=4.26"
 datasets = ">=2.9.0"
 torchmetrics = ">=0.11.0"
 huggingface_hub = ">=0.12.0"
+gensim = ">=4.1.0"
+tensorboard = ">=2.10.0"
+
 pillow = "*"
 black = "*"
 ruff = "*"
 
 [tool.black]
 line-length = 120
 target-version = ['py38', 'py39', 'py310']
@@ -56,8 +59,9 @@
 "*test*.py" = ["F401", "F841"]
 
 [tool.ruff.isort]
 lines-after-imports = 2
 known-first-party = ["hezar"]
 
 [tool.ruff.pydocstyle]
-convention = "google"
+convention = "google"
+
```

### Comparing `hezar-0.14.3/PKG-INFO` & `hezar-0.15.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hezar
-Version: 0.14.3
+Version: 0.15.0
 Summary: Hezar: A seamless AI framework & library for Persian
 Home-page: https://github.com/hezarai
 License: MIT
 Keywords: packaging,poetry
 Author: Aryan Shekarlaban
 Author-email: arxyzan@gmail.com
 Maintainer: Aryan Shekarlaban
@@ -18,18 +18,20 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: black
 Requires-Dist: datasets (>=2.9.0)
+Requires-Dist: gensim (>=4.1.0)
 Requires-Dist: huggingface_hub (>=0.12.0)
 Requires-Dist: omegaconf (>=2.3.0)
 Requires-Dist: pillow
 Requires-Dist: ruff
+Requires-Dist: tensorboard (>=2.10.0)
 Requires-Dist: torch (>=1.10.0)
 Requires-Dist: torchmetrics (>=0.11.0)
 Requires-Dist: transformers (>=4.26)
 Project-URL: Documentation, https://github.com/hezarai/docs
 Project-URL: Repository, https://github.com/hezarai/hezar
 Description-Content-Type: text/markdown
```

