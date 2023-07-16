# Comparing `tmp/LangChainAgentFactory-0.2.tar.gz` & `tmp/LangChainAgentFactory-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LangChainAgentFactory-0.2.tar", last modified: Thu Jul 13 04:49:02 2023, max compression
+gzip compressed data, was "LangChainAgentFactory-0.3.tar", last modified: Sun Jul 16 05:17:54 2023, max compression
```

## Comparing `LangChainAgentFactory-0.2.tar` & `LangChainAgentFactory-0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 04:49:02.946334 LangChainAgentFactory-0.2/
--rw-rw-rw-   0        0        0     3668 2023-07-13 04:21:53.000000 LangChainAgentFactory-0.2/.gitignore
--rw-rw-rw-   0        0        0     1086 2023-07-13 03:47:49.000000 LangChainAgentFactory-0.2/LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 04:49:02.929333 LangChainAgentFactory-0.2/LangChainAgentFactory/
--rw-rw-rw-   0        0        0     6455 2023-07-13 04:32:19.000000 LangChainAgentFactory-0.2/LangChainAgentFactory/AgentFactory.py
--rw-rw-rw-   0        0        0        0 2023-07-13 03:21:41.000000 LangChainAgentFactory-0.2/LangChainAgentFactory/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-13 04:49:02.940337 LangChainAgentFactory-0.2/LangChainAgentFactory.egg-info/
--rw-rw-rw-   0        0        0     2205 2023-07-13 04:49:02.000000 LangChainAgentFactory-0.2/LangChainAgentFactory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2023-07-13 04:49:02.000000 LangChainAgentFactory-0.2/LangChainAgentFactory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 04:49:02.000000 LangChainAgentFactory-0.2/LangChainAgentFactory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 04:49:02.000000 LangChainAgentFactory-0.2/LangChainAgentFactory.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-13 04:49:02.000000 LangChainAgentFactory-0.2/LangChainAgentFactory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2205 2023-07-13 04:49:02.942334 LangChainAgentFactory-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1675 2023-07-13 04:20:32.000000 LangChainAgentFactory-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 04:49:02.946334 LangChainAgentFactory-0.2/setup.cfg
--rw-rw-rw-   0        0        0      751 2023-07-13 04:46:13.000000 LangChainAgentFactory-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 05:17:54.203860 LangChainAgentFactory-0.3/
+-rw-rw-rw-   0        0        0     3668 2023-07-13 04:21:53.000000 LangChainAgentFactory-0.3/.gitignore
+-rw-rw-rw-   0        0        0     1086 2023-07-13 03:47:49.000000 LangChainAgentFactory-0.3/LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 05:17:54.192778 LangChainAgentFactory-0.3/LangChainAgentFactory/
+-rw-rw-rw-   0        0        0     5370 2023-07-16 04:44:41.000000 LangChainAgentFactory-0.3/LangChainAgentFactory/AgentFactory.py
+-rw-rw-rw-   0        0        0        0 2023-07-13 03:21:41.000000 LangChainAgentFactory-0.3/LangChainAgentFactory/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-16 05:17:54.201860 LangChainAgentFactory-0.3/LangChainAgentFactory.egg-info/
+-rw-rw-rw-   0        0        0     5873 2023-07-16 05:17:54.000000 LangChainAgentFactory-0.3/LangChainAgentFactory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2023-07-16 05:17:54.000000 LangChainAgentFactory-0.3/LangChainAgentFactory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 05:17:54.000000 LangChainAgentFactory-0.3/LangChainAgentFactory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-16 05:17:54.000000 LangChainAgentFactory-0.3/LangChainAgentFactory.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-07-16 05:17:54.000000 LangChainAgentFactory-0.3/LangChainAgentFactory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5873 2023-07-16 05:17:54.203860 LangChainAgentFactory-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5309 2023-07-16 03:54:26.000000 LangChainAgentFactory-0.3/README.md
+-rw-rw-rw-   0        0        0      664 2023-07-16 04:40:31.000000 LangChainAgentFactory-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      156 2023-07-16 05:17:54.206369 LangChainAgentFactory-0.3/setup.cfg
```

### Comparing `LangChainAgentFactory-0.2/.gitignore` & `LangChainAgentFactory-0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `LangChainAgentFactory-0.2/LICENSE.txt` & `LangChainAgentFactory-0.3/LICENSE.txt`

 * *Files identical despite different names*

