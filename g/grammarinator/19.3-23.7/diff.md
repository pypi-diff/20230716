# Comparing `tmp/grammarinator-19.3.tar.gz` & `tmp/grammarinator-23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/grammarinator-19.3.tar", last modified: Sat Mar 30 14:45:33 2019, max compression
+gzip compressed data, was "grammarinator-23.7.tar", last modified: Sat Jul 15 22:50:00 2023, max compression
```

## Comparing `grammarinator-19.3.tar` & `grammarinator-23.7.tar`

### file list

```diff
@@ -1,44 +1,129 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1759 2019-03-30 14:45:15.000000 grammarinator-19.3/LICENSE.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     5324 2019-03-30 14:45:15.000000 grammarinator-19.3/README.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)     1223 2019-03-30 14:45:15.000000 grammarinator-19.3/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2740 2019-03-30 14:45:15.000000 grammarinator-19.3/RELNOTES.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3407 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/parser_builder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      415 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/pkgdata.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10708 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/parse.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      467 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/antlr/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9411 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/resources/antlr/ANTLRv4JavaLexer.g4
--rw-rw-r--   0 travis    (2000) travis    (2000)     4651 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/resources/antlr/LexBasic.g4
--rw-rw-r--   0 travis    (2000) travis    (2000)     2424 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/resources/antlr/LexerAdaptor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7565 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/resources/antlr/ANTLRv4Parser.g4
--rw-rw-r--   0 travis    (2000) travis    (2000)     9190 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/resources/antlr/ANTLRv4Lexer.g4
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/antlr/src/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/antlr/src/main/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/antlr/src/main/java/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/antlr/src/main/java/org/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/antlr/src/main/java/org/antlr/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/antlr/src/main/java/org/antlr/parser/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/resources/antlr/src/main/java/org/antlr/parser/antlr4/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2560 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/resources/antlr/src/main/java/org/antlr/parser/antlr4/LexerAdaptor.java
--rw-rw-r--   0 travis    (2000) travis    (2000)        5 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/VERSION
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator/runtime/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4605 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/runtime/tree.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      703 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/runtime/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      599 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/runtime/transformer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4189 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/runtime/grammarinator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    34289 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/process.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13620 2019-03-30 14:45:15.000000 grammarinator-19.3/grammarinator/generate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2019-03-30 14:45:33.000000 grammarinator-19.3/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      205 2019-03-30 14:45:15.000000 grammarinator-19.3/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     6838 2019-03-30 14:45:33.000000 grammarinator-19.3/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       31 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6838 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      179 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      962 2019-03-30 14:45:33.000000 grammarinator-19.3/grammarinator.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.054590 grammarinator-23.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.038589 grammarinator-23.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.042590 grammarinator-23.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-07-15 22:49:38.000000 grammarinator-23.7/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-15 22:49:38.000000 grammarinator-23.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-07-15 22:49:38.000000 grammarinator-23.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-15 22:49:38.000000 grammarinator-23.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-15 22:49:38.000000 grammarinator-23.7/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 22:49:38.000000 grammarinator-23.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-15 22:50:00.054590 grammarinator-23.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8493 2023-07-15 22:49:38.000000 grammarinator-23.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7273 2023-07-15 22:49:38.000000 grammarinator-23.7/RELNOTES.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.042590 grammarinator-23.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/grammarinator.runtime.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/grammarinator.tool.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.042590 grammarinator-23.7/docs/guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/actions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/fuzzer_building.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/grammar_overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/listeners.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7010 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/population.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/serializers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/test_generation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/guide/transformers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/relnotes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-15 22:49:38.000000 grammarinator-23.7/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.038589 grammarinator-23.7/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.042590 grammarinator-23.7/examples/fuzzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-15 22:49:38.000000 grammarinator-23.7/examples/fuzzer/HTMLCustomGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86017 2023-07-15 22:49:38.000000 grammarinator-23.7/examples/fuzzer/HTMLGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-07-15 22:49:38.000000 grammarinator-23.7/examples/fuzzer/html.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.042590 grammarinator-23.7/examples/grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-07-15 22:49:38.000000 grammarinator-23.7/examples/grammars/HTMLLexer.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-15 22:49:38.000000 grammarinator-23.7/examples/grammars/HTMLParser.g4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.046589 grammarinator-23.7/grammarinator/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9150 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/pkgdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.046589 grammarinator-23.7/grammarinator/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/cooldown_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/default_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/dispatching_listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/dispatching_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/runtime/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.050590 grammarinator-23.7/grammarinator/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/default_population.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.050590 grammarinator-23.7/grammarinator/tool/g4/
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/g4/LexerAdaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/g4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11808 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10459 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38599 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.038589 grammarinator-23.7/grammarinator/tool/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.050590 grammarinator-23.7/grammarinator/tool/resources/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/resources/codegen/GeneratorTemplate.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.050590 grammarinator-23.7/grammarinator/tool/resources/g4/
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/resources/g4/ANTLRv4Lexer.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/resources/g4/ANTLRv4Parser.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-07-15 22:49:38.000000 grammarinator-23.7/grammarinator/tool/resources/g4/LexBasic.g4
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.046589 grammarinator-23.7/grammarinator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-07-15 22:50:00.000000 grammarinator-23.7/grammarinator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-07-15 22:50:00.000000 grammarinator-23.7/grammarinator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:50:00.000000 grammarinator-23.7/grammarinator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-15 22:50:00.000000 grammarinator-23.7/grammarinator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-15 22:50:00.000000 grammarinator-23.7/grammarinator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 22:50:00.000000 grammarinator-23.7/grammarinator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-15 22:49:38.000000 grammarinator-23.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-15 22:50:00.058590 grammarinator-23.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.050590 grammarinator-23.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.054590 grammarinator-23.7/tests/grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Alternatives.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Arguments.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Charset.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Curly.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Custom.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/CustomSubclassGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/CustomWeights.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/DefaultRule.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/DispatchingModel.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/DotOption.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/EmptyAlternatives.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Eof.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Hello.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/ImagToken.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Importer.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/LabeledAlternatives.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/LifeCycle.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Listeners.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Locals.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/MinDepth.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/NoAction.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Quantifiers.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Recursive.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Returns.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Semantic.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/SeparateLexer.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/SeparateParser.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/SimpleAlternations.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/SuperClass.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/SuperClassOption.g4
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/SuperGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/SurrogatePairs.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/Whitespace.g4
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/custom_weights.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:50:00.054590 grammarinator-23.7/tests/grammars/import/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/grammars/import/Importee.g4
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/reparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/run_grammars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-07-15 22:49:38.000000 grammarinator-23.7/tests/test_grammars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-15 22:49:38.000000 grammarinator-23.7/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `grammarinator-19.3/LICENSE.rst` & `grammarinator-23.7/LICENSE.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2019 Renata Hodovan, Akos Kiss.
+Copyright (c) 2017-2023 Renata Hodovan, Akos Kiss.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
@@ -25,9 +25,10 @@
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 -----
 
 This software includes components from the "Grammars written for ANTLR v4"
-project under grammarinator/resources/antlr and grammariantor/examples/grammars/,
-which files carry a compatible "BSD license" and their own copyright notices.
+project under grammarinator/resources/antlr, grammarinator/parser, and
+grammariantor/examples/grammars, which files carry a compatible "BSD license"
+and their own copyright notices.
```

### Comparing `grammarinator-19.3/grammarinator/resources/antlr/ANTLRv4Parser.g4` & `grammarinator-23.7/grammarinator/tool/resources/g4/ANTLRv4Parser.g4`

 * *Files 8% similar despite different names*

```diff
@@ -24,96 +24,99 @@
  *  INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
  *  NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
  *  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
  *  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
  *  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF
  *  THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  */
+
 /*	A grammar for ANTLR v4 written in ANTLR v4.
  *
  *	Modified 2015.06.16 gbr
  *	-- update for compatibility with Antlr v4.5
  *	-- add mode for channels
  *	-- moved members to LexerAdaptor
  * 	-- move fragments to imports
  */
-
 parser grammar ANTLRv4Parser;
 
-options
-   { tokenVocab = ANTLRv4Lexer; }
 
+options { tokenVocab = ANTLRv4Lexer; }
 // The main entry point for parsing a v4 grammar.
 grammarSpec
-   : DOC_COMMENT* grammarType identifier SEMI prequelConstruct* rules modeSpec* EOF
+   : grammarDecl prequelConstruct* rules modeSpec* EOF
+   ;
+
+grammarDecl
+   : grammarType identifier SEMI
    ;
 
 grammarType
    : (LEXER GRAMMAR | PARSER GRAMMAR | GRAMMAR)
    ;
+   // This is the list of all constructs that can be declared before
+   // the set of rules that compose the grammar, and is invoked 0..n
+   // times by the grammarPrequel rule.
 
-// This is the list of all constructs that can be declared before
-// the set of rules that compose the grammar, and is invoked 0..n
-// times by the grammarPrequel rule.
 prequelConstruct
    : optionsSpec
    | delegateGrammars
    | tokensSpec
    | channelsSpec
-   | action
+   | action_
    ;
+   // ------------
+   // Options - things that affect analysis and/or code generation
 
-// ------------
-// Options - things that affect analysis and/or code generation
 optionsSpec
-   : OPTIONS LBRACE (option SEMI)* RBRACE
+   : OPTIONS (option SEMI)* RBRACE
    ;
 
 option
    : identifier ASSIGN optionValue
    ;
 
 optionValue
    : identifier (DOT identifier)*
    | STRING_LITERAL
    | actionBlock
    | INT
    ;
+   // ------------
+   // Delegates
 
-// ------------
-// Delegates
 delegateGrammars
    : IMPORT delegateGrammar (COMMA delegateGrammar)* SEMI
    ;
 
 delegateGrammar
    : identifier ASSIGN identifier
    | identifier
    ;
+   // ------------
+   // Tokens & Channels
 
-// ------------
-// Tokens & Channels
 tokensSpec
-   : TOKENS LBRACE idList? RBRACE
+   : TOKENS idList? RBRACE
    ;
 
 channelsSpec
-   : CHANNELS LBRACE idList? RBRACE
+   : CHANNELS idList? RBRACE
    ;
 
 idList
    : identifier (COMMA identifier)* COMMA?
    ;
+   // Match stuff like @parser::members {int i;}
 
-// Match stuff like @parser::members {int i;}
-action
+action_
    : AT (actionScopeName COLONCOLON)? identifier actionBlock
    ;
+   // Scope names could collide with keywords; allow them as ids for action scopes
 
-// Scope names could collide with keywords; allow them as ids for action scopes
 actionScopeName
    : identifier
    | LEXER
    | PARSER
    ;
 
 actionBlock
@@ -134,15 +137,15 @@
 
 ruleSpec
    : parserRuleSpec
    | lexerRuleSpec
    ;
 
 parserRuleSpec
-   : DOC_COMMENT* ruleModifiers? RULE_REF argActionBlock? ruleReturns? throwsSpec? localsSpec? rulePrequel* COLON ruleBlock SEMI exceptionGroup
+   : ruleModifiers? RULE_REF argActionBlock? ruleReturns? throwsSpec? localsSpec? rulePrequel* COLON ruleBlock SEMI exceptionGroup
    ;
 
 exceptionGroup
    : exceptionHandler* finallyClause?
    ;
 
 exceptionHandler
@@ -174,23 +177,23 @@
 
 /** Match stuff like @init {int i;} */
 ruleAction
    : AT identifier actionBlock
    ;
 
 ruleModifiers
-   : ruleModifier +
+   : ruleModifier+
    ;
+   // An individual access modifier for a rule. The 'fragment' modifier
+   // is an internal indication for lexer rules that they do not match
+   // from the input but are like subroutines for other lexer rules to
+   // reuse for certain lexical patterns. The other modifiers are passed
+   // to the code generation templates and may be ignored by the template
+   // if they are of no use in that language.
 
-// An individual access modifier for a rule. The 'fragment' modifier
-// is an internal indication for lexer rules that they do not match
-// from the input but are like subroutines for other lexer rules to
-// reuse for certain lexical patterns. The other modifiers are passed
-// to the code generation templates and may be ignored by the template
-// if they are of no use in that language.
 ruleModifier
    : PUBLIC
    | PRIVATE
    | PROTECTED
    | FRAGMENT
    ;
 
@@ -201,19 +204,19 @@
 ruleAltList
    : labeledAlt (OR labeledAlt)*
    ;
 
 labeledAlt
    : alternative (POUND identifier)?
    ;
+   // --------------------
+   // Lexer rules
 
-// --------------------
-// Lexer rules
 lexerRuleSpec
-   : DOC_COMMENT* FRAGMENT? TOKEN_REF COLON lexerRuleBlock SEMI
+   : FRAGMENT? TOKEN_REF optionsSpec? COLON lexerRuleBlock SEMI
    ;
 
 lexerRuleBlock
    : lexerAltList
    ;
 
 lexerAltList
@@ -223,34 +226,30 @@
 lexerAlt
    : lexerElements lexerCommands?
    |
    // explicitly allow empty alts
    ;
 
 lexerElements
-   : lexerElement +
+   : lexerElement+
+   |
    ;
 
 lexerElement
-   : labeledLexerElement ebnfSuffix?
-   | lexerAtom ebnfSuffix?
+   : lexerAtom ebnfSuffix?
    | lexerBlock ebnfSuffix?
    | actionBlock QUESTION?
    ;
-
-// but preds can be anywhere
-labeledLexerElement
-   : identifier (ASSIGN | PLUS_ASSIGN) (lexerAtom | lexerBlock)
-   ;
+   // but preds can be anywhere
 
 lexerBlock
    : LPAREN lexerAltList RPAREN
    ;
+   // E.g., channel(HIDDEN), skip, more, mode(INSIDE), push(INSIDE), pop
 
-// E.g., channel(HIDDEN), skip, more, mode(INSIDE), push(INSIDE), pop
 lexerCommands
    : RARROW lexerCommand (COMMA lexerCommand)*
    ;
 
 lexerCommand
    : lexerCommandName LPAREN lexerCommandExpr RPAREN
    | lexerCommandName
@@ -261,40 +260,40 @@
    | MODE
    ;
 
 lexerCommandExpr
    : identifier
    | INT
    ;
+   // --------------------
+   // Rule Alts
 
-// --------------------
-// Rule Alts
 altList
    : alternative (OR alternative)*
    ;
 
 alternative
-   : elementOptions? element +
+   : elementOptions? element+
    |
    // explicitly allow empty alts
    ;
 
 element
    : labeledElement (ebnfSuffix |)
    | atom (ebnfSuffix |)
    | ebnf
    | actionBlock QUESTION?
    ;
 
 labeledElement
    : identifier (ASSIGN | PLUS_ASSIGN) (atom | block)
    ;
+   // --------------------
+   // EBNF and blocks
 
-// --------------------
-// EBNF and blocks
 ebnf
    : block blockSuffix?
    ;
 
 blockSuffix
    : ebnfSuffix
    ;
@@ -372,7 +371,8 @@
    | identifier ASSIGN (identifier | STRING_LITERAL)
    ;
 
 identifier
    : RULE_REF
    | TOKEN_REF
    ;
+
```

### Comparing `grammarinator-19.3/grammarinator/process.py` & `grammarinator-23.7/grammarinator/tool/processor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,663 +1,466 @@
-# Copyright (c) 2017-2019 Renata Hodovan, Akos Kiss.
+# Copyright (c) 2017-2023 Renata Hodovan, Akos Kiss.
+# Copyright (c) 2020 Sebastian Kimberk.
 #
 # Licensed under the BSD 3-Clause License
 # <LICENSE.rst or https://opensource.org/licenses/BSD-3-Clause>.
 # This file may not be copied, modified, or distributed except
 # according to those terms.
 
 import logging
 import re
-import sys
 
-from argparse import ArgumentParser
-from collections import defaultdict
-from contextlib import contextmanager
+from collections import defaultdict, OrderedDict
+from itertools import chain
+from math import inf
+from os import getcwd
 from os.path import dirname, exists, join
-from os import getcwd, makedirs
 from pkgutil import get_data
-from shutil import rmtree
+from shutil import copy
+from sys import maxunicode
 
-import antlerinator
 import autopep8
 
 from antlr4 import CommonTokenStream, FileStream, ParserRuleContext
+from jinja2 import Environment
 
-from .parser_builder import build_grammars
-from .pkgdata import __version__, default_antlr_path
-from .runtime.tree import *
+from ..pkgdata import __version__
+from .g4 import ANTLRv4Lexer, ANTLRv4Parser
 
-logger = logging.getLogger('grammarinator')
-logging.basicConfig(format='%(message)s')
+logger = logging.getLogger(__name__)
+
+
+class Edge(object):
+
+    def __init__(self, dst, args=None):
+        self.dst = dst
+        self.args = args
 
 
 class Node(object):
 
-    def __init__(self, id):
+    _cnt = 0
+
+    def __init__(self, id=None):
+        if id is None:
+            id = Node._cnt
+            Node._cnt += 1
         self.id = id
-        self.out_neighbours = []
+        self.out_edges = []
+
+    @property
+    def out_neighbours(self):
+        return [edge.dst for edge in self.out_edges]
+
+    def print_tree(self):
+        def _walk(node):
+            nonlocal indent
+            print(f'{"  " * indent}{str(node)}{"" if node not in visited else " (...recursion)"}')
+            if node in visited:
+                return
+
+            visited.add(node)
+            indent += 1
+            for child in node.out_neighbours:
+                _walk(child)
+            indent -= 1
+
+        visited = set()
+        indent = 0
+        _walk(self)
+
+    def __str__(self):
+        return f'cls: {self.__class__.__name__}'
 
 
 class RuleNode(Node):
-    pass
 
+    def __init__(self, name, label, type):
+        super().__init__(name if label is None else '_'.join((name, label)))
+        self.name = name
+        self.type = type
+        self.min_depth = None
 
-class AlternationNode(Node):
-    pass
+        self.labels = {}
+        self.args = {}
+        self.locals = {}
+        self.returns = {}
 
+    @property
+    def has_var(self):
+        return self.labels or self.attributes
 
-class AlternativeNode(Node):
-    pass
+    @property
+    def attributes(self):
+        return dict(self.args, **self.locals, **self.returns)
 
+    def __str__(self):
+        return f'{super().__str__()}; name: {self.name}; var: {self.has_var}'
 
-class QuantifierNode(Node):
-    pass
 
+class UnlexerRuleNode(RuleNode):
+
+    def __init__(self, name):
+        super().__init__(name, None, 'UnlexerRule')
+        self.start_ranges = None
+
+
+class UnparserRuleNode(RuleNode):
+
+    def __init__(self, name, label=None):
+        super().__init__(name, label, 'UnparserRule')
+
+
+class ImagRuleNode(Node):
+
+    def __init__(self, id):
+        super().__init__(id)
 
-class GrammarGraph(object):
+
+class LiteralNode(Node):
+
+    def __init__(self, src):
+        super().__init__()
+        self.src = src
+
+    def __str__(self):
+        return f'{super().__str__()}; src: {self.src!r}'
+
+
+class CharsetNode(Node):
+
+    def __init__(self, rule_id, idx, charset):
+        super().__init__()
+        self.rule_id = rule_id  # Identifier of the container rule.
+        self.idx = idx  # Index of the charset inside the current rule.
+        self.charset = charset  # Global identifier of the charset.
+
+    def __str__(self):
+        return f'{super().__str__()}; idx: {self.idx}; charset: {self.charset}'
+
+
+class LambdaNode(Node):
 
     def __init__(self):
-        self.vertices = dict()
+        super().__init__()
 
-    def add_node(self, node):
-        self.vertices[node.id] = node
 
-    def add_edge(self, frm, to):
-        assert frm in self.vertices, '{frm} not in vertices.'.format(frm=frm)
-        assert to in self.vertices, '{to} not in vertices.'.format(to=to)
-        self.vertices[frm].out_neighbours.append(self.vertices[to])
+class AlternationNode(Node):
 
-    def calc_min_depths(self):
-        min_depths = defaultdict(lambda: float('inf'))
-        changed = True
+    def __init__(self, rule_id, idx, conditions):
+        super().__init__()
+        self.rule_id = rule_id  # Identifier of the container rule.
+        self.idx = idx  # Index of the alternation in the container rule.
+        self.conditions = conditions
+        self.min_depths = None
+
+    def simple_alternatives(self):
+        # Check if an alternation contains simple alternatives only (simple
+        # literals or rule references), and return a 2-tuple. If the alternation
+        # contains any non-simple alternatives, return None, None. If the
+        # alternation contains simple literals only, the first element of the
+        # tuple is a list of the literal values, while the second element is None.
+        # If the alternation contains rule references only, the first element is
+        # None, while the second element is a list of rule ids. If the alternation
+        # contains both simple literals and rule references, then both elements of
+        # the tuple are lists, which are of identical length, and exactly one of
+        # them contains a non-None value at every index position.
+        if not self.out_neighbours or any(len(alt.out_neighbours) != 1 or not isinstance(alt.out_neighbours[0], (LiteralNode, RuleNode)) for alt in self.out_neighbours):
+            return None, None
+
+        simple_lits = [alt.out_neighbours[0].src if isinstance(alt.out_neighbours[0], LiteralNode) else None for alt in self.out_neighbours]
+        if all(lit is None for lit in simple_lits):
+            simple_lits = None
+
+        simple_rules = [alt.out_neighbours[0].id if isinstance(alt.out_neighbours[0], RuleNode) else None for alt in self.out_neighbours]
+        if all(rule is None for rule in simple_rules):
+            simple_rules = None
 
-        while changed:
-            changed = False
-            for ident in self.vertices:
-                selector = min if isinstance(self.vertices[ident], AlternationNode) else max
-                min_depth = selector([min_depths[node.id] + int(isinstance(self.vertices[node.id], RuleNode))
-                                      for node in self.vertices[ident].out_neighbours if not isinstance(node, QuantifierNode)], default=0)
+        return simple_lits, simple_rules
 
-                if min_depth < min_depths[ident]:
-                    min_depths[ident] = min_depth
-                    changed = True
+    def __str__(self):
+        return f'{super().__str__()}; idx: {self.idx}; cond: {", ".join(self.conditions)}'
 
-        # Lift the minimal depths of the alternatives to the alternations, where the decision will happen.
-        for ident in min_depths:
-            if isinstance(self.vertices[ident], AlternationNode):
-                assert all(min_depths[node.id] < float('inf') for node in self.vertices[ident].out_neighbours), '{ident} has an alternative that isn\'t reachable.'.format(ident=ident)
-                min_depths[ident] = [min_depths[node.id] for node in self.vertices[ident].out_neighbours]
-
-        # Remove the lifted Alternatives and check for infinite derivations.
-        for ident in list(min_depths.keys()):
-            if isinstance(self.vertices[ident], AlternativeNode):
-                del min_depths[ident]
-            else:
-                assert min_depths[ident] != float('inf'), 'Rule with infinite derivation: %s' % ident
 
-        return min_depths
+class AlternativeNode(Node):
 
+    def __init__(self, rule_id, alt_idx, idx):
+        super().__init__()
+        self.rule_id = rule_id  # Identifier of the container rule.
+        self.alt_idx = alt_idx  # Index of the container alternation inside the container rule.
+        self.idx = idx  # Index of the alternative in the container alternation.
 
-class FuzzerGenerator(object):
+    def __str__(self):
+        return f'{super().__str__()}; idx: {self.idx}'
 
-    def __init__(self, antlr_parser_cls, actions):
-        self.antlr_parser_cls = antlr_parser_cls
-        self.actions = actions
-
-        self.indent_level = 0
-        self.charset_idx = 0
-        self.code_id = 0
-
-        self.graph = GrammarGraph()
-
-        self.current_start_range = None
-        self.token_start_ranges = dict()
-
-        self.unlexer_header = None
-        self.unlexer_body = None
-        self.unlexer_name = None
-        self.unparser_header = None
-        self.unparser_body = None
-        self.unparser_name = None
-        self.code_chunks = dict()
-        self.labeled_alts = []
-
-    @contextmanager
-    def indent(self):
-        self.indent_level += 4
-        yield
-        self.indent_level -= 4
-
-    def line(self, src):
-        return (' ' * self.indent_level) + src + '\n'
-
-    def new_code_id(self, code_type):
-        code_name = '{type}_{idx}'.format(type=code_type, idx=self.code_id)
-        self.code_id += 1
-        return code_name
-
-    def new_charset_name(self):
-        charset_name = 'charset_{idx}'.format(idx=self.charset_idx)
-        self.charset_idx += 1
-        return charset_name
-
-    def generate_header(self, grammar_name, fuzzer_type, options, combined):
-        unlexer = fuzzer_type == 'Unlexer'
-        combined_unlexer = unlexer and combined
-        fuzzer_name = '{grammar_name}{fuzzer_type}'.format(grammar_name=grammar_name, fuzzer_type=fuzzer_type)
-        superclass = options.get('superClass', 'Grammarinator') if not combined_unlexer else 'Grammarinator'
-
-        src = self.line('# Generated by Grammarinator {version}\n'.format(version=__version__))
-        src += self.line('from itertools import chain')
-        src += self.line('from grammarinator.runtime import *\n')
-        if superclass != 'Grammarinator':
-            src += self.line('if __name__ is not None and \'.\' in __name__:')
-            with self.indent():
-                src += self.line('from .{superclass} import {superclass}'.format(superclass=superclass))
-            src += self.line('else:')
-            with self.indent():
-                src += self.line('from {superclass} import {superclass}\n'.format(superclass=superclass))
 
-        if unlexer:
-            self.unlexer_header = src
-        else:
-            self.unparser_header = src
-            self.unparser_header += self.line('import {unlexer_name}'.format(unlexer_name=self.unlexer_name))
+class QuantifierNode(Node):
 
-        src = self.line('class {fuzzer_name}({superclass}):\n'.format(fuzzer_name=fuzzer_name, superclass=superclass))
-        with self.indent():
-            src += self.line('def __init__(self, {args}):'.format(args='*, max_depth=float(\'inf\'), weights=None, cooldown=1.0' if unlexer else 'unlexer'))
-
-            with self.indent():
-                src += self.line('super({fuzzer_name}, self).__init__()'.format(fuzzer_name=fuzzer_name))
-                src += self.line('self.unlexer = {unlexer_ref}'.format(unlexer_ref='self' if unlexer else 'unlexer'))
-                if unlexer:
-                    src += self.line('self.max_depth = max_depth')
-                    src += self.line('self.weights = weights or dict()')
-                    src += self.line('self.cooldown = cooldown\n')
-                if options.get('dot'):
-                    src += self.line('self.{base}any_char = self.{dot}'.format(base='' if unlexer else 'unlexer.', dot=options['dot']))
-
-        if unlexer:
-            self.unlexer_body = src
-            with self.indent():
-                self.unlexer_body += self.line('def EOF(self, *args, **kwargs):')
-                with self.indent():
-                    self.unlexer_body += self.line('pass\n')
-        else:
-            self.unparser_body = src
+    def __init__(self, rule_id, idx, min, max):
+        super().__init__()
+        self.rule_id = rule_id  # Identifier of the container rule.
+        self.idx = idx  # Index of the quantifier in the container rule.
+        self.min = min
+        self.max = max
+        self.min_depth = None
 
-        if unlexer:
-            self.unlexer_name = fuzzer_name
-        else:
-            self.unparser_name = fuzzer_name
+    def __str__(self):
+        return f'{super().__str__()}; idx: {self.idx}; min: {self.min}; max: {self.max}'
 
-    def find_conditions(self, node):
-        if not self.actions:
-            return '1'
-
-        if isinstance(node, str):
-            return node
-
-        action_block = getattr(node, 'actionBlock', None)
-        if action_block:
-            if action_block() and action_block().ACTION_CONTENT() and node.QUESTION():
-                return ''.join([str(child) for child in action_block().ACTION_CONTENT()])
-            return '1'
-
-        element = getattr(node, 'element', None) or getattr(node, 'lexerElement', None)
-        if element:
-            if not element():
-                return '1'
-            return self.find_conditions(element(0))
 
-        child_ref = getattr(node, 'alternative', None) or getattr(node, 'lexerElements', None)
+class ActionNode(Node):
 
-        # An alternative can be explicitly empty, in this case it won't have any of the attributes above.
-        if not child_ref:
-            return '1'
-
-        return self.find_conditions(child_ref())
-
-    def character_range_interval(self, node):
-        start = str(node.characterRange().STRING_LITERAL(0))[1:-1]
-        end = str(node.characterRange().STRING_LITERAL(1))[1:-1]
-
-        return (int(start.replace('\\u', '0x'), 16) if '\\u' in start else ord(start),
-                int(end.replace('\\u', '0x'), 16) if '\\u' in end else ord(end) + 1)
-
-    def lexer_charset_interval(self, src):
-        elements = re.split(r'(\w-\w)', src)
-        ranges = []
-        for element in elements:
-            if not element:
-                continue
-
-            # Convert character sequences like \n, \t, etc. into a single character.
-            element = bytes(element, 'utf-8').decode('unicode_escape')
-            if len(element) > 1:
-                if element[1] == '-' and len(element) == 3:
-                    ranges.append((ord(element[0]), ord(element[2]) + 1))
-                else:
-                    for char in element:
-                        ranges.append((ord(char), ord(char) + 1))
-            elif len(element) == 1:
-                ranges.append((ord(element), ord(element) + 1))
-        return ranges
-
-    def chars_from_set(self, node):
-        if node.characterRange():
-            return [self.character_range_interval(node)]
-
-        if node.LEXER_CHAR_SET():
-            return self.lexer_charset_interval(str(node.LEXER_CHAR_SET())[1:-1])
-
-        if node.STRING_LITERAL():
-            assert len(str(node.STRING_LITERAL())) > 2, 'Negated string literal must not be empty.'
-            first_char = ord(str(node.STRING_LITERAL())[1])
-            return [(first_char, first_char + 1)]
-
-        if node.TOKEN_REF():
-            src = str(node.TOKEN_REF())
-            assert src in self.token_start_ranges, '{src} not in token_start_ranges.'.format(src=src)
-            return self.token_start_ranges[src]
+    def __init__(self, src):
+        super().__init__()
+        self.src = src
 
-        return []
+    def __str__(self):
+        return f'{super().__str__()}; src: {self.src}'
 
-    def generate(self, lexer_root, parser_root):
-        for root in [lexer_root, parser_root]:
-            if root:
-                self.generate_grammar(root)
 
-        self.code_chunks.update(self.graph.calc_min_depths())
+class VariableNode(Node):
 
-        return [
-            (self.unlexer_name, (self.unlexer_header + '\n\n' + self.unlexer_body).format(**self.code_chunks)),
-            (self.unparser_name, (self.unparser_header + '\n\n' + self.unparser_body).format(**self.code_chunks)),
-        ]
-
-    def generate_grammar(self, node):
-        assert isinstance(node, self.antlr_parser_cls.GrammarSpecContext)
-
-        options = dict()
-        if node.prequelConstruct():
-            for prequelConstruct in node.prequelConstruct():
-                if prequelConstruct.optionsSpec():
-                    for option in prequelConstruct.optionsSpec().option():
-                        ident = option.identifier()
-                        ident = ident.RULE_REF() or ident.TOKEN_REF()
-                        options[str(ident)] = option.optionValue().getText()
-
-        grammar_name = str(node.identifier().TOKEN_REF() or node.identifier().RULE_REF()).replace('Parser', '').replace('Lexer', '')
-        if node.grammarType().LEXER() or not node.grammarType().PARSER():
-            self.generate_header(grammar_name, 'Unlexer', options, combined=not node.grammarType().LEXER())
-        if node.grammarType().PARSER() or not node.grammarType().LEXER():
-            self.generate_header(grammar_name, 'Unparser', options, combined=not node.grammarType().PARSER())
-
-        if node.prequelConstruct():
-            for prequelConstruct in node.prequelConstruct():
-                if prequelConstruct.tokensSpec():
-                    id_list = prequelConstruct.tokensSpec().idList()
-                    if id_list:
-                        for identifier in id_list.identifier():
-                            assert identifier.TOKEN_REF() is not None, 'Token names must start with uppercase letter.'
-                            rule_name = str(identifier.TOKEN_REF())
-                            self.graph.add_node(RuleNode(id=rule_name))
-
-                            with self.indent():
-                                self.unlexer_body += self.line('def {rule_name}(self):'.format(rule_name=rule_name))
-                                with self.indent():
-                                    self.unlexer_body += self.line('return self.create_node(UnlexerRule(name=\'{rule_name}\'))\n'.format(rule_name=rule_name))
-
-            for prequelConstruct in node.prequelConstruct():
-                if prequelConstruct.action() and self.actions:
-                    action = prequelConstruct.action()
-                    scope_name = action.actionScopeName()
-                    if scope_name:
-                        action_scope = scope_name.LEXER() or scope_name.PARSER()
-                        assert action_scope, '{scope} scope not supported.'.format(scope=scope_name.identifier().RULE_REF() or scope_name.identifier().TOKEN_REF())
-                        action_scope = str(action_scope)
-                    else:
-                        action_scope = 'parser'
+    def __init__(self, name, is_list):
+        super().__init__()
+        self.name = name
+        self.is_list = is_list
 
-                    action_ident = action.identifier()
-                    action_type = str(action_ident.RULE_REF() or action_ident.TOKEN_REF())
-                    raw_action_src = ''.join([str(child) for child in action.actionBlock().ACTION_CONTENT()])
+    def __str__(self):
+        return f'{super().__str__()}; name: {self.name}; list: {self.is_list}'
 
-                    if action_type == 'header':
-                        action_src = raw_action_src
-                    else:
-                        with self.indent():
-                            action_src = ''.join([self.line(line) for line in raw_action_src.splitlines()])
 
-                    code_id = self.new_code_id('action')
-                    self.code_chunks[code_id] = action_src
-                    code_pattern = '{{{code_id}}}'.format(code_id=code_id)
-                    # We simply append both member and header code chunks to the generated source.
-                    # It's the user's responsibility to define them in order.
-                    if action_scope == 'parser':
-                        # Both 'member' and 'members' keywords are accepted.
-                        if action_type.startswith('member'):
-                            self.unparser_body += code_pattern
-                        elif action_type == 'header':
-                            self.unparser_header += code_pattern
-                    elif action_scope == 'lexer':
-                        if action_type.startswith('member'):
-                            self.unlexer_body += code_pattern
-                        elif action_type == 'header':
-                            self.unlexer_header += code_pattern
-
-        rules = node.rules().ruleSpec()
-        lexer_rules, parser_rules = [], []
-        self.graph.add_node(RuleNode(id='EOF'))
-        for rule in rules:
-            if rule.parserRuleSpec():
-                self.graph.add_node(RuleNode(id=str(rule.parserRuleSpec().RULE_REF())))
-                parser_rules.append(rule.parserRuleSpec())
-            elif rule.lexerRuleSpec():
-                self.graph.add_node(RuleNode(id=str(rule.lexerRuleSpec().TOKEN_REF())))
-                lexer_rules.append(rule.lexerRuleSpec())
-            else:
-                assert False, 'Should not get here.'
+def printable_ranges(lower_bound, upper_bound):
+    ranges = []
+    range_start = None
+    for c in range(lower_bound, upper_bound):
+        if chr(c).isprintable():
+            if range_start is None:
+                range_start = c
+        else:
+            if range_start is not None:
+                ranges.append((range_start, c))
+                range_start = None
+
+    if range_start is not None:
+        ranges.append((range_start, upper_bound))
+    return ranges
+
+
+def multirange_diff(r1_list, r2_list):
+    def range_diff(r1, r2):
+        s1, e1 = r1
+        s2, e2 = r2
+        endpoints = sorted((s1, s2, e1, e2))
+        result = []
+        if endpoints[0] == s1:
+            result.append((endpoints[0], endpoints[1]))
+        if endpoints[3] == e1:
+            result.append((endpoints[2], endpoints[3]))
+        return result
+
+    for r2 in r2_list:
+        r1_list = list(chain.from_iterable(range_diff(r1, r2) for r1 in r1_list))
+    return r1_list
+
+
+class Charset(object):
+
+    dot = {
+        'any_ascii_letter': [(ord('A'), ord('Z') + 1), (ord('a'), ord('z') + 1)],
+        'any_ascii_char': printable_ranges(0x00, 0x80),
+        'any_unicode_char': printable_ranges(0, maxunicode + 1),
+    }
+
+    _cnt = 0
+
+    def __init__(self, ranges):
+        self.id = Charset._cnt
+        Charset._cnt += 1
+        self.ranges = ranges
 
-        for mode_spec in node.modeSpec():
-            for lexer_rule in mode_spec.lexerRuleSpec():
-                self.graph.add_node(RuleNode(id=str(lexer_rule.TOKEN_REF())))
-                lexer_rules.append(lexer_rule)
-
-        with self.indent():
-            for rule in lexer_rules:
-                self.unlexer_body += self.generate_single(rule, None)
-            for rule in parser_rules:
-                self.unparser_body += self.generate_single(rule, None)
-
-        if parser_rules:
-            with self.indent():
-                self.unparser_body += self.line('default_rule = {name}\n'.format(name=parser_rules[0].RULE_REF()))
-
-    def generate_single(self, node, parent_id):
-        if isinstance(node, (self.antlr_parser_cls.ParserRuleSpecContext, self.antlr_parser_cls.LexerRuleSpecContext)):
-            parser_rule = isinstance(node, self.antlr_parser_cls.ParserRuleSpecContext)
-            node_type = UnparserRule if parser_rule else UnlexerRule
-            rule_name = str(node.RULE_REF() if parser_rule else node.TOKEN_REF())
-
-            # Mark that the next lexerAtom has to be saved as start range.
-            if not parser_rule:
-                self.current_start_range = []
-
-            rule_header = self.line('@depthcontrol')
-            rule_header += self.line('def {rule_name}(self):'.format(rule_name=rule_name))
-            with self.indent():
-                local_ctx = self.line('local_ctx = dict()')
-                rule_code = self.line('current = self.create_node({node_type}(name=\'{rule_name}\'))'.format(node_type=node_type.__name__,
-                                                                                                             rule_name=rule_name))
-                rule_block = node.ruleBlock() if parser_rule else node.lexerRuleBlock()
-                rule_code += self.generate_single(rule_block, rule_name)
-                rule_code += self.line('return current')
-            rule_code += self.line('{rule_name}.min_depth = {{{rule_name}}}\n'.format(rule_name=rule_name))
-
-            # local_ctx only has to be initialized if we have variable assignment.
-            rule_code = rule_header + (local_ctx if 'local_ctx' in rule_code else '') + rule_code
-
-            if self.labeled_alts:
-                for _ in range(len(self.labeled_alts)):
-                    name, children = self.labeled_alts.pop(0)
-                    labeled_header = self.line('@depthcontrol')
-                    labeled_header += self.line('def {name}(self):'.format(name=name))
-                    with self.indent():
-                        local_ctx = self.line('local_ctx = dict()')
-                        labeled_code = self.line('current = self.create_node(UnparserRule(name=\'{name}\'))'.format(name=name))
-                        for child in children:
-                            labeled_code += self.generate_single(child, name)
-                        labeled_code += self.line('return current')
-                    labeled_code += self.line('{rule_name}.min_depth = {{{rule_name}}}\n'.format(rule_name=name))
-
-                    labeled_code = labeled_header + (local_ctx if 'local_ctx' in labeled_code else '') + labeled_code
-                    rule_code += labeled_code
-
-            if not parser_rule:
-                self.token_start_ranges[rule_name] = self.current_start_range
-                self.current_start_range = None
-
-            return rule_code
-
-        if isinstance(node, (self.antlr_parser_cls.RuleAltListContext, self.antlr_parser_cls.AltListContext, self.antlr_parser_cls.LexerAltListContext)):
-            children = [child for child in node.children if isinstance(child, ParserRuleContext)]
-            if len(children) == 1:
-                return self.generate_single(children[0], parent_id)
-
-            alt_name = self.new_code_id('alt')
-            self.graph.add_node(AlternationNode(id=alt_name))
-            self.graph.add_edge(frm=parent_id, to=alt_name)
-
-            conditions = [(self.new_code_id('cond'), self.find_conditions(child)) for child in children]
-            self.code_chunks.update(conditions)
-            result = self.line('choice = self.choice([0 if {{{alt_name}}}[i] > self.unlexer.max_depth else w * self.unlexer.weights.get(({alt_name!r}, i), 1) for i, w in enumerate([{weights}])])'
-                               .format(weights=', '.join('{{{cond_id}}}'.format(cond_id=cond_id) for cond_id, _ in conditions),
-                                       alt_name=alt_name))
-            result += self.line('self.unlexer.weights[({alt_name!r}, choice)] = self.unlexer.weights.get(({alt_name!r}, choice), 1) * self.unlexer.cooldown'.format(alt_name=alt_name))
-            for i, child in enumerate(children):
-                alternative_name = '{alt_name}_{idx}'.format(alt_name=alt_name, idx=i)
-                self.graph.add_node(AlternativeNode(id=alternative_name))
-                self.graph.add_edge(frm=alt_name, to=alternative_name)
-
-                result += self.line('{if_kw} choice == {idx}:'.format(if_kw='if' if i == 0 else 'elif', idx=i))
-                with self.indent():
-                    result += self.generate_single(child, alternative_name) or self.line('pass')
-            return result
-
-        if isinstance(node, self.antlr_parser_cls.LabeledAltContext) and node.identifier():
-            rule_name = node.parentCtx.parentCtx.parentCtx.RULE_REF().symbol.text
-            name = '{rule_name}_{label_name}'.format(rule_name=rule_name,
-                                                     label_name=(node.identifier().TOKEN_REF() or node.identifier().RULE_REF()).symbol.text)
-            self.graph.add_node(RuleNode(id=name))
-            self.graph.add_edge(frm=parent_id, to=name)
-            # Notify the alternative that it's a labeled one and should be processed later.
-            return self.generate_single(node.alternative(), '#' + name)
-
-        # Sequences.
-        if isinstance(node, (self.antlr_parser_cls.AlternativeContext, self.antlr_parser_cls.LexerAltContext)):
-            if not node.children:
-                return self.line('current += UnlexerRule(src=\'\')')
-
-            if isinstance(node, self.antlr_parser_cls.AlternativeContext):
-                children = node.element()
-            elif isinstance(node, self.antlr_parser_cls.LexerAltContext):
-                children = node.lexerElements().lexerElement()
-            else:
-                children = []
 
-            if parent_id.startswith('#'):
-                # If the current alternative is labeled then it will be processed
-                # later since its content goes to a separate method.
-                parent_id = parent_id[1:]
-                self.labeled_alts.append((parent_id, children))
-                return self.line('current = self.{name}()'.format(name=parent_id))
-
-            return ''.join([self.generate_single(child, parent_id) for child in children])
-
-        if isinstance(node, (self.antlr_parser_cls.ElementContext, self.antlr_parser_cls.LexerElementContext)):
-            if self.actions and node.actionBlock():
-                # Conditions are handled at alternative processing.
-                if node.QUESTION():
-                    return ''
-
-                action_src = ''.join([str(child) for child in node.actionBlock().ACTION_CONTENT()])
-                action_src = re.sub(r'\$(?P<var_name>\w+)', 'local_ctx[\'\\g<var_name>\']', action_src)
-
-                action_id = self.new_code_id('action')
-                self.code_chunks[action_id] = ''.join([self.line(line) for line in action_src.splitlines()])
-                return '{{{action_id}}}'.format(action_id=action_id)
-
-            suffix = None
-            if node.ebnfSuffix():
-                suffix = node.ebnfSuffix()
-            elif hasattr(node, 'ebnf') and node.ebnf() and node.ebnf().blockSuffix():
-                suffix = node.ebnf().blockSuffix().ebnfSuffix()
-
-            if not suffix:
-                return self.generate_single(node.children[0], parent_id)
-
-            suffix = str(suffix.children[0])
-
-            if suffix in ['?', '*']:
-                quant_name = self.new_code_id('quant')
-                self.graph.add_node(QuantifierNode(id=quant_name))
-                self.graph.add_edge(frm=parent_id, to=quant_name)
-                parent_id = quant_name
-
-            quant_type = {'?': 'zero_or_one', '*': 'zero_or_more', '+': 'one_or_more'}[suffix]
-            result = self.line('if self.unlexer.max_depth >= {min_depth}:'.format(min_depth='0' if suffix == '+' else '{{{name}}}'.format(name=parent_id)))
-            with self.indent():
-                result += self.line('for _ in self.{quant_type}():'.format(quant_type=quant_type))
-
-                with self.indent():
-                    result += self.generate_single(node.children[0], parent_id)
-                result += '\n'
-            return result
-
-        if isinstance(node, self.antlr_parser_cls.LabeledElementContext):
-            ident = node.identifier()
-            name = ident.RULE_REF() or ident.TOKEN_REF()
-            result = self.generate_single(node.atom() or node.block(), parent_id)
-            result += self.line('local_ctx[\'{name}\'] = current.last_child'.format(name=name))
-            return result
-
-        if isinstance(node, self.antlr_parser_cls.RulerefContext):
-            self.graph.add_edge(frm=parent_id, to=str(node.RULE_REF()))
-            return self.line('current += self.{rule_name}()'.format(rule_name=node.RULE_REF()))
-
-        if isinstance(node, (self.antlr_parser_cls.LexerAtomContext, self.antlr_parser_cls.AtomContext)):
-            if node.DOT():
-                return self.line('current += UnlexerRule(src=self.any_char())')
-
-            if node.notSet():
-                if node.notSet().setElement():
-                    options = self.chars_from_set(node.notSet().setElement())
-                else:
-                    options = []
-                    for set_element in node.notSet().blockSet().setElement():
-                        options.extend(self.chars_from_set(set_element))
-
-                charset_name = self.new_charset_name()
-                self.unlexer_header += '{charset_name} = list(chain(*multirange_diff(printable_unicode_ranges, [{charset}])))\n'.format(charset_name=charset_name, charset=','.join(['({start}, {end})'.format(start=chr_range[0], end=chr_range[1]) for chr_range in sorted(options, key=lambda x: x[0])]))
-                charset_ref = charset_name if isinstance(node, self.antlr_parser_cls.LexerAtomContext) else '{unlexer_name}.{charset_name}'.format(unlexer_name=self.unlexer_name, charset_name=charset_name)
-                return self.line('current += UnlexerRule(src=self.char_from_list({charset_ref}))'.format(charset_ref=charset_ref))
-
-            if isinstance(node, self.antlr_parser_cls.LexerAtomContext):
-                if node.characterRange():
-                    start, end = self.character_range_interval(node)
-                    if self.current_start_range is not None:
-                        self.current_start_range.append((start, end))
-                    return self.line('current += self.create_node(UnlexerRule(src=self.char_from_list(range({start}, {end}))))'.format(start=start, end=end))
-
-                if node.LEXER_CHAR_SET():
-                    ranges = self.lexer_charset_interval(str(node.LEXER_CHAR_SET())[1:-1])
-
-                    if self.current_start_range is not None:
-                        self.current_start_range.extend(ranges)
-
-                    charset_name = self.new_charset_name()
-                    self.unlexer_header += '{charset_name} = list(chain({charset}))\n'.format(charset_name=charset_name, charset=', '.join(['range({start}, {end})'.format(start=chr_range[0], end=chr_range[1]) for chr_range in ranges]))
-                    return self.line('current += self.create_node(UnlexerRule(src=self.char_from_list({charset_name})))'.format(charset_name=charset_name))
+class GrammarGraph(object):
 
-            return ''.join([self.generate_single(child, parent_id) for child in node.children])
+    def __init__(self):
+        self.name = None
+        self.vertices = OrderedDict()
+        self.options = {}
+        self.charsets = []
+        self.header = ''
+        self.members = ''
+        self.default_rule = None
+
+    @property
+    def superclass(self):
+        return self.options.get('superClass', 'Generator')
+
+    @property
+    def dot(self):
+        return self.options.get('dot', 'any_ascii_char')
+
+    @property
+    def rules(self):
+        return (vertex for vertex in self.vertices.values() if isinstance(vertex, RuleNode))
+
+    @property
+    def imag_rules(self):
+        return (vertex for vertex in self.vertices.values() if isinstance(vertex, ImagRuleNode))
+
+    def print_tree(self, root=None):
+        if not root and not self.default_rule:
+            raise ValueError('Either `root` must be defined or `print` should be called after `default_rule` is set.')
+        (root or self.vertices[self.default_rule]).print_tree()
 
-        if isinstance(node, self.antlr_parser_cls.TerminalContext):
-            if node.TOKEN_REF():
-                self.graph.add_edge(frm=parent_id, to=str(node.TOKEN_REF()))
-                return self.line('current += self.unlexer.{rule_name}()'.format(rule_name=node.TOKEN_REF()))
+    def add_node(self, node):
+        self.vertices[node.id] = node
+        return node.id
 
-            if node.STRING_LITERAL():
-                src = str(node.STRING_LITERAL())[1:-1]
-                if self.current_start_range is not None:
-                    self.current_start_range.append((ord(src[0]), ord(src[0]) + 1))
-                code_id = self.new_code_id('lit')
-                self.code_chunks[code_id] = src
-                return self.line('current += self.create_node(UnlexerRule(src=\'{{{code_id}}}\'))'.format(code_id=code_id))
+    def add_edge(self, frm, to, args=None):
+        assert frm in self.vertices, f'{frm} not in vertices.'
+        assert to in self.vertices, f'{to} not in vertices.'
+        self.vertices[frm].out_edges.append(Edge(dst=self.vertices[to], args=args))
 
-        if isinstance(node, ParserRuleContext) and node.getChildCount():
-            return ''.join([self.generate_single(child, parent_id) for child in node.children])
+    def calc_min_depths(self):
+        min_depths = defaultdict(lambda: inf)
+        changed = True
+
+        while changed:
+            changed = False
+            for ident, node in self.vertices.items():
+                selector = min if isinstance(node, AlternationNode) else max
+                min_depth = selector((min_depths[out_node.id] + int(isinstance(out_node, RuleNode))
+                                      for out_node in node.out_neighbours if not isinstance(out_node, QuantifierNode) or out_node.min > 0), default=0)
+
+                if min_depth < min_depths[ident]:
+                    min_depths[ident] = min_depth
+                    changed = True
+
+        for ident, node in self.vertices.items():
+            if isinstance(node, RuleNode):
+                node.min_depth = min_depths[ident]
+            elif isinstance(node, QuantifierNode):
+                node.min_depth = 0 if node.min > 0 else min_depths[ident]
+            elif isinstance(node, AlternationNode):
+                # Lift the minimal depths of the alternatives to the alternations, where the decision will happen.
+                node.min_depths = [min_depths[alt.id] for alt in node.out_neighbours]
+
+
+def escape_string(s):
+    # To be kept in sync with Python's unicode_escape encoding at CPython's
+    # Objects/unicodeobject.c:PyUnicode_AsUnicodeEscapeString, with the addition
+    # of also escaping quotes.
+    escapes = {
+        '\t': '\\t',
+        '\n': '\\n',
+        '\r': '\\r',
+        '\\': '\\\\',
+        '\'': '\\\''
+    }
+
+    def _iter_escaped_chars(si):
+        for ch in si:
+            esc = escapes.get(ch)
+            if esc is not None:
+                yield esc
+
+            else:
+                cp = ord(ch)
+                if 0x20 <= cp < 0x7f:
+                    yield ch
+                elif cp < 0x100:
+                    yield f'\\x{cp:02x}'
+                elif cp < 0x10000:
+                    yield f'\\u{cp:04x}'
+                else:
+                    yield f'\\U{cp:08x}'
 
-        return ''
+    return ''.join(c for c in _iter_escaped_chars(s))
 
 
-class FuzzerFactory(object):
+class ProcessorTool(object):
     """
-    Class that generates fuzzers from grammars.
+    Class to process ANTLRv4 grammar files, build an internal representation
+    from them and create a generator class that is able to produce textual data
+    according to the grammar files.
     """
-    def __init__(self, work_dir=None, antlr=default_antlr_path):
+    def __init__(self, lang, work_dir=None):
         """
-        :param work_dir: Directory to generate fuzzers into.
-        :param antlr: Path to the ANTLR jar.
+        :param str lang: Language of the generated code (currently, only ``'py'`` is accepted as Python is the only supported language).
+        :param str work_dir: Directory to generate fuzzers into (default: the current working directory).
         """
-        self.work_dir = work_dir or getcwd()
+        self._lang = lang
+        env = Environment(trim_blocks=True,
+                          lstrip_blocks=True,
+                          keep_trailing_newline=False)
+        env.filters['substitute'] = lambda s, frm, to: re.sub(frm, to, str(s))
+        env.filters['escape_string'] = escape_string
+        self._template = env.from_string(get_data(__package__, 'resources/codegen/GeneratorTemplate.' + lang + '.jinja').decode('utf-8'))
+        self._work_dir = work_dir or getcwd()
 
-        antlr_dir = join(self.work_dir, 'antlr')
-        makedirs(antlr_dir, exist_ok=True)
-        # Add the path of the built grammars to the Python path to be available at parsing.
-        if antlr_dir not in sys.path:
-            sys.path.append(antlr_dir)
-
-        # Copy the grammars from the package to the given working directory.
-        antlr_resources = ['ANTLRv4Lexer.g4', 'ANTLRv4Parser.g4', 'LexBasic.g4', 'LexerAdaptor.py']
-        for resource in antlr_resources:
-            with open(join(antlr_dir, resource), 'wb') as f:
-                f.write(get_data(__package__, join('resources', 'antlr', resource)))
-
-        self.antlr_lexer_cls, self.antlr_parser_cls, _ = build_grammars(antlr_resources, antlr_dir, antlr=antlr)
-
-    def generate_fuzzer(self, grammars, *, encoding='utf-8', lib_dir=None, actions=True, pep8=False):
+    def process(self, grammars, *, options=None, default_rule=None, encoding='utf-8', errors='strict', lib_dir=None, actions=True, pep8=False):
         """
-        Generates fuzzers from grammars.
+        Perform the four main steps:
 
-        :param grammars: List of grammar files to generate from.
-        :param encoding: Grammar file encoding.
-        :param lib_dir: Alternative directory to look for imports.
-        :param actions: Boolean to enable or disable grammar actions.
-        :param pep8: Boolean to enable pep8 to beautify the generated fuzzer source.
+          1. Parse the grammar files.
+          2. Build an internal representation of the grammar.
+          3. Translate the internal representation into a generator source code in the target language.
+          4. Save the source code into file.
+
+        :param list[str] grammars: List of grammar files to produce generator from.
+        :param dict options: Options dictionary to override/extend the options set in the grammar.
+               Currenly, the following options are supported:
+
+                 1. ``superClass``: Define the ancestor for the current grammar. The generator of this grammar will be inherited from ``superClass``. (default: :class:`grammarinator.runtime.Generator`)
+                 2. ``dot``: Define how to handle the ``.`` wildcard in the grammar. Three keywords are accepted:
+
+                     1. ``any_ascii_letter``: generate any ASCII letters
+                     2. ``any_ascii_char``: generate any ASCII characters
+                     3. ``any_unicode_char``: generate any Unicode characters
+
+                    (default: ``any_ascii_char``)
+
+        :param str default_rule: Name of the default rule to start generation from (default: first parser rule in the grammar).
+        :param str encoding: Grammar file encoding.
+        :param str errors: Encoding error handling scheme.
+        :param str lib_dir: Alternative directory to look for grammar imports beside the current working directory.
+        :param bool actions: Boolean to enable grammar actions. If they are disabled then the inline actions and semantic
+               predicates of the input grammar (snippets in ``{...}`` and ``{...}?`` form) are disregarded (i.e., no code is
+               generated from them).
+        :param bool pep8: Boolean to enable pep8 to beautify the generated fuzzer source.
         """
         lexer_root, parser_root = None, None
 
         for grammar in grammars:
-            root = self._parse(grammar, encoding, lib_dir)
-            # Lexer and/or combined grammars are processed first to evaluate TOKEN_REF-s.
-            if root.grammarType().LEXER() or not root.grammarType().PARSER():
-                lexer_root = root
+            if grammar.endswith('.g4'):
+                root = self._parse_grammar(grammar, encoding, errors, lib_dir)
+                # Lexer and/or combined grammars are processed first to evaluate TOKEN_REF-s.
+                if root.grammarDecl().grammarType().LEXER() or not root.grammarDecl().grammarType().PARSER():
+                    lexer_root = root
+                else:
+                    parser_root = root
             else:
-                parser_root = root
+                copy(grammar, self._work_dir)
 
-        fuzzer_generator = FuzzerGenerator(self.antlr_parser_cls, actions)
-        for name, src in fuzzer_generator.generate(lexer_root, parser_root):
-            with open(join(self.work_dir, name + '.py'), 'w') as f:
-                if pep8:
-                    src = autopep8.fix_code(src)
-                f.write(src)
+        graph = self._build_graph(actions, lexer_root, parser_root, options, default_rule)
+        self._analyze_graph(graph)
 
-    def _collect_imports(self, root, base_dir, lib_dir):
-        imports = set()
-        for prequel in root.prequelConstruct():
-            if prequel.delegateGrammars():
-                for delegate_grammar in prequel.delegateGrammars().delegateGrammar():
-                    ident = delegate_grammar.identifier(0)
-                    grammar_fn = str(ident.RULE_REF() or ident.TOKEN_REF()) + '.g4'
-                    if lib_dir is not None and exists(join(lib_dir, grammar_fn)):
-                        imports.add(join(lib_dir, grammar_fn))
-                    else:
-                        imports.add(join(base_dir, grammar_fn))
-        return imports
+        src = self._template.render(graph=graph, version=__version__).lstrip()
+        with open(join(self._work_dir, graph.name + '.' + self._lang), 'w') as f:
+            if pep8:
+                src = autopep8.fix_code(src)
+            f.write(src)
 
-    def _parse(self, grammar, encoding, lib_dir):
+    def _parse_grammar(self, grammar, encoding, errors, lib_dir):
         work_list = {grammar}
         root = None
 
         while work_list:
             grammar = work_list.pop()
 
-            antlr_parser = self.antlr_parser_cls(CommonTokenStream(self.antlr_lexer_cls(FileStream(grammar, encoding=encoding))))
+            antlr_parser = ANTLRv4Parser(CommonTokenStream(ANTLRv4Lexer(FileStream(grammar, encoding=encoding, errors=errors))))
             current_root = antlr_parser.grammarSpec()
             # assert antlr_parser._syntaxErrors > 0, 'Parse error in ANTLR grammar.'
 
             # Save the 'outermost' grammar.
             if not root:
                 root = current_root
             else:
@@ -665,53 +468,468 @@
                 for rule in current_root.rules().ruleSpec():
                     root.rules().addChild(rule)
 
             work_list |= self._collect_imports(current_root, dirname(grammar), lib_dir)
 
         return root
 
+    @staticmethod
+    def _collect_imports(root, base_dir, lib_dir):
+        imports = set()
+        for prequel in root.prequelConstruct():
+            if prequel.delegateGrammars():
+                for delegate_grammar in prequel.delegateGrammars().delegateGrammar():
+                    ident = delegate_grammar.identifier(0)
+                    grammar_fn = str(ident.RULE_REF() or ident.TOKEN_REF()) + '.g4'
+                    if lib_dir is not None and exists(join(lib_dir, grammar_fn)):
+                        imports.add(join(lib_dir, grammar_fn))
+                    else:
+                        imports.add(join(base_dir, grammar_fn))
+        return imports
+
+    @staticmethod
+    def _build_graph(actions, lexer_root, parser_root, options, default_rule):
+
+        def find_conditions(node):
+            if not actions:
+                return '1'
+
+            if isinstance(node, str):
+                return node
+
+            action_block = getattr(node, 'actionBlock', None)
+            if action_block:
+                if action_block() and action_block().ACTION_CONTENT() and node.QUESTION():
+                    return ''.join(str(child) for child in action_block().ACTION_CONTENT())
+                return '1'
+
+            element = getattr(node, 'element', None) or getattr(node, 'lexerElement', None)
+            if element:
+                if not element():
+                    return '1'
+                return find_conditions(element(0))
+
+            child_ref = getattr(node, 'alternative', None) or getattr(node, 'lexerElements', None)
+
+            # An alternative can be explicitly empty, in this case it won't have any of the attributes above.
+            if not child_ref:
+                return '1'
+
+            return find_conditions(child_ref())
+
+        def character_range_interval(node):
+            start = str(node.characterRange().STRING_LITERAL(0))[1:-1]
+            end = str(node.characterRange().STRING_LITERAL(1))[1:-1]
+            start_cp, start_offset = process_lexer_char(start, 0)
+            end_cp, end_offset = process_lexer_char(end, 0)
+
+            if start_offset < len(start) or end_offset < len(end):
+                raise ValueError(f'Only single characters are allowed in character ranges ({start!r}..{end!r})')
 
-def execute():
-    parser = ArgumentParser(description='Grammarinator: Processor', epilog="""
-        The tool processes a grammar in ANTLR v4 format (*.g4, either separated
-        to lexer and parser grammar files, or a single combined grammar) and
-        creates a fuzzer (a pair of unlexer and unparser) that can generate
-        randomized content conforming to the format described by the grammar.
-        """)
-    parser.add_argument('grammars', nargs='+', metavar='FILE',
-                        help='ANTLR grammar files describing the expected format to generate.')
-    parser.add_argument('--antlr', metavar='FILE', default=default_antlr_path,
-                        help='path of the ANTLR jar file (default: %(default)s).')
-    parser.add_argument('--no-actions', dest='actions', default=True, action='store_false',
-                        help='do not process inline actions.')
-    parser.add_argument('--encoding', metavar='ENC', default='utf-8',
-                        help='grammar file encoding (default: %(default)s).')
-    parser.add_argument('--lib', metavar='DIR',
-                        help='alternative location of import grammars.')
-    parser.add_argument('--disable-cleanup', dest='cleanup', default=True, action='store_false',
-                        help='disable the removal of intermediate files.')
-    parser.add_argument('--pep8', default=False, action='store_true',
-                        help='enable autopep8 to format the generated fuzzer.')
-    parser.add_argument('--log-level', metavar='LEVEL', default='INFO',
-                        help='verbosity level of diagnostic messages (default: %(default)s).')
-    parser.add_argument('-o', '--out', metavar='DIR', default=getcwd(),
-                        help='temporary working directory (default: %(default)s).')
-    parser.add_argument('--version', action='version', version='%(prog)s {version}'.format(version=__version__))
-    args = parser.parse_args()
-
-    logger.setLevel(args.log_level)
-
-    for grammar in args.grammars:
-        if not exists(grammar):
-            parser.error('{grammar} does not exist.'.format(grammar=grammar))
-
-    if args.antlr == default_antlr_path:
-        antlerinator.install(lazy=True)
+            return start_cp, end_cp + 1
 
-    FuzzerFactory(args.out, args.antlr).generate_fuzzer(args.grammars, encoding=args.encoding, lib_dir=args.lib, actions=args.actions, pep8=args.pep8)
+        def process_lexer_char(s, offset):
+            # To be kept in sync with org.antlr.v4.misc.EscapeSequenceParsing.parseEscape
 
-    if args.cleanup:
-        rmtree(join(args.out, 'antlr'), ignore_errors=True)
+            # Original Java code has to handle unicode codepoints which consist of more than one character,
+            # however in Python 3.3+, we don't have to worry about this: https://stackoverflow.com/a/42262842
 
+            if s[offset] != '\\':
+                return ord(s[offset]), offset + 1
 
-if __name__ == '__main__':
-    execute()
+            if offset + 2 > len(s):
+                raise ValueError('Escape must have at least two characters')
+
+            escaped = s[offset + 1]
+            offset += 2  # Move past backslash and escaped character
+
+            if escaped == 'u':
+                if s[offset] == '{':
+                    # \u{...}
+                    hex_start_offset = offset + 1
+                    hex_end_offset = s.find('}', hex_start_offset)
+                    if hex_end_offset == -1:
+                        raise ValueError('Missing closing bracket for unicode escape')
+                    if hex_start_offset == hex_end_offset:
+                        raise ValueError('Missing codepoint for unicode escape')
+
+                    offset = hex_end_offset + 1  # Skip over last bracket
+                else:
+                    # \uXXXX
+                    hex_start_offset = offset
+                    hex_end_offset = hex_start_offset + 4
+                    if hex_end_offset > len(s):
+                        raise ValueError('Non-bracketed unicode escape must be of form \\uXXXX')
+
+                    offset = hex_end_offset
+
+                try:
+                    codepoint = int(s[hex_start_offset:hex_end_offset], 16)
+                except ValueError as exc:
+                    raise ValueError('Invalid hex value') from exc
+
+                if codepoint < 0 or codepoint > maxunicode:
+                    raise ValueError('Invalid unicode codepoint')
+
+                return codepoint, offset
+
+            if escaped in ('p', 'P'):
+                raise ValueError('Unicode properties (\\p{...}) are not supported')
+
+            # To be kept in sync with org.antlr.v4.misc.CharSupport.ANTLRLiteralEscapedCharValue
+            escaped_values = {
+                'n': '\n',
+                'r': '\r',
+                'b': '\b',
+                't': '\t',
+                'f': '\f',
+                '\\': '\\',
+                # Additional escape sequences defined by org.antlr.v4.misc.EscapeSequenceParsing.parseEscape
+                '-': '-',
+                ']': ']',
+                '\'': '\''
+            }
+
+            if escaped in escaped_values:
+                return ord(escaped_values[escaped]), offset
+
+            raise ValueError('Invalid escaped value')
+
+        def lexer_charset_interval(s):
+            # To be kept in sync with org.antlr.v4.automata.LexerATNFactory.getSetFromCharSetLiteral
+            assert len(s) > 0, 'Charset cannot be empty'
+
+            ranges = []
+
+            offset = 0
+            while offset < len(s):
+                in_range = s[offset] == '-' and offset != 0 and offset != len(s) - 1
+                if in_range:
+                    offset += 1
+
+                codepoint, offset = process_lexer_char(s, offset)
+
+                if in_range:
+                    ranges[-1] = (ranges[-1][0], codepoint + 1)
+                else:
+                    ranges.append((codepoint, codepoint + 1))
+
+            return ranges
+
+        def chars_from_set(node):
+            if node.characterRange():
+                return [character_range_interval(node)]
+
+            if node.LEXER_CHAR_SET():
+                return lexer_charset_interval(str(node.LEXER_CHAR_SET())[1:-1])
+
+            if node.STRING_LITERAL():
+                char = str(node.STRING_LITERAL())[1:-1]
+                char_cp, char_offset = process_lexer_char(char, 0)
+                if char_offset < len(char):
+                    raise ValueError(f'Zero or multi-character literals are not allowed in lexer sets: {char!r}')
+                return [(char_cp, char_cp + 1)]
+
+            if node.TOKEN_REF():
+                src = str(node.TOKEN_REF())
+                assert graph.vertices[src].start_ranges is not None, f'{src} has no character start ranges.'
+                return graph.vertices[src].start_ranges
+
+            return []
+
+        def unescape_string(s):
+            def _iter_unescaped_chars(s):
+                offset = 0
+                while offset < len(s):
+                    codepoint, offset = process_lexer_char(s, offset)
+                    yield chr(codepoint)
+
+            return ''.join(c for c in _iter_unescaped_chars(s))
+
+        def argActionBlock(node):
+            args = {}
+            if node and node.argActionBlock():
+                for arg in ''.join(str(chr_arg) for chr_arg in node.argActionBlock().ARGUMENT_CONTENT()).split(','):
+                    arg_name, arg_value = arg, None
+                    if '=' in arg_name:
+                        arg_name, arg_value = arg_name.split('=')
+                    args[arg_name.strip()] = arg_value.strip() if arg_value else arg_value
+            return args
+
+        def build_rule(rule, node):
+            lexer_rule = isinstance(rule, UnlexerRuleNode)
+            alt_idx, quant_idx, chr_idx = 0, 0, 0  # pylint: disable=unused-variable
+
+            def build_expr(node, parent_id):
+                if isinstance(node, ANTLRv4Parser.ParserRuleSpecContext):
+                    if actions:
+                        rule.args = argActionBlock(node)
+                        rule.locals = argActionBlock(node.localsSpec())
+                        rule.returns = argActionBlock(node.ruleReturns())
+                    build_expr(node.ruleBlock(), parent_id)
+
+                elif isinstance(node, (ANTLRv4Parser.RuleAltListContext, ANTLRv4Parser.AltListContext, ANTLRv4Parser.LexerAltListContext)):
+                    children = [child for child in node.children if isinstance(child, ParserRuleContext)]
+                    if len(children) == 1:
+                        build_expr(children[0], parent_id)
+                        return
+
+                    nonlocal alt_idx
+                    alt_id = graph.add_node(AlternationNode(idx=alt_idx, conditions=[find_conditions(child) for child in children], rule_id=rule.name))
+                    alt_idx += 1
+                    graph.add_edge(frm=parent_id, to=alt_id)
+
+                    for i, child in enumerate(children):
+                        alternative_id = graph.add_node(AlternativeNode(rule_id=rule.name, alt_idx=graph.vertices[alt_id].idx, idx=i))
+                        graph.add_edge(frm=alt_id, to=alternative_id)
+                        build_expr(child, alternative_id)
+
+                elif isinstance(node, ANTLRv4Parser.LabeledAltContext):
+                    if not node.identifier():
+                        build_expr(node.alternative(), parent_id)
+                        return
+
+                    rule_node = UnparserRuleNode(name=rule.name, label=str(node.identifier().TOKEN_REF() or node.identifier().RULE_REF()))
+                    graph.add_edge(frm=parent_id, to=graph.add_node(rule_node))
+                    build_rule(rule_node, node.alternative())
+
+                elif isinstance(node, (ANTLRv4Parser.AlternativeContext, ANTLRv4Parser.LexerAltContext)):
+                    children = node.element() if isinstance(node, ANTLRv4Parser.AlternativeContext) else node.lexerElements().lexerElement()
+                    for child in children:
+                        build_expr(child, parent_id)
+
+                    if not graph.vertices[parent_id].out_neighbours:
+                        graph.add_edge(frm=parent_id, to=lambda_id)
+
+                elif isinstance(node, (ANTLRv4Parser.ElementContext, ANTLRv4Parser.LexerElementContext)):
+                    if node.actionBlock():
+                        # Conditions are handled at alternative processing.
+                        if not actions or node.QUESTION():
+                            return
+
+                        graph.add_edge(frm=parent_id, to=graph.add_node(ActionNode(src=''.join(str(child) for child in node.actionBlock().ACTION_CONTENT()))))
+                        return
+
+                    suffix = None
+                    if node.ebnfSuffix():
+                        suffix = node.ebnfSuffix()
+                    elif hasattr(node, 'ebnf') and node.ebnf() and node.ebnf().blockSuffix():
+                        suffix = node.ebnf().blockSuffix().ebnfSuffix()
+
+                    if not suffix:
+                        build_expr(node.children[0], parent_id)
+                        return
+
+                    nonlocal quant_idx
+                    suffix = str(suffix.children[0])
+                    quant_ranges = {'?': {'min': 0, 'max': 1}, '*': {'min': 0, 'max': 'inf'}, '+': {'min': 1, 'max': 'inf'}}
+                    quant_id = graph.add_node(QuantifierNode(rule_id=rule.name, idx=quant_idx, **quant_ranges[suffix]))
+                    quant_idx += 1
+                    graph.add_edge(frm=parent_id, to=quant_id)
+                    build_expr(node.children[0], quant_id)
+
+                elif isinstance(node, ANTLRv4Parser.LabeledElementContext):
+                    build_expr(node.atom() or node.block(), parent_id)
+                    ident = node.identifier()
+                    name = str(ident.RULE_REF() or ident.TOKEN_REF())
+                    is_list = node.PLUS_ASSIGN() is not None
+                    graph.add_edge(frm=parent_id, to=graph.add_node(VariableNode(name=name, is_list=is_list)))
+                    rule.labels[name] = is_list
+
+                elif isinstance(node, ANTLRv4Parser.RulerefContext):
+                    graph.add_edge(frm=parent_id, to=str(node.RULE_REF()), args=argActionBlock(node) if actions else None)
+
+                elif isinstance(node, (ANTLRv4Parser.LexerAtomContext, ANTLRv4Parser.AtomContext)):
+                    nonlocal chr_idx
+
+                    if node.DOT():
+                        graph.add_edge(frm=parent_id, to=graph.add_node(CharsetNode(rule_id=rule.name, idx=chr_idx, charset=dot_charset.id)))
+                        chr_idx += 1
+
+                    elif node.notSet():
+                        if node.notSet().setElement():
+                            not_ranges = chars_from_set(node.notSet().setElement())
+                        else:
+                            not_ranges = []
+                            for set_element in node.notSet().blockSet().setElement():
+                                not_ranges.extend(chars_from_set(set_element))
+
+                        charset = Charset(multirange_diff(dot_charset.ranges, sorted(not_ranges, key=lambda x: x[0])))
+                        graph.charsets.append(charset)
+                        graph.add_edge(frm=parent_id, to=graph.add_node(CharsetNode(rule_id=rule.name, idx=chr_idx, charset=charset.id)))
+                        chr_idx += 1
+
+                    elif isinstance(node, ANTLRv4Parser.LexerAtomContext) and node.characterRange():
+                        start, end = character_range_interval(node)
+                        if lexer_rule:
+                            rule.start_ranges.append((start, end))
+
+                        charset = Charset([(start, end)])
+                        graph.charsets.append(charset)
+                        graph.add_edge(frm=parent_id, to=graph.add_node(CharsetNode(rule_id=rule.name, idx=chr_idx, charset=charset.id)))
+                        chr_idx += 1
+
+                    elif isinstance(node, ANTLRv4Parser.LexerAtomContext) and node.LEXER_CHAR_SET():
+                        ranges = lexer_charset_interval(str(node.LEXER_CHAR_SET())[1:-1])
+                        if lexer_rule:
+                            rule.start_ranges.extend(ranges)
+
+                        charset = Charset(sorted(ranges, key=lambda x: x[0]))
+                        graph.charsets.append(charset)
+                        graph.add_edge(frm=parent_id, to=graph.add_node(CharsetNode(rule_id=rule.name, idx=chr_idx, charset=charset.id)))
+                        chr_idx += 1
+
+                    for child in node.children:
+                        build_expr(child, parent_id)
+
+                elif isinstance(node, ANTLRv4Parser.TerminalContext):
+                    if node.TOKEN_REF():
+                        graph.add_edge(frm=parent_id, to=str(node.TOKEN_REF()))
+
+                    elif node.STRING_LITERAL():
+                        src = unescape_string(str(node.STRING_LITERAL())[1:-1])
+
+                        if lexer_rule:
+                            rule.start_ranges.append((ord(src[0]), ord(src[0]) + 1))
+
+                        graph.add_edge(frm=parent_id, to=graph.add_node(LiteralNode(src=src)))
+
+                elif isinstance(node, ParserRuleContext) and node.getChildCount():
+                    for child in node.children:
+                        build_expr(child, parent_id)
+
+            if lexer_rule:
+                rule.start_ranges = []
+
+            build_expr(node, rule.id)
+
+        def build_prequel(node):
+            assert isinstance(node, ANTLRv4Parser.GrammarSpecContext)
+
+            if not graph.name:
+                graph.name = re.sub(r'^(.+?)(Lexer|Parser)?$', r'\1Generator', str(node.grammarDecl().identifier().TOKEN_REF() or node.grammarDecl().identifier().RULE_REF()))
+
+            for prequelConstruct in node.prequelConstruct() if node.prequelConstruct() else ():
+                for option in prequelConstruct.optionsSpec().option() if prequelConstruct.optionsSpec() else ():
+                    ident = option.identifier()
+                    ident = str(ident.RULE_REF() or ident.TOKEN_REF())
+                    graph.options[ident] = option.optionValue().getText()
+
+                for identifier in prequelConstruct.tokensSpec().idList().identifier() if prequelConstruct.tokensSpec() and prequelConstruct.tokensSpec().idList() else ():
+                    assert identifier.TOKEN_REF() is not None, 'Token names must start with uppercase letter.'
+                    graph.add_node(ImagRuleNode(id=str(identifier.TOKEN_REF())))
+
+                if prequelConstruct.action_() and actions:
+                    action = prequelConstruct.action_()
+                    action_ident = action.identifier()
+                    action_type = str(action_ident.RULE_REF() or action_ident.TOKEN_REF())
+                    raw_action_src = ''.join(str(child) for child in action.actionBlock().ACTION_CONTENT())
+
+                    # We simply append both members and header code chunks to the generated source.
+                    # It's the user's responsibility to define them in order.
+                    if action_type == 'members':
+                        graph.members += raw_action_src
+                    elif action_type == 'header':
+                        graph.header += raw_action_src
+
+        def build_rules(node):
+            generator_rules, duplicate_rules = [], []
+            for rule in node.rules().ruleSpec():
+                if rule.parserRuleSpec():
+                    rule_spec = rule.parserRuleSpec()
+                    rule_node = UnparserRuleNode(name=str(rule_spec.RULE_REF()))
+                    antlr_node = rule_spec
+                elif rule.lexerRuleSpec():
+                    rule_spec = rule.lexerRuleSpec()
+                    rule_node = UnlexerRuleNode(name=str(rule_spec.TOKEN_REF()))
+                    antlr_node = rule_spec.lexerRuleBlock()
+                else:
+                    assert False, 'Should not get here.'
+
+                if rule_node.id not in graph.vertices:
+                    graph.add_node(rule_node)
+                    generator_rules.append((rule_node, antlr_node))
+                else:
+                    duplicate_rules.append(rule_node.id)
+
+            for mode_spec in node.modeSpec():
+                for rule_spec in mode_spec.lexerRuleSpec():
+                    rule_node = UnlexerRuleNode(name=str(rule_spec.TOKEN_REF()))
+                    if rule_node.id not in graph.vertices:
+                        graph.add_node(rule_node)
+                        generator_rules.append((rule_node, rule_spec.lexerRuleBlock()))
+                    else:
+                        duplicate_rules.append(rule_node.id)
+
+            if duplicate_rules:
+                raise ValueError(f'Rule redefinition(s): {", ".join(duplicate_rules)}')
+
+            for rule_args in generator_rules:
+                build_rule(*rule_args)
+
+            if default_rule:
+                graph.default_rule = default_rule
+            elif node.grammarDecl().grammarType().PARSER() or not (node.grammarDecl().grammarType().LEXER() or node.grammarDecl().grammarType().PARSER()):
+                graph.default_rule = generator_rules[0][0].name
+
+        graph = GrammarGraph()
+        lambda_id = graph.add_node(LambdaNode())
+        graph.add_node(UnlexerRuleNode(name='EOF'))
+
+        for root in [lexer_root, parser_root]:
+            if root:
+                build_prequel(root)
+        graph.options.update(options or {})
+
+        dot_charset = Charset(Charset.dot[graph.dot])
+        graph.charsets.append(dot_charset)
+
+        for root in [lexer_root, parser_root]:
+            if root:
+                build_rules(root)
+
+        graph.calc_min_depths()
+        return graph
+
+    # Calculates the distance of every rule node from the start node. As a result, it can
+    # point out to rules, that are not available from there, furthermore it can give a hint
+    # about the farthest node/rule to help to determine a max_depth that has the chance to
+    # reach every rule. Also checks for infinite derivations.
+    @staticmethod
+    def _analyze_graph(graph, root=None):
+        root = root or graph.default_rule
+        min_distances = defaultdict(lambda: inf)
+        min_distances[root] = 0
+
+        work_list = [root]
+        while work_list:
+            v = work_list.pop(0)
+            for out_v in graph.vertices[v].out_neighbours:
+                d = min_distances[v] + int(isinstance(out_v, RuleNode))
+                if d < min_distances[out_v.id]:
+                    min_distances[out_v.id] = d
+                    work_list.append(out_v.id)
+
+        farthest_ident, max_distance = max(((v_id, d) for v_id, d in min_distances.items() if (isinstance(graph.vertices[v_id], RuleNode) and d != inf)), key=lambda item: item[1])
+        unreachable_rules = [v_id for v_id, v in graph.vertices.items() if isinstance(v, RuleNode) and min_distances[v_id] == inf]
+
+        logger.info('\tThe farthest rule from %r is %r (%d steps).', root, farthest_ident, max_distance)
+        if unreachable_rules:
+            logger.warning('\t%d rule(s) unreachable from %r: %s', len(unreachable_rules), root, ', '.join(map(repr, unreachable_rules)))
+
+        inf_alts = []
+        inf_rules = []
+        for ident, node in graph.vertices.items():
+            if isinstance(node, AlternationNode):
+                for alternative_idx, alternative_node in enumerate(node.out_neighbours):
+                    if node.min_depths[alternative_idx] == inf:
+                        # Generate human-readable description for an alternative in the graph. The output is a
+                        # (rule node, alternation node, alternative node) string, where `rule` defines the container
+                        # rule and the (alternation node, alternative node) sequence defines a derivation reaching the alternative.
+                        inf_alts.append(', '.join(map(str, [graph.vertices[alternative_node.rule_id], node, alternative_node])))
+            elif isinstance(node, RuleNode):
+                if node.min_depth == inf:
+                    inf_rules.append(ident)
+        if inf_alts:
+            logger.warning('\t%d alternative(s) with infinite derivation (rule node, alternation node, alternative node):\n\t%s', len(inf_alts), ',\n\t'.join(inf_alts))
+        if inf_rules:
+            logger.warning('\t%d rule(s) with infinite derivation (possible cycles): %s', len(inf_rules), ', '.join(map(repr, inf_rules)))
```

### Comparing `grammarinator-19.3/PKG-INFO` & `grammarinator-23.7/docs/guide/grammar_overview.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,160 +1,177 @@
-Metadata-Version: 1.0
-Name: grammarinator
-Version: 19.3
-Summary: Grammarinator: Grammar-based Random Test Generator
-Home-page: https://github.com/renatahodovan/grammarinator
-Author: Renata Hodovan, Akos Kiss
-Author-email: hodovan@inf.u-szeged.hu, akiss@inf.u-szeged.hu
-License: BSD
-Description: =============
-        Grammarinator
-        =============
-        *ANTLRv4 grammar-based test generator*
-        
-        .. image:: https://badge.fury.io/py/grammarinator.svg
-           :target: https://badge.fury.io/py/grammarinator
-        .. image:: https://travis-ci.org/renatahodovan/grammarinator.svg?branch=master
-           :target: https://travis-ci.org/renatahodovan/grammarinator
-        .. image:: https://ci.appveyor.com/api/projects/status/0f1vm5x9j9j31hpo/branch/master?svg=true
-           :target: https://ci.appveyor.com/project/renatahodovan/grammarinator/branch/master
-        .. image:: https://coveralls.io/repos/github/renatahodovan/grammarinator/badge.svg
-           :target: https://coveralls.io/github/renatahodovan/grammarinator
-        
-        *Grammarinator* is a random test generator / fuzzer that creates test cases
-        according to an input ANTLR_ v4 grammar. The motivation behind this
-        grammar-based approach is to leverage the large variety of publicly
-        available `ANTLR v4 grammars`_.
-        
-        .. _`ANTLR v4 grammars`: https://github.com/antlr/grammars-v4
-        
-        
-        Requirements
-        ============
-        
-        * Python_ >= 3.4
-        * pip_ and setuptools Python packages (the latter is automatically installed by
-          pip).
-        * ANTLR_ v4
-        
-        .. _Python: https://www.python.org
-        .. _pip: https://pip.pypa.io
-        .. _ANTLR: http://www.antlr.org
-        
-        
-        Install
-        =======
-        
-        The quick way::
-        
-            pip3 install grammarinator
-        
-        Or clone the project and run setuptools::
-        
-            python3 setup.py install
-        
-        
-        Usage
-        =====
-        
-        As a first step, *grammarinator* takes an `ANTLR v4`_ grammar and creates a test
-        generator script in Python3. Such a generator can be subclassed later to
-        customize it further if needed.
-        
-        Example usage to create a test generator::
-        
-            grammarinator-process <grammar-file(s)> -o <output-directory> --no-actions
-        
-        .. _`ANTLR v4`: https://github.com/antlr/grammars-v4
-        
-        **Notes**
-        
-        Grammarinator uses the `ANTLR v4`_ grammar format as its input, which makes
-        existing grammars (lexer and parser rules) easily reusable. However, because
-        of the inherently different goals of a fuzzer and a parser, inlined code
-        (actions and conditions, header and member blocks) are most probably not
-        reusable, or even preventing proper execution. For first experiments with
-        existing grammar files, ``grammarinator-process`` supports the command-line
-        option ``--no-actions``, which skips all such code blocks during fuzzer
-        generation. Once inlined code is tuned for fuzzing, that option may be omitted.
-        
-        After having generated and optionally customized a fuzzer, it can be executed
-        either by the ``grammarinator-generate`` script or by instantiating it
-        manually.
-        
-        Example usage of ``grammarinator-generate``::
-        
-            grammarinator-generate -l <unlexer> -p <unparser> -r <start-rule> -d <max-depth> \
-            -o <output-pattern> -n <number-of-tests> \
-            -t <one-or-more-transformer>
-        
-        **Notes**
-        
-        Real-life grammars often use recursive rules to express certain patterns.
-        However, when using such rule(s) for generation, we can easily end up in an
-        unexpectedly deep call stack. With the ``--max-depth`` or ``-d`` options, this
-        depth - and also the size of the generated test cases - can be controlled.
-        
-        Another speciality of the ANTLR grammars is that they support the so-called
-        hidden tokens. These rules typically describe such elements of the target
-        language that can be placed basically anywhere without breaking the syntax. The
-        most common examples are comments or whitespaces. However, when using these
-        grammars - which don't define explicitly where whitespace may or may not appear
-        in rules - to generate test cases, we have to insert the missing spaces
-        manually. This can be done by applying various transformers (with the ``-t``
-        option) to the tree representation of the output tests. A simple transformer -
-        that inserts a space after every unparser rule - is provided by grammarinator
-        (``grammarinator.runtime.simple_space_transformer``).
-        
-        As a final thought, one must not forget that the original purpose of grammars
-        is the syntax-wise validation of various inputs. As a consequence, these
-        grammars encode syntactic expectations only, and not semantic rules. If we
-        still want to add semantic knowledge into the generated test, then we can
-        inherit custom fuzzers from the generated ones and redefine methods
-        corresponding to lexer or parser rules in ways that encode the required
-        knowledge (e.g.: HTMLCustomUnparser_).
-        
-        .. _HTMLCustomUnparser: examples/fuzzer/HTMLCustomUnparser.py
-        
-        Working Example
-        ===============
-        
-        The repository contains a minimal example_ to generate HTML files. To give it
-        a try, run the processor first::
-        
-            grammarinator-process examples/grammars/HTMLLexer.g4 \
-            examples/grammars/HTMLParser.g4 -o examples/fuzzer/
-        
-        
-        Then, use the generator to produce test cases::
-        
-            grammarinator-generate -l examples/fuzzer/HTMLCustomUnlexer.py \
-            -p examples/fuzzer/HTMLCustomUnparser.py -r htmlDocument \
-            -o examples/tests/test_%d.html -t HTMLUnparser.html_space_transformer -n 100 -d 20
-        
-        .. _example: examples/
-        
-        
-        Compatibility
-        =============
-        
-        *grammarinator* was tested on:
-        
-        * Linux (Ubuntu 16.04 / 18.04)
-        * Mac OS X (Sierra 10.12 / High Sierra 10.13 / Mojave 10.14)
-        
-        
-        Citations
-        =========
-        
-        Background on *grammarinator* is published in (R. Hodovan, A. Kiss, T. Gyimothy:
-        "Grammarinator: A Grammar-Based Open Source Fuzzer", A-TEST 2018).
-        
-        
-        Copyright and Licensing
-        =======================
-        
-        Licensed under the BSD 3-Clause License_.
-        
-        .. _LICENSE: LICENSE.rst
-        
-Platform: UNKNOWN
+================
+Grammar Overview
+================
+
+Grammarinator supports `ANTLRv4 grammar`_ files as input, but it does not
+necessarily utilize all of the grammar's features for fuzzer and test
+generation purposes.
+
+In the following, the supported features are introduced.
+
+.. code-block:: text
+   :caption: The structure of ANTLRv4 grammars
+
+    /** Optional javadoc style comment */
+    grammar GrammarName;
+
+    options {key1=value1; key2=value2; /* ... */ }
+
+    import Grammar1, Grammar2 /* , ... */;
+
+    tokens {Imag1, Imag2 /* , ... */ }
+
+    @header { /* code block in the target language */ }
+    @members { /* code block in the target language */ }
+
+    // Parser and lexer rules, possibly intermingled.
+    rule1: alt1 | alt2 /* | ... */ ;
+    // ...
+    ruleN: /* ... */ ;
+
+
+The grammar starts with the declaration of its type and name. The declaration
+syntax looks like:
+
+.. code-block:: antlr
+
+    grammarDecl : ('lexer' | 'parser')? 'grammar' grammarName ';' ;
+
+
+The name of the grammar and the name of the containing file must match, with
+the file having the extension ``.g4``. The type of the grammar can be indicated
+as a prefix before the ``grammar`` keyword. It can be specified as ``lexer``
+for a lexer grammar, ``parser`` for a parser grammar, or omitted for a combined
+grammar.
+
+A combined grammar can include both lexer and parser rules, while a lexer
+grammar should only contain lexer rules, and a parser grammar should only
+contain parser rules. In the case of Grammarinator, the name of the grammar
+is used to generate the name of the corresponding fuzzer class, following
+the format ``<GrammarName>Generator``.
+
+
+Options, Imports, Tokens, Named Actions
+=======================================
+
+After the grammar definition, the ANTLR grammar file may include optional
+sections such as options, imports, tokens, and named actions. These
+sections can appear in any order.
+
+.. _options:
+
+The **options** section allows for customizing and configuring various aspects
+of the grammar. Options are defined using a key-value pair syntax, similar to
+a dictionary. The supported keys for the ``options`` section in Grammarinator
+are as follows:
+
+  1) ``superClass``: This option defines the ancestor class of the generator
+     created from the current grammar.
+  2) ``dot``: This option specifies how the generator should handle the
+     wildcard character ``.`` in the grammar.
+     The "dot" option accepts three possible values:
+
+     - ``any_ascii_letter``: generates any ASCII letter
+     - ``any_ascii_char``: generates any ASCII character
+     - ``any_unicode_char``: generates any Unicode character
+
+**Imports** allow for the inclusion of external grammars into the importing
+grammar. This means that the rules defined in the imported grammar will be
+treated as if they were part of the importing grammar.
+Consequently, the methods generated for these imported rules will become
+members of the generated fuzzer.
+
+The **tokens** section can be used to define imaginary tokens, which are token
+types that do not have an associated lexical rule. Grammarinator will generate
+empty methods for these imaginary tokens. These empty methods serve as
+placeholders that can be expanded and customized in the subclasses.
+
+ANTLRv4 supports **named actions** in the global scope. Two named actions are
+supported: ``header`` and ``members``. For details on named actions see
+:doc:`actions`.
+
+
+Rules
+=====
+
+Next, the structure of rules is discussed. For the ANTLR documentation of
+rules, see `lexer rules`_ and `parser rules`_.
+
+There are two types of rules: lexer rules and parser rules. (Actually, ANTLR
+defines a specific lexer rule in addition, called fragment rule, which is
+treated the same as lexer rules in Grammarinator). Lexer rule names
+must start with capital letters, while parser rules start with lowercase
+letters.
+
+Both lexer and parser rules consist of zero or more alternatives, separated
+by the ``|`` symbol, like this: ``alt1 | alt2 | ...``.
+
+Alternatives (both in lexer and parser rules) are built from the following elements:
+
+  1) **Reference**: Referring to other lexer or parser rules. Lexer rules can
+     only reference lexer rules, while parser rules can reference both lexer
+     and parser rules.
+  2) **Literals**: Lexer rules and parser rules in combined grammars
+     can define implicit literals by enclosing them in single quotes
+     (e.g., ``'literal'``).
+  3) **Dot**: Representing an arbitrary single character. The behavior of the
+     dot can be customized using the ``dot`` option. See the ``dot`` key in
+     `options`_ for details.
+  4) **Parentheses**: Grouping parts of rules using parentheses to create
+     blocks (e.g., ``(rule1 | 'literal')``).
+  5) **Quantifiers**: Applying quantifiers to references, literals, and blocks
+     to specify repetition:
+
+      a) ``*`` (Kleene-star): The preceding item can be repeated zero or
+         more times.
+      b) ``+`` (Kleene-plus): The preceding item must be repeated one
+         or more times.
+      c) ``?`` (optional): The preceding item is optional, it may either
+         be omitted or it may appear once.
+
+  6) **Actions**: Inline code blocks in the target language used to define
+     operations that cannot be expressed with grammar rules alone.
+     For details see the chapter :doc:`actions`.
+  7) **Semantic predicates**: Inline code blocks in the target language used
+     to guide the selection of alternatives in ways that cannot be expressed
+     with grammar rules alone.
+     For details see the chapter :doc:`actions`.
+  8) **Variables**: Variables in grammar rules allow to save subtrees and use
+     them later within the same rule. Variables are denoted by a dollar sign
+     (``$``) prefix when referring to them.
+
+     The following example uses variables to match the opening and closing tag
+     name of HTML tags:
+
+    .. code-block:: antlr
+
+      htmlElement
+        : '<' open_tag=htmlTagName htmlAttribute* '>'
+          htmlContent
+          '</' htmlTagName {current.last_child.replace(deepcopy($open_tag))} '>'
+        | ...
+        ;
+
+
+Lexer Rule Specific Items
+-------------------------
+
+  1) **Character range**: Defines character range in the form of ``'x'..'y'``,
+     inclusively. Both ``x`` and ``y`` must be a single character or a unicode
+     code point in the form ``\uXXXX`` or ``\u{XXXXXX}``.
+  2) **Character set**: Defines a character set inside square brackets
+     ``[...]``. It may contain single characters or ranges separated with
+     ``-``. It supports the following special characters: ``\n``, ``\r``,
+     ``\b``, ``\t``, ``\f`` and ``\uXXXX`` or ``\u{XXXXXX}``. ``]`` and ``\``
+     must be escaped with ``\``, while ``-`` must be the first item if it is
+     part of the set.
+     Examples: ``[0-9a-fA-F]`` (hex digits) or ``[-a-zA-Z0-9.,;!?]``.
+  3) **Inverted set**: Defines a character set with inverting another one. It
+     is defined in the form ``~x`` where ``x`` can be a single character
+     literal, a character range or a character set.
+     Example: ``~[\r\n]`` means anything except line breaks.
+
+
+
+.. _`ANTLRv4 grammar`: https://github.com/antlr/antlr4/blob/master/doc/index.md
+.. _`lexer rules`: https://github.com/antlr/antlr4/blob/master/doc/lexer-rules.md
+.. _`parser rules`: https://github.com/antlr/antlr4/blob/master/doc/parser-rules.md
```

