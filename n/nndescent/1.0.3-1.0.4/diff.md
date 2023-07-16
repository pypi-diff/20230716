# Comparing `tmp/nndescent-1.0.3.tar.gz` & `tmp/nndescent-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nndescent-1.0.3.tar", last modified: Fri Jul  7 19:13:06 2023, max compression
+gzip compressed data, was "nndescent-1.0.4.tar", last modified: Sun Jul 16 15:57:18 2023, max compression
```

## Comparing `nndescent-1.0.3.tar` & `nndescent-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-07 19:13:06.405541 nndescent-1.0.3/
--rw-r--r--   0 dr_b      (1000) dr_b      (1000)     1300 2023-06-01 12:23:37.000000 nndescent-1.0.3/LICENSE
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      236 2023-07-07 19:07:46.000000 nndescent-1.0.3/MANIFEST.in
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7825 2023-07-07 19:13:06.405541 nndescent-1.0.3/PKG-INFO
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7075 2023-07-07 19:07:46.000000 nndescent-1.0.3/README.md
-drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-07 19:13:06.401541 nndescent-1.0.3/nndescent.egg-info/
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7825 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/PKG-INFO
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      387 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/SOURCES.txt
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)        1 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/dependency_links.txt
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       64 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/requires.txt
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       10 2023-07-07 19:13:06.000000 nndescent-1.0.3/nndescent.egg-info/top_level.txt
-drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-07 19:13:06.401541 nndescent-1.0.3/pybindings/
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    12951 2023-07-07 19:07:46.000000 nndescent-1.0.3/pybindings/pybind11ings.cpp
--rw-r--r--   0 dr_b      (1000) dr_b      (1000)      148 2023-05-27 21:21:15.000000 nndescent-1.0.3/pyproject.toml
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       38 2023-07-07 19:13:06.405541 nndescent-1.0.3/setup.cfg
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     2347 2023-07-07 19:07:46.000000 nndescent-1.0.3/setup.py
-drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-07 19:13:06.405541 nndescent-1.0.3/src/
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      138 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/distances.cpp
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    84644 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/distances.h
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     1812 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/dtypes.cpp
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    32723 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/dtypes.h
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    27254 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/nnd.cpp
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    27219 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/nnd.h
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    17734 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/rp_trees.cpp
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    18575 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/rp_trees.h
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     1871 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/utils.cpp
--rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     5890 2023-07-07 19:07:46.000000 nndescent-1.0.3/src/utils.h
+drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-16 15:57:18.401958 nndescent-1.0.4/
+-rw-r--r--   0 dr_b      (1000) dr_b      (1000)     1300 2023-06-01 12:23:37.000000 nndescent-1.0.4/LICENSE
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      236 2023-07-07 19:07:46.000000 nndescent-1.0.4/MANIFEST.in
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7825 2023-07-16 15:57:18.401958 nndescent-1.0.4/PKG-INFO
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7075 2023-07-07 19:07:46.000000 nndescent-1.0.4/README.md
+drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-16 15:57:18.397958 nndescent-1.0.4/nndescent.egg-info/
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     7825 2023-07-16 15:57:18.000000 nndescent-1.0.4/nndescent.egg-info/PKG-INFO
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      387 2023-07-16 15:57:18.000000 nndescent-1.0.4/nndescent.egg-info/SOURCES.txt
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)        1 2023-07-16 15:57:18.000000 nndescent-1.0.4/nndescent.egg-info/dependency_links.txt
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       64 2023-07-16 15:57:18.000000 nndescent-1.0.4/nndescent.egg-info/requires.txt
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       10 2023-07-16 15:57:18.000000 nndescent-1.0.4/nndescent.egg-info/top_level.txt
+drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-16 15:57:18.397958 nndescent-1.0.4/pybindings/
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    12951 2023-07-07 19:07:46.000000 nndescent-1.0.4/pybindings/pybind11ings.cpp
+-rw-r--r--   0 dr_b      (1000) dr_b      (1000)      148 2023-05-27 21:21:15.000000 nndescent-1.0.4/pyproject.toml
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)       38 2023-07-16 15:57:18.401958 nndescent-1.0.4/setup.cfg
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     2358 2023-07-15 13:03:40.000000 nndescent-1.0.4/setup.py
+drwxrwxr-x   0 dr_b      (1000) dr_b      (1000)        0 2023-07-16 15:57:18.401958 nndescent-1.0.4/src/
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)      138 2023-07-07 19:07:46.000000 nndescent-1.0.4/src/distances.cpp
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    84644 2023-07-16 10:22:46.000000 nndescent-1.0.4/src/distances.h
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     1824 2023-07-16 09:48:30.000000 nndescent-1.0.4/src/dtypes.cpp
+-rw-r--r--   0 dr_b      (1000) dr_b      (1000)    34538 2023-07-16 10:36:36.000000 nndescent-1.0.4/src/dtypes.h
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    27274 2023-07-16 15:25:37.000000 nndescent-1.0.4/src/nnd.cpp
+-rw-r--r--   0 dr_b      (1000) dr_b      (1000)    27335 2023-07-16 14:53:55.000000 nndescent-1.0.4/src/nnd.h
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)    17764 2023-07-16 10:00:41.000000 nndescent-1.0.4/src/rp_trees.cpp
+-rw-r--r--   0 dr_b      (1000) dr_b      (1000)    18623 2023-07-16 10:03:03.000000 nndescent-1.0.4/src/rp_trees.h
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     1871 2023-07-07 19:07:46.000000 nndescent-1.0.4/src/utils.cpp
+-rw-rw-r--   0 dr_b      (1000) dr_b      (1000)     5890 2023-07-07 19:07:46.000000 nndescent-1.0.4/src/utils.h
```

### Comparing `nndescent-1.0.3/LICENSE` & `nndescent-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.3/PKG-INFO` & `nndescent-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nndescent
-Version: 1.0.3
+Version: 1.0.4
 Summary: C++ extension implementing nearest neighbour descent
 Home-page: https://github.com/brj0/nndescent
 Author: Jon Brugger
 License: BSD 2-Clause License
 Keywords: nearest neighbor,knn,ANN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nndescent-1.0.3/README.md` & `nndescent-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.3/nndescent.egg-info/PKG-INFO` & `nndescent-1.0.4/nndescent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nndescent
-Version: 1.0.3
+Version: 1.0.4
 Summary: C++ extension implementing nearest neighbour descent
 Home-page: https://github.com/brj0/nndescent
 Author: Jon Brugger
 License: BSD 2-Clause License
 Keywords: nearest neighbor,knn,ANN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nndescent-1.0.3/pybindings/pybind11ings.cpp` & `nndescent-1.0.4/pybindings/pybind11ings.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.3/setup.py` & `nndescent-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 else:
     compile_args = [
         "-DALL_METRICS",
         "-Ofast",
         "-flto",
         "-fno-math-errno",
         "-fopenmp",
-        "-g",
         "-march=native",
+        "-mtune=native",
     ]
 
 module = Extension(
     name="nndescent",
     sources=glob.glob("pybindings/*.cpp") + glob.glob("src/*.cpp"),
     include_dirs=include_dirs,
     extra_compile_args=compile_args,
```

### Comparing `nndescent-1.0.3/src/distances.h` & `nndescent-1.0.4/src/distances.h`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.3/src/dtypes.cpp` & `nndescent-1.0.4/src/dtypes.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -53,25 +53,25 @@
     {
         std::string row(map[i].begin(), map[i].end());
         std::cout << row;
     }
 }
 
 
-std::ostream& operator<<(std::ostream &out, NNUpdate &update)
+std::ostream& operator<<(std::ostream &out, const NNUpdate &update)
 {
     out << "(idx0=" << update.idx0
         << ", idx1=" << update.idx1
         << ", key=" << update.key
         << ")";
     return out;
 }
 
 
-std::ostream& operator<<(std::ostream &out, std::vector<NNUpdate> &updates)
+std::ostream& operator<<(std::ostream &out, const std::vector<NNUpdate> &updates)
 {
     out << "[";
     for (size_t i = 0; i < updates.size(); ++i)
     {
         if (i > 0)
         {
             out << " ";
```

### Comparing `nndescent-1.0.3/src/dtypes.h` & `nndescent-1.0.4/src/dtypes.h`

 * *Files 2% similar despite different names*

```diff
@@ -1009,14 +1009,26 @@
      * @param key The key associated with the node.
      *
      * @return 1 if the node was added to the heap, 0 otherwise.
      */
     int checked_push(size_t i, int idx, KeyType key);
 
     /*
+     * Pushes a node with the specified index and key into the specified heap
+     * if its key is smaller.
+     *
+     * @param i The index of the heap.
+     * @param idx The index of the node.
+     * @param key The key associated with the node.
+     *
+     * @return 1 if the node was added to the heap, 0 otherwise.
+     */
+    int simple_push(size_t i, int idx, KeyType key);
+
+    /*
      * Performs a "siftdown" operation on the specified heap starting from the
      * given index.
      *
      * The "siftdown" operation descends the top node down the heap by swapping
      * values until the maximum heap criterion is met or 'stop' is reached.
      *
      * @param i The index of the heap to perform the siftdown operation on.
@@ -1276,14 +1288,83 @@
     keys(i, current) = key;
 
     return 1;
 }
 
 
 template <class KeyType>
+int HeapList<KeyType>::simple_push(size_t i, int idx, KeyType key)
+{
+    if (key >= keys(i, 0))
+    {
+        return 0;
+    }
+
+    // Siftdown: Descend the heap, swapping values until the max heap
+    // criterion is met.
+    size_t current = 0;
+    size_t swap;
+
+    while (true)
+    {
+        size_t left_child = 2*current + 1;
+        size_t right_child = left_child + 1;
+
+        if (left_child >= n_nodes)
+        {
+            break;
+        }
+        else if (right_child >= n_nodes)
+        {
+            if (keys(i, left_child) > key)
+            {
+                swap = left_child;
+            }
+            else
+            {
+                break;
+            }
+        }
+        else if (keys(i, left_child) >= keys(i, right_child))
+        {
+            if (keys(i, left_child) > key)
+            {
+                swap = left_child;
+            }
+            else
+            {
+                break;
+            }
+        }
+        else
+        {
+            if (keys(i, right_child) > key)
+            {
+                swap = right_child;
+            }
+            else
+            {
+                break;
+            }
+        }
+        indices(i, current) = indices(i, swap);
+        keys(i, current) = keys(i, swap);
+
+        current = swap;
+    }
+
+    // Insert node at current position.
+    indices(i, current) = idx;
+    keys(i, current) = key;
+
+    return 1;
+}
+
+
+template <class KeyType>
 size_t HeapList<KeyType>::size(size_t i) const
 {
     size_t count = count_if_not_equal(indices.begin(i), indices.end(i), NONE);
     return count;
 }
 
 
@@ -1405,17 +1486,17 @@
     float key;
 } NNUpdate;
 
 
 /*
  * @brief Prints a NNUpdate object to an output stream.
  */
-std::ostream& operator<<(std::ostream &out, NNUpdate &update);
+std::ostream& operator<<(std::ostream &out, const NNUpdate &update);
 
 
 /*
  * @brief Prints a vector of NNUpdate objects to an output stream.
  */
-std::ostream& operator<<(std::ostream &out, std::vector<NNUpdate> &updates);
+std::ostream& operator<<(std::ostream &out, const std::vector<NNUpdate> &updates);
 
 
 } // namespace nndescent
```

### Comparing `nndescent-1.0.3/src/nnd.cpp` & `nndescent-1.0.4/src/nnd.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 
     // Generate leaf updates
     #pragma omp parallel for
     for (int thread = 0; thread < n_threads; ++thread)
     {
         int block_start  = thread * block_size;
         int block_end = (thread + 1) * block_size;
-        block_end = (thread == n_threads) ? n_leaves : block_end;
+        block_end = (thread == n_threads - 1) ? n_leaves : block_end;
 
         for (int i = block_start; i < block_end; ++i)
         {
             for (int j = 0; j < leaf_size; ++j)
             {
                 int idx0 = leaf_array(i, j);
                 if (idx0 == NONE)
@@ -182,15 +182,15 @@
  * @param rng_state The random state used for randomization.
  * @param n_threads The number of threads to use for parallelization.
  */
 void sample_candidates(
     HeapList<float> &current_graph,
     HeapList<int> &new_candidates,
     HeapList<int> &old_candidates,
-    RandomState rng_state,
+    const RandomState &rng_state,
     int n_threads
 )
 {
     #pragma omp parallel for
     for (int thread = 0; thread < n_threads; ++thread)
     {
         RandomState local_rng_state;
@@ -359,15 +359,15 @@
  * potential graph updates.
  * @param n_threads The number of threads to use for parallelization.
  *
  * @return The number of updates applied to the graph.
  */
 int apply_graph_updates(
     HeapList<float> &current_graph,
-    std::vector<std::vector<NNUpdate>> &updates,
+    const std::vector<std::vector<NNUpdate>> &updates,
     int n_threads
 )
 {
     int n_changes = 0;
 
     #pragma omp parallel for
     for (int thread = 0; thread < n_threads; ++thread)
@@ -821,40 +821,42 @@
             "Forward graph pruning reduced edges from "
                 + std::to_string(edges_cnt_before)
                 + " to "
                 + std::to_string(edges_cnt_after)
         );
     }
 
-    size_t n_seach_cols = std::round(n_neighbors * pruning_degree_multiplier);
-    search_graph = HeapList<float>(data_size, n_seach_cols, FLOAT_MAX);
+    size_t n_search_cols = std::round(n_neighbors * pruning_degree_multiplier);
+    search_graph = HeapList<float>(data_size, n_search_cols, FLOAT_MAX);
 
     for (size_t i = 0; i < forward_graph.nheaps(); ++i)
     {
         for (size_t j = 0; j < forward_graph.nnodes(); ++j)
         {
             int idx = forward_graph.indices(i, j);
             if (idx != NONE)
             {
                 float d = forward_graph.keys(i, j);
                 search_graph.checked_push(i, idx, d);
                 search_graph.checked_push(idx, i, d);
             }
         }
     }
+
     search_graph.heapsort();
 
     if (verbose)
     {
         log(
             "Merging pruned graph with its transpose results in "
                 + std::to_string(search_graph.indices.non_none_cnt())
                 + " edges for the search graph."
         );
     }
+
 }
 
 
 template<class MatrixType, class DistType>
 void NNDescent::start_brute_force(
     const MatrixType &train_data, const DistType &dist
 )
@@ -863,15 +865,15 @@
     #pragma omp parallel for num_threads(n_threads)
     for (size_t idx0 = 0; idx0 < train_data.nrows(); ++idx0)
     {
         bar.show();
         for (size_t idx1 = 0; idx1 < train_data.nrows(); ++idx1)
         {
             float d = dist(train_data, idx0, idx1);
-            current_graph.checked_push(idx0, idx1, d);
+            current_graph.simple_push(idx0, idx1, d);
         }
     }
     current_graph.heapsort();
     neighbor_indices = current_graph.indices;
     correct_distances(
         dist, current_graph.keys, neighbor_distances
     );
```

### Comparing `nndescent-1.0.3/src/nnd.h` & `nndescent-1.0.4/src/nnd.h`

 * *Files 1% similar despite different names*

```diff
@@ -50,17 +50,17 @@
 
 
 namespace nndescent
 {
 
 
 /**
- * @version 1.0.3
+ * @version 1.0.4
  */
-const std::string PROJECT_VERSION = "1.0.3";
+const std::string PROJECT_VERSION = "1.0.4";
 
 
 // Constants
 const char OLD = '0';
 const char NEW = '1';
 const int MAX_INT = std::numeric_limits<int>::max();
 const int DEFAULT_K = 10;
@@ -556,15 +556,15 @@
     #pragma omp parallel for num_threads(n_threads)
     for (size_t idx_q = 0; idx_q < query_data.nrows(); ++idx_q)
     {
         bar.show();
         for (size_t idx_t = 0; idx_t < data_size; ++idx_t)
         {
             float d = dist(train_data, idx_t, query_data, idx_q);
-            query_nn.checked_push(idx_q, idx_t, d);
+            query_nn.simple_push(idx_q, idx_t, d);
         }
     }
     query_nn.heapsort();
     query_indices = query_nn.indices;
     query_distances = query_nn.keys;
     correct_distances(
         dist, query_distances, query_distances
@@ -826,84 +826,89 @@
     }
     // Check if search_graph already prepared.
     if (search_graph.nheaps() == 0)
     {
         prepare(dist);
     }
     HeapList<float> query_nn(_query_data.nrows(), k, FLOAT_MAX);
+    #pragma omp parallel for num_threads(n_threads)
     for (size_t i = 0; i < query_nn.nheaps(); ++i)
     {
 
         // Initialization
         Heap<Candidate> search_candidates;
-        std::vector<int> visited(data_size, 0);
+        std::vector<bool> visited(data_size, 0);
         std::vector<int> initial_candidates = search_tree.get_leaf(
             _query_data, i, rng_state
         );
 
         for (auto const &idx : initial_candidates)
         {
             float d = dist(train_data, idx, _query_data, i);
             // Don't need to check as indices are guaranteed to be different.
-            // TODO implement push without check.
-            query_nn.checked_push(i, idx, d);
-            visited[idx] = 1;
+            query_nn.simple_push(i, idx, d);
             search_candidates.push({idx, d});
+            visited[idx] = 1;
         }
         int n_random_samples = k - initial_candidates.size();
         for (int j = 0; j < n_random_samples; ++j)
         {
             int idx = rand_int(rng_state) % data_size;
             if (!visited[idx])
             {
                 float d = dist(train_data, idx, _query_data, i);
-                query_nn.checked_push(i, idx, d);
-                visited[idx] = 1;
+                query_nn.simple_push(i, idx, d);
                 search_candidates.push({idx, d});
+                visited[idx] = 1;
             }
         }
 
         // Search
         Candidate candidate = search_candidates.pop();
         float distance_bound = (1.0f + epsilon) * query_nn.max(i);
         while (candidate.key < distance_bound)
         {
-            for (size_t j = 0; j < search_graph.nnodes(); ++j)
+            for (
+                auto it = search_graph.indices.begin(candidate.idx);
+                it != search_graph.indices.end(candidate.idx);
+                ++it
+            )
             {
-                int idx = search_graph.indices(candidate.idx, j);
+                int idx = *it;
                 if (idx == NONE)
                 {
                     break;
                 }
                 if (visited[idx])
                 {
                     continue;
                 }
                 visited[idx] = 1;
                 float d = dist(train_data, idx, _query_data, i);
                 if (d < distance_bound)
                 {
-                    query_nn.checked_push(i, idx, d);
+                    query_nn.simple_push(i, idx, d);
                     search_candidates.push({idx, d});
-
                     // Update bound
                     distance_bound = (1.0f + epsilon) * query_nn.max(i);
                 }
             }
-            // Find new nearest candidate point.
+            // The next candidate is the nearest among the search_candidates.
             if (search_candidates.empty())
             {
                 break;
             }
             else
             {
                 candidate = search_candidates.pop();
             }
         }
+
     }
+
     query_nn.heapsort();
     query_indices = query_nn.indices;
     query_distances = query_nn.keys;
     correct_distances(
         dist, query_distances, query_distances
     );
 }
```

### Comparing `nndescent-1.0.3/src/rp_trees.cpp` & `nndescent-1.0.4/src/rp_trees.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 {
 
 
 template<>
 std::tuple<std::vector<int>, std::vector<int>, std::vector<float>, float>
 random_projection_split<EuclideanSplit>(
     const Matrix<float> &data,
-    std::vector<int> &indices,
+    const std::vector<int> &indices,
     RandomState &rng_state
 )
 {
     size_t dim = data.ncols();
     size_t size = indices.size();
 
     size_t rand0 = rand_int(rng_state) % size;
@@ -132,15 +132,15 @@
 }
 
 
 template<>
 std::tuple<std::vector<int>, std::vector<int>, std::vector<float>, float>
 random_projection_split<AngularSplit>(
     const Matrix<float> &data,
-    std::vector<int> &indices,
+    const std::vector<int> &indices,
     RandomState &rng_state
 )
 {
     size_t dim = data.ncols();
     size_t size = indices.size();
 
     size_t rand0 = rand_int(rng_state) % size;
@@ -291,15 +291,15 @@
     std::vector<int>,
     std::vector<size_t>,
     std::vector<float>,
     float
 >
 sparse_random_projection_split<EuclideanSplit>(
     const CSRMatrix<float> &data,
-    std::vector<int> &indices,
+    const std::vector<int> &indices,
     RandomState &rng_state
 )
 {
     size_t size = indices.size();
 
     size_t rand0 = rand_int(rng_state) % size;
     size_t rand1 = rand_int(rng_state) % size;
@@ -439,15 +439,15 @@
     std::vector<int>,
     std::vector<size_t>,
     std::vector<float>,
     float
 >
 sparse_random_projection_split<AngularSplit>(
     const CSRMatrix<float> &data,
-    std::vector<int> &indices,
+    const std::vector<int> &indices,
     RandomState &rng_state
 )
 {
     size_t size = indices.size();
 
     size_t rand0 = rand_int(rng_state) % size;
     size_t rand1 = rand_int(rng_state) % size;
@@ -612,15 +612,15 @@
         hyperplane_data,
         0.0f
     );
 }
 
 
 Matrix<int> get_leaves_from_forest(
-    std::vector<RPTree> &forest
+    const std::vector<RPTree> &forest
 )
 {
     size_t leaf_size = forest[0].leaf_size;
     size_t n_leaves = 0;
     for (const auto& tree : forest)
     {
         n_leaves += tree.n_leaves;
```

### Comparing `nndescent-1.0.3/src/rp_trees.h` & `nndescent-1.0.4/src/rp_trees.h`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         float *query_data,
         RandomState &rng_state
     ) const
     {
         size_t index = get_index();
         while (nodes[index].left != NONE)
         {
-            std::vector<float> hyperplane_vector = nodes[index].hyperplane;
+            const std::vector<float> &hyperplane_vector = nodes[index].hyperplane;
             float hyperplane_offset = nodes[index].offset;
 
             float margin = std::inner_product(
                 hyperplane_vector.begin(),
                 hyperplane_vector.end(),
                 query_data,
                 -hyperplane_offset
@@ -302,31 +302,31 @@
     /*
      * @brief Add an internal node to the tree, containing no indices.
      */
     void add_node(
         size_t left_subtree,
         size_t right_subtree,
         float offset,
-        std::vector<float> &hyperplane
+        const std::vector<float> &hyperplane
     )
     {
         RPTNode node(left_subtree, right_subtree, offset, hyperplane, {});
         nodes.push_back(node);
     }
 
     /*
      * @brief Add an internal node to the tree, containing no indices (sparse
      * case).
      */
     void add_node(
         size_t left_subtree,
         size_t right_subtree,
         float offset,
-        std::vector<size_t> &hyperplane_ind,
-        std::vector<float> &hyperplane
+        const std::vector<size_t> &hyperplane_ind,
+        const std::vector<float> &hyperplane
     )
     {
         RPTNode node(
             left_subtree,
             right_subtree,
             offset,
             hyperplane_ind,
@@ -405,15 +405,15 @@
  * @return A tuple containing the left child indices, right child indices,
  * hyperplane normal vector, and hyperplane offset.
  */
 template<class SplitType>
 std::tuple<std::vector<int>, std::vector<int>, std::vector<float>, float>
 random_projection_split(
     const Matrix<float> &data,
-    std::vector<int> &indices,
+    const std::vector<int> &indices,
     RandomState &rng_state
 );
 
 
 /*
  * @brief Performs a random projection tree split (sparse version).
  *
@@ -439,15 +439,15 @@
     std::vector<int>,
     std::vector<size_t>,
     std::vector<float>,
     float
 >
 sparse_random_projection_split(
     const CSRMatrix<float> &data,
-    std::vector<int> &indices,
+    const std::vector<int> &indices,
     RandomState &rng_state
 );
 
 
 /*
  * @brief Builds a random projection tree by recursively splitting.
  *
@@ -672,15 +672,15 @@
  * @return The constructed forest of random projection trees.
  */
 template<class MatrixType>
 std::vector<RPTree> make_forest(
     const MatrixType &data,
     int n_trees,
     int leaf_size,
-    RandomState &rng_state
+    const RandomState &rng_state
 )
 {
     std::vector<RPTree> forest(n_trees);
     #pragma omp parallel for
     for (int i = 0; i < n_trees; ++i)
     {
         RandomState local_rng_state;
@@ -704,15 +704,15 @@
  * 'n_leaves' x 'leaf_size'. If a leaf has fewer than 'leaf_size' elements, the
  * remaining elements in the row are filled with the special value 'NONE'.
  *
  * @param forest The random projection tree forest.
  *
  * @return A matrix containing the extracted leaves.
  */
-Matrix<int> get_leaves_from_forest( std::vector<RPTree> &forest);
+Matrix<int> get_leaves_from_forest(const std::vector<RPTree> &forest);
 
 
 /*
  * @brief Prints a RPTNode object to an output stream.
  */
 std::ostream& operator<<(std::ostream &out, const RPTNode &node);
```

### Comparing `nndescent-1.0.3/src/utils.cpp` & `nndescent-1.0.4/src/utils.cpp`

 * *Files identical despite different names*

### Comparing `nndescent-1.0.3/src/utils.h` & `nndescent-1.0.4/src/utils.h`

 * *Files identical despite different names*

