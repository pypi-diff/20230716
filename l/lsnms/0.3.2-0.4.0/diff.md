# Comparing `tmp/lsnms-0.3.2.tar.gz` & `tmp/lsnms-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsnms-0.3.2.tar", max compression
+gzip compressed data, was "lsnms-0.4.0.tar", max compression
```

## Comparing `lsnms-0.3.2.tar` & `lsnms-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0    10940 2023-01-21 16:35:25.460010 lsnms-0.3.2/README.md
--rw-r--r--   0        0        0       80 2023-01-21 16:35:25.460263 lsnms-0.3.2/lsnms/__init__.py
--rw-r--r--   0        0        0     7135 2023-01-21 16:44:56.566500 lsnms-0.3.2/lsnms/nms.py
--rw-r--r--   0        0        0    10147 2023-01-21 16:53:09.608295 lsnms-0.3.2/lsnms/rtree.py
--rw-r--r--   0        0        0    13403 2023-01-21 16:35:25.460758 lsnms-0.3.2/lsnms/util.py
--rw-r--r--   0        0        0     6255 2023-01-21 16:35:25.460909 lsnms-0.3.2/lsnms/wbc.py
--rw-r--r--   0        0        0      820 2023-01-21 16:43:58.713082 lsnms-0.3.2/pyproject.toml
--rw-r--r--   0        0        0    11765 1970-01-01 00:00:00.000000 lsnms-0.3.2/setup.py
--rw-r--r--   0        0        0    11777 1970-01-01 00:00:00.000000 lsnms-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0    10940 2023-07-16 16:25:36.000000 lsnms-0.4.0/README.md
+-rw-r--r--   0        0        0       80 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/__init__.py
+-rw-r--r--   0        0        0     7135 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/nms.py
+-rw-r--r--   0        0        0    10147 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/rtree.py
+-rw-r--r--   0        0        0    13403 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/util.py
+-rw-r--r--   0        0        0     6255 2023-07-16 16:25:36.000000 lsnms-0.4.0/lsnms/wbc.py
+-rw-r--r--   0        0        0      814 2023-07-16 16:53:36.000000 lsnms-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11738 1970-01-01 00:00:00.000000 lsnms-0.4.0/PKG-INFO
```

### Comparing `lsnms-0.3.2/README.md` & `lsnms-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `lsnms-0.3.2/lsnms/nms.py` & `lsnms-0.4.0/lsnms/nms.py`

 * *Files identical despite different names*

### Comparing `lsnms-0.3.2/lsnms/rtree.py` & `lsnms-0.4.0/lsnms/rtree.py`

 * *Files identical despite different names*

### Comparing `lsnms-0.3.2/lsnms/util.py` & `lsnms-0.4.0/lsnms/util.py`

 * *Files identical despite different names*

### Comparing `lsnms-0.3.2/lsnms/wbc.py` & `lsnms-0.4.0/lsnms/wbc.py`

 * *Files identical despite different names*

### Comparing `lsnms-0.3.2/pyproject.toml` & `lsnms-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "lsnms"
-version = "0.3.2"
+version = "0.4.0"
 description = "Large Scale Non Maximum Suppression"
 authors = ["Rémy Dubois <remydubois14@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/remydubois/lsnms"
 keywords = ["NMS", "Non Maximum Suppression", "Histology image", "Satellite images", "Object detection"]
 classifiers=["Programming Language :: Python :: 3", "Topic :: Scientific/Engineering"]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<3.10"
-numpy = "1.20.0"
-numba = "0.54.1"
+python = ">=3.8,<3.11"
+numpy = "1.24.0"
+numba = "^0.57.1"
 
-[tool.poetry.dev-dependencies]
-pytest = "6.2.5"
-tox = "3.24.4"
-torch = "1.10.2"
-torchvision = "0.11.3"
-pillow = "9.3.0"
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+pillow = "^10.0.0"
+torch = "2.0.0"
+torchvision = "0.15.1"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 profile = "black"
```

### Comparing `lsnms-0.3.2/setup.py` & `lsnms-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,176 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: lsnms
+Version: 0.4.0
+Summary: Large Scale Non Maximum Suppression
+Home-page: https://github.com/remydubois/lsnms
+License: MIT
+Keywords: NMS,Non Maximum Suppression,Histology image,Satellite images,Object detection
+Author: Rémy Dubois
+Author-email: remydubois14@gmail.com
+Requires-Python: >=3.8,<3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering
+Requires-Dist: numba (>=0.57.1,<0.58.0)
+Requires-Dist: numpy (==1.24.0)
+Project-URL: Repository, https://github.com/remydubois/lsnms
+Description-Content-Type: text/markdown
+
+# LSNMS
+Speeding up Non Maximum Suppression with a multiclass support ran on very large images by a several folds factor, using a sparse implementation of NMS.
+This project becomes useful in the case of very high dimensional images data, when the amount of predicted instances to prune becomes considerable (> 10,000 objects).
+
+<p float="center">
+  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/simple_rtree_timings.png" width="700" />
+  <figcaption>Run times (on a virtual image of 10kx10k pixels)</figcaption></center>
+</p>
+
+
+## Installation
+This project is fully installable with pip:
+```
+pip install lsnms --upgrade
+```
+or by cloning this repo with poetry
+```
+git clone https://github.com/remydubois/lsnms
+cd lsnms/
+poetry install
+```
+Only dependencies are numpy and numba.
+
+## Example usage:
+```python
+import numpy as np
+from lsnms import nms, wbc
+
+# Create boxes: approx 30 pixels wide / high in Pascal VOC format:
+# bbox = (x0, y0, x1, y1) with x1 > x0, y1 > y0
+image_size = 10_000
+n_predictions = 10_000
+topleft = np.random.uniform(0.0, high=image_size, size=(n_predictions, 2))
+wh = np.random.uniform(15, 45, size=topleft.shape)
+boxes = np.concatenate([topleft, topleft + wh], axis=1).astype(np.float64)
+# Create scores
+scores = np.random.uniform(0., 1., size=(len(boxes), ))
+
+# Create class_ids if multiclass, 3 classes here
+class_ids = np.random.randint(0, 2, size=(len(boxes), ))
+
+# Apply NMS
+# During the process, overlapping boxes are queried using a R-Tree, ensuring a log-time search
+keep = nms(boxes, scores, iou_threshold=0.5)
+# Or, in a multiclass setting
+keep = nms(boxes, scores, iou_threshold=0.5, class_ids=class_ids)
+boxes = boxes[keep]
+scores = scores[keep]
+
+# Apply WBC
+pooled_boxes, pooled_scores, cluster_indices = wbc(boxes, scores, iou_threshold=0.5)
+```
+# Description
+## Non Maximum Suppression
+<!-- Non maximum suppression is an essential step of object detection tasks, aiming at pruning away multiple predictions actually predicting the same instance. This algorithm works greedily by sorting in decreasing order predicted boxes, and step by step, pruning away boxes having an high intersection over union with any other box with higher confidence score (it deletes all the non maximally-scored overlapping boxes). Picture below depicts the overall process: in the left image, several bounding boxes actuually predict the same instance (the model's face). In the right image, NMS was applied to prune away redundant boxes and keep only the highest scoring box.
+Note: confidence score are not represented on this image.
+<p float="center">
+  <center><img src="./assets/images/nms_fast_03.jpeg" width="700" />
+  <figcaption>NMS example (source https://www.pyimagesearch.com/2015/02/16/faster-non-maximum-suppression-python/)</figcaption></center>
+</p> -->
+A nice introduction of the non maximum suppression algorithm can be found here: https://www.coursera.org/lecture/convolutional-neural-networks/non-max-suppression-dvrjH.
+Basically, NMS discards redundant boxes in a set of predicted instances. It is an essential - and often unavoidable, step of object detection pipelines.
+
+
+## Scaling up the Non Maximum Suppression process
+### Complexity
+* In the best case scenario, NMS is a **linear-complex** process (`O(n)`): if all boxes are perfectly overlapping, then one pass of the algorithm discards all the boxes except the highest scoring one.
+* In worst case scenario, NMS is a **quadratic-complex** operation (one needs to perform `n * (n - 1) / 2 ` iou comparisons): if all boxes are perfectly disconnected, each NMS step will discard only one box (the highest scoring one, by decreasing order of score).  Hence, one needs to perform `(n-1) + (n-2) + ... + 1 = n * (n - 1) / 2 ` iou computations.
+### Working with huge images
+When working with high-dimensional images (such as satellital or histology images), one often runs object detection inference by patching (with overlap) the input image and applying NMS to independant patches. Because patches do overlap, a final NMS needs to be re-applied afterward.
+In that final case, one is close to be in the worst case scenario since each NMS step will discard only a very low amount of candidate instances (actually, pretty much the amount of overlapping passes over each instance, usually <= 10). Hence, depending on the size of the input image, computation time can reach several minutes on CPU.
+A more natural way to speed up NMS could be through parallelization, like it is done for GPU-based implementations, but:
+1. Efficiently parallelizing NMS is not a straightforward process
+2. If too many instances are predicted, GPU VRAM will often not be sufficient, retaining one from using GPU accelerators
+3. The process remains quadratic, and does not scale well.
+### LSNMS
+This project offers a way to overcome the aforementioned issues elegantly:
+1. Before the NMS process, a R-Tree is built on bounding boxes (in a `O(n*log(n))` time)
+2. At each NMS step, only boxes overlapping with the current highest scoring box are queried in the tree (in a `O(log(n))` complexity time), and only those neighbors are considered in the pruning process: IoU computation + pruning if necessary. Hence, the overall NMS process is turned from a `O(n**2)` into a `O(n * log(n))` process. See a comparison of run times on the graph below (results obtained on sets of instances whose coordinates vary between 0 and 10,000 (x and y)).
+A nice introduction of R-Tree can be found here: https://iq.opengenus.org/r-tree/.
+
+Note that the timing reported below are all inclusive: it notably includes the tree building process, otherwise comparison would not be fair.
+
+<p float="center">
+  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/simple_rtree_timings.png" width="700" />
+  <figcaption>Run times (on a virtual image of 10kx10k pixels)</figcaption></center>
+</p>
+
+
+For the sake of speed, this repo is entirely (including the binary tree) built using Numba's just-in-time compilation.
+
+>Concrete example:
+>Some tests were ran considering ~ 40k x 40k pixels images, and detection inference ran on 512 x 512 overlapping patches (256-strided). Aproximately 300,000 bounding boxes (post patchwise NMS) resulted. Naive NMS ran in approximately 5 minutes on modern CPU, while this implementation ran in 5 seconds, hence offering a close to 60 folds speed up.
+
+### Going further: weighted box clustering
+For the sake of completeness, this repo also implements a variant of the Weighted Box Clustering algorithm (from https://arxiv.org/pdf/1811.08661.pdf). Since NMS can artificially push up confidence scores (by selecting only the highest scoring box per instance), WBC overcomes this by averaging box coordinates and scores of all the overlapping boxes (instead of discarding all the non-maximally scored overlaping boxes).
+
+## Disclaimer:
+1. The tree implementation could probably be further optimized, see implementation notes below.
+2. Much simpler implementation could rely on existing KD-Tree implementations (such as sklearn's), query the tree before NMS, and tweak the NMS process to accept tree query's result. This repo implements it from scratch in full numba for the sake of completeness and elegance.
+3. The main parameter deciding the speed up brought by this method is (along with the amount of instances) the **density** of boxes over the image: in other words, the amount of overlapping boxes trimmed at each step of the NMS process. The lower the density of boxes, the higher the speed up factor.
+4. Due to numba's compiling process, the first call to each jitted function might lag a bit, second and further function calls (per python session) should not suffer this overhead.
+
+-> Will I benefit from this sparse NMS implementation ?
+As said above, the main parameter guiding speed up from naive NMS is instance (or boxes) **density** (rather than image size or amount of instances):
+- If a million boxes overlap perfectly on a 100k x 100k pixels image, no speed up will be obersved (even a slow down, related to tree building time)
+- If 1,000 boxes are far appart from each other on a small image, the optimal speed up will be observed (with a good choice of neighborhood radius query)
+
+---
+# Implementations notes
+## Tree implementation
+Due to Numba compiler's limitations, tree implementations has some specificities:
+Because jit-class methods can not be recursive, the tree building process (node splitting + children instanciation) can not be entirely done inside the `Node.__init__` method:
+* Otherwise, the `__init__` method would be recursive (children instanciation)
+* However, methods can call recursive (instance-external) functions: a `build` function is dedicated to this
+* Hence the tree building process must be as follows:
+```python
+# instanciate root
+root = Node(data, leaf_size=16)
+# recursively split and attach children if necessary
+root.build()  # This calls build(root) under the hood
+```
+* For convenience: a wrapper class `RTree` was implemented, encapsulating the above steps in `__init__`:
+```python
+tree = RTree(data, leaf_size=16)
+```
+## Multiclass support
+For multiclass support, a peculiar method to offset bounding boxes was used (offseting bounding boxes class-wise is the standard way to apply NMS class-wise).
+Note that the standard way to offset bboxes is to create a "diagonal per block" aspect, with each class' bboxes being positioned along a virtual diagonal.
+
+Note that this would hurt performances because the underlying RTree that we would build on this would be suboptimal: many regions would actually be empty (because RTree builds rectangular
+regions) and the query time would be impacted.
+
+Instead, here the boxes are offseted forming a "mosaic" of class-wise regions, see figure below.
+<p float="center">
+  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/multiclass_offset.png" width="700" />
+  <figcaption>Illustration of the bbox offsetting process for multiclass support</figcaption></center>
+</p>
+
+## Performances
+The RTree implemented in this repo was timed against scikit-learn's `neighbors` one. Note that runtimes are not fair to compare since sklearn implementation allows for node to contain
+between `leaf_size` and `2 * leaf_size` datapoints. To account for this, I timed my implementation against sklearn tree with `int(0.67 * leaf_size)`  as `leaf_size`.
+### Tree building time
+<p float="center">
+  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/tree_building_times.png" width="700" />
+  <figcaption>Trees building times comparison</figcaption></center>
+</p>
+
+
+### Tree query time
+<p float="center">
+  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/naive_vs_rtree_query.png" width="700" />
+  <figcaption>Trees query times comparison (single query) in a 1000x1000 space</figcaption></center>
+</p>
 
-packages = \
-['lsnms']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numba==0.54.1', 'numpy==1.20.0']
-
-setup_kwargs = {
-    'name': 'lsnms',
-    'version': '0.3.2',
-    'description': 'Large Scale Non Maximum Suppression',
-    'long_description': '# LSNMS\nSpeeding up Non Maximum Suppression with a multiclass support ran on very large images by a several folds factor, using a sparse implementation of NMS.\nThis project becomes useful in the case of very high dimensional images data, when the amount of predicted instances to prune becomes considerable (> 10,000 objects).\n\n<p float="center">\n  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/simple_rtree_timings.png" width="700" />\n  <figcaption>Run times (on a virtual image of 10kx10k pixels)</figcaption></center>\n</p>\n\n\n## Installation\nThis project is fully installable with pip:\n```\npip install lsnms --upgrade\n```\nor by cloning this repo with poetry\n```\ngit clone https://github.com/remydubois/lsnms\ncd lsnms/\npoetry install\n```\nOnly dependencies are numpy and numba.\n\n## Example usage:\n```python\nimport numpy as np\nfrom lsnms import nms, wbc\n\n# Create boxes: approx 30 pixels wide / high in Pascal VOC format:\n# bbox = (x0, y0, x1, y1) with x1 > x0, y1 > y0\nimage_size = 10_000\nn_predictions = 10_000\ntopleft = np.random.uniform(0.0, high=image_size, size=(n_predictions, 2))\nwh = np.random.uniform(15, 45, size=topleft.shape)\nboxes = np.concatenate([topleft, topleft + wh], axis=1).astype(np.float64)\n# Create scores\nscores = np.random.uniform(0., 1., size=(len(boxes), ))\n\n# Create class_ids if multiclass, 3 classes here\nclass_ids = np.random.randint(0, 2, size=(len(boxes), ))\n\n# Apply NMS\n# During the process, overlapping boxes are queried using a R-Tree, ensuring a log-time search\nkeep = nms(boxes, scores, iou_threshold=0.5)\n# Or, in a multiclass setting\nkeep = nms(boxes, scores, iou_threshold=0.5, class_ids=class_ids)\nboxes = boxes[keep]\nscores = scores[keep]\n\n# Apply WBC\npooled_boxes, pooled_scores, cluster_indices = wbc(boxes, scores, iou_threshold=0.5)\n```\n# Description\n## Non Maximum Suppression\n<!-- Non maximum suppression is an essential step of object detection tasks, aiming at pruning away multiple predictions actually predicting the same instance. This algorithm works greedily by sorting in decreasing order predicted boxes, and step by step, pruning away boxes having an high intersection over union with any other box with higher confidence score (it deletes all the non maximally-scored overlapping boxes). Picture below depicts the overall process: in the left image, several bounding boxes actuually predict the same instance (the model\'s face). In the right image, NMS was applied to prune away redundant boxes and keep only the highest scoring box.\nNote: confidence score are not represented on this image.\n<p float="center">\n  <center><img src="./assets/images/nms_fast_03.jpeg" width="700" />\n  <figcaption>NMS example (source https://www.pyimagesearch.com/2015/02/16/faster-non-maximum-suppression-python/)</figcaption></center>\n</p> -->\nA nice introduction of the non maximum suppression algorithm can be found here: https://www.coursera.org/lecture/convolutional-neural-networks/non-max-suppression-dvrjH.\nBasically, NMS discards redundant boxes in a set of predicted instances. It is an essential - and often unavoidable, step of object detection pipelines.\n\n\n## Scaling up the Non Maximum Suppression process\n### Complexity\n* In the best case scenario, NMS is a **linear-complex** process (`O(n)`): if all boxes are perfectly overlapping, then one pass of the algorithm discards all the boxes except the highest scoring one.\n* In worst case scenario, NMS is a **quadratic-complex** operation (one needs to perform `n * (n - 1) / 2 ` iou comparisons): if all boxes are perfectly disconnected, each NMS step will discard only one box (the highest scoring one, by decreasing order of score).  Hence, one needs to perform `(n-1) + (n-2) + ... + 1 = n * (n - 1) / 2 ` iou computations.\n### Working with huge images\nWhen working with high-dimensional images (such as satellital or histology images), one often runs object detection inference by patching (with overlap) the input image and applying NMS to independant patches. Because patches do overlap, a final NMS needs to be re-applied afterward.\nIn that final case, one is close to be in the worst case scenario since each NMS step will discard only a very low amount of candidate instances (actually, pretty much the amount of overlapping passes over each instance, usually <= 10). Hence, depending on the size of the input image, computation time can reach several minutes on CPU.\nA more natural way to speed up NMS could be through parallelization, like it is done for GPU-based implementations, but:\n1. Efficiently parallelizing NMS is not a straightforward process\n2. If too many instances are predicted, GPU VRAM will often not be sufficient, retaining one from using GPU accelerators\n3. The process remains quadratic, and does not scale well.\n### LSNMS\nThis project offers a way to overcome the aforementioned issues elegantly:\n1. Before the NMS process, a R-Tree is built on bounding boxes (in a `O(n*log(n))` time)\n2. At each NMS step, only boxes overlapping with the current highest scoring box are queried in the tree (in a `O(log(n))` complexity time), and only those neighbors are considered in the pruning process: IoU computation + pruning if necessary. Hence, the overall NMS process is turned from a `O(n**2)` into a `O(n * log(n))` process. See a comparison of run times on the graph below (results obtained on sets of instances whose coordinates vary between 0 and 10,000 (x and y)).\nA nice introduction of R-Tree can be found here: https://iq.opengenus.org/r-tree/.\n\nNote that the timing reported below are all inclusive: it notably includes the tree building process, otherwise comparison would not be fair.\n\n<p float="center">\n  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/simple_rtree_timings.png" width="700" />\n  <figcaption>Run times (on a virtual image of 10kx10k pixels)</figcaption></center>\n</p>\n\n\nFor the sake of speed, this repo is entirely (including the binary tree) built using Numba\'s just-in-time compilation.\n\n>Concrete example:\n>Some tests were ran considering ~ 40k x 40k pixels images, and detection inference ran on 512 x 512 overlapping patches (256-strided). Aproximately 300,000 bounding boxes (post patchwise NMS) resulted. Naive NMS ran in approximately 5 minutes on modern CPU, while this implementation ran in 5 seconds, hence offering a close to 60 folds speed up.\n\n### Going further: weighted box clustering\nFor the sake of completeness, this repo also implements a variant of the Weighted Box Clustering algorithm (from https://arxiv.org/pdf/1811.08661.pdf). Since NMS can artificially push up confidence scores (by selecting only the highest scoring box per instance), WBC overcomes this by averaging box coordinates and scores of all the overlapping boxes (instead of discarding all the non-maximally scored overlaping boxes).\n\n## Disclaimer:\n1. The tree implementation could probably be further optimized, see implementation notes below.\n2. Much simpler implementation could rely on existing KD-Tree implementations (such as sklearn\'s), query the tree before NMS, and tweak the NMS process to accept tree query\'s result. This repo implements it from scratch in full numba for the sake of completeness and elegance.\n3. The main parameter deciding the speed up brought by this method is (along with the amount of instances) the **density** of boxes over the image: in other words, the amount of overlapping boxes trimmed at each step of the NMS process. The lower the density of boxes, the higher the speed up factor.\n4. Due to numba\'s compiling process, the first call to each jitted function might lag a bit, second and further function calls (per python session) should not suffer this overhead.\n\n-> Will I benefit from this sparse NMS implementation ?\nAs said above, the main parameter guiding speed up from naive NMS is instance (or boxes) **density** (rather than image size or amount of instances):\n- If a million boxes overlap perfectly on a 100k x 100k pixels image, no speed up will be obersved (even a slow down, related to tree building time)\n- If 1,000 boxes are far appart from each other on a small image, the optimal speed up will be observed (with a good choice of neighborhood radius query)\n\n---\n# Implementations notes\n## Tree implementation\nDue to Numba compiler\'s limitations, tree implementations has some specificities:\nBecause jit-class methods can not be recursive, the tree building process (node splitting + children instanciation) can not be entirely done inside the `Node.__init__` method:\n* Otherwise, the `__init__` method would be recursive (children instanciation)\n* However, methods can call recursive (instance-external) functions: a `build` function is dedicated to this\n* Hence the tree building process must be as follows:\n```python\n# instanciate root\nroot = Node(data, leaf_size=16)\n# recursively split and attach children if necessary\nroot.build()  # This calls build(root) under the hood\n```\n* For convenience: a wrapper class `RTree` was implemented, encapsulating the above steps in `__init__`:\n```python\ntree = RTree(data, leaf_size=16)\n```\n## Multiclass support\nFor multiclass support, a peculiar method to offset bounding boxes was used (offseting bounding boxes class-wise is the standard way to apply NMS class-wise).\nNote that the standard way to offset bboxes is to create a "diagonal per block" aspect, with each class\' bboxes being positioned along a virtual diagonal.\n\nNote that this would hurt performances because the underlying RTree that we would build on this would be suboptimal: many regions would actually be empty (because RTree builds rectangular\nregions) and the query time would be impacted.\n\nInstead, here the boxes are offseted forming a "mosaic" of class-wise regions, see figure below.\n<p float="center">\n  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/multiclass_offset.png" width="700" />\n  <figcaption>Illustration of the bbox offsetting process for multiclass support</figcaption></center>\n</p>\n\n## Performances\nThe RTree implemented in this repo was timed against scikit-learn\'s `neighbors` one. Note that runtimes are not fair to compare since sklearn implementation allows for node to contain\nbetween `leaf_size` and `2 * leaf_size` datapoints. To account for this, I timed my implementation against sklearn tree with `int(0.67 * leaf_size)`  as `leaf_size`.\n### Tree building time\n<p float="center">\n  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/tree_building_times.png" width="700" />\n  <figcaption>Trees building times comparison</figcaption></center>\n</p>\n\n\n### Tree query time\n<p float="center">\n  <center><img src="https://raw.githubusercontent.com/remydubois/lsnms/main/assets/images/naive_vs_rtree_query.png" width="700" />\n  <figcaption>Trees query times comparison (single query) in a 1000x1000 space</figcaption></center>\n</p>\n',
-    'author': 'Rémy Dubois',
-    'author_email': 'remydubois14@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/remydubois/lsnms',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.10',
-}
-
-
-setup(**setup_kwargs)
```

