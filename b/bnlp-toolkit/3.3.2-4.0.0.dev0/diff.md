# Comparing `tmp/bnlp_toolkit-3.3.2.tar.gz` & `tmp/bnlp_toolkit-4.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlp_toolkit-3.3.2.tar", last modified: Mon Jul 10 05:51:39 2023, max compression
+gzip compressed data, was "bnlp_toolkit-4.0.0.dev0.tar", last modified: Sun Jul 16 05:44:36 2023, max compression
```

## Comparing `bnlp_toolkit-3.3.2.tar` & `bnlp_toolkit-4.0.0.dev0.tar`

### file list

```diff
@@ -1,36 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22844 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/cleantext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/cleantext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/cleantext/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/cleantext/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/corpus/
--rw-r--r--   0 runner    (1001) docker     (123)     9095 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/corpus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/corpus/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/doc2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/fasttext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/glove.py
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/embedding/word2vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/pos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.019692 bnlp_toolkit-3.3.2/bnlp/tokenizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/tokenizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/tokenizer/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/tokenizer/nltk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/bnlp/tokenizer/sentencepiece.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-10 05:51:39.000000 bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 05:51:39.023692 bnlp_toolkit-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-07-10 05:51:26.000000 bnlp_toolkit-3.3.2/tests/test.py
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.348094 bnlp_toolkit-4.0.0.dev0/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     1069 2023-07-05 05:00:54.000000 bnlp_toolkit-4.0.0.dev0/LICENSE
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)    23282 2023-07-16 05:44:36.348094 bnlp_toolkit-4.0.0.dev0/PKG-INFO
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)    22797 2023-07-16 05:34:47.000000 bnlp_toolkit-4.0.0.dev0/README.md
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.324094 bnlp_toolkit-4.0.0.dev0/bnlp/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)      730 2023-07-13 07:37:46.000000 bnlp_toolkit-4.0.0.dev0/bnlp/__init__.py
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.324094 bnlp_toolkit-4.0.0.dev0/bnlp/cleantext/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2023-07-05 05:00:54.000000 bnlp_toolkit-4.0.0.dev0/bnlp/cleantext/__init__.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     4121 2023-07-12 07:05:42.000000 bnlp_toolkit-4.0.0.dev0/bnlp/cleantext/clean.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     2466 2023-07-10 06:04:13.000000 bnlp_toolkit-4.0.0.dev0/bnlp/cleantext/constants.py
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.336094 bnlp_toolkit-4.0.0.dev0/bnlp/corpus/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2023-07-10 06:04:13.000000 bnlp_toolkit-4.0.0.dev0/bnlp/corpus/__init__.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     9849 2023-07-10 07:18:08.000000 bnlp_toolkit-4.0.0.dev0/bnlp/corpus/_stopwords.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)      919 2023-07-12 16:52:08.000000 bnlp_toolkit-4.0.0.dev0/bnlp/corpus/corpus.py
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.336094 bnlp_toolkit-4.0.0.dev0/bnlp/embedding/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2023-07-05 05:00:54.000000 bnlp_toolkit-4.0.0.dev0/bnlp/embedding/__init__.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     3703 2023-07-12 17:07:19.000000 bnlp_toolkit-4.0.0.dev0/bnlp/embedding/doc2vec.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     3165 2023-07-10 17:52:33.000000 bnlp_toolkit-4.0.0.dev0/bnlp/embedding/fasttext.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     1155 2023-07-10 06:04:13.000000 bnlp_toolkit-4.0.0.dev0/bnlp/embedding/glove.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     6181 2023-07-12 17:07:07.000000 bnlp_toolkit-4.0.0.dev0/bnlp/embedding/word2vec.py
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.336094 bnlp_toolkit-4.0.0.dev0/bnlp/token_classification/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2023-07-10 07:11:47.000000 bnlp_toolkit-4.0.0.dev0/bnlp/token_classification/__init__.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     1026 2023-07-10 07:13:22.000000 bnlp_toolkit-4.0.0.dev0/bnlp/token_classification/ner.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)      885 2023-07-10 07:13:31.000000 bnlp_toolkit-4.0.0.dev0/bnlp/token_classification/pos.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)      992 2023-07-10 06:04:13.000000 bnlp_toolkit-4.0.0.dev0/bnlp/token_classification/token_classification_trainer.py
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.336094 bnlp_toolkit-4.0.0.dev0/bnlp/tokenizer/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2023-07-05 05:00:54.000000 bnlp_toolkit-4.0.0.dev0/bnlp/tokenizer/__init__.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     3233 2023-07-10 06:48:28.000000 bnlp_toolkit-4.0.0.dev0/bnlp/tokenizer/basic.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     1148 2023-07-10 06:04:13.000000 bnlp_toolkit-4.0.0.dev0/bnlp/tokenizer/nltk.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     1180 2023-07-10 06:04:13.000000 bnlp_toolkit-4.0.0.dev0/bnlp/tokenizer/sentencepiece.py
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.344094 bnlp_toolkit-4.0.0.dev0/bnlp/utils/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)        0 2023-07-10 06:04:13.000000 bnlp_toolkit-4.0.0.dev0/bnlp/utils/__init__.py
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)     1559 2023-07-10 06:04:13.000000 bnlp_toolkit-4.0.0.dev0/bnlp/utils/utils.py
+drwxrwxr-x   0 sagor     (1000) sagor     (1000)        0 2023-07-16 05:44:36.344094 bnlp_toolkit-4.0.0.dev0/bnlp_toolkit.egg-info/
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)    23282 2023-07-16 05:44:36.000000 bnlp_toolkit-4.0.0.dev0/bnlp_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)      815 2023-07-16 05:44:36.000000 bnlp_toolkit-4.0.0.dev0/bnlp_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)        1 2023-07-16 05:44:36.000000 bnlp_toolkit-4.0.0.dev0/bnlp_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)       78 2023-07-16 05:44:36.000000 bnlp_toolkit-4.0.0.dev0/bnlp_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)        5 2023-07-16 05:44:36.000000 bnlp_toolkit-4.0.0.dev0/bnlp_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)       38 2023-07-16 05:44:36.348094 bnlp_toolkit-4.0.0.dev0/setup.cfg
+-rw-rw-r--   0 sagor     (1000) sagor     (1000)      892 2023-07-13 07:37:55.000000 bnlp_toolkit-4.0.0.dev0/setup.py
```

### Comparing `bnlp_toolkit-3.3.2/LICENSE` & `bnlp_toolkit-4.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlp_toolkit-3.3.2/PKG-INFO` & `bnlp_toolkit-4.0.0.dev0/bnlp_toolkit.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bnlp_toolkit
-Version: 3.3.2
+Name: bnlp-toolkit
+Version: 4.0.0.dev0
 Summary: BNLP is a natural language processing toolkit for Bengali Language
 Home-page: https://github.com/sagorbrur/bnlp
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -75,15 +75,15 @@
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
   ```
-  - Python: 3.6, 3.7, 3.8, 3.9
+  - Python: 3.6, 3.7, 3.8, 3.9, 3.10
   - OS: Linux, Windows, Mac
 
 
 
 ## Pretrained Model
 
 ### Download Links
@@ -115,238 +115,256 @@
 ## Tokenization
 
 ### Basic Tokenizer
 
   ```py
   from bnlp import BasicTokenizer
   
-  basic_tokenizer = BasicTokenizer()
+  tokenizer = BasicTokenizer()
+
   raw_text = "আমি বাংলায় গান গাই।"
-  tokens = basic_tokenizer.tokenize(raw_text)
+  tokens = tokenizer(raw_text)
   print(tokens)
-
   # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
   ```
 
 ### NLTK Tokenization
 
   ```py
   from bnlp import NLTKTokenizer
 
   bnltk = NLTKTokenizer()
+
   text = "আমি ভাত খাই। সে বাজারে যায়। তিনি কি সত্যিই ভালো মানুষ?"
   word_tokens = bnltk.word_tokenize(text)
   sentence_tokens = bnltk.sentence_tokenize(text)
   print(word_tokens)
   print(sentence_tokens)
-
   # output
   # word_token: ["আমি", "ভাত", "খাই", "।", "সে", "বাজারে", "যায়", "।", "তিনি", "কি", "সত্যিই", "ভালো", "মানুষ", "?"]
   # sentence_token: ["আমি ভাত খাই।", "সে বাজারে যায়।", "তিনি কি সত্যিই ভালো মানুষ?"]
   ```
 
 
 ### Bengali SentencePiece Tokenization
 
 #### Tokenization using trained model
 ```py
 from bnlp import SentencepieceTokenizer
 
-bsp = SentencepieceTokenizer()
 model_path = "./model/bn_spm.model"
+bsp = SentencepieceTokenizer(model_path)
+
+
 input_text = "আমি ভাত খাই। সে বাজারে যায়।"
-tokens = bsp.tokenize(model_path, input_text)
+tokens = bsp.tokenize(input_text)
 print(tokens)
-text2id = bsp.text2id(model_path, input_text)
+text2id = bsp.text2id(input_text)
 print(text2id)
-id2text = bsp.id2text(model_path, text2id)
+id2text = bsp.id2text(text2id)
 print(id2text)
 ```
 
 #### Training SentencePiece
 ```py
-from bnlp import SentencepieceTokenizer
+from bnlp import SentencepieceTrainer
 
-bsp = SentencepieceTokenizer()
 data = "raw_text.txt"
-model_prefix = "test"
-vocab_size = 5
-bsp.train(data, model_prefix, vocab_size)
+vocab_size = 32000
+model_prefix = "model"
+
+trainer = SentencepieceTrainer(
+   data=data,
+   vocab_size=vocab_size,
+   model_prefix=model_prefix
+)
+trainer.train()
+
 ```
 
 ## Word Embedding
 
 ### Bengali Word2Vec
 
 #### Generate Vector using pretrain model
 
 ```py
 from bnlp import BengaliWord2Vec
 
-bwv = BengaliWord2Vec()
 model_path = "bengali_word2vec.model"
+bwv = BengaliWord2Vec(model_path)
+
 word = 'গ্রাম'
-vector = bwv.generate_word_vector(model_path, word)
+vector = bwv.get_word_vector(word)
 print(vector.shape)
-print(vector)
 ```
 
 #### Find Most Similar Word Using Pretrained Model
 
 ```py
 from bnlp import BengaliWord2Vec
 
-bwv = BengaliWord2Vec()
 model_path = "bengali_word2vec.model"
+bwv = BengaliWord2Vec(model_path)
+
 word = 'গ্রাম'
-similar = bwv.most_similar(model_path, word, topn=10)
-print(similar)
+similar_words = bwv.get_most_similar_words(word, topn=10)
+print(similar_words)
 ```
+
 #### Train Bengali Word2Vec with your own data
 
 Train Bengali word2vec with your custom raw data or tokenized sentences.
 
 Custom tokenized sentence format example:
 ```py
 sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
 ```
 Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
 ```py
-from bnlp import BengaliWord2Vec
-bwv = BengaliWord2Vec()
+from bnlp import Word2VecTraining
+
+trainer = Word2VecTraining()
+
 data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
 model_name = "test_model.model"
 vector_name = "test_vector.vector"
-bwv.train(data_file, model_name, vector_name, epochs=5)
+trainer.train(data_file, model_name, vector_name, epochs=5)
 ```
 
 #### Pre-train or resume word2vec training with same or new corpus or tokenized sentences
 
 Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
 ```py
-from bnlp import BengaliWord2Vec
-bwv = BengaliWord2Vec()
+from bnlp import Word2VecTraining
+
+trainer = Word2VecTraining()
 
 trained_model_path = "mytrained_model.model"
 data_file = "raw_text.txt"
 model_name = "test_model.model"
 vector_name = "test_vector.vector"
-bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+trainer.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+
 ```
 
 ### Bengali FastText
 
 To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
 
 NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
 
 ### Generate Vector Using Pretrained Model
 
   ```py
   from bnlp.embedding.fasttext import BengaliFasttext
 
-  bft = BengaliFasttext()
-  word = "গ্রাম"
   model_path = "bengali_fasttext_wiki.bin"
-  word_vector = bft.generate_word_vector(model_path, word)
+  bft = BengaliFasttext(model_path)
+
+  word = "গ্রাম"
+  word_vector = bft.get_word_vector(model_path, word)
   print(word_vector.shape)
-  print(word_vector)
   ```
 
+### Generate Vector File from Fasttext Binary Model
+
+```py
+from bnlp.embedding.fasttext import BengaliFasttext
+
+model_path = "mymodel.bin"
+bft = BengaliFasttext(model_path)
+
+out_vector_name = "myvector.txt"
+bft.bin2vec(out_vector_name)
+```
+
 ### Train Bengali FastText Model
 
 Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
 
   ```py
-  from bnlp.embedding.fasttext import BengaliFasttext
+  from bnlp.embedding.fasttext import FasttextTrainer
+
+  trainer = FasttextTrainer()
 
-  bft = BengaliFasttext()
   data = "raw_text.txt"
   model_name = "saved_model.bin"
   epoch = 50
-  bft.train(data, model_name, epoch)
+  trainer.train(data, model_name, epoch)
   ```
 
-### Generate Vector File from Fasttext Binary Model
-
-```py
-from bnlp.embedding.fasttext import BengaliFasttext
-
-bft = BengaliFasttext()
-
-model_path = "mymodel.bin"
-out_vector_name = "myvector.txt"
-bft.bin2vec(model_path, out_vector_name)
-```
-
 ## Bengali GloVe Word Vectors
 
 We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
 You can download and use it on your different machine learning purposes.
 
 ```py
 from bnlp import BengaliGlove
+
 glove_path = "bn_glove.39M.100d.txt"
+bengali_glove = BengaliGlove(glove_path)
+
 word = "গ্রাম"
-bng = BengaliGlove()
-res = bng.closest_word(glove_path, word)
-print(res)
-vec = bng.word2vec(glove_path, word)
-print(vec)
+vector = bengali_glove.get_word_vector(word)
+print(vector.shape)
+
+similar_words = bengali_glove.get_closest_word(glove_path, word)
+print(similar_words)
 ```
 
 ## Document Embedding
 
 ### Bengali Doc2Vec
 #### Get document vector from input document
 
 ```py
 from bnlp import BengaliDoc2vec
 
-bn_doc2vec = BengaliDoc2vec()
-
 model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+bn_doc2vec = BengaliDoc2vec(model_path)
+
 document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
+vector = bn_doc2vec.get_document_vector(text)
+print(vector.shape)
 
-vector = bn_doc2vec.get_document_vector(model_path, text)
-print(vector)
 ```
 
 #### Find document similarity between two document
 
 ```py
 from bnlp import BengaliDoc2vec
 
-bn_doc2vec = BengaliDoc2vec()
-
 model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+bn_doc2vec = BengaliDoc2vec(model_path)
+
 article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
 similarity = bn_doc2vec.get_document_similarity(
-  model_path,
   article_1,
   article_2
 )
 print(similarity)
+
 ```
 
 #### Train doc2vec vector with custom text files
 
 ```py
-from bnlp import BengaliDoc2vec
+from bnlp import BengaliDoc2vecTrainer
 
-bn_doc2vec = BengaliDoc2vec()
+trainer = BengaliDoc2vecTrainer()
 
 text_files = "path/myfiles"
 checkpoint_path = "msc/logs"
 
-bn_doc2vec.train_doc2vec(
+trainer.train(
   text_files,
   checkpoint_path=checkpoint_path,
   vector_size=100,
   min_count=2,
   epochs=10
 )
 
@@ -356,89 +374,88 @@
 ## Bengali POS Tagging
 
 ### Bengali CRF POS Tagging
 
 #### Find Pos Tag Using Pretrained Model
 
 ```py
-from bnlp import POS
-bn_pos = POS()
+from bnlp import BengaliPOS
+
 model_path = "model/bn_pos.pkl"
+bn_pos = BengaliPOS(model_path)
+
 text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
-res = bn_pos.tag(model_path, text)
+res = bn_pos.tag(text)
 print(res)
 # [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
 ```
 
 #### Train POS Tag Model
 
 ```py
-from bnlp import POS
-bn_pos = POS()
+from bnlp import CRFTaggerTrainer
+
+trainer = CRFTaggerTrainer()
+
 model_name = "pos_model.pkl"
 train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা',  'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
 test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-bn_pos.train(model_name, train_data, test_data)
+trainer.train(model_name, train_data, test_data)
+
 ```
 
 ## Bengali NER
 
 ### Bengali CRF NER
 
 #### Find NER Tag Using Pretrained Model
 
 ```py
-from bnlp import NER
-bn_ner = NER()
+from bnlp import BengaliNER
+
 model_path = "model/bn_ner.pkl"
+bn_ner = BengaliNER(model_path)
+
 text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
-result = bn_ner.tag(model_path, text)
+result = bn_ner.tag(text)
 print(result)
 # [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
 ```
 
 #### Train NER Tag Model
 
 ```py
-from bnlp import NER
-bn_ner = NER()
+from bnlp import CRFTaggerTrainer
+
+trainer = CRFTaggerTrainer()
+
 model_name = "ner_model.pkl"
 train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
 test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-bn_ner.train(model_name, train_data, test_data)
+trainer.train(model_name, train_data, test_data)
 ```
 
 
 ## Bengali Corpus Class
 
 ### Stopwords and Punctuations
 
 ```py
-from bnlp.corpus import stopwords, punctuations, letters, digits
-
-print(stopwords)
-print(punctuations)
-print(letters)
-print(digits)
-```
-
-### Remove stopwords from Text
+from bnlp import BengaliCorpus as corpus
 
-```py
-from bnlp.corpus import stopwords
-from bnlp.corpus.util import remove_stopwords
+print(corpus.stopwords)
+print(corpus.punctuations)
+print(corpus.letters)
+print(corpus.digits)
+print(corpus.vowels)
 
-raw_text = 'আমি ভাত খাই।'
-result = remove_stopwords(raw_text, stopwords)
-print(result)
-# ['ভাত', 'খাই', '।']
 ```
 
 ## Text Cleaning
 We adopted different text cleaning formula, codes from [clean-text](https://github.com/jfilter/clean-text) and modified for Bangla. Now you can normalize and clean your text using the following methods.
 
 ```py
 from bnlp import CleanText
```

### Comparing `bnlp_toolkit-3.3.2/README.md` & `bnlp_toolkit-4.0.0.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -60,15 +60,15 @@
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
   ```
-  - Python: 3.6, 3.7, 3.8, 3.9
+  - Python: 3.6, 3.7, 3.8, 3.9, 3.10
   - OS: Linux, Windows, Mac
 
 
 
 ## Pretrained Model
 
 ### Download Links
@@ -100,238 +100,256 @@
 ## Tokenization
 
 ### Basic Tokenizer
 
   ```py
   from bnlp import BasicTokenizer
   
-  basic_tokenizer = BasicTokenizer()
+  tokenizer = BasicTokenizer()
+
   raw_text = "আমি বাংলায় গান গাই।"
-  tokens = basic_tokenizer.tokenize(raw_text)
+  tokens = tokenizer(raw_text)
   print(tokens)
-
   # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
   ```
 
 ### NLTK Tokenization
 
   ```py
   from bnlp import NLTKTokenizer
 
   bnltk = NLTKTokenizer()
+
   text = "আমি ভাত খাই। সে বাজারে যায়। তিনি কি সত্যিই ভালো মানুষ?"
   word_tokens = bnltk.word_tokenize(text)
   sentence_tokens = bnltk.sentence_tokenize(text)
   print(word_tokens)
   print(sentence_tokens)
-
   # output
   # word_token: ["আমি", "ভাত", "খাই", "।", "সে", "বাজারে", "যায়", "।", "তিনি", "কি", "সত্যিই", "ভালো", "মানুষ", "?"]
   # sentence_token: ["আমি ভাত খাই।", "সে বাজারে যায়।", "তিনি কি সত্যিই ভালো মানুষ?"]
   ```
 
 
 ### Bengali SentencePiece Tokenization
 
 #### Tokenization using trained model
 ```py
 from bnlp import SentencepieceTokenizer
 
-bsp = SentencepieceTokenizer()
 model_path = "./model/bn_spm.model"
+bsp = SentencepieceTokenizer(model_path)
+
+
 input_text = "আমি ভাত খাই। সে বাজারে যায়।"
-tokens = bsp.tokenize(model_path, input_text)
+tokens = bsp.tokenize(input_text)
 print(tokens)
-text2id = bsp.text2id(model_path, input_text)
+text2id = bsp.text2id(input_text)
 print(text2id)
-id2text = bsp.id2text(model_path, text2id)
+id2text = bsp.id2text(text2id)
 print(id2text)
 ```
 
 #### Training SentencePiece
 ```py
-from bnlp import SentencepieceTokenizer
+from bnlp import SentencepieceTrainer
 
-bsp = SentencepieceTokenizer()
 data = "raw_text.txt"
-model_prefix = "test"
-vocab_size = 5
-bsp.train(data, model_prefix, vocab_size)
+vocab_size = 32000
+model_prefix = "model"
+
+trainer = SentencepieceTrainer(
+   data=data,
+   vocab_size=vocab_size,
+   model_prefix=model_prefix
+)
+trainer.train()
+
 ```
 
 ## Word Embedding
 
 ### Bengali Word2Vec
 
 #### Generate Vector using pretrain model
 
 ```py
 from bnlp import BengaliWord2Vec
 
-bwv = BengaliWord2Vec()
 model_path = "bengali_word2vec.model"
+bwv = BengaliWord2Vec(model_path)
+
 word = 'গ্রাম'
-vector = bwv.generate_word_vector(model_path, word)
+vector = bwv.get_word_vector(word)
 print(vector.shape)
-print(vector)
 ```
 
 #### Find Most Similar Word Using Pretrained Model
 
 ```py
 from bnlp import BengaliWord2Vec
 
-bwv = BengaliWord2Vec()
 model_path = "bengali_word2vec.model"
+bwv = BengaliWord2Vec(model_path)
+
 word = 'গ্রাম'
-similar = bwv.most_similar(model_path, word, topn=10)
-print(similar)
+similar_words = bwv.get_most_similar_words(word, topn=10)
+print(similar_words)
 ```
+
 #### Train Bengali Word2Vec with your own data
 
 Train Bengali word2vec with your custom raw data or tokenized sentences.
 
 Custom tokenized sentence format example:
 ```py
 sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
 ```
 Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
 ```py
-from bnlp import BengaliWord2Vec
-bwv = BengaliWord2Vec()
+from bnlp import Word2VecTraining
+
+trainer = Word2VecTraining()
+
 data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
 model_name = "test_model.model"
 vector_name = "test_vector.vector"
-bwv.train(data_file, model_name, vector_name, epochs=5)
+trainer.train(data_file, model_name, vector_name, epochs=5)
 ```
 
 #### Pre-train or resume word2vec training with same or new corpus or tokenized sentences
 
 Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
 ```py
-from bnlp import BengaliWord2Vec
-bwv = BengaliWord2Vec()
+from bnlp import Word2VecTraining
+
+trainer = Word2VecTraining()
 
 trained_model_path = "mytrained_model.model"
 data_file = "raw_text.txt"
 model_name = "test_model.model"
 vector_name = "test_vector.vector"
-bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+trainer.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+
 ```
 
 ### Bengali FastText
 
 To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
 
 NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
 
 ### Generate Vector Using Pretrained Model
 
   ```py
   from bnlp.embedding.fasttext import BengaliFasttext
 
-  bft = BengaliFasttext()
-  word = "গ্রাম"
   model_path = "bengali_fasttext_wiki.bin"
-  word_vector = bft.generate_word_vector(model_path, word)
+  bft = BengaliFasttext(model_path)
+
+  word = "গ্রাম"
+  word_vector = bft.get_word_vector(model_path, word)
   print(word_vector.shape)
-  print(word_vector)
   ```
 
+### Generate Vector File from Fasttext Binary Model
+
+```py
+from bnlp.embedding.fasttext import BengaliFasttext
+
+model_path = "mymodel.bin"
+bft = BengaliFasttext(model_path)
+
+out_vector_name = "myvector.txt"
+bft.bin2vec(out_vector_name)
+```
+
 ### Train Bengali FastText Model
 
 Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
 
   ```py
-  from bnlp.embedding.fasttext import BengaliFasttext
+  from bnlp.embedding.fasttext import FasttextTrainer
+
+  trainer = FasttextTrainer()
 
-  bft = BengaliFasttext()
   data = "raw_text.txt"
   model_name = "saved_model.bin"
   epoch = 50
-  bft.train(data, model_name, epoch)
+  trainer.train(data, model_name, epoch)
   ```
 
-### Generate Vector File from Fasttext Binary Model
-
-```py
-from bnlp.embedding.fasttext import BengaliFasttext
-
-bft = BengaliFasttext()
-
-model_path = "mymodel.bin"
-out_vector_name = "myvector.txt"
-bft.bin2vec(model_path, out_vector_name)
-```
-
 ## Bengali GloVe Word Vectors
 
 We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
 You can download and use it on your different machine learning purposes.
 
 ```py
 from bnlp import BengaliGlove
+
 glove_path = "bn_glove.39M.100d.txt"
+bengali_glove = BengaliGlove(glove_path)
+
 word = "গ্রাম"
-bng = BengaliGlove()
-res = bng.closest_word(glove_path, word)
-print(res)
-vec = bng.word2vec(glove_path, word)
-print(vec)
+vector = bengali_glove.get_word_vector(word)
+print(vector.shape)
+
+similar_words = bengali_glove.get_closest_word(glove_path, word)
+print(similar_words)
 ```
 
 ## Document Embedding
 
 ### Bengali Doc2Vec
 #### Get document vector from input document
 
 ```py
 from bnlp import BengaliDoc2vec
 
-bn_doc2vec = BengaliDoc2vec()
-
 model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+bn_doc2vec = BengaliDoc2vec(model_path)
+
 document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
+vector = bn_doc2vec.get_document_vector(text)
+print(vector.shape)
 
-vector = bn_doc2vec.get_document_vector(model_path, text)
-print(vector)
 ```
 
 #### Find document similarity between two document
 
 ```py
 from bnlp import BengaliDoc2vec
 
-bn_doc2vec = BengaliDoc2vec()
-
 model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+bn_doc2vec = BengaliDoc2vec(model_path)
+
 article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
 similarity = bn_doc2vec.get_document_similarity(
-  model_path,
   article_1,
   article_2
 )
 print(similarity)
+
 ```
 
 #### Train doc2vec vector with custom text files
 
 ```py
-from bnlp import BengaliDoc2vec
+from bnlp import BengaliDoc2vecTrainer
 
-bn_doc2vec = BengaliDoc2vec()
+trainer = BengaliDoc2vecTrainer()
 
 text_files = "path/myfiles"
 checkpoint_path = "msc/logs"
 
-bn_doc2vec.train_doc2vec(
+trainer.train(
   text_files,
   checkpoint_path=checkpoint_path,
   vector_size=100,
   min_count=2,
   epochs=10
 )
 
@@ -341,89 +359,88 @@
 ## Bengali POS Tagging
 
 ### Bengali CRF POS Tagging
 
 #### Find Pos Tag Using Pretrained Model
 
 ```py
-from bnlp import POS
-bn_pos = POS()
+from bnlp import BengaliPOS
+
 model_path = "model/bn_pos.pkl"
+bn_pos = BengaliPOS(model_path)
+
 text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
-res = bn_pos.tag(model_path, text)
+res = bn_pos.tag(text)
 print(res)
 # [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
 ```
 
 #### Train POS Tag Model
 
 ```py
-from bnlp import POS
-bn_pos = POS()
+from bnlp import CRFTaggerTrainer
+
+trainer = CRFTaggerTrainer()
+
 model_name = "pos_model.pkl"
 train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা',  'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
 test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-bn_pos.train(model_name, train_data, test_data)
+trainer.train(model_name, train_data, test_data)
+
 ```
 
 ## Bengali NER
 
 ### Bengali CRF NER
 
 #### Find NER Tag Using Pretrained Model
 
 ```py
-from bnlp import NER
-bn_ner = NER()
+from bnlp import BengaliNER
+
 model_path = "model/bn_ner.pkl"
+bn_ner = BengaliNER(model_path)
+
 text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
-result = bn_ner.tag(model_path, text)
+result = bn_ner.tag(text)
 print(result)
 # [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
 ```
 
 #### Train NER Tag Model
 
 ```py
-from bnlp import NER
-bn_ner = NER()
+from bnlp import CRFTaggerTrainer
+
+trainer = CRFTaggerTrainer()
+
 model_name = "ner_model.pkl"
 train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
 test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-bn_ner.train(model_name, train_data, test_data)
+trainer.train(model_name, train_data, test_data)
 ```
 
 
 ## Bengali Corpus Class
 
 ### Stopwords and Punctuations
 
 ```py
-from bnlp.corpus import stopwords, punctuations, letters, digits
-
-print(stopwords)
-print(punctuations)
-print(letters)
-print(digits)
-```
-
-### Remove stopwords from Text
+from bnlp import BengaliCorpus as corpus
 
-```py
-from bnlp.corpus import stopwords
-from bnlp.corpus.util import remove_stopwords
+print(corpus.stopwords)
+print(corpus.punctuations)
+print(corpus.letters)
+print(corpus.digits)
+print(corpus.vowels)
 
-raw_text = 'আমি ভাত খাই।'
-result = remove_stopwords(raw_text, stopwords)
-print(result)
-# ['ভাত', 'খাই', '।']
 ```
 
 ## Text Cleaning
 We adopted different text cleaning formula, codes from [clean-text](https://github.com/jfilter/clean-text) and modified for Bangla. Now you can normalize and clean your text using the following methods.
 
 ```py
 from bnlp import CleanText
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/cleantext/clean.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/cleantext/clean.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This cleantext scripts functions solely depends on clean-text library.
 Most of the functions are copied from clean-text.
 """
 import re
-from bnlp.corpus import punctuations
 from bnlp.cleantext import constants
+from bnlp.corpus.corpus import BengaliCorpus as corpus
 
 from ftfy import fix_text
 from unicodedata import category, normalize
 from emoji import UNICODE_EMOJI, demojize, emojize
 
 def fix_bad_unicode(text, normalization="NFC"):
     return fix_text(text, normalization=normalization)
@@ -53,15 +53,15 @@
 def remove_emoji(text):
     return remove_substrings(text, UNICODE_EMOJI["en"])
 
 def remove_number_or_digit(text, replace_with=""):
     return re.sub(constants.BANGLA_DIGIT_REGEX, replace_with, text)
 
 def remove_punctuations(text, replace_with=""):
-    for punc in punctuations:
+    for punc in corpus.punctuations:
         print(punc)
         text = text.replace(punc, replace_with)
     
     return text
 
 class CleanText(object):
     def __init__(
@@ -93,15 +93,15 @@
         
         self.replace_with_url = replace_with_url
         self.replace_with_email = replace_with_email
         self.replace_with_number = replace_with_number
         self.replace_with_digit = replace_with_digit
         self.replace_with_punct = replace_with_punct
 
-    def __call__(self, text):
+    def __call__(self, text: str) -> str:
         if text is None:
             text = ""
         text = str(text)
         text = fix_strange_quotes(text)
 
         if self.fix_unicode:
             text = fix_bad_unicode(text)
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/cleantext/constants.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/cleantext/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 Constant symbols and compiled RegExs use for cleaning.
 This part solely copied from package clean-text
 """
 import re
 import sys
 import unicodedata
 
-# EMOJI_LANGUAGE = ['en', 'es', 'pt', 'it', 'fr', 'de', 'fa', 'id', 'zh', 'alias']
 
 BANGLA_DIGIT_REGEX = re.compile(
     r'[০-৯]+'
 )
 
 # taken hostname, domainname, tld from URL regex below
 EMAIL_REGEX = re.compile(
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/embedding/doc2vec.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/embedding/doc2vec.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,94 @@
+import warnings
+warnings.filterwarnings("ignore")
+
 import os
 import glob
 import gensim
+import numpy as np
 from tqdm import tqdm
 from scipy import spatial
+from typing import Callable, List
 from gensim.models.doc2vec import Doc2Vec
+
 from bnlp.tokenizer.basic import BasicTokenizer
 
 default_tokenizer = BasicTokenizer()
 
 
-def read_corpus(files, tokenizer=None):
+def _read_corpus(files: List[str], tokenizer=None):
     for i, file in tqdm(enumerate(files)):
         with open(file) as f:
             text = f.read()
             if tokenizer:
                 tokens = tokenizer(text)
             else:
                 tokens = default_tokenizer.tokenize(text)
             yield gensim.models.doc2vec.TaggedDocument(tokens, [i])
 
 
 class BengaliDoc2vec:
-    def __init__(self, tokenizer=None):
+    def __init__(
+        self,
+        model_path: str,
+        tokenizer: Callable = None
+        ):
         self.tokenizer = tokenizer
+        self.model = Doc2Vec.load(model_path)
 
-    def get_document_vector(self, model_path, document):
+    def get_document_vector(self, document: str) -> np.ndarray:
         """Get document vector using trained doc2vec model
 
         Args:
-            model_path (bin): trained doc2vec model path
             document (str): input documents
 
         Returns:
             ndarray: generated vector
         """
-        model = Doc2Vec.load(model_path)
+        
         if self.tokenizer:
             tokens = self.tokenizer(document)
         else:
             tokens = default_tokenizer.tokenize(document)
 
-        vector = model.infer_vector(tokens)
+        vector = self.model.infer_vector(tokens)
 
         return vector
 
-    def get_document_similarity(self, model_path, document_1, document_2):
+    def get_document_similarity(self, document_1: str, document_2: str) -> float:
         """Get document similarity score from input two document using pretrained doc2vec model
 
         Args:
-            model_path (bin): pretrained doc2vec
             document_1 (str): input document
             document_2 (str): input document
 
         Returns:
             float: output similarity score
         """
         if self.tokenizer:
             document_1_tokens = self.tokenizer(document_1)
             document_2_tokens = self.tokenizer(document_2)
         else:
             document_1_tokens = default_tokenizer.tokenize(document_1)
             document_2_tokens = default_tokenizer.tokenize(document_2)
 
-        model = Doc2Vec.load(model_path)
-
-        document_1_vector = model.infer_vector(document_1_tokens)
-        document_2_vector = model.infer_vector(document_2_tokens)
+        document_1_vector = self.model.infer_vector(document_1_tokens)
+        document_2_vector = self.model.infer_vector(document_2_tokens)
 
         similarity = round(
             1 - spatial.distance.cosine(document_1_vector, document_2_vector), 2
         )
 
         return similarity
 
-    def train_doc2vec(
+class BengaliDoc2vecTrainer:
+    def __init__(self, tokenizer: Callable = None):
+        self.tokenizer = tokenizer
+
+    def train(
         self,
         text_files,
         checkpoint_path="ckpt",
         vector_size=100,
         min_count=2,
         epochs=10,
     ):
@@ -88,20 +99,20 @@
             checkpoint_path (str, optional): checkpoint save path. Defaults to 'ckpt'.
             vector_size (int, optional): size of the vector. Defaults to 100.
             min_count (int, optional): minimum word count. Defaults to 2.
             epochs (int, optional): training iteration number. Defaults to 10.
         """
         text_files = glob.glob(text_files + "/*.txt")
         if self.tokenizer:
-            train_corpus = list(read_corpus(text_files, self.tokenizer))
+            train_corpus = list(_read_corpus(text_files, self.tokenizer))
         else:
-            train_corpus = list(read_corpus(text_files))
+            train_corpus = list(_read_corpus(text_files))
 
         model = Doc2Vec(vector_size=vector_size, min_count=min_count, epochs=epochs)
         model.build_vocab(train_corpus)
         model.train(
             train_corpus, total_examples=model.corpus_count, epochs=model.epochs
         )
 
         os.makedirs(checkpoint_path, exist_ok=True)
         output_model_name = os.path.join(checkpoint_path, "custom_doc2vec_model.model")
-        model.save(output_model_name)
+        model.save(output_model_name)
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/embedding/fasttext.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/embedding/fasttext.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,53 @@
 import multiprocessing
+import numpy as np
 
 try:
     import fasttext
 except ImportError:
     print("fasttext not installed. Install it by 'pip install fasttext'")
 
-
 class BengaliFasttext:
+    def __init__(self, model_path: str):
+        self.model = fasttext.load_model(model_path)
+
+    def get_word_vector(self, word: str) -> np.ndarray:
+        """generate word vector from given input word
+
+        Args:
+            word (str): input word or token
+
+        Returns:
+            str: word or token vector
+        """
+        word_vector = self.model[word]
+
+        return word_vector
+
+    def bin2vec(self, vector_name: str):
+        """Generate vector text file from fasttext binary model
+
+        Args:
+            vector_name (str): name of the output vector with extension
+        """
+        output_vector = open(vector_name, "w")
+
+        words = self.model.get_words()
+        vocab_len = str(len(words))
+        dimension = str(self.model.get_dimension())
+        output_vector.write(vocab_len + " " + dimension + "\n")
+        for w in words:
+            v = self.model.get_word_vector(w)
+            vstr = ""
+            for vi in v:
+                vstr += " " + str(vi)
+            output_vector.write(w + vstr + "\n")
+        output_vector.close()
+
+class FasttextTrainer:
     def train(
         self,
         data,
         model_name,
         epoch,
         lr=0.05,
         dim=300,
@@ -57,44 +94,7 @@
             wordNgrams=wordNgrams,
             loss=loss,
             bucket=bucket,
             thread=thread,
         )
         print(f"training done! saving as {model_name}")
         model.save_model(model_name)
-
-    def bin2vec(self, bin_model, vector_name):
-        """Generate vector text file from fasttext binary model
-
-        Args:
-            bin_model (bin): fasttext trained binary model
-            vector_name (str): name of the output vector with extension
-        """
-        output_vector = open(vector_name, "w")
-
-        f = fasttext.load_model(bin_model)
-        words = f.get_words()
-        vocab_len = str(len(words))
-        dimension = str(f.get_dimension())
-        output_vector.write(vocab_len + " " + dimension + "\n")
-        for w in words:
-            v = f.get_word_vector(w)
-            vstr = ""
-            for vi in v:
-                vstr += " " + str(vi)
-            output_vector.write(w + vstr + "\n")
-        output_vector.close()
-
-    def generate_word_vector(self, model_path, word):
-        """generate word vector from given input word
-
-        Args:
-            model_path (str): fasttext trained model path
-            word (str): input word or token
-
-        Returns:
-            str: word or token vector
-        """
-        model = fasttext.load_model(model_path)
-        word_vector = model[word]
-
-        return word_vector
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/embedding/word2vec.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/embedding/word2vec.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,39 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from __future__ import print_function
 
+import warnings
+warnings.filterwarnings("ignore")
+
 import os
 import sys
 import multiprocessing
+import numpy as np
 from gensim.models import Word2Vec
 from gensim.models.word2vec import LineSentence
 from bnlp.tokenizer.nltk import NLTKTokenizer
 
+from typing import List, Tuple
+
+
+class BengaliWord2Vec:
+    def __init__(self, model_path: str):
+        self.model = Word2Vec.load(model_path)
+    
+    def get_word_vector(self, word: str) -> np.ndarray:
+        vector = self.model.wv[word]
+        return vector
+
+    def get_most_similar_words(self, word: str, topn: int = 10) -> List[Tuple[str, float]]:
+        
+        similar_word = self.model.wv.most_similar(word, topn=topn)
+        return similar_word
+
 
 class MyCorpus:
     """An iterator that yields sentences (lists of str).
     We used NLTKTokenizer from bnlp to tokenize sentence words
     """
 
     def __init__(self, data_path):
@@ -24,15 +44,15 @@
         for line in open(self.data_path):
             sentences = self.bnltk.sentence_tokenize(line)
             for sentence in sentences:
                 tokens = self.bnltk.word_tokenize(sentence)
                 yield tokens
 
 
-class BengaliWord2Vec:
+class Word2VecTraining:
     def train(
         self,
         data_path,
         model_name,
         vector_name,
         vector_size=100,
         alpha=0.025,
@@ -105,15 +125,15 @@
             callbacks=callbacks,
         )
         # getting the training loss value
         training_loss = model.get_latest_training_loss()
 
         print("train completed successfully")
         print(f"trianing loss: {training_loss}")
-        print(f"model and vector saving...")
+        print("model and vector saving...")
         model.save(model_name)
         model.wv.save_word2vec_format(vector_name, binary=False)
         print(f"model and vector saved as {model_name} and {vector_name}")
 
     def pretrain(
         self, model_path, new_sentences, output_model_name, output_vector_name, epochs=5
     ):
@@ -124,47 +144,27 @@
             new_sentences (list): list of new sentences
             output_model_name (str): output model name
             output_vector_name (str): output vector name
             epoch(int): number of training iteration
         """
         if isinstance(new_sentences, str):
             new_sentences = MyCorpus(new_sentences)
-        print(f"model loading ....")
+        print("model loading ....")
         model = Word2Vec.load(model_path)
-        print(f"vocab building with new sentences")
+        print("vocab building with new sentences")
         model.build_vocab(new_sentences, update=True)
         print("pre-training started.......")
         print(
             "please wait.....it will take time according to your data size and computation capability"
         )
         model.train(new_sentences, total_examples=model.corpus_count, epochs=epochs)
         # getting the training loss value
         training_loss = model.get_latest_training_loss()
 
         print("pre-train completed successfully")
         print(f"pre-trianing loss: {training_loss}")
-        print(f"model and vector saving...")
+        print("model and vector saving...")
         model.save(output_model_name)
         model.wv.save_word2vec_format(output_vector_name, binary=False)
         print(
             f"model and vector saved as {output_model_name} and {output_vector_name}"
-        )
-
-    def generate_word_vector(self, model_path, input_word):
-        """
-        :model_name: (str) model path with file name and extension
-        :input_word: (str) word to generate vector
-
-        """
-        model = Word2Vec.load(model_path)
-        vector = model.wv[input_word]
-        return vector
-
-    def most_similar(self, model_path, word, topn=10):
-        """
-        :model_name: (str) model path with file name and extension
-        :word: (str) word to find similar word
-
-        """
-        model = Word2Vec.load(model_path)
-        similar_word = model.wv.most_similar(word, topn=topn)
-        return similar_word
+        )
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/pos.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/utils/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-"""
-tool: We used sklearn crf_suite for bengali pos tagging
-https://sklearn-crfsuite.readthedocs.io/en/latest/
-"""
-
 import pickle
 from sklearn_crfsuite import CRF
-from sklearn_crfsuite import metrics
 from nltk.tag.util import untag
-from bnlp.tokenizer.basic import BasicTokenizer
-
 
 def features(sentence, index):
     """sentence: [w1, w2, ...], index: the index of the word"""
     return {
         "word": sentence[index],
         "is_first": index == 0,
         "is_last": index == len(sentence) - 1,
@@ -28,60 +20,24 @@
         "prev_word": "" if index == 0 else sentence[index - 1],
         "next_word": "" if index == len(sentence) - 1 else sentence[index + 1],
         "has_hyphen": "-" in sentence[index],
         "is_numeric": sentence[index].isdigit(),
         "capitals_inside": sentence[index][1:].lower() != sentence[index][1:],
     }
 
-
 def transform_to_dataset(tagged_sentences):
     X, y = [], []
 
     for tagged in tagged_sentences:
         try:
             X.append([features(untag(tagged), index) for index in range(len(tagged))])
             y.append([tag for _, tag in tagged])
         except Exception as e:
             print(e)
 
     return X, y
 
-
-class POS:
-    def tag(self, model_path, text):
-        with open(model_path, "rb") as pkl_model:
-            model = pickle.load(pkl_model)
-            if not isinstance(text, list):
-                basic_t = BasicTokenizer()
-                tokens = basic_t.tokenize(text)
-            else:
-                tokens = text
-            sentence_features = [
-                features(tokens, index) for index in range(len(tokens))
-            ]
-            result = list(zip(tokens, model.predict([sentence_features])[0]))
-            pkl_model.close()
-            return result
-
-    def train(self, model_name, train_data, test_data, average="micro"):
-
-        X_train, y_train = transform_to_dataset(train_data)
-        X_test, y_test = transform_to_dataset(test_data)
-        print(len(X_train))
-        print(len(X_test))
-
-        print("Training Started........")
-        print("it will take time according to your dataset size..")
-        model = CRF()
-        model.fit(X_train, y_train)
-        print("Training Finished!")
-
-        print("Evaluating with Test Data...")
-        y_pred = model.predict(X_test)
-        print("Accuracy is: ")
-        print(metrics.flat_accuracy_score(y_test, y_pred))
-
-        print(f"F1 Score({average}) is: ")
-        print(metrics.flat_f1_score(y_test, y_pred, average=average))
-
-        pickle.dump(model, open(model_name, "wb"))
-        print("Model Saved!")
+def load_pickle_model(model_path: str) -> CRF:
+    with open(model_path, "rb") as pkl_model:
+        model = pickle.load(pkl_model)
+        
+    return model
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/tokenizer/basic.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/tokenizer/basic.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Basic Tokenization
 Basic tokenization tokenize sentence using white spaces, punctuation mark
 Code shamelessly copied from BERT tokenization
 To check Original Code: https://github.com/google-research/bert/blob/master/tokenization.py
 """
 import six
 import unicodedata
-
+from typing import List
 
 def convert_to_unicode(text):
     """Converts `text` to Unicode (if it's not already), assuming utf-8 input."""
     if six.PY3:
         if isinstance(text, str):
             return text
         elif isinstance(text, bytes):
@@ -24,22 +24,20 @@
             return text
         else:
             raise ValueError("Unsupported string type: %s" % (type(text)))
     else:
         raise ValueError("Not running on Python2 or Python 3?")
 
 
-def whitespace_tokenize(text):
+def whitespace_tokenize(text: str) -> List[str]:
     """Runs basic whitespace cleaning and splitting on a piece of text."""
     text = text.strip()
-    # print("Text: ", text)
     if not text:
         return []
     tokens = text.split()
-    # print("tokens : ", tokens)
     return tokens
 
 
 def _is_punctuation(char):
     """Checks whether `chars` is a punctuation character."""
     cp = ord(char)
     # We treat all non-letter/number ASCII as punctuation.
@@ -55,42 +53,38 @@
         return True
     cat = unicodedata.category(char)
     if cat.startswith("P"):
         return True
     return False
 
 
+DUMMYTOKEN = 'XTEMPDOT'
+
 class BasicTokenizer:
     """Runs basic tokenization (punctuation splitting, lower casing, etc.)."""
 
-    def tokenize(self, text):
+    def __call__(self, text: str) -> List[str]:
+        return self.tokenize(text)
+
+    def tokenize(self, text: str) -> List[str]:
         """Tokenizes a piece of text."""
         text = convert_to_unicode(text)
+        # handle (.) in bangla text
+        text = text.replace('.', DUMMYTOKEN)
 
         orig_tokens = whitespace_tokenize(text)
-        # print("original tokens: ", orig_tokens)
         split_tokens = []
         for token in orig_tokens:
             split_tokens.extend(self._run_split_on_punc(token))
 
-        # print("split tokens: ", split_tokens)
         output_tokens = whitespace_tokenize(" ".join(split_tokens))
+        # get (.) back in output tokens
+        output_tokens = [token.replace(DUMMYTOKEN, '.') for token in output_tokens]
         return output_tokens
-
-    def _run_strip_accents(self, text):
-        """Strips accents from a piece of text."""
-        text = unicodedata.normalize("NFD", text)
-        output = []
-        for char in text:
-            cat = unicodedata.category(char)
-            if cat == "Mn":
-                continue
-            output.append(char)
-        return "".join(output)
-
+        
     def _run_split_on_punc(self, text):
         """Splits punctuation on a piece of text."""
         chars = list(text)
         i = 0
         start_new_word = True
         output = []
         while i < len(chars):
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/tokenizer/nltk.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/tokenizer/nltk.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import nltk
+from typing import List
 
 try:
     nltk.data.find("tokenizers/punkt")
 except LookupError:
     print("punkt not found. downloading...")
     nltk.download("punkt")
 
-DUMMYTOKEN = "XTEMPTOKEN"
+
+DUMMYTOKEN = "XTEMPDOT"
 
 class NLTKTokenizer:
-    def word_tokenize(self, text):
+    def word_tokenize(self, text: str) -> List[str]:
+        text = text.replace(".", DUMMYTOKEN)  # to deal with abbreviations
+        text = text.replace("।", ".")
         tokens = nltk.word_tokenize(text)
         new_tokens = []
         for token in tokens:
-            if token[-1] == "।" and len(token) > 1:
-                token_1 = token[:-1]
-                token_2 = token[-1]
-                new_tokens.append(token_1)
-                new_tokens.append(token_2)
-            else:
-                new_tokens.append(token)
+            token = token.replace(".", "।")  # do operation in reverse order
+            token = token.replace(DUMMYTOKEN, ".")
+            new_tokens.append(token)
+
         return new_tokens
 
-    def sentence_tokenize(self, text):
+    def sentence_tokenize(self, text: str) -> List[str]:
         text = text.replace(".", DUMMYTOKEN)  # to deal with abbreviations
         text = text.replace("।", ".")
         tokens = nltk.tokenize.sent_tokenize(text)
         new_tokens = []
         for token in tokens:
             token = token.replace(".", "।")  # do operation in reverse order
             token = token.replace(DUMMYTOKEN, ".")
```

### Comparing `bnlp_toolkit-3.3.2/bnlp/tokenizer/sentencepiece.py` & `bnlp_toolkit-4.0.0.dev0/bnlp/tokenizer/sentencepiece.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 import os
+from typing import List
 import sentencepiece as bsp
 
 
 class SentencepieceTokenizer:
-    def train(self, data, model_prefix, vocab_size):
-        """
-        :data: (str) data path with extension
-        :model_prefix: (str) model name prefix
-        :vocab_size: (int) size of train vocabulary
+    def __init__(self, model_path: str):
+        self.model = bsp.SentencePieceProcessor()
+        self.model.Load(model_path)
 
-        """
+    def tokenize(self, text: str) -> List[str]:
+        tokens = self.model.EncodeAsPieces(text)
+
+        return tokens
+
+    def text2id(self, text: str) -> List[int]:
+        ids = self.model.EncodeAsIds(text)
+        return ids
+
+    def id2text(self, ids: List[int]) -> str:
+        text = self.model.DecodeIds(ids)
+        return text
+
+class SentencepieceTrainer:
+    def __init__(self, data, vocab_size, model_prefix):
+        self.data = data
+        self.vocab_size = vocab_size
+        self.model_prefix = model_prefix
+
+    def train(self):
         train_args = (
             "--model_prefix="
-            + model_prefix
+            + self.model_prefix
             + " --input="
-            + data
+            + self.data
             + " --vocab_size="
-            + str(vocab_size)
+            + str(self.vocab_size)
         )
         bsp.SentencePieceTrainer.train(train_args)
         print(
             "%s.model and %s.vocab is saved on your current directory"
-            % (model_prefix, model_prefix)
-        )
-
-    def tokenize(self, model_path, text):
-        """
-        :model_path: (str) path of the model with extension
-        :text: (str) input text for tokenization
-
-        """
-        model = bsp.SentencePieceProcessor()
-        model.Load(model_path)
-        tokens = model.EncodeAsPieces(text)
-
-        return tokens
-
-    def text2id(self, model_path, text):
-        model = bsp.SentencePieceProcessor()
-        model.Load(model_path)
-        ids = model.EncodeAsIds(text)
-        return ids
-
-    def id2text(self, model_path, ids):
-        model = bsp.SentencePieceProcessor()
-        model.Load(model_path)
-        text = model.DecodeIds(ids)
-        return text
+            % (self.model_prefix, self.model_prefix)
+        )
```

### Comparing `bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/PKG-INFO` & `bnlp_toolkit-4.0.0.dev0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: bnlp-toolkit
-Version: 3.3.2
+Name: bnlp_toolkit
+Version: 4.0.0.dev0
 Summary: BNLP is a natural language processing toolkit for Bengali Language
 Home-page: https://github.com/sagorbrur/bnlp
 Author: Sagor Sarker
 Author-email: sagorhem3532@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -75,15 +75,15 @@
   pip install bnlp_toolkit
   ```
   **or Upgrade**
 
   ```
   pip install -U bnlp_toolkit
   ```
-  - Python: 3.6, 3.7, 3.8, 3.9
+  - Python: 3.6, 3.7, 3.8, 3.9, 3.10
   - OS: Linux, Windows, Mac
 
 
 
 ## Pretrained Model
 
 ### Download Links
@@ -115,238 +115,256 @@
 ## Tokenization
 
 ### Basic Tokenizer
 
   ```py
   from bnlp import BasicTokenizer
   
-  basic_tokenizer = BasicTokenizer()
+  tokenizer = BasicTokenizer()
+
   raw_text = "আমি বাংলায় গান গাই।"
-  tokens = basic_tokenizer.tokenize(raw_text)
+  tokens = tokenizer(raw_text)
   print(tokens)
-
   # output: ["আমি", "বাংলায়", "গান", "গাই", "।"]
   ```
 
 ### NLTK Tokenization
 
   ```py
   from bnlp import NLTKTokenizer
 
   bnltk = NLTKTokenizer()
+
   text = "আমি ভাত খাই। সে বাজারে যায়। তিনি কি সত্যিই ভালো মানুষ?"
   word_tokens = bnltk.word_tokenize(text)
   sentence_tokens = bnltk.sentence_tokenize(text)
   print(word_tokens)
   print(sentence_tokens)
-
   # output
   # word_token: ["আমি", "ভাত", "খাই", "।", "সে", "বাজারে", "যায়", "।", "তিনি", "কি", "সত্যিই", "ভালো", "মানুষ", "?"]
   # sentence_token: ["আমি ভাত খাই।", "সে বাজারে যায়।", "তিনি কি সত্যিই ভালো মানুষ?"]
   ```
 
 
 ### Bengali SentencePiece Tokenization
 
 #### Tokenization using trained model
 ```py
 from bnlp import SentencepieceTokenizer
 
-bsp = SentencepieceTokenizer()
 model_path = "./model/bn_spm.model"
+bsp = SentencepieceTokenizer(model_path)
+
+
 input_text = "আমি ভাত খাই। সে বাজারে যায়।"
-tokens = bsp.tokenize(model_path, input_text)
+tokens = bsp.tokenize(input_text)
 print(tokens)
-text2id = bsp.text2id(model_path, input_text)
+text2id = bsp.text2id(input_text)
 print(text2id)
-id2text = bsp.id2text(model_path, text2id)
+id2text = bsp.id2text(text2id)
 print(id2text)
 ```
 
 #### Training SentencePiece
 ```py
-from bnlp import SentencepieceTokenizer
+from bnlp import SentencepieceTrainer
 
-bsp = SentencepieceTokenizer()
 data = "raw_text.txt"
-model_prefix = "test"
-vocab_size = 5
-bsp.train(data, model_prefix, vocab_size)
+vocab_size = 32000
+model_prefix = "model"
+
+trainer = SentencepieceTrainer(
+   data=data,
+   vocab_size=vocab_size,
+   model_prefix=model_prefix
+)
+trainer.train()
+
 ```
 
 ## Word Embedding
 
 ### Bengali Word2Vec
 
 #### Generate Vector using pretrain model
 
 ```py
 from bnlp import BengaliWord2Vec
 
-bwv = BengaliWord2Vec()
 model_path = "bengali_word2vec.model"
+bwv = BengaliWord2Vec(model_path)
+
 word = 'গ্রাম'
-vector = bwv.generate_word_vector(model_path, word)
+vector = bwv.get_word_vector(word)
 print(vector.shape)
-print(vector)
 ```
 
 #### Find Most Similar Word Using Pretrained Model
 
 ```py
 from bnlp import BengaliWord2Vec
 
-bwv = BengaliWord2Vec()
 model_path = "bengali_word2vec.model"
+bwv = BengaliWord2Vec(model_path)
+
 word = 'গ্রাম'
-similar = bwv.most_similar(model_path, word, topn=10)
-print(similar)
+similar_words = bwv.get_most_similar_words(word, topn=10)
+print(similar_words)
 ```
+
 #### Train Bengali Word2Vec with your own data
 
 Train Bengali word2vec with your custom raw data or tokenized sentences.
 
 Custom tokenized sentence format example:
 ```py
 sentences = [['আমি', 'ভাত', 'খাই', '।'], ['সে', 'বাজারে', 'যায়', '।']]
 ```
 Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
 ```py
-from bnlp import BengaliWord2Vec
-bwv = BengaliWord2Vec()
+from bnlp import Word2VecTraining
+
+trainer = Word2VecTraining()
+
 data_file = "raw_text.txt" # or you can pass custom sentence tokens as list of list
 model_name = "test_model.model"
 vector_name = "test_vector.vector"
-bwv.train(data_file, model_name, vector_name, epochs=5)
+trainer.train(data_file, model_name, vector_name, epochs=5)
 ```
 
 #### Pre-train or resume word2vec training with same or new corpus or tokenized sentences
 
 Check [gensim word2vec api](https://radimrehurek.com/gensim/models/word2vec.html#gensim.models.word2vec.Word2Vec) for details of training parameter
 
 ```py
-from bnlp import BengaliWord2Vec
-bwv = BengaliWord2Vec()
+from bnlp import Word2VecTraining
+
+trainer = Word2VecTraining()
 
 trained_model_path = "mytrained_model.model"
 data_file = "raw_text.txt"
 model_name = "test_model.model"
 vector_name = "test_vector.vector"
-bwv.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+trainer.pretrain(trained_model_path, data_file, model_name, vector_name, epochs=5)
+
 ```
 
 ### Bengali FastText
 
 To use `fasttext` you need to install fasttext manually by `pip install fasttext==0.9.2`
 
 NB: `fasttext` may not be worked in `windows`, it will only work in `linux`
 
 ### Generate Vector Using Pretrained Model
 
   ```py
   from bnlp.embedding.fasttext import BengaliFasttext
 
-  bft = BengaliFasttext()
-  word = "গ্রাম"
   model_path = "bengali_fasttext_wiki.bin"
-  word_vector = bft.generate_word_vector(model_path, word)
+  bft = BengaliFasttext(model_path)
+
+  word = "গ্রাম"
+  word_vector = bft.get_word_vector(model_path, word)
   print(word_vector.shape)
-  print(word_vector)
   ```
 
+### Generate Vector File from Fasttext Binary Model
+
+```py
+from bnlp.embedding.fasttext import BengaliFasttext
+
+model_path = "mymodel.bin"
+bft = BengaliFasttext(model_path)
+
+out_vector_name = "myvector.txt"
+bft.bin2vec(out_vector_name)
+```
+
 ### Train Bengali FastText Model
 
 Check [fasttext documentation](https://fasttext.cc/docs/en/options.html) for details of training parameter
 
   ```py
-  from bnlp.embedding.fasttext import BengaliFasttext
+  from bnlp.embedding.fasttext import FasttextTrainer
+
+  trainer = FasttextTrainer()
 
-  bft = BengaliFasttext()
   data = "raw_text.txt"
   model_name = "saved_model.bin"
   epoch = 50
-  bft.train(data, model_name, epoch)
+  trainer.train(data, model_name, epoch)
   ```
 
-### Generate Vector File from Fasttext Binary Model
-
-```py
-from bnlp.embedding.fasttext import BengaliFasttext
-
-bft = BengaliFasttext()
-
-model_path = "mymodel.bin"
-out_vector_name = "myvector.txt"
-bft.bin2vec(model_path, out_vector_name)
-```
-
 ## Bengali GloVe Word Vectors
 
 We trained glove model with bengali data(wiki+news articles) and published bengali glove word vectors</br>
 You can download and use it on your different machine learning purposes.
 
 ```py
 from bnlp import BengaliGlove
+
 glove_path = "bn_glove.39M.100d.txt"
+bengali_glove = BengaliGlove(glove_path)
+
 word = "গ্রাম"
-bng = BengaliGlove()
-res = bng.closest_word(glove_path, word)
-print(res)
-vec = bng.word2vec(glove_path, word)
-print(vec)
+vector = bengali_glove.get_word_vector(word)
+print(vector.shape)
+
+similar_words = bengali_glove.get_closest_word(glove_path, word)
+print(similar_words)
 ```
 
 ## Document Embedding
 
 ### Bengali Doc2Vec
 #### Get document vector from input document
 
 ```py
 from bnlp import BengaliDoc2vec
 
-bn_doc2vec = BengaliDoc2vec()
-
 model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+bn_doc2vec = BengaliDoc2vec(model_path)
+
 document = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
+vector = bn_doc2vec.get_document_vector(text)
+print(vector.shape)
 
-vector = bn_doc2vec.get_document_vector(model_path, text)
-print(vector)
 ```
 
 #### Find document similarity between two document
 
 ```py
 from bnlp import BengaliDoc2vec
 
-bn_doc2vec = BengaliDoc2vec()
-
 model_path = "bangla_news_article_doc2vec.model" # keep other .npy model files also in same folder
+bn_doc2vec = BengaliDoc2vec(model_path)
+
 article_1 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 article_2 = "রাষ্ট্রবিরোধী ও উসকানিমূলক বক্তব্য দেওয়ার অভিযোগে গাজীপুরের গাছা থানায় ডিজিটাল নিরাপত্তা আইনে করা মামলায় আলোচিত ‘শিশুবক্তা’ রফিকুল ইসলামের বিরুদ্ধে অভিযোগ গঠন করেছেন আদালত। ফলে মামলার আনুষ্ঠানিক বিচার শুরু হলো। আজ বুধবার (২৬ জানুয়ারি) ঢাকার সাইবার ট্রাইব্যুনালের বিচারক আসসামছ জগলুল হোসেন এ অভিযোগ গঠন করেন। এর আগে, রফিকুল ইসলামকে কারাগার থেকে আদালতে হাজির করা হয়। এরপর তাকে নির্দোষ দাবি করে তার আইনজীবী শোহেল মো. ফজলে রাব্বি অব্যাহতি চেয়ে আবেদন করেন। অন্যদিকে, রাষ্ট্রপক্ষ অভিযোগ গঠনের পক্ষে শুনানি করেন। উভয় পক্ষের শুনানি শেষে আদালত অব্যাহতির আবেদন খারিজ করে অভিযোগ গঠনের মাধ্যমে বিচার শুরুর আদেশ দেন। একইসঙ্গে সাক্ষ্যগ্রহণের জন্য আগামী ২২ ফেব্রুয়ারি দিন ধার্য করেন আদালত।"
 
 similarity = bn_doc2vec.get_document_similarity(
-  model_path,
   article_1,
   article_2
 )
 print(similarity)
+
 ```
 
 #### Train doc2vec vector with custom text files
 
 ```py
-from bnlp import BengaliDoc2vec
+from bnlp import BengaliDoc2vecTrainer
 
-bn_doc2vec = BengaliDoc2vec()
+trainer = BengaliDoc2vecTrainer()
 
 text_files = "path/myfiles"
 checkpoint_path = "msc/logs"
 
-bn_doc2vec.train_doc2vec(
+trainer.train(
   text_files,
   checkpoint_path=checkpoint_path,
   vector_size=100,
   min_count=2,
   epochs=10
 )
 
@@ -356,89 +374,88 @@
 ## Bengali POS Tagging
 
 ### Bengali CRF POS Tagging
 
 #### Find Pos Tag Using Pretrained Model
 
 ```py
-from bnlp import POS
-bn_pos = POS()
+from bnlp import BengaliPOS
+
 model_path = "model/bn_pos.pkl"
+bn_pos = BengaliPOS(model_path)
+
 text = "আমি ভাত খাই।" # or you can pass ['আমি', 'ভাত', 'খাই', '।']
-res = bn_pos.tag(model_path, text)
+res = bn_pos.tag(text)
 print(res)
 # [('আমি', 'PPR'), ('ভাত', 'NC'), ('খাই', 'VM'), ('।', 'PU')]
 ```
 
 #### Train POS Tag Model
 
 ```py
-from bnlp import POS
-bn_pos = POS()
+from bnlp import CRFTaggerTrainer
+
+trainer = CRFTaggerTrainer()
+
 model_name = "pos_model.pkl"
 train_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা',  'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
 test_data = [[('রপ্তানি', 'JJ'), ('দ্রব্য', 'NC'), ('-', 'PU'), ('তাজা', 'JJ'), ('ও', 'CCD'), ('শুকনা', 'JJ'), ('ফল', 'NC'), (',', 'PU'), ('আফিম', 'NC'), (',', 'PU'), ('পশুচর্ম', 'NC'), ('ও', 'CCD'), ('পশম', 'NC'), ('এবং', 'CCD'),('কার্পেট', 'NC'), ('৷', 'PU')], [('মাটি', 'NC'), ('থেকে', 'PP'), ('বড়জোর', 'JQ'), ('চার', 'JQ'), ('পাঁচ', 'JQ'), ('ফুট', 'CCL'), ('উঁচু', 'JJ'), ('হবে', 'VM'), ('৷', 'PU')]]
 
-bn_pos.train(model_name, train_data, test_data)
+trainer.train(model_name, train_data, test_data)
+
 ```
 
 ## Bengali NER
 
 ### Bengali CRF NER
 
 #### Find NER Tag Using Pretrained Model
 
 ```py
-from bnlp import NER
-bn_ner = NER()
+from bnlp import BengaliNER
+
 model_path = "model/bn_ner.pkl"
+bn_ner = BengaliNER(model_path)
+
 text = "সে ঢাকায় থাকে।" # or you can pass ['সে', 'ঢাকায়', 'থাকে', '।']
-result = bn_ner.tag(model_path, text)
+result = bn_ner.tag(text)
 print(result)
 # [('সে', 'O'), ('ঢাকায়', 'S-LOC'), ('থাকে', 'O')]
 ```
 
 #### Train NER Tag Model
 
 ```py
-from bnlp import NER
-bn_ner = NER()
+from bnlp import CRFTaggerTrainer
+
+trainer = CRFTaggerTrainer()
+
 model_name = "ner_model.pkl"
 train_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
 test_data = [[('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')], [('ত্রাণ', 'O'),('ও', 'O'),('সমাজকল্যাণ', 'O'),('সম্পাদক', 'S-PER'),('সুজিত', 'B-PER'),('রায়', 'I-PER'),('নন্দী', 'E-PER'),('প্রমুখ', 'O'),('সংবাদ', 'O'),('সম্মেলনে', 'O'),('উপস্থিত', 'O'),('ছিলেন', 'O')]]
 
-bn_ner.train(model_name, train_data, test_data)
+trainer.train(model_name, train_data, test_data)
 ```
 
 
 ## Bengali Corpus Class
 
 ### Stopwords and Punctuations
 
 ```py
-from bnlp.corpus import stopwords, punctuations, letters, digits
-
-print(stopwords)
-print(punctuations)
-print(letters)
-print(digits)
-```
-
-### Remove stopwords from Text
+from bnlp import BengaliCorpus as corpus
 
-```py
-from bnlp.corpus import stopwords
-from bnlp.corpus.util import remove_stopwords
+print(corpus.stopwords)
+print(corpus.punctuations)
+print(corpus.letters)
+print(corpus.digits)
+print(corpus.vowels)
 
-raw_text = 'আমি ভাত খাই।'
-result = remove_stopwords(raw_text, stopwords)
-print(result)
-# ['ভাত', 'খাই', '।']
 ```
 
 ## Text Cleaning
 We adopted different text cleaning formula, codes from [clean-text](https://github.com/jfilter/clean-text) and modified for Bangla. Now you can normalize and clean your text using the following methods.
 
 ```py
 from bnlp import CleanText
```

### Comparing `bnlp_toolkit-3.3.2/bnlp_toolkit.egg-info/SOURCES.txt` & `bnlp_toolkit-4.0.0.dev0/bnlp_toolkit.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 LICENSE
 README.md
 setup.py
 bnlp/__init__.py
-bnlp/ner.py
-bnlp/pos.py
 bnlp/cleantext/__init__.py
 bnlp/cleantext/clean.py
 bnlp/cleantext/constants.py
 bnlp/corpus/__init__.py
-bnlp/corpus/util.py
+bnlp/corpus/_stopwords.py
+bnlp/corpus/corpus.py
 bnlp/embedding/__init__.py
 bnlp/embedding/doc2vec.py
 bnlp/embedding/fasttext.py
 bnlp/embedding/glove.py
 bnlp/embedding/word2vec.py
+bnlp/token_classification/__init__.py
+bnlp/token_classification/ner.py
+bnlp/token_classification/pos.py
+bnlp/token_classification/token_classification_trainer.py
 bnlp/tokenizer/__init__.py
 bnlp/tokenizer/basic.py
 bnlp/tokenizer/nltk.py
 bnlp/tokenizer/sentencepiece.py
+bnlp/utils/__init__.py
+bnlp/utils/utils.py
 bnlp_toolkit.egg-info/PKG-INFO
 bnlp_toolkit.egg-info/SOURCES.txt
 bnlp_toolkit.egg-info/dependency_links.txt
 bnlp_toolkit.egg-info/requires.txt
-bnlp_toolkit.egg-info/top_level.txt
-tests/test.py
+bnlp_toolkit.egg-info/top_level.txt
```

### Comparing `bnlp_toolkit-3.3.2/setup.py` & `bnlp_toolkit-4.0.0.dev0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import codecs
 import setuptools
 
 
 setuptools.setup(
     name="bnlp_toolkit",
-    version="3.3.2",
+    version="4.0.0dev0",
     author="Sagor Sarker",
     author_email="sagorhem3532@gmail.com",
     description="BNLP is a natural language processing toolkit for Bengali Language",
     long_description=codecs.open("README.md", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/sagorbrur/bnlp",
     license="MIT",
```

