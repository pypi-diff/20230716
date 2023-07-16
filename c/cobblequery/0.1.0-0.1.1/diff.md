# Comparing `tmp/cobblequery-0.1.0.tar.gz` & `tmp/cobblequery-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cobblequery-0.1.0.tar", last modified: Tue Mar 24 13:49:26 2020, max compression
+gzip compressed data, was "cobblequery-0.1.1.tar", last modified: Sun Jul 16 21:13:01 2023, max compression
```

## Comparing `cobblequery-0.1.0.tar` & `cobblequery-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2020-03-24 13:49:26.000000 cobblequery-0.1.0/
--rw-r--r--   0 kj         (501) staff       (20)      469 2020-03-24 13:49:26.000000 cobblequery-0.1.0/PKG-INFO
--rw-r--r--   0 kj         (501) staff       (20)       25 2020-03-21 14:04:02.000000 cobblequery-0.1.0/README.md
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2020-03-24 13:49:26.000000 cobblequery-0.1.0/bin/
--rwxr-xr-x   0 kj         (501) staff       (20)      458 2020-03-24 03:59:18.000000 cobblequery-0.1.0/bin/cobble
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2020-03-24 13:49:26.000000 cobblequery-0.1.0/cobblelib/
--rw-r--r--   0 kj         (501) staff       (20)        0 2020-03-21 14:06:11.000000 cobblequery-0.1.0/cobblelib/__init__.py
--rw-r--r--   0 kj         (501) staff       (20)     2826 2020-03-24 04:04:01.000000 cobblequery-0.1.0/cobblelib/aggregators.py
--rw-r--r--   0 kj         (501) staff       (20)      768 2020-03-24 13:26:02.000000 cobblequery-0.1.0/cobblelib/cli.py
--rw-r--r--   0 kj         (501) staff       (20)     7365 2020-03-24 13:42:12.000000 cobblequery-0.1.0/cobblelib/commands.py
--rw-r--r--   0 kj         (501) staff       (20)     1184 2020-03-24 04:17:31.000000 cobblequery-0.1.0/cobblelib/core.py
--rw-r--r--   0 kj         (501) staff       (20)     2290 2020-03-24 02:50:21.000000 cobblequery-0.1.0/cobblelib/extractor.py
--rw-r--r--   0 kj         (501) staff       (20)      289 2020-03-21 14:06:11.000000 cobblequery-0.1.0/cobblelib/parsers.py
--rw-r--r--   0 kj         (501) staff       (20)     7943 2020-03-24 13:45:49.000000 cobblequery-0.1.0/cobblelib/query_language.py
--rw-r--r--   0 kj         (501) staff       (20)     2455 2020-03-24 03:53:05.000000 cobblequery-0.1.0/cobblelib/utils.py
-drwxr-xr-x   0 kj         (501) staff       (20)        0 2020-03-24 13:49:26.000000 cobblequery-0.1.0/cobblequery.egg-info/
--rw-r--r--   0 kj         (501) staff       (20)      469 2020-03-24 13:49:26.000000 cobblequery-0.1.0/cobblequery.egg-info/PKG-INFO
--rw-r--r--   0 kj         (501) staff       (20)      364 2020-03-24 13:49:26.000000 cobblequery-0.1.0/cobblequery.egg-info/SOURCES.txt
--rw-r--r--   0 kj         (501) staff       (20)        1 2020-03-24 13:49:26.000000 cobblequery-0.1.0/cobblequery.egg-info/dependency_links.txt
--rw-r--r--   0 kj         (501) staff       (20)       10 2020-03-24 13:49:26.000000 cobblequery-0.1.0/cobblequery.egg-info/top_level.txt
--rw-r--r--   0 kj         (501) staff       (20)       38 2020-03-24 13:49:26.000000 cobblequery-0.1.0/setup.cfg
--rw-r--r--   0 kj         (501) staff       (20)      668 2020-03-24 13:37:13.000000 cobblequery-0.1.0/setup.py
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-07-16 21:13:01.843079 cobblequery-0.1.1/
+-rw-r--r--   0 kj         (501) staff       (20)      426 2023-07-16 21:13:01.842948 cobblequery-0.1.1/PKG-INFO
+-rw-r--r--   0 kj         (501) staff       (20)       25 2023-07-08 22:56:29.000000 cobblequery-0.1.1/README.md
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-07-16 21:13:01.841356 cobblequery-0.1.1/bin/
+-rwxr-xr-x   0 kj         (501) staff       (20)      653 2023-07-08 23:36:46.000000 cobblequery-0.1.1/bin/cobble
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-07-16 21:13:01.842321 cobblequery-0.1.1/cobblelib/
+-rw-r--r--   0 kj         (501) staff       (20)        0 2023-07-08 22:56:29.000000 cobblequery-0.1.1/cobblelib/__init__.py
+-rw-r--r--   0 kj         (501) staff       (20)     2826 2023-07-08 22:56:29.000000 cobblequery-0.1.1/cobblelib/aggregators.py
+-rw-r--r--   0 kj         (501) staff       (20)     1115 2023-07-08 23:34:29.000000 cobblequery-0.1.1/cobblelib/cli.py
+-rw-r--r--   0 kj         (501) staff       (20)     8575 2023-07-16 21:09:46.000000 cobblequery-0.1.1/cobblelib/commands.py
+-rw-r--r--   0 kj         (501) staff       (20)     1184 2023-07-08 22:56:29.000000 cobblequery-0.1.1/cobblelib/core.py
+-rw-r--r--   0 kj         (501) staff       (20)     2290 2023-07-08 22:56:29.000000 cobblequery-0.1.1/cobblelib/extractor.py
+-rw-r--r--   0 kj         (501) staff       (20)      289 2023-07-08 22:56:29.000000 cobblequery-0.1.1/cobblelib/parsers.py
+-rw-r--r--   0 kj         (501) staff       (20)     7991 2023-07-10 01:00:54.000000 cobblequery-0.1.1/cobblelib/query_language.py
+-rw-r--r--   0 kj         (501) staff       (20)     2455 2023-07-08 22:56:29.000000 cobblequery-0.1.1/cobblelib/utils.py
+drwxr-xr-x   0 kj         (501) staff       (20)        0 2023-07-16 21:13:01.842788 cobblequery-0.1.1/cobblequery.egg-info/
+-rw-r--r--   0 kj         (501) staff       (20)      426 2023-07-16 21:13:01.000000 cobblequery-0.1.1/cobblequery.egg-info/PKG-INFO
+-rw-r--r--   0 kj         (501) staff       (20)      364 2023-07-16 21:13:01.000000 cobblequery-0.1.1/cobblequery.egg-info/SOURCES.txt
+-rw-r--r--   0 kj         (501) staff       (20)        1 2023-07-16 21:13:01.000000 cobblequery-0.1.1/cobblequery.egg-info/dependency_links.txt
+-rw-r--r--   0 kj         (501) staff       (20)       10 2023-07-16 21:13:01.000000 cobblequery-0.1.1/cobblequery.egg-info/top_level.txt
+-rw-r--r--   0 kj         (501) staff       (20)       38 2023-07-16 21:13:01.843123 cobblequery-0.1.1/setup.cfg
+-rw-r--r--   0 kj         (501) staff       (20)      668 2023-07-10 01:02:19.000000 cobblequery-0.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cobblequery-0.1.0/cobblelib/aggregators.py` & `cobblequery-0.1.1/cobblelib/aggregators.py`

 * *Files identical despite different names*

### Comparing `cobblequery-0.1.0/cobblelib/cli.py` & `cobblequery-0.1.1/cobblelib/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,25 @@
 import json
 
 DEFAULT_GENERATOR = {
     'function': 'from',
     'args': '-',
 }
 
+def parse_query(query_text):
+    try:
+        query = QL.parse_pipeline(query_text)
+    except ValueError as e:
+        error = str(e)
+        print('Error parsing query: {}'.format(error))
+        print('Given query:\n{}'.format(query_text))
+        return False
+    print('Given query:\n{}'.format(json.dumps(query, indent=4)))
+    return True
+
 
 def execute(query_text):
     try:
         query = QL.parse_pipeline(query_text)
     except ValueError as e:
         error = str(e)
         print('Error parsing query: {}'.format(error))
```

### Comparing `cobblequery-0.1.0/cobblelib/commands.py` & `cobblequery-0.1.1/cobblelib/commands.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class SkipError(ValueError):
     pass
 
 class GenerateSeries():
     is_generator = True
     preparsed_arguments = True
     
-    def __init__(self, start=0, end=20):
+    def __init__(self, end=20, start=0):
         self.start = int(start)
         self.end = int(end)
 
     def generate(self):
         for i in range(self.start, self.end):
             yield {'i': i}
 
@@ -88,14 +88,40 @@
             context = {'value': utils.DotWrapper(entry)}
             expression_results = []
             for e in self.executors:
                 expression_results.append(e(context)[1])
             if all(expression_results):
                 yield entry
 
+class SliceFilter():
+    preparsed_arguments = True
+    accepts_kwargs = False
+
+    def __init__(self, *args):
+        if len(args) == 1:
+            start = 0
+            end = int(args[0])
+        elif len(args) > 1:
+            start = int(args[0])
+            end = int(args[1])
+        if end < 1:
+            end = None
+        if start < 0:
+            start = 0
+        self.end = end
+        self.start = start
+
+    def stream(self, source):
+        for i, entry in enumerate(source):
+            if self.start is not None and i < self.start:
+                continue
+            if self.end is not None and i >= self.end:
+                continue
+            yield entry
+
 class PyExecSet():
     preparsed_arguments = True
 
     def __init__(self, **kwargs):
         self.executors = {}
         for target, expression in kwargs.items():
             self.executors[target] = utils.py_executor(expression)
@@ -186,22 +212,23 @@
             record.update(agg_results)
             yield record
 
 class JoinPipeline():
     preparsed_arguments = True
     accepts_sub_commands = True
 
-    def __init__(self, *keys, type='left', sub_commands=None):
+    def __init__(self, *keys, type='left', first=False, output=None, sub_commands=None):
         self.sub_pipeline = query_language.parse_pipeline(sub_commands)
         if not keys:
             raise ValueError('Join must have at least one condition')
         self.join_keys = keys
         self.join_extractors = [Extractor(f) for f in self.join_keys]
         self.join_type = type
 
+
     def get_join_key(self, entry):
         if self.join_keys is None:
             return None
         if len(self.join_keys) == 1:
             return self.join_extractors[0](entry)
         return tuple(extractor(entry) in self.by_extractors)
 
@@ -224,18 +251,37 @@
             yield entry
 
         if self.join_type == 'outer':
             for key, entry in index.items():
                 if key not in used:
                     yield entry
 
+class AppendPipeline():
+    preparsed_arguments = True
+    accepts_sub_commands = True
+
+    def __init__(self, sub_commands=None):
+        self.sub_pipeline = query_language.parse_pipeline(sub_commands)
+
+    def stream(self, source):
+        from .core import run_pipeline
+
+        for entry in source:
+            yield entry
+
+        for entry in run_pipeline(self.sub_pipeline):
+            yield entry
+
 
 COMMANDS = {
     'from': FileLoader,
     'range': GenerateSeries,
+    'append': AppendPipeline,
     'where': PyExecFilter,
+    'slice': SliceFilter,
     'set': PyExecSet,
     'eval': PyExecSet,          # Alias
     'aggregate': Aggregate,
     'stats': Aggregate,         # Alias
+    'agg': Aggregate,         # Alias
     'join': JoinPipeline,
 }
```

### Comparing `cobblequery-0.1.0/cobblelib/core.py` & `cobblequery-0.1.1/cobblelib/core.py`

 * *Files identical despite different names*

### Comparing `cobblequery-0.1.0/cobblelib/extractor.py` & `cobblequery-0.1.1/cobblelib/extractor.py`

 * *Files identical despite different names*

### Comparing `cobblequery-0.1.0/cobblelib/query_language.py` & `cobblequery-0.1.1/cobblelib/query_language.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,18 +190,18 @@
         if closing_token is None:
             if function_name:
                 pipeline.append({'function': function_name, 'args': '', 'sub': sub})
             break
         elif closing_token == '|':
             continue
 
-        parens = closing_token is '('
+        parens = closing_token == '('
         if parens:
             arguments = lexer.seek_closing_pair('(', ')', keep_quotes=True)
-            closing_token = ')'
+            garbage, closing_token = lexer.seek_till('|', re.compile(r'\{|\['))
         else:
             arguments, closing_token = lexer.seek_till('|', re.compile(r'\{|\['))
 
         if closing_token in ('[', '{'):
             sub = lexer.seek_closing_pair(closing_token, SUB_PIPELINE_PAIRS[closing_token], keep_quotes=True).strip()
             garbage, closing_token = lexer.seek_till('|')
         elif closing_token == ')':
```

### Comparing `cobblequery-0.1.0/cobblelib/utils.py` & `cobblequery-0.1.1/cobblelib/utils.py`

 * *Files identical despite different names*

### Comparing `cobblequery-0.1.0/setup.py` & `cobblequery-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name = 'cobblequery',
     scripts=['bin/cobble'],
     packages=['cobblelib'],
-    version = '0.1.0',
+    version = '0.1.1',
     description = 'CLI tool for doing data joining',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author = 'KJ',
     author_email = 'jdotpy@users.noreply.github.com',
     url = 'https://github.com/jdotpy/cobble',
     download_url = 'https://github.com/jdotpy/cobble/tarball/master',
```

