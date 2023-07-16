# Comparing `tmp/ghastoolkit-0.5.0.tar.gz` & `tmp/ghastoolkit-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.5.0.tar", last modified: Sat Jul 15 17:25:12 2023, max compression
+gzip compressed data, was "ghastoolkit-0.5.1.tar", last modified: Sun Jul 16 19:23:06 2023, max compression
```

## Comparing `ghastoolkit-0.5.0.tar` & `ghastoolkit-0.5.1.tar`

### file list

```diff
@@ -1,61 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.614526 ghastoolkit-0.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.618526 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 17:25:12.000000 ghastoolkit-0.5.0/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 17:25:12.622526 ghastoolkit-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-15 17:24:41.000000 ghastoolkit-0.5.0/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.775337 ghastoolkit-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.779337 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-16 19:23:06.000000 ghastoolkit-0.5.1/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 19:23:06.783336 ghastoolkit-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-16 19:22:36.000000 ghastoolkit-0.5.1/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.5.0/LICENSE` & `ghastoolkit-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/PKG-INFO` & `ghastoolkit-0.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.5.0/README.md` & `ghastoolkit-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/pyproject.toml` & `ghastoolkit-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 [project]
 name = "ghastoolkit"
-version = "0.5.0"
-authors = [
-  { name="GeekMasher" },
-]
+version = "0.5.1"
+authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -19,18 +17,17 @@
 dependencies = [
     "certifi==2023.5.7",
     "charset-normalizer==3.2.0",
     "idna==3.4",
     "PyYAML==6.0",
     "ratelimit==2.2.1",
     "requests==2.31.0",
-    "urllib3==2.0.3"
+    "urllib3==2.0.3",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/GeekMasher/ghastoolkit"
 "Bug Tracker" = "https://github.com/GeekMasher/ghastoolkit/issues"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
-
```

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/__init__.py` & `ghastoolkit-0.5.1/src/ghastoolkit/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
@@ -37,11 +37,13 @@
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 from ghastoolkit.supplychain.dependencies import Dependency, Dependencies
 from ghastoolkit.supplychain.licensing import Licenses
 
 # CodeQL
 from ghastoolkit.codeql.databases import CodeQLDatabases, CodeQLDatabase
 from ghastoolkit.codeql.cli import CodeQL
+from ghastoolkit.codeql.packs.pack import CodeQLPack
+from ghastoolkit.codeql.packs.packs import CodeQLPacks
 from ghastoolkit.codeql.results import CodeQLResults, CodeLocation, CodeResult
 
 # CodeQL Data Extensions / Models as Data
 from ghastoolkit.codeql.dataextensions.ext import DataExtensions
```

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/__main__.py` & `ghastoolkit-0.5.1/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.5.1/src/ghastoolkit/codeql/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,111 @@
+"""This is the CodeQL CLI Module."""
+import os
 import json
 import logging
-import os
-import subprocess
-from sys import stdout
 import tempfile
-from typing import Optional, Union
+import subprocess
+from typing import List, Optional, Union
 
 from ghastoolkit.codeql.databases import CodeQLDatabase
 from ghastoolkit.codeql.results import CodeQLResults
-from ghastoolkit.codeql.utils import findCodeBinary
 
 
 logger = logging.getLogger("ghastoolkit.codeql.cli")
 
 
+def findCodeQLBinary() -> Optional[List[str]]:
+    """Find CodeQL Binary on current system."""
+    locations = [["codeql"], ["gh", "codeql"], ["/usr/bin/codeql/codeql"]]
+
+    for location in locations:
+        try:
+            cmd = location + ["version"]
+            with open(os.devnull, "w") as null:
+                subprocess.check_call(cmd, stdout=null, stderr=null)
+
+            return location
+        except Exception as err:
+            logger.debug(f"Failed to find codeql :: {err}")
+    return []
+
+
 class CodeQL:
-    """CodeQL CLI"""
+    """CodeQL CLI."""
 
     def __init__(self, binary: Optional[str] = None) -> None:
+        """Initialise CodeQL CLI Class."""
         if binary:
             self.path_binary = [binary]
         else:
-            self.path_binary: Optional[list[str]] = findCodeBinary()
+            self.path_binary: Optional[list[str]] = findCodeQLBinary()
 
     def exists(self) -> bool:
-        """
-        Check codeql is present on the system
-        """
+        """Check codeql is present on the system."""
         return self.path_binary != None
 
     def runCommand(self, *argvs, display: bool = False) -> Optional[str]:
-        """Run CodeQL command without the binary / path"""
+        """Run CodeQL command without the binary / path."""
+        logger.debug(f"Running CodeQL Command :: {argvs[0]}...")
         if not self.path_binary:
             raise Exception("CodeQL binary / path was not found")
         cmd = []
         cmd.extend(self.path_binary)
         cmd.extend(argvs)
 
         if argvs[0] == "database":
             cmd.extend(["--threads", "0", "--ram", "0"])
 
-        if not display:
-            with open(os.devnull, "w") as null:
-                result = subprocess.run(cmd, stdout=null, stderr=null)
+        if display:
+            subprocess.check_output(cmd)
         else:
-            result = subprocess.check_output(cmd)
-            return result.decode().strip()
+            result = subprocess.run(cmd, capture_output=True)
+            return result.stdout.decode().strip()
 
     @property
     def version(self) -> str:
-        """Get CodeQL Version"""
-        return self.runCommand("version", "--format", "terse", display=True)
+        """Get CodeQL Version from the CLI binary."""
+        version = self.runCommand("version", "--format", "terse", display=True)
+        if not version:
+            raise Exception("CodeQL version not found")
+        return version
 
     def runQuery(
         self, database: CodeQLDatabase, path: Optional[str] = None
     ) -> CodeQLResults:
-        """Runs Query on a CodeQL Database"""
+        """Run a CodeQL Query on a CodeQL Database."""
         if not database.path:
             raise Exception("CodeQL Database path is not set")
 
         path = path or database.default_pack
 
         self.runCommand("database", "run-queries", database.path, path)
         return self.getResults(database, path)
 
     def runRawQuery(
         self, path: str, database: CodeQLDatabase, outputtype: str = "bqrs"
     ) -> Union[dict, list]:
-        """Run raw query"""
+        """Run raw query on a CodeQL Database."""
         if not database.path:
             raise Exception("CodeQL Database path is not set")
         if not path.endswith(".ql"):
             raise Exception("runRawQuery requires a QL file")
 
         self.runCommand("database", "run-queries", database.path, path)
         if outputtype == "bqrs":
             bqrs = os.path.join(
                 database.path, "results", path.replace(":", "/").replace(".ql", ".bqrs")
             )
             return self.readBqrs(bqrs)
-        else:
-            return
+        return {}
 
     def getResults(
         self, database: CodeQLDatabase, path: Optional[str] = None
     ) -> CodeQLResults:
-        """Get interpret results from CodeQL"""
+        """Get the interpreted results from CodeQL."""
         sarif = os.path.join(tempfile.gettempdir(), "codeql-result.sarif")
         cmd = [
             "database",
             "interpret-results",
             "--format",
             "sarif-latest",
             "--output",
@@ -104,21 +120,22 @@
         with open(sarif, "r") as handle:
             data = json.load(handle)
 
         results = data.get("runs", [])[0].get("results", [])
         return CodeQLResults.loadSarifResults(results)
 
     def readBqrs(self, bqrsfile: str) -> dict:
-        """Read BQRS"""
+        """Read a BQRS file to get the raw results."""
         output = os.path.join(tempfile.gettempdir(), "codeql-result.bqrs")
 
         self.runCommand(
             "bqrs", "decode", "--format", "json", "--output", output, bqrsfile
         )
 
         with open(output, "r") as handle:
             return json.load(handle)
 
     def __str__(self) -> str:
+        """To String."""
         if self.path_binary:
             return f"CodeQL('{self.version}')"
         return "CodeQL()"
```

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.5.1/src/ghastoolkit/codeql/databases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import date, datetime
+from datetime import datetime
 import os
 import shutil
 import zipfile
 import tempfile
 from typing import *
 from dataclasses import dataclass
 
@@ -25,25 +25,32 @@
         os.environ.get("RUNNER_TEMP", "/home/runner/work/_temp"), "codeql_databases"
     ),
 ]
 
 
 @dataclass
 class CodeQLDatabase:
+    """CodeQL Database Abstraction to make our lives easier"""
+
     name: str
+    """Name"""
     language: str
+    """CodeQL Langauge"""
     repository: Optional[Repository] = None
-
-    # path to when the DB should be
+    """GitHub Repository (optional)"""
     path: Optional[str] = None
+    """Path to the CodeQL Database"""
     path_download: Optional[str] = None
+    """Path to download CodeQL DB if not path is set"""
 
     loc_baseline: int = 0
+    """Lines of Code baseline in DB"""
 
     created: Optional[datetime] = None
+    """Created datetime infomation"""
 
     def __post_init__(self):
         if self.path:
             if not os.path.exists(self.path):
                 raise Exception("Database folder incorrect")
             # TODO: check and load DB data
         else:
@@ -69,37 +76,41 @@
         """Check if the current database path is a real CodeQL DB"""
         if self.path and self.exists():
             codeql_db_file = os.path.join(self.path, "codeql-database.yml")
             return os.path.exists(codeql_db_file)
         return False
 
     def exists(self) -> bool:
+        """Checks if the CodeQL Database exists"""
         return False if not self.path else os.path.exists(self.path)
 
     @property
     def default_pack(self) -> str:
+        """Gets the default query pack for language"""
         return f"codeql/{self.language}-queries"
 
     def getSuite(self, name: str) -> str:
+        """Gets suite based on default pack"""
         return f"{self.default_pack}:codeql-suites/{self.language}-{name}.qls"
 
     def display_name(self, owner: Optional[str] = None) -> str:
-        """Display Name"""
+        """Get the display name"""
         if self.repository:
             own = self.repository.owner
             repo = self.repository.repo
 
             if own and own == owner:
                 return self.repository.repo.title().replace(" ", "")
 
             return f"{own.title()}{repo.title()}".replace(" ", "")
         new_name = self.name.replace("-", " ")
         return new_name.title().replace(" ", "")
 
     def createPath(self) -> Optional[str]:
+        """Create a path for CodeQL Database"""
         for root in __CODEQL_DATABASE_PATHS__:
             if not os.path.exists(root):
                 continue
 
             return os.path.join(root, self.database_folder)
         return
 
@@ -111,41 +122,47 @@
             return os.path.join(
                 root, self.language, self.repository.owner, self.repository.repo
             )
         return os.path.join(root, self.language, self.name)
 
     @property
     def database_folder(self) -> str:
+        """Get CodeQL Database folder"""
         if self.repository:
             result = f"{self.language}-{self.repository.owner}-{self.repository.repo}"
             if self.repository.sha:
                 result += f"-{self.repository.sha}"
         else:
             result = f"{self.name}"
 
         return result
 
     @staticmethod
     def loadFromYml(path: str) -> "CodeQLDatabase":
-        """Load from YAML / YML file"""
+        """Load from YAML / YML file
+
+        **Example:**
+        >>> db = CodeQLDatabase.loadFromYml("codeql-db")
+
+        """
         if not os.path.exists(path):
             raise Exception("CodeQL Database YML does not exist")
         if not path.endswith(".yml"):
             raise Exception("File is not a YML file")
         dirname = os.path.dirname(path)
         name = os.path.basename(dirname)
         db = CodeQLDatabase(name, "python", path=dirname)
         db.loadDatabaseYml(path)
         if db.language == "":
             logger.error(f"CodeQLDatabase Language not set from YML")
             raise Exception(f"Unable to load DB correctly")
         return db
 
     def loadDatabaseYml(self, path: str):
-        """Load content from YML"""
+        """Load content from YML file"""
         if not os.path.exists(path):
             raise Exception("CodeQL Database YML does not exist")
         if not path.endswith(".yml"):
             raise Exception("File is not a YML file")
 
         with open(path, "r") as handle:
             data = safe_load(handle)
@@ -159,15 +176,15 @@
         if isinstance(creation_time, datetime):
             self.created = creation_time
         else:
             creation_time, _ = creation_time.split(".", 1)
             self.created = datetime.fromisoformat(creation_time)
 
     def downloadDatabase(self, output: Optional[str], use_cache: bool = True) -> str:
-        """Download CodeQL database"""
+        """Download CodeQL Database"""
         output = output or self.path or self.path_download
         if not output:
             raise Exception(f"CodeQL Database path not set")
 
         if not self.language or not self.repository:
             raise Exception(
                 f"Database download requires a repository and language to be set"
```

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.5.1/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.5.1/src/ghastoolkit/codeql/results.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,54 @@
+"""CodeQL Results."""
 from dataclasses import dataclass, field
 from typing import Optional
 
 
 @dataclass
 class CodeLocation:
-    """Code Location Module"""
+    """Code Location Module."""
 
     uri: str
     """URI to the location where the result occurs"""
 
     start_line: int
     """Start line of the result"""
     start_column: Optional[int] = None
     """Start column of the result"""
     end_line: Optional[int] = None
     """End line of the result"""
     end_column: Optional[int] = None
     """End line of the result"""
 
     def __str__(self) -> str:
+        """To String."""
         return f"{self.uri}#{self.start_line}"
 
 
 @dataclass
 class CodeResult:
-    """Code Result"""
+    """Code Result."""
 
     rule_id: str
     """Rule ID"""
     message: str
     """Message of the result"""
 
     locations: list[CodeLocation] = field(default_factory=list)
     """Locations of the results"""
 
     def __str__(self) -> str:
+        """To String."""
         if len(self.locations) == 1:
             return f"CodeResult('{self.rule_id}', '{self.locations[0]}')"
         return f"CodeResult('{self.rule_id}', {len(self.locations)})"
 
     @staticmethod
     def loadSarifLocations(data: list[dict]) -> list["CodeLocation"]:
-        """Load SARIF Locations"""
+        """Load SARIF Locations."""
         locations = []
         for loc in data:
             physical = loc.get("physicalLocation", {})
             region = physical.get("region", {})
             locations.append(
                 CodeLocation(
                     physical.get("artifactLocation", {}).get("uri", ""),
@@ -55,19 +58,19 @@
                     end_column=region.get("endColumn"),
                 )
             )
         return locations
 
 
 class CodeQLResults(list):
-    """CodeQL Results"""
+    """CodeQL Results."""
 
     @staticmethod
     def loadSarifResults(results: list[dict]) -> "CodeQLResults":
-        """Load SARIF Results"""
+        """Load SARIF Results."""
         result = CodeQLResults()
 
         for alert in results:
             result.append(
                 CodeResult(
                     alert.get("ruleId", "NA"),
                     alert.get("message", {}).get("text", "NA"),
```

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.5.1/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.5.1/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.5.1/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.5.1/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.5.1/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.5.1/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.5.1/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.5.1/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.5.1/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.5.1/src/ghastoolkit/supplychain/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.5.1/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.5.1/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.5.1/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.5.1/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.5.0
+Version: 0.5.1
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.5.0/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.5.1/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,19 +9,22 @@
 src/ghastoolkit.egg-info/requires.txt
 src/ghastoolkit.egg-info/top_level.txt
 src/ghastoolkit/codeql/__init__.py
 src/ghastoolkit/codeql/cli.py
 src/ghastoolkit/codeql/consts.py
 src/ghastoolkit/codeql/databases.py
 src/ghastoolkit/codeql/results.py
-src/ghastoolkit/codeql/utils.py
 src/ghastoolkit/codeql/dataextensions/__init__.py
 src/ghastoolkit/codeql/dataextensions/__main__.py
 src/ghastoolkit/codeql/dataextensions/ext.py
 src/ghastoolkit/codeql/dataextensions/models.py
+src/ghastoolkit/codeql/packs/__init__.py
+src/ghastoolkit/codeql/packs/__main__.py
+src/ghastoolkit/codeql/packs/pack.py
+src/ghastoolkit/codeql/packs/packs.py
 src/ghastoolkit/octokit/__init__.py
 src/ghastoolkit/octokit/clearlydefined.py
 src/ghastoolkit/octokit/codescanning.py
 src/ghastoolkit/octokit/dependabot.py
 src/ghastoolkit/octokit/dependencygraph.py
 src/ghastoolkit/octokit/github.py
 src/ghastoolkit/octokit/octokit.py
```

### Comparing `ghastoolkit-0.5.0/tests/test_advisories.py` & `ghastoolkit-0.5.1/tests/test_advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_codeql_dataext.py` & `ghastoolkit-0.5.1/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_codeqldb.py` & `ghastoolkit-0.5.1/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_codescanning.py` & `ghastoolkit-0.5.1/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_default.py` & `ghastoolkit-0.5.1/tests/test_default.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 
     def test_codeql(self):
         codeql = CodeQL("codeql")
         alerts = CodeQLResults()
 
         dataext = DataExtensions("python")
 
+        pack = CodeQLPack()
+        packs = CodeQLPacks()
+
     def test_secretscanning(self):
         ss = SecretScanning()
         alert = SecretAlert(
             0, "open", "", "geekmasher_token", "GeekMasher Token", "ABCD"
         )
 
     def test_licenses(self):
```

### Comparing `ghastoolkit-0.5.0/tests/test_dependencies.py` & `ghastoolkit-0.5.1/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_depgraph.py` & `ghastoolkit-0.5.1/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_github.py` & `ghastoolkit-0.5.1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_licenses.py` & `ghastoolkit-0.5.1/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_octokit.py` & `ghastoolkit-0.5.1/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.0/tests/test_secretscanning.py` & `ghastoolkit-0.5.1/tests/test_secretscanning.py`

 * *Files identical despite different names*

