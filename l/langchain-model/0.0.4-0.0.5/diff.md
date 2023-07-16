# Comparing `tmp/langchain_model-0.0.4.tar.gz` & `tmp/langchain_model-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_model-0.0.4.tar", last modified: Sun Jul 16 15:09:03 2023, max compression
+gzip compressed data, was "langchain_model-0.0.5.tar", last modified: Sun Jul 16 15:58:50 2023, max compression
```

## Comparing `langchain_model-0.0.4.tar` & `langchain_model-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:09:03.321624 langchain_model-0.0.4/
--rw-r--r--   0 harrisonchase   (501) staff       (20)      108 2023-07-16 15:09:03.321438 langchain_model-0.0.4/PKG-INFO
--rw-r--r--   0 harrisonchase   (501) staff       (20)      107 2023-07-16 14:03:13.000000 langchain_model-0.0.4/README.md
--rw-r--r--   0 harrisonchase   (501) staff       (20)       38 2023-07-16 15:09:03.321671 langchain_model-0.0.4/setup.cfg
--rw-r--r--   0 harrisonchase   (501) staff       (20)      305 2023-07-16 15:08:55.000000 langchain_model-0.0.4/setup.py
-drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:09:03.318255 langchain_model-0.0.4/src/
-drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:09:03.319266 langchain_model-0.0.4/src/langchain_model/
--rw-r--r--   0 harrisonchase   (501) staff       (20)     1901 2023-07-16 14:59:55.000000 langchain_model-0.0.4/src/langchain_model/__init__.py
-drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:09:03.321035 langchain_model-0.0.4/src/langchain_model.egg-info/
--rw-r--r--   0 harrisonchase   (501) staff       (20)      108 2023-07-16 15:09:03.000000 langchain_model-0.0.4/src/langchain_model.egg-info/PKG-INFO
--rw-r--r--   0 harrisonchase   (501) staff       (20)      264 2023-07-16 15:09:03.000000 langchain_model-0.0.4/src/langchain_model.egg-info/SOURCES.txt
--rw-r--r--   0 harrisonchase   (501) staff       (20)        1 2023-07-16 15:09:03.000000 langchain_model-0.0.4/src/langchain_model.egg-info/dependency_links.txt
--rw-r--r--   0 harrisonchase   (501) staff       (20)       21 2023-07-16 15:09:03.000000 langchain_model-0.0.4/src/langchain_model.egg-info/requires.txt
--rw-r--r--   0 harrisonchase   (501) staff       (20)       16 2023-07-16 15:09:03.000000 langchain_model-0.0.4/src/langchain_model.egg-info/top_level.txt
+drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:58:50.065023 langchain_model-0.0.5/
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      108 2023-07-16 15:58:50.064908 langchain_model-0.0.5/PKG-INFO
+-rw-r--r--   0 harrisonchase   (501) staff       (20)     3767 2023-07-16 15:58:41.000000 langchain_model-0.0.5/README.md
+drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:58:50.063953 langchain_model-0.0.5/langchain_model/
+-rw-r--r--   0 harrisonchase   (501) staff       (20)     2572 2023-07-16 15:35:52.000000 langchain_model-0.0.5/langchain_model/__init__.py
+drwxr-xr-x   0 harrisonchase   (501) staff       (20)        0 2023-07-16 15:58:50.064771 langchain_model-0.0.5/langchain_model.egg-info/
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      108 2023-07-16 15:58:50.000000 langchain_model-0.0.5/langchain_model.egg-info/PKG-INFO
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      240 2023-07-16 15:58:50.000000 langchain_model-0.0.5/langchain_model.egg-info/SOURCES.txt
+-rw-r--r--   0 harrisonchase   (501) staff       (20)        1 2023-07-16 15:58:50.000000 langchain_model-0.0.5/langchain_model.egg-info/dependency_links.txt
+-rw-r--r--   0 harrisonchase   (501) staff       (20)       21 2023-07-16 15:58:50.000000 langchain_model-0.0.5/langchain_model.egg-info/requires.txt
+-rw-r--r--   0 harrisonchase   (501) staff       (20)       16 2023-07-16 15:58:50.000000 langchain_model-0.0.5/langchain_model.egg-info/top_level.txt
+-rw-r--r--   0 harrisonchase   (501) staff       (20)       38 2023-07-16 15:58:50.065055 langchain_model-0.0.5/setup.cfg
+-rw-r--r--   0 harrisonchase   (501) staff       (20)      265 2023-07-16 15:58:41.000000 langchain_model-0.0.5/setup.py
```

### Comparing `langchain_model-0.0.4/src/langchain_model/__init__.py` & `langchain_model-0.0.5/langchain_model/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,25 +18,44 @@
     ),
     HumanMessage(
         content="Use the given format to extract information from the following input:"
     ),
     HumanMessagePromptTemplate.from_template("{input}"),
     HumanMessage(content="Tips: Make sure to answer in the correct format"),
 ]
-default_prompt = ChatPromptTemplate(messages=prompt_msgs)
+default_extraction_prompt = ChatPromptTemplate(messages=prompt_msgs)
+
+generation_prompt_msgs = [
+    SystemMessage(
+        content="Generate fake data based on user input."
+    ),
+    HumanMessagePromptTemplate.from_template("{input}"),
+]
+default_generation_prompt = ChatPromptTemplate(messages=generation_prompt_msgs)
 
 
 def langchain_model(
     _cls=None,
-    _llm: Optional[ChatOpenAI] = None,
-    _prompt: Optional[BasePromptTemplate] = None,
+    llm: Optional[ChatOpenAI] = None,
+    prompt: Optional[BasePromptTemplate] = None,
+    mode: Optional[str] = None,
     **kwargs: Any
 ) -> Callable[[Type[M]], Type[M]]:
-    llm = _llm or ChatOpenAI(model="gpt-3.5-turbo", temperature=0)
-    prompt = _prompt or default_prompt
+    llm = llm or ChatOpenAI(model="gpt-3.5-turbo", temperature=0)
+    if mode is None:
+        prompt = prompt or default_extraction_prompt
+    else:
+        if prompt is not None:
+            raise ValueError(
+                "If prompt is passed in, mode should NOT be (all mode does is set the default prompt)"
+            )
+        if mode == "extract":
+            prompt = default_extraction_prompt
+        elif mode == "generate":
+            prompt = default_generation_prompt
     if _cls is None:
 
         def class_rebuilder(cls):
             chain = create_structured_output_chain(cls, llm, prompt, **kwargs)
 
             class NewClass(cls):
                 def __init__(self, *args, **kwargs):
```

