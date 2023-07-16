# Comparing `tmp/cloudlanguagetools-5.7.tar.gz` & `tmp/cloudlanguagetools-5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudlanguagetools-5.7.tar", last modified: Fri Jul 14 14:29:46 2023, max compression
+gzip compressed data, was "cloudlanguagetools-5.8.tar", last modified: Sun Jul 16 13:29:56 2023, max compression
```

## Comparing `cloudlanguagetools-5.7.tar` & `cloudlanguagetools-5.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/
--rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/LICENSE
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/README.rst
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/cloudlanguagetools/
--rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/__init__.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/amazon.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/argostranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/azure.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/cereproc.py
--rw-r--r--   0 luc       (1000) luc       (1000)    16859 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/chatapi.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8739 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/chatmodel.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/constants.py
--rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/deepl.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/dictionarylookup.py
--rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-5.7/cloudlanguagetools/easypronunciation.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6883 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/elevenlabs.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/encryption.py
--rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/epitran.py
--rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/errors.py
--rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/forvo.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/fptai.py
--rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/google.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/keys.py
--rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/languages.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/libretranslate.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/mandarincantonese.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/naver.py
--rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/openai.py
--rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/options.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/pythainlp.py
--rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/service.py
--rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/servicemanager.py
--rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/spacy.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/test_services.py
--rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/tokenization.py
--rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/translationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/transliterationlanguage.py
--rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-5.7/cloudlanguagetools/ttsvoice.py
--rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/vocalware.py
--rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/voicen.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/watson.py
--rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-5.7/cloudlanguagetools/wenlin.py
-drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/
--rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/PKG-INFO
--rw-r--r--   0 luc       (1000) luc       (1000)     1462 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/SOURCES.txt
--rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/dependency_links.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/requires.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-14 14:29:46.000000 cloudlanguagetools-5.7/cloudlanguagetools.egg-info/top_level.txt
--rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-14 14:29:46.418700 cloudlanguagetools-5.7/setup.cfg
--rwxr-xr-x   0 luc       (1000) luc       (1000)      929 2023-07-14 14:29:43.000000 cloudlanguagetools-5.7/setup.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/
+-rw-r--r--   0 luc       (1000) luc       (1000)    35149 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/LICENSE
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)      169 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/README.rst
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/cloudlanguagetools/
+-rw-r--r--   0 luc       (1000) luc       (1000)        0 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/__init__.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13412 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/amazon.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2667 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/argostranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    23928 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/azure.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4388 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/cereproc.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    17939 2023-07-16 13:29:35.000000 cloudlanguagetools-5.8/cloudlanguagetools/chatapi.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    11935 2023-07-16 13:29:35.000000 cloudlanguagetools-5.8/cloudlanguagetools/chatmodel.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2165 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/constants.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     4023 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/deepl.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1232 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/dictionarylookup.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     9171 2023-07-05 00:37:32.000000 cloudlanguagetools-5.8/cloudlanguagetools/easypronunciation.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6883 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/elevenlabs.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1052 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/encryption.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     7015 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/epitran.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      218 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/errors.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    13308 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/forvo.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/fptai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     8801 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/google.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6355 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/keys.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    14056 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/languages.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2806 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/libretranslate.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3980 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/mandarincantonese.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18680 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/naver.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     2511 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/openai.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      339 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/options.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3310 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/pythainlp.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      432 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/service.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    18797 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/servicemanager.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     3006 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/spacy.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5539 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/test_services.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      528 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/tokenization.py
+-rw-r--r--   0 luc       (1000) luc       (1000)      515 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/translationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1187 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/transliterationlanguage.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     1239 2023-07-14 14:25:16.000000 cloudlanguagetools-5.8/cloudlanguagetools/ttsvoice.py
+-rw-r--r--   0 luc       (1000) luc       (1000)    30649 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/vocalware.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     5479 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/voicen.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6491 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/watson.py
+-rw-r--r--   0 luc       (1000) luc       (1000)     6384 2023-05-24 03:51:37.000000 cloudlanguagetools-5.8/cloudlanguagetools/wenlin.py
+drwxr-xr-x   0 luc       (1000) luc       (1000)        0 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/
+-rw-r--r--   0 luc       (1000) luc       (1000)      640 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/PKG-INFO
+-rw-r--r--   0 luc       (1000) luc       (1000)     1462 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/SOURCES.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)        1 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/dependency_links.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       59 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/requires.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       19 2023-07-16 13:29:56.000000 cloudlanguagetools-5.8/cloudlanguagetools.egg-info/top_level.txt
+-rw-r--r--   0 luc       (1000) luc       (1000)       38 2023-07-16 13:29:56.100390 cloudlanguagetools-5.8/setup.cfg
+-rwxr-xr-x   0 luc       (1000) luc       (1000)      929 2023-07-16 13:29:53.000000 cloudlanguagetools-5.8/setup.py
```

### Comparing `cloudlanguagetools-5.7/LICENSE` & `cloudlanguagetools-5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/PKG-INFO` & `cloudlanguagetools-5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.7
+Version: 5.8
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/amazon.py` & `cloudlanguagetools-5.8/cloudlanguagetools/amazon.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/argostranslate.py` & `cloudlanguagetools-5.8/cloudlanguagetools/argostranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/azure.py` & `cloudlanguagetools-5.8/cloudlanguagetools/azure.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/cereproc.py` & `cloudlanguagetools-5.8/cloudlanguagetools/cereproc.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/chatapi.py` & `cloudlanguagetools-5.8/cloudlanguagetools/chatapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,26 +31,27 @@
 
 class TransliterateQuery(pydantic.BaseModel):
     input_text: str = Field(description="text to transliterate")
     language: cloudlanguagetools.languages.CommonLanguage = Field(description="language the text is in")
     service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use for transliteration')
 
 class DictionaryLookup(pydantic.BaseModel):
-    input_text: str = Field(description="text lookup in the dictionary")
-    language: cloudlanguagetools.languages.CommonLanguage = Field(description="language the text is in")
+    input_text: str = Field(description="text to lookup in the dictionary")
+    source_language: cloudlanguagetools.languages.CommonLanguage = Field(description="language of the text to look up")
+    target_language: cloudlanguagetools.languages.CommonLanguage = Field(description="language for the dictionary definition")
     service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use for dictionary lookup')
 
 class AudioQuery(pydantic.BaseModel):
-    input_text: str = Field(description="text to pronounce")
+    input_text: str = Field(description="text to pronounce / generate audio")
     language: cloudlanguagetools.languages.CommonLanguage = Field(description="language the text is in")
     service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use audio pronunciation')
     gender: Optional[cloudlanguagetools.constants.Gender] = Field(default=None, description='gender of the voice to pronounce the text in')
 
 class BreakdownQuery(pydantic.BaseModel):
-    input_text: str = Field(description="text to breakdown")
+    input_text: str = Field(description="text to breakdown into words")
     language: cloudlanguagetools.languages.CommonLanguage = Field(description="language the text is in")
     translation_language: cloudlanguagetools.languages.CommonLanguage = Field(default=cloudlanguagetools.languages.CommonLanguage.en, description="language to translate into")
     translation_service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use for translation')
     transliteration_service: Optional[cloudlanguagetools.constants.Service] = Field(default=None, description='service to use for transliteration')
 
 
 class ChatAPI():
@@ -157,44 +158,59 @@
             query.input_text,
             transliteration_option.service,
             transliteration_option.get_transliteration_key()
         )
         return transliterated_text
 
     def dictionary_lookup(self, query: DictionaryLookup):
-        language = cloudlanguagetools.languages.Language[query.language.name]
+        logger.info(f'dictionary lookup {query}')
+        source_language = cloudlanguagetools.languages.Language[query.source_language.name]
+        target_language = cloudlanguagetools.languages.Language[query.target_language.name]
         dictionary_option_list = self.manager.get_dictionary_lookup_options()
-        candidates = [x for x in dictionary_option_list if x.language == language]
+        candidates = [x for x in dictionary_option_list if x.language == source_language and x.target_language == target_language]
         if len(candidates) == 0:
-            raise NoDataFoundException(f'No dictionary service found for language {language.lang_name}')
+            raise NoDataFoundException(f'No dictionary service found for source language {query.source_language.lang_name} / target language: {query.target_language.lang_name}')
 
         service_list = set([x.service for x in candidates])
 
+        preferred_service = query.service
+        # for Chinese, always enforce Wenlin
+        if source_language in [
+            cloudlanguagetools.languages.Language.yue,
+            cloudlanguagetools.languages.Language.zh_cn,
+            cloudlanguagetools.languages.Language.zh_tw,
+            cloudlanguagetools.languages.Language.zh_lit
+        ]:
+            preferred_service = cloudlanguagetools.constants.Service.Wenlin
+
         service_preference = self.get_service_preference([
             cloudlanguagetools.constants.Service.Wenlin,
             cloudlanguagetools.constants.Service.Azure,
-        ], query.service)
+        ], preferred_service)
 
         while service_preference[0] not in service_list:
             service_preference.pop(0)
             if len(service_preference) == 0:
-                raise NoDataFoundException(f'No service found for dictionary lookup of {language.lang_name}')
+                raise NoDataFoundException(f'No service found for dictionary lookup of {query.source_language.lang_name}')
             
         service = service_preference[0]
         final_candidates = [x for x in candidates if x.service == service]
 
         dictionary_option = final_candidates[0]
         logger.debug(f'Using dictionary option {pprint.pformat(dictionary_option.json_obj())}')
 
-        dictionary_result = self.manager.get_dictionary_lookup(
-            query.input_text,
-            service,
-            dictionary_option.get_lookup_key()
-        )
-        result = ' / '.join(dictionary_result)
+        try:
+            dictionary_result = self.manager.get_dictionary_lookup(
+                query.input_text,
+                service,
+                dictionary_option.get_lookup_key()
+            )
+            result = ' / '.join(dictionary_result)
+        except cloudlanguagetools.errors.NotFoundError as e:
+            result = f'No dictionary lookup results found for {query.input_text}'
         return result
         
 
     def audio(self, query: AudioQuery, format: cloudlanguagetools.options.AudioFormat) -> tempfile.NamedTemporaryFile:
         logger.info(f'processing audio query: {query}')
         language = cloudlanguagetools.languages.Language[query.language.name]
         # get full voice list, filter down to correct language
```

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/chatmodel.py` & `cloudlanguagetools-5.8/cloudlanguagetools/chatmodel.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import openai
 import time
 import cloudlanguagetools.chatapi
 import cloudlanguagetools.options
 
 logger = logging.getLogger(__name__)
 
+class IsNewSentenceQuery(pydantic.BaseModel):
+    is_new_sentence: bool = pydantic.Field(description="true if the last user message is a new input sentence for translation, transliteration, pronuncation or dictionary lookup," 
+                                           "false if it is a question regarding the meaning, grammar, or vocabulary of the previous sentence")
+
 
 """
 holds an instance of a conversation
 """
 class ChatModel():
     FUNCTION_NAME_TRANSLATE = 'translate'
     FUNCTION_NAME_TRANSLITERATE = 'transliterate'
@@ -21,52 +25,61 @@
     FUNCTION_NAME_PRONOUNCE = 'pronounce'
 
     def __init__(self, manager):
         self.manager = manager
         self.chatapi = cloudlanguagetools.chatapi.ChatAPI(self.manager)
         self.instruction = None
         self.message_history = []
+        self.last_call_messages = None
         self.total_tokens = 0
         self.latest_token_usage = 0
+        self.last_input_sentence = None
     
     def set_instruction(self, instruction):
         self.instruction = instruction
 
     def get_instruction(self):
         return self.instruction
 
+    def get_last_call_messages(self):
+        return self.last_call_messages
+
     def set_send_message_callback(self, send_message_fn, send_audio_fn, send_error_fn):
         self.send_message_fn = send_message_fn
         self.send_audio_fn = send_audio_fn
         self.send_error_fn = send_error_fn
 
     def send_message(self, message):
         self.send_message_fn(message)
 
     def send_audio(self, audio_tempfile):
         self.send_audio_fn(audio_tempfile)
 
     def send_error(self, error: str):
         self.send_error_fn(error)        
 
-    def call_openai(self):
+    def get_system_messages(self):
         # do we have any instructions ?
         instruction_message_list = []
         if self.instruction != None:
             instruction_message_list = [{"role": "system", "content": self.instruction}]
 
         messages = [
-            {"role": "system", "content": "You are a helpful assistant specialized in translation and language learning. " +
-             "You will receive instructions in English telling you what to do. " +
-             "If you receive a message in another language, it means the user is asking you to execute some commands."}
+            {"role": "system", "content": "You are a helpful assistant specialized in translation and language learning."}
         ] + instruction_message_list
 
+        return messages
 
+    def call_openai(self):
+
+        messages = self.get_system_messages()
         messages.extend(self.message_history)
 
+        self.last_call_messages = messages
+
         logger.debug(f"sending messages to openai: {pprint.pformat(messages)}")
 
         response = openai.ChatCompletion.create(
             model="gpt-3.5-turbo-0613",
             # require larger context
             # model="gpt-3.5-turbo-16k",
             messages=messages,
@@ -81,90 +94,148 @@
         self.total_tokens += self.latest_token_usage
 
         return response
 
     def status(self):
         return f'total_tokens: {self.total_tokens}, latest_token_usage: {self.latest_token_usage} (prompt: {self.latest_prompt_usage} completion: {self.latest_completion_usage})'
 
-    def process_message(self, message):
+    def is_new_sentence(self, input_sentence) -> bool:
+        """return true if input is a new sentence. we'll use this to clear history"""
+
+        messages = [
+            {"role": "system", "content": "You are a helpful assistant specialized in translation and language learning."},
+            {"role": "user", "content": self.last_input_sentence},
+            {"role": "user", "content": input_sentence}
+        ]
+
+        new_sentence_function_name = 'is_new_sentence'
+
+        response = openai.ChatCompletion.create(
+            model="gpt-3.5-turbo-0613",
+            messages=messages,
+            functions=[{
+                'name': new_sentence_function_name,
+                'description': "Determine whether the last user message is a new sentence or a question regarding the meaning, grammar, or vocabulary of the previous sentence",
+                'parameters': IsNewSentenceQuery.model_json_schema(),
+            }],
+            function_call={'name': new_sentence_function_name},
+            temperature=0.0
+        )
+
+        message = response['choices'][0]['message']
+        function_name = message['function_call']['name']
+        assert function_name == new_sentence_function_name
+        arguments = json.loads(message["function_call"]["arguments"])
+        is_new_sentence_arg = IsNewSentenceQuery(**arguments)
+        
+        logger.info(f'input sentence: [{input_sentence}] is new sentence: {is_new_sentence_arg.is_new_sentence}')
+        return is_new_sentence_arg.is_new_sentence
+
+
+
+    def process_message(self, input_message):
     
+        # do we need to clear history ?
+        if len(self.message_history) > 0 and self.is_new_sentence(input_message):
+            self.message_history = []
+
         max_calls = 10
         continue_processing = True
 
         # message_history contains the most recent request
-        self.message_history.append({"role": "user", "content": message})
+        self.message_history.append({"role": "user", "content": input_message})
 
-        # if the processing loop resulted in no functions getting called, see what the bot has to say
-        had_function_calls = False
 
         function_call_cache = {}
+        at_least_one_message_to_user = False
 
         try:
             while continue_processing and max_calls > 0:
                 max_calls -= 1
                 response = self.call_openai()
                 logger.debug(pprint.pformat(response))
                 message = response['choices'][0]['message']
+                message_content = message.get('content', None)
                 if 'function_call' in message:
                     function_name = message['function_call']['name']
                     logger.info(f'function_call: function_name: {function_name}')
                     try:
                         arguments = json.loads(message["function_call"]["arguments"])
                     except json.decoder.JSONDecodeError as e:
                         logger.exception(f'error decoding json: {message}')
                     arguments_str = json.dumps(arguments, indent=4)
                     # check whether we've called that function with exact same arguments before
                     if arguments_str not in function_call_cache.get(function_name, {}):
                         # haven't called it with these arguments before
-                        function_call_result = self.process_function_call(function_name, arguments)
+                        function_call_result, sent_message_to_user = self.process_function_call(function_name, arguments)
+                        at_least_one_message_to_user = at_least_one_message_to_user or sent_message_to_user
                         self.message_history.append({"role": "function", "name": function_name, "content": function_call_result})
                         # cache function call results
                         if function_name not in function_call_cache:
                             function_call_cache[function_name] = {}
                         function_call_cache[function_name][arguments_str] = function_call_result
-                        had_function_calls = True
                     else:
                         # we've called that function already with same arguments, we won't call again, but
                         # add to history again, so that chatgpt doesn't call the function again
                         self.message_history.append({"role": "function", "name": function_name, "content": function_call_result})
                 else:
                     continue_processing = False
-                    if had_function_calls == False:
-                        # no functions were called. maybe chatgpt is trying to explain something
+                    if at_least_one_message_to_user == False:
+                        # or nothing has been shown to the user yet, so we should show the final message. maybe chatgpt is trying to explain something
                         self.send_message(message['content'])
+                
+                # if there was a message, append it to the history
+                if message_content != None:
+                    self.message_history.append({"role": "assistant", "content": message_content})
         except Exception as e:
             logger.exception(f'error processing function call')
             self.send_error(str(e))                
 
+        # clear history after processing one input sentence
+        # self.message_history = []
+        self.last_input_sentence = input_message
+
     def process_function_call(self, function_name, arguments):
+        # by default, don't send output to user
+        send_message_to_user = False
         if function_name == self.FUNCTION_NAME_PRONOUNCE:
             query = cloudlanguagetools.chatapi.AudioQuery(**arguments)
             audio_tempfile = self.chatapi.audio(query, cloudlanguagetools.options.AudioFormat.mp3)
             result = query.input_text
             self.send_audio(audio_tempfile)
+            send_message_to_user = True
         else:
+            # text-based functions
             try:
                 if function_name == self.FUNCTION_NAME_TRANSLATE:
                     translate_query = cloudlanguagetools.chatapi.TranslateQuery(**arguments)
                     result = self.chatapi.translate(translate_query)
+                    send_message_to_user = True
                 elif function_name == self.FUNCTION_NAME_TRANSLITERATE:
                     query = cloudlanguagetools.chatapi.TransliterateQuery(**arguments)
                     result = self.chatapi.transliterate(query)
+                    send_message_to_user = True
                 elif function_name == self.FUNCTION_NAME_DICTIONARY_LOOKUP:
                     query = cloudlanguagetools.chatapi.DictionaryLookup(**arguments)
                     result = self.chatapi.dictionary_lookup(query)
+                    send_message_to_user = True
                 elif function_name == self.FUNCTION_NAME_BREAKDOWN:
                     query = cloudlanguagetools.chatapi.BreakdownQuery(**arguments)
                     result = self.chatapi.breakdown(query)
+                    send_message_to_user = True
+                else:
+                    # report unknown function
+                    result = f'unknown function: {function_name}'
             except cloudlanguagetools.chatapi.NoDataFoundException as e:
                 result = str(e)
             logger.info(f'function: {function_name} result: {result}')
-            self.send_message(result)
+            if send_message_to_user:
+                self.send_message(result)
         # need to echo the result back to chatgpt
-        return result        
+        return result, send_message_to_user    
 
     def get_openai_functions(self):
         return [
             {
                 'name': self.FUNCTION_NAME_TRANSLATE,
                 'description': "Translate input text from source language to target language",
                 'parameters': cloudlanguagetools.chatapi.TranslateQuery.model_json_schema(),
```

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/constants.py` & `cloudlanguagetools-5.8/cloudlanguagetools/constants.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/deepl.py` & `cloudlanguagetools-5.8/cloudlanguagetools/deepl.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/dictionarylookup.py` & `cloudlanguagetools-5.8/cloudlanguagetools/dictionarylookup.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/easypronunciation.py` & `cloudlanguagetools-5.8/cloudlanguagetools/easypronunciation.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/elevenlabs.py` & `cloudlanguagetools-5.8/cloudlanguagetools/elevenlabs.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/encryption.py` & `cloudlanguagetools-5.8/cloudlanguagetools/encryption.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/epitran.py` & `cloudlanguagetools-5.8/cloudlanguagetools/epitran.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/forvo.py` & `cloudlanguagetools-5.8/cloudlanguagetools/forvo.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/fptai.py` & `cloudlanguagetools-5.8/cloudlanguagetools/fptai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/google.py` & `cloudlanguagetools-5.8/cloudlanguagetools/google.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/keys.py` & `cloudlanguagetools-5.8/cloudlanguagetools/keys.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/languages.py` & `cloudlanguagetools-5.8/cloudlanguagetools/languages.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/libretranslate.py` & `cloudlanguagetools-5.8/cloudlanguagetools/libretranslate.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/mandarincantonese.py` & `cloudlanguagetools-5.8/cloudlanguagetools/mandarincantonese.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/naver.py` & `cloudlanguagetools-5.8/cloudlanguagetools/naver.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/openai.py` & `cloudlanguagetools-5.8/cloudlanguagetools/openai.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/pythainlp.py` & `cloudlanguagetools-5.8/cloudlanguagetools/pythainlp.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/servicemanager.py` & `cloudlanguagetools-5.8/cloudlanguagetools/servicemanager.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/spacy.py` & `cloudlanguagetools-5.8/cloudlanguagetools/spacy.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/test_services.py` & `cloudlanguagetools-5.8/cloudlanguagetools/test_services.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/tokenization.py` & `cloudlanguagetools-5.8/cloudlanguagetools/tokenization.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/translationlanguage.py` & `cloudlanguagetools-5.8/cloudlanguagetools/translationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/transliterationlanguage.py` & `cloudlanguagetools-5.8/cloudlanguagetools/transliterationlanguage.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/ttsvoice.py` & `cloudlanguagetools-5.8/cloudlanguagetools/ttsvoice.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/vocalware.py` & `cloudlanguagetools-5.8/cloudlanguagetools/vocalware.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/voicen.py` & `cloudlanguagetools-5.8/cloudlanguagetools/voicen.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/watson.py` & `cloudlanguagetools-5.8/cloudlanguagetools/watson.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools/wenlin.py` & `cloudlanguagetools-5.8/cloudlanguagetools/wenlin.py`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools.egg-info/PKG-INFO` & `cloudlanguagetools-5.8/cloudlanguagetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudlanguagetools
-Version: 5.7
+Version: 5.8
 Summary: Interface with various cloud APIs for language processing such as translation, text to speech
 Home-page: https://github.com/Language-Tools/cloud-language-tools-core
 Author: Luc
 Author-email: languagetools@mailc.net
 License: GPL
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cloudlanguagetools-5.7/cloudlanguagetools.egg-info/SOURCES.txt` & `cloudlanguagetools-5.8/cloudlanguagetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudlanguagetools-5.7/setup.py` & `cloudlanguagetools-5.8/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools.command.install import install
 
 # build instructions
 # python setup.py sdist
 # twine upload dist/*
 
 setup(name='cloudlanguagetools',
-      version='5.7',
+      version='5.8',
       description='Interface with various cloud APIs for language processing such as translation, text to speech',
       long_description=open('README.rst', encoding='utf-8').read(),
       url='https://github.com/Language-Tools/cloud-language-tools-core',
       author='Luc',
       author_email='languagetools@mailc.net',
       classifiers=[
         'Programming Language :: Python :: 3.7',
```

