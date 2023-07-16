# Comparing `tmp/nographs-3.2.0.tar.gz` & `tmp/nographs-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nographs-3.2.0.tar", last modified: Tue Jun  6 07:00:21 2023, max compression
+gzip compressed data, was "nographs-3.3.0.tar", last modified: Sun Jul 16 12:18:14 2023, max compression
```

## Comparing `nographs-3.2.0.tar` & `nographs-3.3.0.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.798009 nographs-3.2.0/
--rw-rw-rw-   0        0        0     9657 2023-06-06 07:00:21.797011 nographs-3.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     8142 2023-06-06 06:52:14.000000 nographs-3.2.0/README.rst
--rw-rw-rw-   0        0        0      162 2022-11-27 13:28:03.000000 nographs-3.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 07:00:21.798009 nographs-3.2.0/setup.cfg
--rw-rw-rw-   0        0        0     2100 2023-06-06 06:52:14.000000 nographs-3.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.646988 nographs-3.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.718495 nographs-3.2.0/src/nographs/
--rw-rw-rw-   0        0        0     7660 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/__init__.py
--rw-rw-rw-   0        0        0    41869 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/_bidir_search.py
--rw-rw-rw-   0        0        0      953 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/_compatibility.py
--rw-rw-rw-   0        0        0     8188 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_edge_gadgets.py
--rw-rw-rw-   0        0        0    42642 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_gear_collections.py
--rw-rw-rw-   0        0        0    35184 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_gears.py
--rw-rw-rw-   0        0        0    13918 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_matrix_gadgets.py
--rw-rw-rw-   0        0        0     9679 2023-05-09 07:48:46.000000 nographs-3.2.0/src/nographs/_path.py
--rw-rw-rw-   0        0        0    19478 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_paths.py
--rw-rw-rw-   0        0        0    16057 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/_strategies.py
--rw-rw-rw-   0        0        0   148710 2023-06-06 06:52:14.000000 nographs-3.2.0/src/nographs/_traversals.py
--rw-rw-rw-   0        0        0     3232 2023-05-09 06:38:46.000000 nographs-3.2.0/src/nographs/_types.py
--rw-rw-rw-   0        0        0        0 2022-11-27 13:28:03.000000 nographs-3.2.0/src/nographs/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.724497 nographs-3.2.0/src/nographs.egg-info/
--rw-rw-rw-   0        0        0     9657 2023-06-06 07:00:21.000000 nographs-3.2.0/src/nographs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      834 2023-06-06 07:00:21.000000 nographs-3.2.0/src/nographs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 07:00:21.000000 nographs-3.2.0/src/nographs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-06 07:00:21.000000 nographs-3.2.0/src/nographs.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-06 07:00:21.796010 nographs-3.2.0/tests/
--rw-rw-rw-   0        0        0     5033 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_docs_examples.py
--rw-rw-rw-   0        0        0     5963 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_edge_gadgets.py
--rw-rw-rw-   0        0        0    11625 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_gear_collections.py
--rw-rw-rw-   0        0        0     2065 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_gears.py
--rw-rw-rw-   0        0        0     1923 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_matrix_gadgets.py
--rw-rw-rw-   0        0        0     2171 2023-06-06 06:52:14.000000 nographs-3.2.0/tests/test_nographs.py
--rw-rw-rw-   0        0        0      510 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_path.py
--rw-rw-rw-   0        0        0     5828 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_paths.py
--rw-rw-rw-   0        0        0     2783 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_strategies.py
--rw-rw-rw-   0        0        0   157579 2023-06-06 06:52:14.000000 nographs-3.2.0/tests/test_traversals_and_searches.py
--rw-rw-rw-   0        0        0     1419 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_types.py
--rw-rw-rw-   0        0        0     3389 2023-05-09 06:38:46.000000 nographs-3.2.0/tests/test_unit_typed.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:18:14.890804 nographs-3.3.0/
+-rw-rw-rw-   0        0        0    10387 2023-07-16 12:18:14.889804 nographs-3.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8859 2023-07-16 12:04:29.000000 nographs-3.3.0/README.rst
+-rw-rw-rw-   0        0        0      162 2022-11-27 13:28:03.000000 nographs-3.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-16 12:18:14.891804 nographs-3.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2113 2023-07-16 12:04:29.000000 nographs-3.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 12:18:14.839803 nographs-3.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-16 12:18:14.865804 nographs-3.3.0/src/nographs/
+-rw-rw-rw-   0        0        0     8274 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/__init__.py
+-rw-rw-rw-   0        0        0    42304 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/_bidir_search.py
+-rw-rw-rw-   0        0        0      953 2023-06-19 19:35:12.000000 nographs-3.3.0/src/nographs/_compatibility.py
+-rw-rw-rw-   0        0        0     8345 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/_extra_edge_gadgets.py
+-rw-rw-rw-   0        0        0    12705 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/_extra_infinite_branching.py
+-rw-rw-rw-   0        0        0    14037 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/_extra_matrix_gadgets.py
+-rw-rw-rw-   0        0        0    21189 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/_extra_tsp.py
+-rw-rw-rw-   0        0        0    42642 2023-05-09 06:38:46.000000 nographs-3.3.0/src/nographs/_gear_collections.py
+-rw-rw-rw-   0        0        0    35093 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/_gears.py
+-rw-rw-rw-   0        0        0     9679 2023-05-09 07:48:46.000000 nographs-3.3.0/src/nographs/_path.py
+-rw-rw-rw-   0        0        0    19478 2023-06-20 06:57:15.000000 nographs-3.3.0/src/nographs/_paths.py
+-rw-rw-rw-   0        0        0    16057 2023-06-06 06:52:14.000000 nographs-3.3.0/src/nographs/_strategies.py
+-rw-rw-rw-   0        0        0   150641 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/_traversals.py
+-rw-rw-rw-   0        0        0     3618 2023-07-16 12:04:29.000000 nographs-3.3.0/src/nographs/_types.py
+-rw-rw-rw-   0        0        0        0 2022-11-27 13:28:03.000000 nographs-3.3.0/src/nographs/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-16 12:18:14.871803 nographs-3.3.0/src/nographs.egg-info/
+-rw-rw-rw-   0        0        0    10387 2023-07-16 12:18:14.000000 nographs-3.3.0/src/nographs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2023-07-16 12:18:14.000000 nographs-3.3.0/src/nographs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 12:18:14.000000 nographs-3.3.0/src/nographs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 12:18:14.000000 nographs-3.3.0/src/nographs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-16 12:18:14.888804 nographs-3.3.0/tests/
+-rw-rw-rw-   0        0        0     5033 2023-05-09 06:38:46.000000 nographs-3.3.0/tests/test_docs_examples.py
+-rw-rw-rw-   0        0        0     5963 2023-07-16 12:04:29.000000 nographs-3.3.0/tests/test_extra_edge_gadgets.py
+-rw-rw-rw-   0        0        0     1011 2023-07-16 12:04:29.000000 nographs-3.3.0/tests/test_extra_infinite_branching.py
+-rw-rw-rw-   0        0        0     1923 2023-07-16 12:04:29.000000 nographs-3.3.0/tests/test_extra_matrix_gadgets.py
+-rw-rw-rw-   0        0        0    13522 2023-07-16 12:04:29.000000 nographs-3.3.0/tests/test_extra_tsp.py
+-rw-rw-rw-   0        0        0    11625 2023-05-09 06:38:46.000000 nographs-3.3.0/tests/test_gear_collections.py
+-rw-rw-rw-   0        0        0     2065 2023-05-09 06:38:46.000000 nographs-3.3.0/tests/test_gears.py
+-rw-rw-rw-   0        0        0     1599 2023-07-16 12:04:29.000000 nographs-3.3.0/tests/test_nographs.py
+-rw-rw-rw-   0        0        0      510 2023-05-09 06:38:46.000000 nographs-3.3.0/tests/test_path.py
+-rw-rw-rw-   0        0        0     5828 2023-05-09 06:38:46.000000 nographs-3.3.0/tests/test_paths.py
+-rw-rw-rw-   0        0        0     2783 2023-05-09 06:38:46.000000 nographs-3.3.0/tests/test_strategies.py
+-rw-rw-rw-   0        0        0   163656 2023-07-16 12:04:29.000000 nographs-3.3.0/tests/test_traversals_and_searches.py
+-rw-rw-rw-   0        0        0     1419 2023-05-09 06:38:46.000000 nographs-3.3.0/tests/test_types.py
+-rw-rw-rw-   0        0        0     3886 2023-07-16 12:04:29.000000 nographs-3.3.0/tests/test_unit_typed.py
```

### Comparing `nographs-3.2.0/PKG-INFO` & `nographs-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nographs
-Version: 3.2.0
+Version: 3.3.0
 Summary: Graph analysis – the lazy (evaluation) way: Analysis on the fly, for graphs, that are computed and/or adapted on the fly.
 Home-page: https://github.com/HeWeMel/nographs
 Author: Dr. Helmut Melcher
 Author-email: HeWeMel@web.de
 Project-URL: Documentation, https://nographs.readthedocs.io/
 Project-URL: Source, https://github.com/hewemel/nographs/
 Project-URL: Bug Reports, https://github.com/hewemel/nographs/issues
-Keywords: graph,network,search,traverse,analysis,infinite,lazy,shortest,distance,depth,DFS,breadth,BFS,Dijkstra,topological,MST
+Keywords: graph,network,search,traverse,analysis,infinite,lazy,shortest,distance,depth,DFS,breadth,BFS,Dijkstra,topological,spanning,MST,TSP
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -74,14 +74,22 @@
 **computed and/or adapted in application code on the fly**
 (when needed and as far as needed). Also,
 **the analysis and the reporting of results by the library happen on the fly**
 (when, and as far as, results can already be derived).
 
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
+**Documentation**
+
+- `Homepage of the documentation <https://nographs.readthedocs.io>`__
+- `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
+- `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
+  (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
+- `API reference <https://nographs.readthedocs.io/en/latest/api.html>`__
+
 **Feature overview**
 
 - Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
 - Bidirectional search algorithms: BFS and Dijkstra.
 - Results: Reachability, depth, distance, paths and trees.
   Paths can be
@@ -89,15 +97,15 @@
   and can be iterated in both directions.
 - Flexible graph notion:
 
   - Infinite directed multigraphs with loops and
     attributes (this includes
     multiple adjacency, cycles, self-loops,
     directed edges,
-    weighted edges and edges with application specific attributes).
+    weighted edges and attributed edges).
   - Infinite graphs are supported, but need to be
     locally finite (i.e., a vertex has only finitely many outgoing edges).
 
 - Generic API:
 
   - Vertices: Can be anything except for None. Hashable vertices can be
     used directly, unhashable vertices can be used together with
@@ -116,33 +124,38 @@
     efficiently
 
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
   allows for an API that eases
   operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
-  computation of search-aware graphs, and
-  traversals of vertex equivalence classes on the fly.
+  computation of search-aware graphs,  the combination of
+  problem reduction with lazy evaluation,
+  and traversals of vertex equivalence classes on the fly.
   Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
 - CI tests: For all supported versions of Python and both supported interpreters
   CPython and PyPy, both code and docs, 100% code coverage.
 - Runtime and memory performance: Have been goals (CPython). In its domain, it often
-  even outperforms Rust- and C-based libraries.
-  If you need an even higher performance, using PyPy could be an option.
+  even outperforms Rust- and C-based libraries. Using PyPy improves its performance
+  further.
 
-**Documentation**
+**Extras** (outside of the core of NoGraphs)
 
-- `Homepage of the documentation <https://nographs.readthedocs.io>`__
-- `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
-- `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
-  (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
-- `API reference <https://nographs.readthedocs.io/en/latest/api.html>`__
+- Computation of exact solutions for (small)
+  traveling salesman problems (shortest / longest route,
+  positive / zero / negative edge weights, graph does not need to be complete)
+- Dijkstra shortest paths algorithm for
+  infinitely branching graphs with locally sorted edges.
+- Gadget functions for test purposes. They make the easy task of
+  adapting existing explicit test graphs a no brainer, may they be
+  stored in edge indices or edge iterables
+  or in arrays.
 
 **Example**
 
 Our graph is directed, weighted and has infinitely many edges. These edges are
 defined in application code by the following function. For a vertex *i*
 (here: an integer) as the first of two
 parameters, it yields the edges that start at *i* as tuples
@@ -209,14 +222,17 @@
 
 - An infinite generator of primes, defined by just a graph and
   a call to a standard graph algorithm?
 - Or a graph that defines an infinite set
   of Towers of Hanoi problems in a generic way, without fixing the number of
   towers, disk sizes, and the start and goal configuration - and a specific
   problem instance is solved by just one library call?
+- Or a way for computing an exact solution for traveling salesman problems,
+  that is based on just a graph and a call of the Dijkstra single source shortest path
+  algorithm?
 - Or graphs that are dynamically
   computed based on other graphs, or on analysis results about other graphs,
-  or even on partial analysis results from already processed parts of the same graph?
+  or even on partial analysis results for already processed parts of the same graph?
 
 Let's `build it <https://nographs.readthedocs.io/en/latest/installation.html>`__.
 
 Welcome to NoGraphs!
```

### Comparing `nographs-3.2.0/README.rst` & `nographs-3.3.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,22 @@
 **computed and/or adapted in application code on the fly**
 (when needed and as far as needed). Also,
 **the analysis and the reporting of results by the library happen on the fly**
 (when, and as far as, results can already be derived).
 
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
+**Documentation**
+
+- `Homepage of the documentation <https://nographs.readthedocs.io>`__
+- `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
+- `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
+  (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
+- `API reference <https://nographs.readthedocs.io/en/latest/api.html>`__
+
 **Feature overview**
 
 - Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
 - Bidirectional search algorithms: BFS and Dijkstra.
 - Results: Reachability, depth, distance, paths and trees.
   Paths can be
@@ -60,15 +68,15 @@
   and can be iterated in both directions.
 - Flexible graph notion:
 
   - Infinite directed multigraphs with loops and
     attributes (this includes
     multiple adjacency, cycles, self-loops,
     directed edges,
-    weighted edges and edges with application specific attributes).
+    weighted edges and attributed edges).
   - Infinite graphs are supported, but need to be
     locally finite (i.e., a vertex has only finitely many outgoing edges).
 
 - Generic API:
 
   - Vertices: Can be anything except for None. Hashable vertices can be
     used directly, unhashable vertices can be used together with
@@ -87,33 +95,38 @@
     efficiently
 
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
   allows for an API that eases
   operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
-  computation of search-aware graphs, and
-  traversals of vertex equivalence classes on the fly.
+  computation of search-aware graphs,  the combination of
+  problem reduction with lazy evaluation,
+  and traversals of vertex equivalence classes on the fly.
   Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
 - CI tests: For all supported versions of Python and both supported interpreters
   CPython and PyPy, both code and docs, 100% code coverage.
 - Runtime and memory performance: Have been goals (CPython). In its domain, it often
-  even outperforms Rust- and C-based libraries.
-  If you need an even higher performance, using PyPy could be an option.
+  even outperforms Rust- and C-based libraries. Using PyPy improves its performance
+  further.
 
-**Documentation**
+**Extras** (outside of the core of NoGraphs)
 
-- `Homepage of the documentation <https://nographs.readthedocs.io>`__
-- `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
-- `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
-  (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
-- `API reference <https://nographs.readthedocs.io/en/latest/api.html>`__
+- Computation of exact solutions for (small)
+  traveling salesman problems (shortest / longest route,
+  positive / zero / negative edge weights, graph does not need to be complete)
+- Dijkstra shortest paths algorithm for
+  infinitely branching graphs with locally sorted edges.
+- Gadget functions for test purposes. They make the easy task of
+  adapting existing explicit test graphs a no brainer, may they be
+  stored in edge indices or edge iterables
+  or in arrays.
 
 **Example**
 
 Our graph is directed, weighted and has infinitely many edges. These edges are
 defined in application code by the following function. For a vertex *i*
 (here: an integer) as the first of two
 parameters, it yields the edges that start at *i* as tuples
@@ -180,14 +193,17 @@
 
 - An infinite generator of primes, defined by just a graph and
   a call to a standard graph algorithm?
 - Or a graph that defines an infinite set
   of Towers of Hanoi problems in a generic way, without fixing the number of
   towers, disk sizes, and the start and goal configuration - and a specific
   problem instance is solved by just one library call?
+- Or a way for computing an exact solution for traveling salesman problems,
+  that is based on just a graph and a call of the Dijkstra single source shortest path
+  algorithm?
 - Or graphs that are dynamically
   computed based on other graphs, or on analysis results about other graphs,
-  or even on partial analysis results from already processed parts of the same graph?
+  or even on partial analysis results for already processed parts of the same graph?
 
 Let's `build it <https://nographs.readthedocs.io/en/latest/installation.html>`__.
 
 Welcome to NoGraphs!
```

### Comparing `nographs-3.2.0/setup.py` & `nographs-3.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / 'README.rst').read_text(encoding='utf-8')
 
 setup(
     name="nographs",
-    version="3.2.0",
+    version="3.3.0",
     description=("Graph analysis – the lazy (evaluation) way: Analysis on the fly, "
                  + "for graphs, that are computed and/or adapted on the fly."),
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/HeWeMel/nographs",
     author="Dr. Helmut Melcher",
     author_email='HeWeMel@web.de',
@@ -33,15 +33,15 @@
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Typing :: Typed",
     ],
     keywords=('graph,network,search,traverse,analysis,infinite,lazy,shortest,distance,'
-              + 'depth,DFS,breadth,BFS,Dijkstra,topological,MST'),
+              + 'depth,DFS,breadth,BFS,Dijkstra,topological,spanning,MST,TSP'),
     python_requires='>=3.9, <4',
     project_urls={
         'Documentation': 'https://nographs.readthedocs.io/',
         'Source': 'https://github.com/hewemel/nographs/',
         'Bug Reports': 'https://github.com/hewemel/nographs/issues',
         # 'Say Thanks!': 'http://saythanks.io/to/HeWeMel',
     },
```

### Comparing `nographs-3.2.0/src/nographs/__init__.py` & `nographs-3.3.0/src/nographs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,27 +12,29 @@
     # vertex_as_id is the only exception, it is defined here because
     # it is used as a singleton, and is the only predefined instance of VertexToID.
     T,
     Weight,
     T_vertex,
     T_vertex_id,
     T_weight,
+    # T_weight_zero_inf_or,
     T_labels,
     VertexToID,
     vertex_as_id,
     UnweightedLabeledOutEdge,
     WeightedUnlabeledOutEdge,
     WeightedLabeledOutEdge,
     WeightedOutEdge,
     LabeledOutEdge,
     OutEdge,
     UnweightedUnlabeledFullEdge,
     UnweightedLabeledFullEdge,
     WeightedFullEdge,
     WeightedOrLabeledFullEdge,
+    AnyFullEdge,
 )
 from ._gear_collections import (
     # --- Gear collection types ---
     VertexSet,
     VertexMapping,
     # --- Gear collections for dense integer keys ---
     # -- Protocols for the used kind of sequences and the wrappers
@@ -138,45 +140,56 @@
 from ._path import Path
 from ._bidir_search import (
     BSearchBreadthFirstFlex,
     BSearchBreadthFirst,
     BSearchShortestPathFlex,
     BSearchShortestPath,
 )
-from ._matrix_gadgets import (
+from ._extra_edge_gadgets import (
+    adapt_edge_index,
+    adapt_edge_iterable,
+)
+from ._extra_infinite_branching import (
+    TraversalShortestPathsInfBranchingSortedFlex,
+    TraversalShortestPathsInfBranchingSorted,
+)
+from ._extra_matrix_gadgets import (
     Vector,
     Limits,
     Position,
     Array,
 )
-from ._edge_gadgets import (
-    adapt_edge_index,
-    adapt_edge_iterable,
+from ._extra_tsp import (
+    GettableProto,
+    traveling_salesman_flex,
+    traveling_salesman,
 )
 
 __all__ = (
     # -- types --
     "T",
     "Weight",
     "T_vertex",
     "T_vertex_id",
     "T_weight",
+    # "T_weight_zero_inf_or",
     "T_labels",
     "VertexToID",
     "vertex_as_id",
     "UnweightedLabeledOutEdge",
     "WeightedUnlabeledOutEdge",
     "WeightedLabeledOutEdge",
     "WeightedOutEdge",
     "LabeledOutEdge",
     "OutEdge",
     "UnweightedUnlabeledFullEdge",
     "UnweightedLabeledFullEdge",
     "WeightedFullEdge",
     "WeightedOrLabeledFullEdge",
+    "AnyFullEdge",
     # -- gear collections --
     "VertexSet",
     "VertexMapping",
     "GettableSettableForGearProto",
     "SequenceForGearProto",
     "VertexSequenceWrapperForSetProto",
     "VertexSequenceWrapperForMappingProto",
@@ -239,16 +252,23 @@
     "TraversalMinimumSpanningTreeFlex",
     "TraversalMinimumSpanningTree",
     # -- bidir search --
     "BSearchBreadthFirstFlex",
     "BSearchBreadthFirst",
     "BSearchShortestPathFlex",
     "BSearchShortestPath",
-    # -- matrix gadgets --
+    # -- extra_edge_gadgets --
+    "adapt_edge_index",
+    "adapt_edge_iterable",
+    # -- extra_infinite_branching --
+    "TraversalShortestPathsInfBranchingSortedFlex",
+    "TraversalShortestPathsInfBranchingSorted",
+    # -- extra_matrix_gadgets --
     "Vector",
     "Limits",
     "Position",
     "Array",
-    # -- edge gadgets --
-    "adapt_edge_index",
-    "adapt_edge_iterable",
+    # -- extra_tsp --
+    "GettableProto",
+    "traveling_salesman_flex",
+    "traveling_salesman",
 )
```

### Comparing `nographs-3.2.0/src/nographs/_bidir_search.py` & `nographs-3.3.0/src/nographs/_bidir_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,14 +451,19 @@
     is a short form for
 
     .. code-block:: python
 
        BSearchBreadthFirstFlex[
            T_vertex, T_vertex, T_labels],
       ](nog.vertex_as_id, nog.GearDefault(), *args, **keywords)
+
+    Implication:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_vertices: Optional[
             BNextVertices[
                 T_vertex, TraversalBreadthFirstFlex[T_vertex, T_vertex, T_labels]
@@ -984,14 +989,20 @@
     is a short form for
 
     .. code-block:: python
 
        BSearchShortestPathFlex[
            T_vertex, T_vertex, Union[T_weight, float], T_labels],
       ](nog.vertex_as_id, nog.GearDefault(), *args, **keywords)
+
+    Implication:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - The used weights are defined by Union[T_weight, float], see `GearDefault`
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_edges: Optional[
             BNextWeightedEdges[
                 T_vertex,
```

### Comparing `nographs-3.2.0/src/nographs/_compatibility.py` & `nographs-3.3.0/src/nographs/_compatibility.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/src/nographs/_edge_gadgets.py` & `nographs-3.3.0/src/nographs/_extra_edge_gadgets.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     ...
 
 
 def adapt_edge_index(
     index: Union[Mapping, Sequence], *, add_inverted: bool, attributes: bool
 ) -> Callable:
     """
-    Read a test graph from a Mapping (e.g. a Dict) or from a Sequence (e.g. a tuple
+    Read a graph from a Mapping (e.g. a Dict) or from a Sequence (e.g. a tuple
     or list, if integers are used as the vertices) and provide a neighbor function
     (`NextVertices` or `NextEdges`) from that data. Typically only used for test
     purposes.
 
     :param index: Mapping or Sequence with vertices as key, resp. as index. For each
         vertex, you provide:
 
@@ -175,19 +175,22 @@
     """
     Read a graph from an Iterable of edges and provide a neighbor function
     (`NextVertices` or `NextEdges`) from that data. Typically only used for test
     purposes.
 
     :param edges: The edges of your graph, each as Sequence (start_vertex, end_vertex,
         optional_attributes...), where edge data can be either a weight, or labels,
-        or both (see `WeightedOrLabeledFullEdge`).
+        or both (see `WeightedOrLabeledFullEdge`) or none
+        (see `AnyFullEdge`).
 
     :param attributes: If set to True, the resulting neighbor function will yield
         edges with edge attributes for a given vertex and
-        can be used as `NextEdges` function.
+        can be used as `NextEdges` function, but the edges of the given graph
+        need to have attributes (`WeightedOrLabeledFullEdge`, not
+        `AnyFullEdge`).
 
         If set to False, it will yield neighbor vertices, and can be
         used as `NextVertices` function, and edge data that your edges
         may contain will be ignored.
 
     :param add_inverted: If False, the resulting neighbor function will only yield
         for *edges*. If True, the function will also provide the
```

### Comparing `nographs-3.2.0/src/nographs/_gear_collections.py` & `nographs-3.3.0/src/nographs/_gear_collections.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/src/nographs/_gears.py` & `nographs-3.3.0/src/nographs/_gears.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,20 @@
     MutableSequence,
 )
 from typing import (
     Protocol,
     Literal,
     Generic,
     Union,
-    TypeVar,
-    Tuple,
 )
+
+# Sphinx has an issue with documenting tuple[T] in HTML. Thus, for
+# type annotations, typing.Tuple is used. It is depreciated,
+# but still supported....
+from typing import Tuple
 from abc import abstractmethod
 from array import array
 from itertools import repeat
 from decimal import Decimal
 
 from ._types import (
     T_vertex,
@@ -30,24 +33,14 @@
     VertexSetWrappingSequenceNoBitPacking,
     VertexSetWrappingSequenceBitPacking,
     VertexMappingWrappingSequenceWithoutNone,
     VertexMappingWrappingSequenceWithNone,
 )
 
 
-# With the following, for this module, tuple is replaced by typing.Tuple.
-# (Reason: Error in Sphinx with correctly documenting tuple[T] in HTML.
-#  In the meantime, this workaround is used. typing.Tuple is depreciated,
-#  but still supported...)
-U = TypeVar("U")
-V = TypeVar("V")
-
-tuple = Tuple[U, V]
-
-
 # --- ABCs for the needed collection kinds for NoGraphs ---
 
 # The following type aliases are not documented as part of the API documentation.
 # In the API documentation, they are replaced by their respective definition.
 
 """
 ABC for a collection that is intended to be used by NoGraphs for storing sets
@@ -143,25 +136,25 @@
 
         :param initial_content: The collection is created with this initial content.
         """
         raise NotImplementedError
 
     @abstractmethod
     def vertex_id_to_vertex_mapping(
-        self, initial_content: Iterable[tuple[T_vertex_id, T_vertex]]
+        self, initial_content: Iterable[Tuple[T_vertex_id, T_vertex]]
     ) -> VertexIdToVertexMapping[T_vertex_id, T_vertex]:
         """Factory for a mapping from a vertex id to a vertex.
 
         :param initial_content: The collection is created with this initial content.
         """
         raise NotImplementedError
 
     @abstractmethod
     def vertex_id_to_path_attributes_mapping(
-        self, initial_content: Iterable[tuple[T_vertex_id, T_labels]]
+        self, initial_content: Iterable[Tuple[T_vertex_id, T_labels]]
     ) -> VertexIdToPathEdgeDataMapping[T_vertex_id, T_labels]:
         """Factory for a mapping from a vertex id to edge data.
 
         :param initial_content: The collection is created with this initial content.
         """
         raise NotImplementedError
 
@@ -219,15 +212,15 @@
     def infinity(self) -> T_weight:
         """Return the positive infinity value of T_weight for the gear, e.g.,
         float("infinity") for float."""
         raise NotImplementedError
 
     @abstractmethod
     def vertex_id_to_distance_mapping(
-        self, initial_content: Iterable[tuple[T_vertex_id, T_weight]]
+        self, initial_content: Iterable[Tuple[T_vertex_id, T_weight]]
     ) -> VertexIdToDistanceMapping[T_vertex_id, T_weight]:
         """Factory for a mapping from a vertex id to a distance value.
 
         If the returned mapping does not contain a value for some key,
         its method __getitem__ needs to return the positive infinity value.
 
         :param initial_content: The collection is created with this initial content.
@@ -252,18 +245,19 @@
 
 class DefaultdictWithNiceStr(collections.defaultdict[T_vertex_id, T_weight]):
     def __str__(self) -> str:
         return str(dict(self))
 
 
 class GearForHashableVertexIDs(Gear[T_vertex, T_vertex_id, T_weight, T_labels]):
-    """Factory methods for bookkeeping collections. For graphs with hashable vertices
+    """Factory methods for bookkeeping collections. For graphs with
+    **hashable vertices**
     (or vertices made hashable by providing a `VertexToID` function to the traversal).
 
-    Uses hash-based collections (e.g., set and dict) for storing data.
+    It uses **hash-based collections** (e.g., set and dict) for storing data.
 
     :param zero: Value of type T_weight that is used to represent zero distance.
 
     :param inf: Value of type T_weight that is used to represent infinite distance
       (larger than any finite distance that might occur)
     """
 
@@ -273,20 +267,20 @@
 
     def vertex_id_set(
         self, initial_content: Iterable[T_vertex_id]
     ) -> VertexSet[T_vertex_id]:
         return set[T_vertex_id](initial_content)
 
     def vertex_id_to_vertex_mapping(
-        self, initial_content: Iterable[tuple[T_vertex_id, T_vertex]]
+        self, initial_content: Iterable[Tuple[T_vertex_id, T_vertex]]
     ) -> VertexMapping[T_vertex_id, T_vertex]:
         return dict[T_vertex_id, T_vertex](initial_content)
 
     def vertex_id_to_path_attributes_mapping(
-        self, initial_content: Iterable[tuple[T_vertex_id, T_labels]]
+        self, initial_content: Iterable[Tuple[T_vertex_id, T_labels]]
     ) -> VertexMapping[T_vertex_id, T_labels]:
         return dict[T_vertex_id, T_labels](initial_content)
 
     def sequence_of_vertices(
         self, initial_content: Iterable[T_vertex]
     ) -> MutableSequenceOfVertices[T_vertex]:
         return list[T_vertex](initial_content)
@@ -294,15 +288,15 @@
     def zero(self) -> T_weight:
         return self._zero_value
 
     def infinity(self) -> T_weight:
         return self._infinity_value
 
     def vertex_id_to_distance_mapping(
-        self, initial_content: Iterable[tuple[T_vertex_id, T_weight]]
+        self, initial_content: Iterable[Tuple[T_vertex_id, T_weight]]
     ) -> VertexMapping[T_vertex_id, T_weight]:
         return DefaultdictWithNiceStr[T_vertex_id, T_weight](
             lambda: self._infinity_value, initial_content
         )
 
 
 # Implementation note:
@@ -320,20 +314,23 @@
 # The same holds for the other classes for specific weight type.
 
 
 class GearDefault(
     Generic[T_vertex, T_vertex_id, T_weight, T_labels],
     GearForHashableVertexIDs[T_vertex, T_vertex_id, Union[T_weight, float], T_labels],
 ):
-    """A `GearForHashableVertexIDs` that uses the integer 0 for zero
-    distance, and float("infinity") for infinite distance and thus,
-    Union[T_weight, float] as type of distances.
+    """A `GearForHashableVertexIDs` (see there).
 
-    When using GearDefault, the choice of these two numbers has the following
-    consequences:
+    For functionality of NoGraphs that deals with edge weights and distances:
+
+    It uses the integer **0 for zero distance**, and
+    **float("infinity") for infinite distance**
+    and thus, Union[T_weight, float] as type of distances.
+
+    The choice of these two numbers has the following consequences:
 
     - Additional requirement for T_weight: Additionally to the usual requirements
       for edge weights in NoGraphs (see `T_weight`), it needs to be possible to
       add the integer 0 to a weight, and a weight needs to be comparable
       to *float("infinity")*.
 
     - Distances calculated and returned by NoGraphs can not only be values of the
@@ -345,50 +342,53 @@
       generated by GearDefault as distance (otherwise, your typing is inconsistent,
       and a static type checker will report an error).
 
     **Examples for typical T_weight number types** that can be used with GearDefault,
     because they fulfil the requirements described above:
 
        *float*, *int*, *Decimal* and class *mpf* of library *mpmath*.
+
+    Due to this wide range of supported scenarios, GearDefault is the
+    gear that is used most often in NoGraphs.
     """
 
     def __init__(self) -> None:
         super().__init__(0, float("inf"))
 
 
 class GearForHashableVertexIDsAndIntsMaybeFloats(
     GearForHashableVertexIDs[T_vertex, T_vertex_id, float, T_labels]
 ):
-    """A `GearForHashableVertexIDs` for weights that are of type float or integer.
+    """A `GearForHashableVertexIDs` for **weights that are of type float or integer**.
 
-    It uses the integer 0 for zero distance. If all occurring edge weights
+    It uses the integer **0 for zero distance**. If all occurring edge weights
     are also integers, all reported distances of reached vertices will also be
     integers. So, this gear can also be used for calculations within the integers.
 
-    It uses *float("infinity")* for infinite distance. So, infinite distance will
+    It uses **float("infinity") for infinite distance**. So, infinite distance will
     always be reported as float.
     """
 
     def __init__(self) -> None:
         super().__init__(0, float("inf"))
 
 
 class GearForHashableVertexIDsAndDecimals(
     GearForHashableVertexIDs[T_vertex, T_vertex_id, Decimal, T_labels]
 ):
-    """A `GearForHashableVertexIDs` for weights that are of type Decimal."""
+    """A `GearForHashableVertexIDs` for **weights that are of type Decimal**."""
 
     def __init__(self) -> None:
         super().__init__(Decimal(0), Decimal("inf"))
 
 
 class GearForHashableVertexIDsAndFloats(
     GearForHashableVertexIDs[T_vertex, T_vertex_id, float, T_labels]
 ):
-    """A `GearForHashableVertexIDs` for weights that are of type float."""
+    """A `GearForHashableVertexIDs` for **weights that are of type float**."""
 
     def __init__(self) -> None:
         super().__init__(0.0, float("inf"))
 
 
 # --- Integers ----------------------------------------------------------
 
@@ -398,21 +398,21 @@
 
 
 class GearForIntVertexIDs(
     Gear[T_vertex, IntVertexID, T_weight, T_labels],
     Generic[T_vertex, T_weight, T_labels],
 ):
     """Factory methods for bookkeeping collections. For graphs with
-    vertex IDs that are non-negative integers (to be exact: they should be
+    **vertex IDs that are non-negative integers** (to be exact: they should be
     a dense subset of the natural numbers starting at 0).
     (Either, your vertices are such numbers, or you assign such numbers as IDs to
     them, see tutorial section about `vertex identity <vertex_identity>`).
 
     Trades type flexibility and runtime for an (often large) reduction of the memory
-    consumption: Uses sequence-based collections (instead of hash-based collections
+    consumption: Uses **sequence-based collections** (instead of hash-based collections
     like dict and set) for bookkeeping. Arrays are preferred over lists, since there,
     data can be stored as C-native values. Boolean values are packed into integers.
 
     Notes:
 
     - If you are on a 32-bit system, lists and arrays can not be larger than
       sys.maxsize/4 = 536,870,912 entries, what limits your vertex ids (and vertices,
@@ -476,22 +476,22 @@
             VertexSetWrappingSequenceNoBitPacking
             if self._no_bit_packing
             else VertexSetWrappingSequenceBitPacking
         )
         return collection_class(sequence_factory, extend_size, initial_content)
 
     def vertex_id_to_vertex_mapping(
-        self, initial_content: Iterable[tuple[IntVertexID, T_vertex]]
+        self, initial_content: Iterable[Tuple[IntVertexID, T_vertex]]
     ) -> VertexMapping[IntVertexID, T_vertex]:
         return VertexMappingWrappingSequenceWithNone[T_vertex](
             lambda: [None] * self._pre_allocate, None, 1024, initial_content
         )
 
     def vertex_id_to_path_attributes_mapping(
-        self, initial_content: Iterable[tuple[IntVertexID, T_labels]]
+        self, initial_content: Iterable[Tuple[IntVertexID, T_labels]]
     ) -> VertexMapping[IntVertexID, T_labels]:
         return VertexMappingWrappingSequenceWithNone[T_labels](
             lambda: [None] * self._pre_allocate, None, 1024, initial_content
         )
 
     def sequence_of_vertices(
         self, initial_content: Iterable[T_vertex]
@@ -501,34 +501,34 @@
     def zero(self) -> T_weight:
         return self._zero_value
 
     def infinity(self) -> T_weight:
         return self._infinity_value
 
     def vertex_id_to_distance_mapping(
-        self, initial_content: Iterable[tuple[IntVertexID, T_weight]]
+        self, initial_content: Iterable[Tuple[IntVertexID, T_weight]]
     ) -> VertexMapping[IntVertexID, T_weight]:
         return VertexMappingWrappingSequenceWithoutNone[T_weight](
             lambda: [self._infinity_value] * self._pre_allocate,
             self._infinity_value,
             1024,
             initial_content,
         )
 
 
 class GearForIntVertexIDsAndIntsMaybeFloats(
     GearForIntVertexIDs[T_vertex, float, T_labels]
 ):
-    """A `GearForIntVertexIDs` for weights that are of type float or integer.
+    """A `GearForIntVertexIDs` for **weights that are of type float or integer**.
 
-    It uses the integer 0 for zero distances. If all occurring edge weights are
+    It uses the integer **0 for zero distances**. If all occurring edge weights are
     also integers, all reported distances of reached vertices will also be integers.
     So, this gear can also be used for calculations within the integers.
 
-    It uses float(“infinity”) for infinite distance. So, infinite distance
+    It uses **float(“infinity”) for infinite distance**. So, infinite distance
     will always be reported as float.
 
     :param no_arrays: Use only lists, no arrays. See `GearForIntVertexIDs`.
 
     :param no_bit_packing: Store boolean values in vertex sets as integers instead of
       bits. See `GearForIntVertexIDs`.
 
@@ -542,15 +542,15 @@
         no_bit_packing: bool = False,
         pre_allocate: int = 0,
     ) -> None:
         super().__init__(0, float("inf"), no_arrays, no_bit_packing, pre_allocate)
 
 
 class GearForIntVertexIDsAndDecimals(GearForIntVertexIDs[T_vertex, Decimal, T_labels]):
-    """A `GearForIntVertexIDs` for weights that are of type Decimal.
+    """A `GearForIntVertexIDs` for **weights that are of type Decimal**.
 
     :param no_arrays: Use lists instead of arrays. See `GearForIntVertexIDs`.
 
     :param no_bit_packing: Store boolean values in vertex sets as integers instead of
       bits. See `GearForIntVertexIDs`.
 
     :param pre_allocate: Space for this number of vertices is pre-allocated when a
@@ -565,16 +565,16 @@
     ) -> None:
         super().__init__(
             Decimal(0), Decimal("inf"), no_arrays, no_bit_packing, pre_allocate
         )
 
 
 class GearForIntVertexIDsAndCFloats(GearForIntVertexIDs[T_vertex, float, T_labels]):
-    """A `GearForIntVertexIDs` for weights that are floats in the limits
-    of some C-native float type.
+    """A `GearForIntVertexIDs` for **weights that are floats in the limits**
+    **of some C-native float type**.
 
     Here, arrays and C-native storage of data are also used for distances.
 
     :param no_bit_packing: Store boolean values in vertex sets as integers instead of
       bits. See `GearForIntVertexIDs`.
 
     :param distance_type_code: Number of bytes used to store distances float values,
@@ -593,30 +593,30 @@
         distance_type_code: Literal["f", "d"] = "f",
         pre_allocate: int = 0,
     ) -> None:
         self.distance_type_code = distance_type_code
         super().__init__(0.0, float("inf"), False, no_bit_packing, pre_allocate)
 
     def vertex_id_to_distance_mapping(
-        self, initial_content: Iterable[tuple[IntVertexID, float]]
+        self, initial_content: Iterable[Tuple[IntVertexID, float]]
     ) -> VertexMapping[IntVertexID, float]:
         return VertexMappingWrappingSequenceWithoutNone[float](
             lambda: array(
                 self.distance_type_code,
                 repeat(self._infinity_value, self._pre_allocate),
             ),
             self._infinity_value,
             1024,
             initial_content,
         )
 
 
 class GearForIntVertexIDsAndCInts(GearForIntVertexIDs[T_vertex, int, T_labels]):
-    """A `GearForIntVertexIDs` for weights that are integers in the limits
-    of some C-native integer type.
+    """A `GearForIntVertexIDs` for **weights that are integers in the limits**
+    **of some C-native integer type.**
 
     Here, arrays and C-native storage of data are also used for distances.
 
     :param no_bit_packing: Store boolean values in vertex sets as integers instead of
       bits. See `GearForIntVertexIDs`.
 
     :param distance_type_code: Number of bytes used to store distances integer values,
@@ -641,15 +641,15 @@
         # Highest possible vertex value will be used as NaN value.
         # If this value is stored for some vertex as index, this means that
         # the collection stores no value for the index vertex so far.
         self.max_type_value = max_value_for_integer_array_type_code(distance_type_code)
         super().__init__(0, self.max_type_value, False, no_bit_packing, pre_allocate)
 
     def vertex_id_to_distance_mapping(
-        self, initial_content: Iterable[tuple[IntVertexID, int]]
+        self, initial_content: Iterable[Tuple[IntVertexID, int]]
     ) -> VertexMapping[IntVertexID, int]:
         return VertexMappingWrappingSequenceWithoutNone[int](
             lambda: array(
                 self.distance_type_code,
                 repeat(self._infinity_value, self._pre_allocate),
             ),
             self._infinity_value,
@@ -659,18 +659,18 @@
 
 
 # --- Integer vertices ---
 
 
 class GearForIntVerticesAndIDs(GearForIntVertexIDs[IntVertexID, T_weight, T_labels]):
     """A `GearForIntVertexIDs` (see there for constraints on vertex ids)
-    for graphs with vertices, that are non-negative
-    integers and fulfil one of the offered size constraints.
+    for graphs with **vertices, that are non-negative integers**
+    and **fulfil one of the offered size constraints**.
 
-    Here, arrays and C-native storage of data are also used for vertices.
+    Here, **arrays and C-native storage of data are also used for vertices**.
 
     :param zero: Value used to represent zero distance.
 
     :param inf: Value used to represent infinite distance.
 
     :param no_bit_packing: Store boolean values of vertex ID sets as integers instead
       of bits. (Depending on the used traversal and the graph, bit packing can reduce
@@ -702,15 +702,15 @@
         vertex_type_code: Literal["L", "Q", "I"] = "L",
         pre_allocate: int = 0,
     ) -> None:
         self.vertex_type_code = vertex_type_code
         super().__init__(zero, inf, False, no_bit_packing, pre_allocate)
 
     def vertex_id_to_vertex_mapping(
-        self, initial_content: Iterable[tuple[IntVertexID, IntVertexID]]
+        self, initial_content: Iterable[Tuple[IntVertexID, IntVertexID]]
     ) -> VertexMapping[IntVertexID, IntVertexID]:
         bytes_of_vertex_type_code = {"L": 4, "Q": 8, "I": 2}[self.vertex_type_code]
         # Highest possible vertex value will be used as NaN value.
         # If this value is stored for some vertex as index, this means that
         # the collection stores no value for the index vertex so far.
         max_vertex_type_value = 256**bytes_of_vertex_type_code - 1
 
@@ -728,21 +728,21 @@
     ) -> MutableSequenceOfVertices[IntVertexID]:
         return array(self.vertex_type_code, initial_content)
 
 
 class GearForIntVerticesAndIDsAndIntsMaybeFloats(
     GearForIntVerticesAndIDs[float, T_labels]
 ):
-    """A `GearForIntVerticesAndIDs` for weights that are of type float or integer.
+    """A `GearForIntVerticesAndIDs` for **weights that are of type float or integer**.
 
-    It uses the integer 0 for zero distances. If all occurring edge weights are
+    It uses the integer **0 for zero distances**. If all occurring edge weights are
     also integers, all reported distances of reached vertices will also be integers.
     So, this gear can also be used for calculations within the integers.
 
-    It uses float(“infinity”) for infinite distance. So, infinite distance
+    It uses **float(“infinity”) for infinite distance**. So, infinite distance
     will always be reported as float.
 
     :param no_bit_packing: Store boolean values in vertex sets as integers instead of
       bits. See `GearForIntVerticesAndIDs`.
 
     :param vertex_type_code: Number of bytes used to store one of your integer
       vertices, as type_code. See `GearForIntVerticesAndIDs`.
@@ -759,15 +759,15 @@
     ) -> None:
         super().__init__(
             0, float("inf"), no_bit_packing, vertex_type_code, pre_allocate
         )
 
 
 class GearForIntVerticesAndIDsAndDecimals(GearForIntVerticesAndIDs[Decimal, T_labels]):
-    """A `GearForIntVerticesAndIDs` for weights that are of type Decimal.
+    """A `GearForIntVerticesAndIDs` for **weights that are of type Decimal**.
 
     :param no_bit_packing: Store boolean values of vertex id sets as integers instead
       of bits. See `GearForIntVerticesAndIDs`.
 
     :param vertex_type_code: Number of bytes used to store one of your integer
       vertices, as type_code. See `GearForIntVerticesAndIDs`.
 
@@ -783,21 +783,18 @@
     ) -> None:
         super().__init__(
             Decimal(0), Decimal("inf"), no_bit_packing, vertex_type_code, pre_allocate
         )
 
 
 class GearForIntVerticesAndIDsAndCFloats(GearForIntVerticesAndIDs[float, T_labels]):
-    """A `GearForIntVerticesAndIDs` for graphs with dense non-negative integers of
-    constrained size in bytes as vertex ids AND as vertices, and edge weights
-    that are floats in the limits of some C-native float type.
-
-    for edge weight and distance values.
+    """A `GearForIntVerticesAndIDs` for
+    **weights that are floats in the limits of some C-native float type**.
 
-    Here, arrays and C-native storage of data are also used for vertices.
+    Here, **arrays and C-native storage of data are also used for weights**.
 
     :param no_bit_packing: Store boolean values of vertex id sets as integers instead
       of bits. See `GearForIntVerticesAndIDs`.
 
     :param vertex_type_code: Number of bytes used to store one of your integer
       vertices, as type_code. See `GearForIntVerticesAndIDs`.
 
@@ -821,33 +818,32 @@
     ) -> None:
         self.distance_type_code = distance_type_code
         super().__init__(
             0.0, float("inf"), no_bit_packing, vertex_type_code, pre_allocate
         )
 
     def vertex_id_to_distance_mapping(
-        self, initial_content: Iterable[tuple[IntVertexID, float]]
+        self, initial_content: Iterable[Tuple[IntVertexID, float]]
     ) -> VertexMapping[IntVertexID, float]:
         return VertexMappingWrappingSequenceWithoutNone[float](
             lambda: array(
                 self.distance_type_code,
                 repeat(self._infinity_value, self._pre_allocate),
             ),
             self._infinity_value,
             1024,
             initial_content,
         )
 
 
 class GearForIntVerticesAndIDsAndCInts(GearForIntVerticesAndIDs[int, T_labels]):
-    """A `GearForIntVerticesAndIDs` for graphs with dense non-negative integers of
-    constrained size in bytes as vertex ids AND as vertices, and integers in the limits
-    of some C-native integer type.
+    """A `GearForIntVerticesAndIDs` for
+    **weights that are integers in the limits of some C-native integer type**.
 
-    Here, arrays and C-native storage of data are also used for vertices.
+    Here, **arrays and C-native storage of data are also used for weights**.
 
     :param no_bit_packing: Store boolean values of vertex id sets as integers instead
       of bits. See `GearForIntVerticesAndIDs`.
 
     :param vertex_type_code: Number of bytes used to store one of your integer
       vertices, as type_code. See `GearForIntVerticesAndIDs`.
 
@@ -877,15 +873,15 @@
         # the collection stores no (real) value for the index vertex so far.
         self.max_type_value = max_value_for_integer_array_type_code(distance_type_code)
         super().__init__(
             0, self.max_type_value, no_bit_packing, vertex_type_code, pre_allocate
         )
 
     def vertex_id_to_distance_mapping(
-        self, initial_content: Iterable[tuple[IntVertexID, int]]
+        self, initial_content: Iterable[Tuple[IntVertexID, int]]
     ) -> VertexMapping[IntVertexID, int]:
         return VertexMappingWrappingSequenceWithoutNone[int](
             lambda: array(
                 self.distance_type_code,
                 repeat(self._infinity_value, self._pre_allocate),
             ),
             self._infinity_value,
```

### Comparing `nographs-3.2.0/src/nographs/_matrix_gadgets.py` & `nographs-3.3.0/src/nographs/_extra_matrix_gadgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,16 +324,18 @@
         weight such a move has w.r.t. the content of the matrix at this
         position (parameter *content_to_weight*, and no assigned weight means
         the move is impossible).
 
         :param content_to_weight: Returns the weight of a move to a given position.
         :param wrap: Positions are wrapped at the array limits.
         :param diagonals: Diagonal moves are allowed.
+
+        :rtype: Callable[[Position, Any], Iterable[tuple[Position, T_weight]]]
         """
-        # inspection PyShadowingNames
+        # For reason for manually documented rtype see method items above.
         limits = self.limits()
         moves = Position.moves(dimensions=self.dimensions, diagonals=diagonals)
 
         def next_edges(vector: Position, _: Any) -> Iterator[tuple[Position, T_weight]]:
             for neighbor in vector.neighbors(moves=moves, limits=limits, wrap=wrap):
                 weight = content_to_weight.get(self[neighbor], None)
                 if weight is not None:
```

### Comparing `nographs-3.2.0/src/nographs/_path.py` & `nographs-3.3.0/src/nographs/_path.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/src/nographs/_paths.py` & `nographs-3.3.0/src/nographs/_paths.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/src/nographs/_strategies.py` & `nographs-3.3.0/src/nographs/_strategies.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/src/nographs/_traversals.py` & `nographs-3.3.0/src/nographs/_traversals.py`

 * *Files 2% similar despite different names*

```diff
@@ -846,14 +846,19 @@
 
     Uses the following standard arguments for the respective parameters of
     the parent class:
 
     - vertex_to_id = `vertex_as_id`
     - gear = `GearDefault`
     - `T_vertex_id` = `T_vertex`
+
+    Implications:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_vertices: Optional[
             NextVertices[
                 T_vertex, TraversalBreadthFirstFlex[T_vertex, T_vertex, T_labels]
@@ -1230,14 +1235,19 @@
 
     Uses the following standard arguments for the respective parameters of
     the parent class:
 
     - vertex_to_id = `vertex_as_id`
     - gear = `GearDefault`
     - `T_vertex_id` = `T_vertex`
+
+    Implications:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_vertices: Optional[
             NextVertices[
                 T_vertex, TraversalDepthFirstFlex[T_vertex, T_vertex, T_labels]
@@ -1534,14 +1544,19 @@
 
     Uses the following standard arguments for the respective parameters of
     the parent class:
 
     - vertex_to_id = `vertex_as_id`
     - gear = `GearDefault`
     - `T_vertex_id` = `T_vertex`
+
+    Implications:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_vertices: Optional[
             NextVertices[
                 T_vertex, TraversalNeighborsThenDepthFlex[T_vertex, T_vertex, T_labels]
@@ -2145,14 +2160,19 @@
 
     Uses the following standard arguments for the respective parameters of
     the parent class:
 
     - vertex_to_id = `vertex_as_id`
     - gear = `GearDefault`
     - `T_vertex_id` = `T_vertex`
+
+    Implications:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_vertices: Optional[
             NextVertices[
                 T_vertex, TraversalTopologicalSortFlex[T_vertex, T_vertex, T_labels]
@@ -2187,27 +2207,133 @@
 
 
 class _TraversalWithWeights(
     Generic[T_vertex, T_vertex_id, T_weight, T_labels],
     Traversal[T_vertex, T_vertex_id, T_labels],
     ABC,
 ):
+    """A Traversal that needs weighted edges and uses a gear suitable for this."""
+
     def __init__(
         self,
         labeled_edges: bool,
         is_tree: bool,
         vertex_to_id: VertexToID[T_vertex, T_vertex_id],
         gear: Gear[T_vertex, T_vertex_id, T_weight, T_labels],
     ) -> None:
         self._gear = gear
         super().__init__(labeled_edges, is_tree, vertex_to_id)
 
 
+class _TraversalWithDistances(
+    _TraversalWithWeights[T_vertex, T_vertex_id, T_weight, T_labels],
+    ABC,
+):
+    """
+    A _TraversalWithWeights that provides a distances collection as part of
+    its state.
+    """
+
+    def __init__(
+        self,
+        labeled_edges: bool,
+        is_tree: bool,
+        vertex_to_id: VertexToID[T_vertex, T_vertex_id],
+        gear: Gear[T_vertex, T_vertex_id, T_weight, T_labels],
+    ) -> None:
+        super().__init__(labeled_edges, is_tree, vertex_to_id, gear)
+
+        self.distances: VertexIdToDistanceMapping[
+            T_vertex_id, T_weight
+        ] = NoDistancesMapping[T_vertex_id, T_weight]()
+        """ Provisional or final distance values of some vertices
+        (distance from a start vertex). Without option *keep_distances*,
+        the value for a vertex is removed once the vertex has been reported. With
+        option *keep_distances*, values are never removed, and that means: During a
+        traversal, the distance values for already reported vertices can be found in
+        the collection. After an exhaustive search, the collection contains exactly
+        and only the distances of all vertices that are reachable from the start
+        vertices and of the start vertices themselves.
+        """
+
+    def _improve_state(
+        self, state: dict[str, Any], vertices: Optional[Iterable[T_vertex]] = None
+    ) -> None:
+        # Assignments in distances are only valid for reported vertices. Thus,
+        # we need to convert only keys/values for requested vertices to a string,
+        # not the whole MutableMapping. So, we special case this attribute here.
+        del state["distances"]
+        if vertices is not None:
+            vertex_to_id, distances = self._vertex_to_id, self.distances
+            state["distances"] = StrRepr.from_iterable(
+                (v_id := vertex_to_id(vertex), distances[v_id]) for vertex in vertices
+            )
+        super()._improve_state(state, vertices)
+
+
+class _TraversalWithDistance(
+    _TraversalWithDistances[T_vertex, T_vertex_id, T_weight, T_labels],
+    ABC,
+):
+    """
+    A _TraversalWithDistances that provides a distance as part of its staste.
+    If offers the go_for_distance_range method based on the distance.
+    """
+
+    def __init__(
+        self,
+        labeled_edges: bool,
+        is_tree: bool,
+        vertex_to_id: VertexToID[T_vertex, T_vertex_id],
+        gear: Gear[T_vertex, T_vertex_id, T_weight, T_labels],
+    ) -> None:
+        super().__init__(labeled_edges, is_tree, vertex_to_id, gear)
+
+        # The following value is not used by NoGraphs. It is only set
+        # to have some initialization.
+        self.distance: T_weight = self._gear.infinity()
+        """ The length of the shortest path (sum of edge weights) from a
+        start vertex to the visited vertex
+        """
+
+    def go_for_distance_range(self, start: Real, stop: Real) -> Iterator[T_vertex]:
+        """
+        For a started traversal, return an iterator. During the traversal,
+        the iterator skips vertices as long as their distance is lower than *start*.
+        From then on, is reports the found vertices. It stops when the reached
+        distance is equal to or higher than *stop*.
+
+        Note: The first vertex with a distance equal or higher than stop will be
+        consumed from the traversal, but will not be reported, so it is lost (compare
+        itertools.takewhile).
+        """
+        if not isinstance(type(self), type(Traversal)):
+            raise RuntimeError(
+                "Method go_for_distance_range can only be called "
+                + "on a Traversal object."
+            )
+
+        # In order to make the above check work, the following generator functionality
+        # needs to be encapsulated in a local function
+        def my_generator() -> Iterator[T_vertex]:
+            for v in self._generator:
+                if self.distance >= start:
+                    if self.distance < stop:
+                        yield v
+                    break
+            for v in self._generator:
+                if self.distance >= stop:
+                    break
+                yield v
+
+        return my_generator()
+
+
 class TraversalShortestPathsFlex(
-    _TraversalWithWeights[T_vertex, T_vertex_id, T_weight, T_labels]
+    _TraversalWithDistance[T_vertex, T_vertex_id, T_weight, T_labels]
 ):
     """
     | Bases: Generic[`T_vertex`, `T_vertex_id`, `T_weight`, `T_labels`],
     | `Traversal` [`T_vertex`, `T_vertex_id`, `T_labels`]
 
     :param vertex_to_id: See `VertexToID` function.
 
@@ -2267,33 +2393,16 @@
         super().__init__(labeled_edges, is_tree, vertex_to_id, gear)
 
         self._known_distances: Optional[
             VertexIdToDistanceMapping[T_vertex_id, T_weight]
         ] = None
         self._keep_distances = False
 
-        self.distances: VertexIdToDistanceMapping[
-            T_vertex_id, T_weight
-        ] = NoDistancesMapping[T_vertex_id, T_weight]()
-        """ Provisional or final distance values of some vertices
-        (distance from a start vertex). Without option *keep_distances*,
-        the value for a vertex is removed once the vertex has been reported. With
-        option *keep_distances*, values are never removed, and that means: During a
-        traversal, the distance values for already reported vertices can be found in
-        the collection. After an exhaustive search, the collection contains exactly
-        and only the distances of all vertices that are reachable from the start
-        vertices and of the start vertices themselves.
-        """
-
-        # The following three values are not used by NoGraphs. They are only set
+        # The following value is not used by NoGraphs. It is only set
         # to have some initialization.
-        self.distance: T_weight = self._gear.infinity()
-        """ The length of the shortest path (sum of edge weights) from a
-        start vertex to the visited vertex
-        """
         self.depth: int = -1
         """  At this *search depth*, the reported (resp. the expanded) vertex has been
         found. It equals the length (number of edges) of the created path to the
         vertex, if path creation is demanded.
         Note: The search depth does not need to be the depth of the vertex
         (see `TraversalBreadthFirstFlex`).
         When a traversal has been started, but no vertex has been reported or expanded
@@ -2537,60 +2646,14 @@
                         n_path_weight,
                         next(unique_no),
                         neighbor,
                         n_path_edge_count,
                     ),
                 )
 
-    def go_for_distance_range(self, start: Real, stop: Real) -> Iterator[T_vertex]:
-        """
-        For a started traversal, return an iterator. During the traversal,
-        the iterator skips vertices as long as their distance is lower than *start*.
-        From then on, is reports the found vertices. It stops when the reached
-        distance is equal to or higher than *stop*.
-
-        Note: The first vertex with a distance equal or higher than stop will be
-        consumed from the traversal, but will not be reported, so it is lost (compare
-        itertools.takewhile).
-        """
-        if not isinstance(type(self), type(Traversal)):
-            raise RuntimeError(
-                "Method go_for_distance_range can only be called "
-                + "on a Traversal object."
-            )
-
-        # In order to make the above check work, the following generator functionality
-        # needs to be encapsulated in a local function
-        def my_generator() -> Iterator[T_vertex]:
-            for v in self._generator:
-                if self.distance >= start:
-                    if self.distance < stop:
-                        yield v
-                    break
-            for v in self._generator:
-                if self.distance >= stop:
-                    break
-                yield v
-
-        return my_generator()
-
-    def _improve_state(
-        self, state: dict[str, Any], vertices: Optional[Iterable[T_vertex]] = None
-    ) -> None:
-        # Assignments in distances are only valid for reported vertices. Thus,
-        # we need to convert only keys/values for requested vertices to a string,
-        # not the whole MutableMapping. So, we special case this attribute here.
-        del state["distances"]
-        if vertices is not None:
-            vertex_to_id, distances = self._vertex_to_id, self.distances
-            state["distances"] = StrRepr.from_iterable(
-                (v_id := vertex_to_id(vertex), distances[v_id]) for vertex in vertices
-            )
-        super()._improve_state(state, vertices)
-
 
 class TraversalShortestPaths(
     Generic[T_vertex, T_weight, T_labels],
     TraversalShortestPathsFlex[T_vertex, T_vertex, Union[T_weight, float], T_labels],
 ):
     """
     Eases the use of `TraversalShortestPathsFlex` for typical cases.
@@ -2603,14 +2666,20 @@
     is a short form for
 
     .. code-block:: python
 
        TraversalShortestPathsFlex[
            T_vertex, T_vertex, Union[T_weight, float], T_labels],
       ](nog.vertex_as_id, nog.GearDefault(), *args, **keywords)
+
+    Implications:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - The used weights are defined by Union[T_weight, float], see `GearDefault`
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_edges: Optional[
             NextWeightedEdges[
                 T_vertex,
@@ -2639,15 +2708,15 @@
             next_edges,
             next_labeled_edges=next_labeled_edges,
             is_tree=is_tree,
         )
 
 
 class TraversalAStarFlex(
-    _TraversalWithWeights[T_vertex, T_vertex_id, T_weight, T_labels]
+    _TraversalWithDistances[T_vertex, T_vertex_id, T_weight, T_labels]
 ):
     """
     | Bases: Generic[`T_vertex`, `T_vertex_id`, `T_weight`, `T_labels`],
     | `Traversal` [`T_vertex`, `T_vertex_id`, `T_labels`]
 
     :param vertex_to_id: See `VertexToID` function.
 
@@ -2739,18 +2808,14 @@
         self._heuristic: Optional[Callable[[T_vertex], Real]] = None
         self._known_distances: Optional[
             VertexIdToDistanceMapping[T_vertex_id, T_weight]
         ] = None
         self._known_path_length_guesses: Optional[
             VertexIdToDistanceMapping[T_vertex_id, T_weight]
         ] = None
-
-        self.distances: VertexIdToDistanceMapping[
-            T_vertex_id, T_weight
-        ] = NoDistancesMapping[T_vertex_id, T_weight]()
         self._path_length_guesses: Optional[
             VertexIdToDistanceMapping[T_vertex_id, T_weight]
         ] = None
 
     def start_from(
         self,
         heuristic: Callable[[T_vertex], Real],
@@ -3021,28 +3086,14 @@
                     except IndexError:
                         path_length_guesses_wrapper.extend_and_set(n_id, n_guess)
                 heappush(
                     to_visit,
                     (n_guess, next(unique_no), neighbor, n_path_edge_count),
                 )
 
-    def _improve_state(
-        self, state: dict[str, Any], vertices: Optional[Iterable[T_vertex]] = None
-    ) -> None:
-        # Assignments in distances are only valid for reported vertices. Thus,
-        # we need to convert only keys/values for requested vertices to a string,
-        # not the whole MutableMapping. So, we special case this attribute here.
-        del state["distances"]
-        if vertices is not None:
-            vertex_to_id, distances = self._vertex_to_id, self.distances
-            state["distances"] = StrRepr.from_iterable(
-                (v_id := vertex_to_id(vertex), distances[v_id]) for vertex in vertices
-            )
-        super()._improve_state(state, vertices)
-
 
 class TraversalAStar(
     Generic[T_vertex, T_weight, T_labels],
     TraversalAStarFlex[T_vertex, T_vertex, Union[T_weight, float], T_labels],
 ):
     """
     Eases the use of `TraversalAStarFlex` for typical cases.
@@ -3055,14 +3106,20 @@
     is a short form for
 
     .. code-block:: python
 
        TraversalAStarFlex[
            T_vertex, T_vertex, Union[T_weight, float], T_labels],
        ](nog.vertex_as_id, nog.GearDefault(), *args, **keywords)
+
+    Implications:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - The used weights are defined by Union[T_weight, float], see `GearDefault`
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_edges: Optional[
             NextWeightedEdges[
                 T_vertex,
@@ -3401,14 +3458,20 @@
     is a short form for
 
     .. code-block:: python
 
        TraversalMinimumSpanningTreeFlex[
            T_vertex, T_vertex, Union[T_weight, float], T_labels],
        ](nog.vertex_as_id, nog.GearDefault(), *args, **keywords)
+
+    Implications:
+
+    - `GearDefault` is used, see there how it and its superclass work
+    - The used weights are defined by Union[T_weight, float], see `GearDefault`
+    - T_vertex is bound to Hashable (T_vertex is used as `T_vertex_id`, see there)
     """
 
     def __init__(
         self,
         next_edges: Optional[
             NextWeightedEdges[
                 T_vertex,
```

### Comparing `nographs-3.2.0/src/nographs/_types.py` & `nographs-3.3.0/src/nographs/_types.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,43 +6,55 @@
 from abc import abstractmethod
 
 """
 Basic types used in NoGraphs.
 """
 
 
+T = TypeVar("T")
 T_vertex = TypeVar("T_vertex")
 T_vertex_id = TypeVar("T_vertex_id", bound=Hashable)
-T = TypeVar("T")
+T_weight = TypeVar("T_weight", bound="Weight")
 
 
 # The following class is manually documented in api.rst, keep docs consistent.
-class Weight(Protocol[T]):
+class Weight(Protocol[T_weight]):
     @abstractmethod
-    def __add__(self: T, value: T) -> T:
+    def __add__(self: T_weight, value: T_weight) -> T_weight:
         """Return self+value."""
         raise NotImplementedError
 
     @abstractmethod
-    def __sub__(self: T, value: T) -> T:
+    def __sub__(self: T_weight, value: T_weight) -> T_weight:
         """Return self-value."""
         raise NotImplementedError
 
     @abstractmethod
-    def __lt__(self: T, value: T) -> bool:
+    def __lt__(self: T_weight, value: T_weight) -> bool:
         # inherited doc string
         raise NotImplementedError
 
     @abstractmethod
-    def __le__(self: T, value: T) -> bool:
+    def __le__(self: T_weight, value: T_weight) -> bool:
         # inherited doc string
         raise NotImplementedError
 
 
-T_weight = TypeVar("T_weight", bound=Weight)
+# class IntZero(int):
+#     def __new__(cls) -> "IntZero":
+#         return super(IntZero, cls).__new__(cls, 0)
+#
+#
+# class FloatInf(float):
+#     def __new__(cls) -> "FloatInf":
+#         return super(FloatInf, cls).__new__(cls, "inf")
+#
+#
+# T_weight_zero_inf_or = Union[IntZero, FloatInf, T]
+
 
 T_labels = TypeVar("T_labels")
 
 """ Basic type aliases, part 1 """
 VertexToID = Callable[[T_vertex], T_vertex_id]
```

### Comparing `nographs-3.2.0/src/nographs.egg-info/PKG-INFO` & `nographs-3.3.0/src/nographs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nographs
-Version: 3.2.0
+Version: 3.3.0
 Summary: Graph analysis – the lazy (evaluation) way: Analysis on the fly, for graphs, that are computed and/or adapted on the fly.
 Home-page: https://github.com/HeWeMel/nographs
 Author: Dr. Helmut Melcher
 Author-email: HeWeMel@web.de
 Project-URL: Documentation, https://nographs.readthedocs.io/
 Project-URL: Source, https://github.com/hewemel/nographs/
 Project-URL: Bug Reports, https://github.com/hewemel/nographs/issues
-Keywords: graph,network,search,traverse,analysis,infinite,lazy,shortest,distance,depth,DFS,breadth,BFS,Dijkstra,topological,MST
+Keywords: graph,network,search,traverse,analysis,infinite,lazy,shortest,distance,depth,DFS,breadth,BFS,Dijkstra,topological,spanning,MST,TSP
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -74,14 +74,22 @@
 **computed and/or adapted in application code on the fly**
 (when needed and as far as needed). Also,
 **the analysis and the reporting of results by the library happen on the fly**
 (when, and as far as, results can already be derived).
 
 Think of it as *graph analysis - the lazy (evaluation) way*.
 
+**Documentation**
+
+- `Homepage of the documentation <https://nographs.readthedocs.io>`__
+- `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
+- `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
+  (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
+- `API reference <https://nographs.readthedocs.io/en/latest/api.html>`__
+
 **Feature overview**
 
 - Unidirectional traversal algorithms: DFS, BFS, topological search,
   Dijkstra, A\* and MST.
 - Bidirectional search algorithms: BFS and Dijkstra.
 - Results: Reachability, depth, distance, paths and trees.
   Paths can be
@@ -89,15 +97,15 @@
   and can be iterated in both directions.
 - Flexible graph notion:
 
   - Infinite directed multigraphs with loops and
     attributes (this includes
     multiple adjacency, cycles, self-loops,
     directed edges,
-    weighted edges and edges with application specific attributes).
+    weighted edges and attributed edges).
   - Infinite graphs are supported, but need to be
     locally finite (i.e., a vertex has only finitely many outgoing edges).
 
 - Generic API:
 
   - Vertices: Can be anything except for None. Hashable vertices can be
     used directly, unhashable vertices can be used together with
@@ -116,33 +124,38 @@
     efficiently
 
 - Flexible API: The concept of implicit graphs that NoGraphs is based on
   allows for an API that eases
   operations like
   graph pruning, graph abstraction, the typical binary
   graph operations (union, intersection, several types of products), the
-  computation of search-aware graphs, and
-  traversals of vertex equivalence classes on the fly.
+  computation of search-aware graphs,  the combination of
+  problem reduction with lazy evaluation,
+  and traversals of vertex equivalence classes on the fly.
   Bookkeeping data can be
   pre-initialized and accessed during computations.
 - Typing: The API can be used fully typed (optionally).
 - Implementation: Pure Python (>=3.9). It introduces no further dependencies.
 - CI tests: For all supported versions of Python and both supported interpreters
   CPython and PyPy, both code and docs, 100% code coverage.
 - Runtime and memory performance: Have been goals (CPython). In its domain, it often
-  even outperforms Rust- and C-based libraries.
-  If you need an even higher performance, using PyPy could be an option.
+  even outperforms Rust- and C-based libraries. Using PyPy improves its performance
+  further.
 
-**Documentation**
+**Extras** (outside of the core of NoGraphs)
 
-- `Homepage of the documentation <https://nographs.readthedocs.io>`__
-- `Installation guide <https://nographs.readthedocs.io/en/latest/installation.html>`__
-- `Tutorial <https://nographs.readthedocs.io/en/latest/concept_and_examples.html>`__
-  (contains many `examples <https://nographs.readthedocs.io/en/latest/concept_and_examples.html#examples>`__)
-- `API reference <https://nographs.readthedocs.io/en/latest/api.html>`__
+- Computation of exact solutions for (small)
+  traveling salesman problems (shortest / longest route,
+  positive / zero / negative edge weights, graph does not need to be complete)
+- Dijkstra shortest paths algorithm for
+  infinitely branching graphs with locally sorted edges.
+- Gadget functions for test purposes. They make the easy task of
+  adapting existing explicit test graphs a no brainer, may they be
+  stored in edge indices or edge iterables
+  or in arrays.
 
 **Example**
 
 Our graph is directed, weighted and has infinitely many edges. These edges are
 defined in application code by the following function. For a vertex *i*
 (here: an integer) as the first of two
 parameters, it yields the edges that start at *i* as tuples
@@ -209,14 +222,17 @@
 
 - An infinite generator of primes, defined by just a graph and
   a call to a standard graph algorithm?
 - Or a graph that defines an infinite set
   of Towers of Hanoi problems in a generic way, without fixing the number of
   towers, disk sizes, and the start and goal configuration - and a specific
   problem instance is solved by just one library call?
+- Or a way for computing an exact solution for traveling salesman problems,
+  that is based on just a graph and a call of the Dijkstra single source shortest path
+  algorithm?
 - Or graphs that are dynamically
   computed based on other graphs, or on analysis results about other graphs,
-  or even on partial analysis results from already processed parts of the same graph?
+  or even on partial analysis results for already processed parts of the same graph?
 
 Let's `build it <https://nographs.readthedocs.io/en/latest/installation.html>`__.
 
 Welcome to NoGraphs!
```

### Comparing `nographs-3.2.0/tests/test_docs_examples.py` & `nographs-3.3.0/tests/test_docs_examples.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/tests/test_edge_gadgets.py` & `nographs-3.3.0/tests/test_extra_edge_gadgets.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/tests/test_gear_collections.py` & `nographs-3.3.0/tests/test_gear_collections.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/tests/test_gears.py` & `nographs-3.3.0/tests/test_gears.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/tests/test_matrix_gadgets.py` & `nographs-3.3.0/tests/test_extra_matrix_gadgets.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/tests/test_paths.py` & `nographs-3.3.0/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/tests/test_strategies.py` & `nographs-3.3.0/tests/test_strategies.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/tests/test_traversals_and_searches.py` & `nographs-3.3.0/tests/test_traversals_and_searches.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,19 @@
 import sys
 from abc import abstractmethod, ABC
 from collections.abc import Callable, Hashable, Iterator
 from typing import Any, Iterable, Union, TypeVar, Optional, Protocol, Generic
 
 import nographs as nog
 from nographs import T, Strategy, T_vertex, T_vertex_id, T_labels, T_weight
+
+# noinspection PyProtectedMember
 from nographs._compatibility import pairwise
+
+# noinspection PyProtectedMember
 from nographs._strategies import StrRepr  # NOQA F401 (import needed by doc tests)
 
 # ----- Utilities: Printing test results -----
 
 
 def eprint(*args: Any, **kwargs: Any) -> None:
     """Print to stderr. For typing see print.
@@ -202,69 +206,14 @@
 
         def next_edges_backwards(vertex: T_vertex, strategy: Strategy) -> Iterable:
             return edge_dict_backwards.get(vertex_to_key(vertex), [])
 
     return next_edges_forwards, next_edges_backwards
 
 
-# ---- Utilities: Defining adjacency functions by other means, currently unused ---
-
-# def adj_func_with_reporting_from_mapping(
-#     edges: Mapping[T_vertex, tuple[T, ...]]
-# ) -> Callable[[T_vertex, Strategy], tuple[T, ...]]:
-#     """Adapt a graph given either as NextVertices mapping or as NextEdges mapping.
-#     Return an adjacency function of the respective type that prints attributes
-#     vertex, depth and visited of the given traversal before returning
-#     adjacent vertices or edges.
-#     """
-#
-#     def graph(vertex: T_vertex, strategy: Strategy) -> tuple[T, ...]:
-#         print_filled(f"? {vertex}: {strategy.state_to_str([vertex])}")
-#         return edges.get(vertex, tuple[T, ...]())
-#
-#     return graph
-
-# def adj_func_backwards_from_forwards(
-#     next_forwards_edges: Callable[[T_vertex, Any], Iterable],
-#     vertices: Iterable[T_vertex],
-# ) -> Callable[[T_vertex, Any], Iterable]:
-#     """Create NextEdges function for backward direction based on NextEdges
-#     function (optionally with weights and/or labels) for forward direction
-#     and a vertex list. No log printing happens. Typically used if the given
-#     function also does not print log texts.
-#     """
-#     edge_dict_backwards = collections.defaultdict(list)
-#     for v in vertices:
-#         for w, *others in next_forwards_edges(v, None):
-#             edge_dict_backwards[w].append((v, *others))
-#
-#     def next_edges_backwards(vertex: T_vertex, _: Any) -> Iterable:
-#         return edge_dict_backwards.get(vertex, ())
-#
-#     return next_edges_backwards
-
-
-# def edges_from_next_vertices_dict(
-#     next_vertices_dict: Mapping[T_vertex, tuple[T_vertex, ...]]
-# ) -> Iterator[tuple[T_vertex, T_vertex]]:
-#     """List the edges that are contained in the next_vertices_dict."""
-#     for vertex, to_vertices in next_vertices_dict.items():
-#         for to_vertex in to_vertices:
-#             yield (vertex, to_vertex)
-#
-#
-# def edges_from_next_edges_dict(
-#     edge_edges_dict: Mapping[T_vertex, tuple[tuple, ...]]
-# ) -> Iterator[tuple]:
-#     """List the edges that are contained in the next_edges_dict."""
-#     for vertex, out_edges in edge_edges_dict.items():
-#         for out_edge in out_edges:
-#             yield (vertex, *out_edge)
-
-
 # ----- Test fixtures (here: graphs and special vertices -----
 
 
 def first_of(lst: list[T]) -> T:
     """VertexToID function for test graphs that use [v] as vertices and v
     as vertex id.
     """
@@ -413,14 +362,26 @@
             lambda v: 1 if v == 0 else 0,
             report=True,
         )
         self.vertex_for_already_visited = 1
         self.values_for_known_distances = ((0, 2), (1, 0))
 
 
+class FDiamondSorted(FixtureFull[int, tuple[int, int, int]]):
+    """Diamond-shaped graph of fixed size. Variant with sorted edges (as needed by
+    TraversalShortestPathsInfBranchingSorted). No heuristic is given, since it is
+    not used for this strategy.
+    """
+
+    def __init__(self) -> None:
+        super().__init__(
+            [(0, 2, 1), (0, 1, 2), (1, 3, 2), (2, 3, 2)], 0, 3, lambda v: 0, report=True
+        )
+
+
 class FDiamond2(FixtureFull[int, tuple[int, int, int]]):
     """Diamond-shaped graph of fixed size. Variant with weight 3 from vertices 1 and
     2 to 3 (used for MST). No heuristic is given, since it is not used for A*.
     """
 
     def __init__(self) -> None:
         super().__init__(
@@ -452,29 +413,31 @@
             4,
             lambda v: 0,
             report=True,
         )
 
 
 class FSmallBinaryTree(FixtureFull[int, tuple[int, int, int]]):
-    """Graphs forming a binary tree with just 6 vertices"""
+    """Graphs forming a binary tree with just 6 vertices. Outgoing edges are sorted
+    by ascending weight."""
 
     def __init__(self) -> None:
         super().__init__(
             [(1, 2, 2), (1, 3, 3), (2, 4, 4), (2, 5, 5), (3, 6, 6), (3, 7, 7)],
             1,
             4,
             lambda v: {6: 0, 3: 3}.get(v, 11),
             report=True,
         )
 
 
 class FMultiStart(FixtureFull[int, tuple[int, int, int]]):
     """Graph for testing multiple start vertices. Used for all strategies
-    except of A* and the bidirectional search strategies."""
+    except of A* and the bidirectional search strategies. Outgoing edges
+    are sorted by ascending weight, since all weights are equal."""
 
     def __init__(self) -> None:
         super().__init__(
             [
                 (0, 1, 1),
                 (1, 2, 1),
                 (5, 6, 1),
@@ -529,31 +492,43 @@
         )
         self.start_vertices = (0, 5)
         self.goal_vertices = (4,)
         self.start_vertices_bi = (self.start_vertices, self.goal_vertices)
 
 
 class FSpiral(Fixture[int, tuple[int, int, int]]):
-    """Graph for testing TraversalShortestPathsFlex with all gears"""
+    """Graph for testing TraversalShortestPathsFlex with all gears.
+    Outgoing edges are sorted by ascending weight.
+    """
 
     @staticmethod
-    def next_edges(i: int, _: Any) -> Iterator[tuple[int, int, int]]:
+    def next_edges(i: int, _: Any) -> Iterable[tuple[int, int, int]]:
         j = (i + i // 6) % 6
         yield i + 1, j * 2 + 1, j * 2 + 1
         if i % 2 == 0:
             yield i + 6, 7 - j, 7 - j
         elif i % 1200000 > 5:
             yield i - 6, 1, 1
 
     def __init__(self) -> None:
         super().__init__(0)
         self.goal = 5
         self.focus = 2  # number of vertices at path start and end to print
 
 
+class FSpiralSorted(FSpiral):
+    """A variant of FSpiral where outgoing edges are sorted by ascending weight."""
+
+    @staticmethod
+    def next_edges(i: int, _: Any) -> Iterable[tuple[int, int, int]]:
+        out_edges = list(super(FSpiralSorted, FSpiralSorted).next_edges(i, None))
+        out_edges.sort(key=lambda e: e[1])
+        return out_edges
+
+
 class FOvertaking(FixtureFull[int, tuple[int, int, int, int]]):
     """Graph for testing all strategies with different gears. It can be used
     to create a distance overflow for distance values stored in an array of
     byte."""
 
     def __init__(self) -> None:
         _enough_for_index_error = (1 + 128) * 8  # index error even for seq of bits
@@ -634,14 +609,18 @@
     []
     >>> list(nog.TraversalTopologicalSort(f.next_vertices).start_from(f.start))
     ? 0: {'depth': 0, 'cycle_from_start': [], 'visited': {0}, 'paths': {}}
     [0]
     >>> list(nog.TraversalShortestPaths(f.next_edges).start_from(f.start))
     ? 0: {'distance': 0, 'depth': 0, 'distances': {0: 0}, 'paths': {}}
     []
+    >>> list(nog.TraversalShortestPathsInfBranchingSorted(f.next_edges).
+    ...      start_from(f.start))
+    ? 0: {'distance': 0, 'distances': {0: inf}, 'paths': {}}
+    []
     >>> list(nog.TraversalMinimumSpanningTree(f.next_edges).start_from(f.start))
     ? 0: {'edge': None, 'paths': {}}
     []
     >>> list(nog.TraversalAStar(f.next_edges).start_from(f.heuristic, f.start))
     ? 0: {'path_length': 0, 'depth': 0, 'distances': {0: 0}, 'paths': {}}
     []
     >>> d, p = nog.BSearchBreadthFirst(f.next_vertices_bi).start_from(f.start_bi)
@@ -865,14 +844,21 @@
     (0, 1)
     >>> traversal = nog.TraversalShortestPaths(next_edges=fw.next_edges)
     >>> test(traversal, fw.goal, False, fw.start)
     [1]
     True
     1
     (0, 1)
+    >>> traversal = nog.TraversalShortestPathsInfBranchingSorted(
+    ...     next_edges=fw.next_edges)
+    >>> test(traversal, fw.goal, False, fw.start)
+    [1]
+    True
+    1
+    (0, 1)
     >>> traversal = nog.TraversalMinimumSpanningTree(next_edges=fw.next_edges)
     >>> test(traversal, fw.goal, False, fw.start)
     [1]
     True
     1
     (0, 1)
     >>> traversal = nog.TraversalAStar(next_edges=fw.next_edges)
@@ -916,14 +902,20 @@
     RuntimeError: Number of visited vertices reached limit
     >>> traversal = nog.TraversalShortestPaths(next_edges=fw.next_edges)
     >>> list(traversal.start_from(fw.start, calculation_limit=2))
     [1]
     >>> _ = list(traversal.start_from(fw.start, calculation_limit=1))
     Traceback (most recent call last):
     RuntimeError: Number of visited vertices reached limit
+    >>> traversal = nog.TraversalShortestPathsInfBranchingSorted(fw.next_edges)
+    >>> list(traversal.start_from(fw.start, combined_calculation_limit=3))
+    [1]
+    >>> _ = list(traversal.start_from(fw.start, combined_calculation_limit=2))
+    Traceback (most recent call last):
+    RuntimeError: Number of visited vertices reached limit
     >>> traversal = nog.TraversalMinimumSpanningTree(next_edges=fw.next_edges)
     >>> list(traversal.start_from(fw.start, calculation_limit=2))
     [1]
     >>> _ = list(traversal.start_from(fw.start, calculation_limit=1))
     Traceback (most recent call last):
     RuntimeError: Number of visited vertices reached limit
     >>> # Test early exceeded limit, during traversal of edges from start vertex in MST
@@ -1970,14 +1962,53 @@
     ? 3: {'distance': 5, 'depth': 2, 'distances': {3: 0}, 'paths': {3: (0, 2, 3)}}
     All paths: [(0,), (0, 2), (0, 2, 3)]
     All distances: {0: 0, 1: 0, 2: 0, 3: 0}
     >>> traversal.distances is known_distances
     True
 
 
+    -- TraversalShortestPathsInfBranchingSorted --
+    First we test with option store_distances.
+    We also check here, whether distances and paths stay the same from
+    start_from till traversal.
+    Note: Distances are stored (and thus: printed) in order of reporting, whilst
+    TraversalShortestPaths results in an other order
+    >>> f = FDiamondSorted()
+    >>> traversal = nog.TraversalShortestPathsInfBranchingSorted(f.next_edges)
+    >>> traversal = traversal.start_from(f.start, build_paths=True,
+    ...     store_distances=True)
+    >>> results_with_distances(traversal, {f.start})
+    After start: {'distance': inf, 'distances': {0: 0}, 'paths': {0: (0,)}}
+    ? 0: {'distance': 0, 'distances': {0: 0}, 'paths': {0: (0,)}}
+    -> 2: {'distance': 1, 'distances': {2: 1}, 'paths': {2: (0, 2)}}
+    ? 2: {'distance': 1, 'distances': {2: 1}, 'paths': {2: (0, 2)}}
+    -> 1: {'distance': 2, 'distances': {1: 2}, 'paths': {1: (0, 1)}}
+    ? 1: {'distance': 2, 'distances': {1: 2}, 'paths': {1: (0, 1)}}
+    -> 3: {'distance': 3, 'distances': {3: 3}, 'paths': {3: (0, 2, 3)}}
+    ? 3: {'distance': 3, 'distances': {3: 3}, 'paths': {3: (0, 2, 3)}}
+    All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
+    All distances: {0: 0, 2: 1, 1: 2, 3: 3}
+
+    Now we test without option store_distances.
+    >>> f = FDiamondSorted()
+    >>> traversal = nog.TraversalShortestPathsInfBranchingSorted(f.next_edges)
+    >>> traversal = traversal.start_from(f.start, build_paths=True)
+    >>> results_with_distances(traversal, {f.start})
+    After start: {'distance': inf, 'distances': {0: inf}, 'paths': {0: (0,)}}
+    ? 0: {'distance': 0, 'distances': {0: inf}, 'paths': {0: (0,)}}
+    -> 2: {'distance': 1, 'distances': {2: inf}, 'paths': {2: (0, 2)}}
+    ? 2: {'distance': 1, 'distances': {2: inf}, 'paths': {2: (0, 2)}}
+    -> 1: {'distance': 2, 'distances': {1: inf}, 'paths': {1: (0, 1)}}
+    ? 1: {'distance': 2, 'distances': {1: inf}, 'paths': {1: (0, 1)}}
+    -> 3: {'distance': 3, 'distances': {3: inf}, 'paths': {3: (0, 2, 3)}}
+    ? 3: {'distance': 3, 'distances': {3: inf}, 'paths': {3: (0, 2, 3)}}
+    All paths: [(0,), (0, 1), (0, 2), (0, 2, 3)]
+    All distances: {0: inf, 2: inf, 1: inf, 3: inf}
+
+
     -- TraversalMinimumSpanningTree --
     >>> fmst = FDiamond2()
     >>> traversal = nog.TraversalMinimumSpanningTree(next_edges=fmst.next_edges)
     >>> traversal = traversal.start_from(fmst.start, build_paths=True)
     >>> results_standard(traversal, {fmst.start})
     After start: {'edge': None, 'paths': {0: (0,)}}
     ? 0: {'edge': None, 'paths': {0: (0,)}}
@@ -2063,16 +2094,16 @@
     ?<3: {}
     ? 1: {}
     >>> print(l, fsp.goal in p)
     90 False
 
 
 
-    All traversals, with option is_tree (except for MST and BSearchShortestPath,
-    they do not have the option):
+    All traversals, with option is_tree (except for MST, BSearchShortestPath,
+    and TraversalShortestPathsInfBranchingSorted, since they do not have the option):
     >>> fsb = FSmallBinaryTree()
     >>> traversal = nog.TraversalShortestPaths(fsb.next_edges, is_tree=True)
     >>> traversal = traversal.start_from(fsb.start, build_paths=True)
     >>> results_with_distances(traversal, {fsb.start})
     After start: {'distance': inf, 'depth': 0, 'distances': {1: 0}, 'paths': {1:
       (1,)}}
     ? 1: {'distance': 0, 'depth': 0, 'distances': {1: 0}, 'paths': {1: (1,)}}
@@ -2480,15 +2511,15 @@
     ? 5: {'depth': 0, 'visited': {0, 1, 5}, 'paths': {5: (5,)}}
     ?<2: {'depth': 1, 'visited': {2, 3, 4}, 'paths': {2: (4, 2)}}
     >>> print(l, list(p))
     3 [4, 2, 1, 0]
     """
 
 
-class MultipleStartVerticesTraversalsWithLabels:
+class MultipleStartVerticesTraversalsWithWeights:
     """-- Traversal with multiple start vertex, last 3 traversal strategies --
     Correct traversal in case of multiple start vertices. No traversal in case of no
     start vertex.
 
     >>> f = FMultiStart()
     >>> fb = FMultiStartB()
 
@@ -2515,14 +2546,39 @@
       4)}}
     All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
     All distances: {0: 0, 5: 0, 6: 0, 1: 0, 2: 0, 3: 0, 4: 0}
     >>> traversal = traversal.start_from(start_vertices=(), build_paths=True)
     >>> list(traversal)
     []
 
+    >>> traversal = nog.TraversalShortestPathsInfBranchingSorted(
+    ...     next_edges=f.next_edges)
+    >>> traversal = traversal.start_from(
+    ...     start_vertices=f.start_vertices, build_paths=True)
+    >>> results_with_distances(traversal, f.start_vertices)
+    After start: {'distance': inf, 'distances': {0: inf, 5: inf}, 'paths': {0: (0,),
+      5: (5,)}}
+    ? 5: {'distance': 0, 'distances': {5: inf}, 'paths': {5: (5,)}}
+    ? 0: {'distance': 0, 'distances': {0: inf}, 'paths': {0: (0,)}}
+    -> 1: {'distance': 1, 'distances': {1: inf}, 'paths': {1: (0, 1)}}
+    ? 1: {'distance': 1, 'distances': {1: inf}, 'paths': {1: (0, 1)}}
+    -> 6: {'distance': 1, 'distances': {6: inf}, 'paths': {6: (5, 6)}}
+    ? 6: {'distance': 1, 'distances': {6: inf}, 'paths': {6: (5, 6)}}
+    -> 3: {'distance': 2, 'distances': {3: inf}, 'paths': {3: (5, 6, 3)}}
+    ? 3: {'distance': 2, 'distances': {3: inf}, 'paths': {3: (5, 6, 3)}}
+    -> 2: {'distance': 2, 'distances': {2: inf}, 'paths': {2: (0, 1, 2)}}
+    ? 2: {'distance': 2, 'distances': {2: inf}, 'paths': {2: (0, 1, 2)}}
+    -> 4: {'distance': 3, 'distances': {4: inf}, 'paths': {4: (5, 6, 3, 4)}}
+    ? 4: {'distance': 3, 'distances': {4: inf}, 'paths': {4: (5, 6, 3, 4)}}
+    All paths: [(0,), (0, 1), (0, 1, 2), (5, 6, 3), (5, 6, 3, 4), (5,), (5, 6)]
+    All distances: {0: inf, 5: inf, 1: inf, 6: inf, 3: inf, 2: inf, 4: inf}
+    >>> traversal = traversal.start_from(start_vertices=(), build_paths=True)
+    >>> list(traversal)
+    []
+
     >>> traversal = nog.TraversalMinimumSpanningTree(
     ...     next_edges=f.next_edges)
     >>> traversal = traversal.start_from(
     ...     start_vertices=f.start_vertices, build_paths=True)
     >>> results_standard(traversal, f.start_vertices)
     After start: {'edge': None, 'paths': {0: (0,), 5: (5,)}}
     ? 0: {'edge': None, 'paths': {0: (0,)}}
@@ -2683,14 +2739,31 @@
     >>> nog.TraversalShortestPaths.go_for_vertices_in(None, None)
     Traceback (most recent call last):
     RuntimeError: Method go_for_vertices_in can only be called on a Traversal object.
     >>> nog.TraversalShortestPaths.go_for_distance_range(None, None, None)
     Traceback (most recent call last):
     RuntimeError: Method go_for_distance_range can only be called on a Traversal object.
 
+    >>> nog.TraversalShortestPathsInfBranchingSorted.start_from(None)
+    Traceback (most recent call last):
+    RuntimeError: Method start_from can only be called on a Traversal object.
+    >>> nog.TraversalShortestPathsInfBranchingSorted.__iter__(None)
+    Traceback (most recent call last):
+    RuntimeError: Method go can only be called on a Traversal object.
+    >>> nog.TraversalShortestPathsInfBranchingSorted.go_to(None, None)
+    Traceback (most recent call last):
+    RuntimeError: Method go_to can only be called on a Traversal object.
+    >>> nog.TraversalShortestPathsInfBranchingSorted.go_for_vertices_in(None, None)
+    Traceback (most recent call last):
+    RuntimeError: Method go_for_vertices_in can only be called on a Traversal object.
+    >>> nog.TraversalShortestPathsInfBranchingSorted.go_for_distance_range(
+    ...     None, None, None)
+    Traceback (most recent call last):
+    RuntimeError: Method go_for_distance_range can only be called on a Traversal object.
+
     >>> nog.TraversalAStar.start_from(None, None)
     Traceback (most recent call last):
     RuntimeError: Method start_from can only be called on a Traversal object.
     >>> nog.TraversalAStar.__iter__(None)
     Traceback (most recent call last):
     RuntimeError: Method go can only be called on a Traversal object.
     >>> nog.TraversalAStar.go_to(None, None)
@@ -2800,15 +2873,16 @@
 
 
 # --------- Tests for compatibility with different gears  -----------
 
 
 class GearTestsTraversalsWithOrWithoutLabels:
     """
-    -- TraversalShortestPathsFlex with all kinds of gears --
+    -- TraversalShortestPathsFlex and TraversalBreadthFirstFlex
+    with all kinds of gears --
 
     >>> def gear_test(gear):
     ...    f = FSpiral()
     ...    traversal = nog.TraversalShortestPathsFlex(nog.vertex_as_id,
     ...        gear, next_labeled_edges=f.next_edges)
     ...    vertex = traversal.start_from(f.start, build_paths=True).go_to(f.goal)
     ...    path = traversal.paths[vertex]
@@ -2884,17 +2958,53 @@
     [24.0, ((0, 1, 1), (1, 2, 3)), ((17, 11, 1), (11, 5, 1))]
     [5, ((0, 1, 1), (1, 2, 3)), ((3, 4, 7), (4, 5, 9))]
     >>> gear_test(nog.GearForIntVerticesAndIDsAndCInts())
     [24, ((0, 1, 1), (1, 2, 3)), ((17, 11, 1), (11, 5, 1))]
     [5, ((0, 1, 1), (1, 2, 3)), ((3, 4, 7), (4, 5, 9))]
 
 
-    Three main gear types, one also without bit_packing, used for each of the
-    traversals, graph is no tree. For traversals dealing with distances, we
-    need to test this gear functionality additionally.
+    -- TraversalShortestPathsInfBranchingSortedFlex with gears for Hashable --
+    (output of TraversalShortestPathsFlex also shown, as comparison)
+
+    >>> def gear_test(gear):
+    ...    f = FSpiralSorted()
+    ...    traversal = nog.TraversalShortestPathsFlex(nog.vertex_as_id,
+    ...        gear, next_labeled_edges=f.next_edges)
+    ...    vertex = traversal.start_from(f.start, build_paths=True).go_to(f.goal)
+    ...    path = traversal.paths.iter_vertices_from_start(vertex)
+    ...    print([traversal.distance, tuple(path)])
+    ...    traversal = nog.TraversalShortestPathsInfBranchingSortedFlex(
+    ...        gear, gear, f.next_edges)
+    ...    vertex = traversal.start_from(f.start, build_paths=True).go_to(f.goal)
+    ...    path = traversal.paths[vertex]
+    ...    print([traversal.distance, tuple(path)])
+    ...    # print([traversal.distance, tuple(path[:f.focus]), tuple(path[-f.focus:])])
+
+    >>> gear_test(nog.GearForHashableVertexIDs(0, float("infinity")))
+    [24, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    [24, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    >>> gear_test(nog.GearDefault())
+    [24, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    [24, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    >>> gear_test(nog.GearForHashableVertexIDsAndIntsMaybeFloats())
+    [24, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    [24, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    >>> gear_test(nog.GearForHashableVertexIDsAndDecimals())
+    [Decimal('24'), (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    [Decimal('24'), (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    >>> gear_test(nog.GearForHashableVertexIDsAndFloats())
+    [24.0, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+    [24.0, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5)]
+
+
+    -- Three main gear types, one also without bit_packing, used for each of the
+    traversals, graph is no tree. --
+
+    For traversals dealing with distances, we need to test this gear functionality
+    additionally.
 
     >>> f = FOvertaking()
     >>> test_gears = [nog.GearForHashableVertexIDsAndIntsMaybeFloats(),
     ...               nog.GearForIntVertexIDsAndCFloats(),
     ...               nog.GearForIntVerticesAndIDsAndCFloats(),
     ...               nog.GearForIntVerticesAndIDsAndCFloats(no_bit_packing=True),
     ...              ]
```

### Comparing `nographs-3.2.0/tests/test_types.py` & `nographs-3.3.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `nographs-3.2.0/tests/test_unit_typed.py` & `nographs-3.3.0/tests/test_unit_typed.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,24 +7,27 @@
     from typing import assert_type
 import unittest
 
 from mpmath import mp, mpf  # type: ignore
 
 import nographs as nog
 
+# noinspection PyProtectedMember
+from nographs._extra_tsp import GettableProto
+
 
 # --- Types ---
 
 T_any_typical_weight_type = TypeVar("T_any_typical_weight_type", float, Decimal, mpf)
 
 
 # --- Tests ---
 
 
-class Test1(unittest.TestCase):
+class TestWithTypes(unittest.TestCase):
     def test_variable_edge_weights(self) -> None:
         def test_with_small_weights(
             zero: T_any_typical_weight_type,
             one_half: T_any_typical_weight_type,
             one: T_any_typical_weight_type,
         ) -> int:
             def next_edges(
@@ -56,15 +59,15 @@
         self.assertEquals(
             test_with_small_weights(Decimal(0), Decimal("0.5"), Decimal(1)), 65
         )
 
         mp.prec = 64
         self.assertEquals(test_with_small_weights(mpf(0), mpf("0.5"), mpf(1)), 65)
 
-    def test_typing_docs_example(self) -> None:
+    def test_traversal_typing_docs_example(self) -> None:
         def next_edges(i: int, _: Any) -> Iterator[tuple[int, int]]:
             j = (i + i // 6) % 6
             yield i + 1, j * 2 + 1
             if i % 2 == 0:
                 yield i + 6, 7 - j
             elif i % 1200000 > 5:
                 yield i - 6, 1
@@ -85,7 +88,16 @@
             if TYPE_CHECKING:
                 reveal_type(v)  # reveals: int
                 reveal_type(d)  # reveals: Union[int, float]
                 reveal_type(p)  # reveals: tuple[int, ...]
         self.assertEquals(v, 5)
         self.assertEquals(d, 24)
         self.assertEquals(p, (0, 1, 2, 3, 4, 10, 16, 17, 11, 5))
+
+    def test_tsp_typing_docs_example(self) -> None:
+        """The MyPy run will detect if the typing goes wrong here.
+
+        The NOQA tells flake8 that it is on purpose that g1 and g2 are
+        assigned but never used.
+        """
+        g1: GettableProto[int, str] = dict[int, str]([(0, "a"), (1, "b")])  # NOQA F841
+        g2: GettableProto[int, str] = ["a", "b"]  # NOQA F841
```

