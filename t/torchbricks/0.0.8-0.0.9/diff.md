# Comparing `tmp/torchbricks-0.0.8.tar.gz` & `tmp/torchbricks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbricks-0.0.8.tar", last modified: Wed Jul 12 14:10:32 2023, max compression
+gzip compressed data, was "torchbricks-0.0.9.tar", last modified: Sat Jul 15 22:55:55 2023, max compression
```

## Comparing `torchbricks-0.0.8.tar` & `torchbricks-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.308501 torchbricks-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-12 14:10:13.000000 torchbricks-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-12 14:10:13.000000 torchbricks-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-07-12 14:10:32.308501 torchbricks-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-07-12 14:10:13.000000 torchbricks-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-12 14:10:13.000000 torchbricks-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 14:10:32.308501 torchbricks-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.304501 torchbricks-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.308501 torchbricks-0.0.8/src/torchbricks/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/bag_of_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/brick_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/bricks_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 14:10:13.000000 torchbricks-0.0.8/src/torchbricks/custom_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.308501 torchbricks-0.0.8/src/torchbricks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21039 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-12 14:10:32.000000 torchbricks-0.0.8/src/torchbricks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 14:10:32.308501 torchbricks-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-12 14:10:13.000000 torchbricks-0.0.8/tests/test_bag_of_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-12 14:10:13.000000 torchbricks-0.0.8/tests/test_brick_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10691 2023-07-12 14:10:13.000000 torchbricks-0.0.8/tests/test_bricks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-12 14:10:13.000000 torchbricks-0.0.8/tests/test_bricks_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:55.670523 torchbricks-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-15 22:55:35.000000 torchbricks-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-15 22:55:35.000000 torchbricks-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25271 2023-07-15 22:55:55.670523 torchbricks-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23481 2023-07-15 22:55:35.000000 torchbricks-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-15 22:55:35.000000 torchbricks-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 22:55:55.670523 torchbricks-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:55.666522 torchbricks-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:55.670523 torchbricks-0.0.9/src/torchbricks/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 22:55:35.000000 torchbricks-0.0.9/src/torchbricks/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 22:55:35.000000 torchbricks-0.0.9/src/torchbricks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-15 22:55:35.000000 torchbricks-0.0.9/src/torchbricks/bag_of_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-15 22:55:35.000000 torchbricks-0.0.9/src/torchbricks/brick_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13864 2023-07-15 22:55:35.000000 torchbricks-0.0.9/src/torchbricks/bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-07-15 22:55:35.000000 torchbricks-0.0.9/src/torchbricks/bricks_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-15 22:55:35.000000 torchbricks-0.0.9/src/torchbricks/custom_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:55.670523 torchbricks-0.0.9/src/torchbricks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25271 2023-07-15 22:55:55.000000 torchbricks-0.0.9/src/torchbricks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-15 22:55:55.000000 torchbricks-0.0.9/src/torchbricks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:55:55.000000 torchbricks-0.0.9/src/torchbricks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-15 22:55:55.000000 torchbricks-0.0.9/src/torchbricks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 22:55:55.000000 torchbricks-0.0.9/src/torchbricks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:55:55.670523 torchbricks-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-15 22:55:35.000000 torchbricks-0.0.9/tests/test_bag_of_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-15 22:55:35.000000 torchbricks-0.0.9/tests/test_brick_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14366 2023-07-15 22:55:35.000000 torchbricks-0.0.9/tests/test_bricks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-15 22:55:35.000000 torchbricks-0.0.9/tests/test_bricks_helper.py
```

### Comparing `torchbricks-0.0.8/LICENSE` & `torchbricks-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.8/PKG-INFO` & `torchbricks-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchbricks
-Version: 0.0.8
+Version: 0.0.9
 Summary: Decoupled and modular approach to building multi-task ML models
 Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Peter Christiansen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -103,37 +103,43 @@
 from torchbricks.bricks import Stage
 
 bricks = {
     'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'], output_names=['processed']),
     'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['processed'], output_names=['embedding']),
     'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=['embedding'], output_names=['logits', "softmaxed"]),
 }
+brick_collection = BrickCollection(bricks)
+print(brick_collection)
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+# )
 ```
 
-All modules are added as entries in a regular dictionary and for each module, we provide a name (dictionary key) and 
-input and output names. The number of input and output names should match the actually number of input and outputs 
-for each function. 
-
-Each module is wrapped inside a brick - here either `BrickTrainable` and `BrickNotTrainable`.
+All modules are added as entries in a regular dictionary and for each module, we wrap it inside a brick (here either `BrickTrainable` and 
+`BrickNotTrainable`), provide a name (dictionary key) and input and output names. The number of input and output names should match the 
+actually number of input and outputs for each function. 
 
-The `bricks`-dictionary describe how data is passed between bricks: The `preprocessor` uses a `raw` input tensor and passes the
+Input and output names specify how tensors move between bricks: The `preprocessor` uses a `raw` input tensor and passes the
 `processed` tensor to the `backbone`. The backbone returns the `embedding` tensor and passes it to the `head` determining 
 both `logits` and `softmaxed` tensors. 
 
-Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
-returns a dictionary with both intermediated and resulting tensors. 
+Bricks are passed to a `BrickCollection` for executing them as showed in below:
 
 ```python
-brick_collection = BrickCollection(bricks)
 batch_size=2
 batch_images = torch.rand((batch_size, 3, 100, 200))
 named_outputs = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
-print(named_outputs.keys())
+print("Brick outputs:", named_outputs.keys())
+# Brick outputs: dict_keys(['raw', 'stage', 'processed', 'embedding', 'logits', 'softmaxed'])
 ```
 
+The brick collection accepts a dictionary and returns a dictionary with both intermediated and resulting tensors. 
+
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
   to a specific device/precision, you can save/load a model, management of parameters, onnx exportable etc. 
 - A brick collection is also a simple DAG, it accepts a dictionary (`named_inputs`), 
 executes each bricks and ensures that the outputs are passed to the inputs of other bricks with matching names. 
 Structuring the model as a DAG, makes it easy to add/remove outputs for a given module during development, add new modules to the
@@ -165,14 +171,22 @@
                                alive_stages="all"),
     'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), input_names=['embedding'], 
                            output_names=['logits', 'softmaxed'], alive_stages="all"),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'], 
                       alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST], loss_output_names="all")
 }
 brick_collection = BrickCollection(bricks)
+
+print(brick_collection)
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], alive_stages=['TRAIN', 'VALIDATION', 'TEST'])
+# )
 ```
 
 We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
 similar to before. 
 
 For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to calculate loss during train, validation and test
 stages. 
@@ -298,15 +312,15 @@
                       brick_collection=brick_collection, 
                       named_inputs=named_inputs, 
                       dynamic_batch_size=True, 
                       stage=Stage.EXPORT)
 ```
 
 ### Brick features: Act as a nn.Module
-A brick collection acts as a 'nn.Module' mean we can do the following: 
+A brick collection acts as a 'nn.Module' meaning:
 
 ```python
 # Move to specify device (CPU/GPU) or precision to automatically move model parameters
 brick_collection_half = brick_collection.to(torch.float16)
 
 
 # Save model parameters
@@ -314,20 +328,63 @@
 torch.save(brick_collection_half.state_dict(), path_model)
 
 # Load model parameters
 brick_collection_half.load_state_dict(torch.load(path_model))
 
 # Access parameters
 brick_collection_half.named_parameters()
+
+# Using compile with pytorch >= 2.0
+torch.compile(brick_collection)
 ```
 
+### Brick features: Act as a dictionary (nn.ModuleDict)
+
 
 
+```python
+from typing import Dict
+
+from torchbricks.bricks import BrickInterface
 
 
+def image_classifier_head(num_classes: int, in_channels: int) -> Dict[str, BrickInterface]:
+    """Image classifier bricks: Classifier, loss and metrics """
+    head = {
+        'classify': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=in_channels),
+                                   input_names=['features'], output_names=['./logits', './probabilities', './class_prediction']),
+        'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=['./class_prediction', 'targets']),
+        'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['./logits', 'targets'], output_names=['./loss_ce'])
+    }
+    return head
+
+
+bricks = {
+    'preprocessor': BrickNotTrainable(Preprocessor(), input_names=['raw'], output_names=['normalized']),
+    'backbone': resnet_brick,
+    'head0': image_classifier_head(num_classes=3, in_channels=resnet_brick.model.n_backbone_features),
+    'head1': image_classifier_head(num_classes=5, in_channels=resnet_brick.model.n_backbone_features),
+}
+print(BrickCollection(bricks))
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(Preprocessor, input_names=['raw'], output_names=['normalized'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(BackboneResnet, input_names=['normalized'], output_names=['features'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head0): BrickCollection(
+#     (classify): BrickTrainable(ImageClassifier, input_names=['features'], output_names=['head0/logits', 'head0/probabilities', 'head0/class_prediction'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#     (accuracy): BrickMetricSingle(['MulticlassAccuracy'], input_names=['head0/class_prediction', 'targets'], output_names=[], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#     (loss): BrickLoss(CrossEntropyLoss, input_names=['head0/logits', 'targets'], output_names=['head0/loss_ce'], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#   )
+#   (head1): BrickCollection(
+#     (classify): BrickTrainable(ImageClassifier, input_names=['features'], output_names=['head1/logits', 'head1/probabilities', 'head1/class_prediction'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#     (accuracy): BrickMetricSingle(['MulticlassAccuracy'], input_names=['head1/class_prediction', 'targets'], output_names=[], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#     (loss): BrickLoss(CrossEntropyLoss, input_names=['head1/logits', 'targets'], output_names=['head1/loss_ce'], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#   )
+# )
+```
+
 ### Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick 
 (without a classifier).
 
 
@@ -418,14 +475,16 @@
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
 - [x] Fix the release process. It should be as simple as running `make release`.
 - [x] Add onnx export example to the README.md
+- [ ] Pretty print bricks
+- [ ] Relative input/output names
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
```

### Comparing `torchbricks-0.0.8/README.md` & `torchbricks-0.0.9/src/torchbricks.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,43 @@
+Metadata-Version: 2.1
+Name: torchbricks
+Version: 0.0.9
+Summary: Decoupled and modular approach to building multi-task ML models
+Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2023 Peter Christiansen
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/PeteHeine/torchbricks
+Keywords: torch,multi-task,machine learning
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <!--
 
 ---
 jupyter:
   jupytext:
     hide_notebook_metadata: true
     text_representation:
@@ -67,37 +103,43 @@
 from torchbricks.bricks import Stage
 
 bricks = {
     'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'], output_names=['processed']),
     'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['processed'], output_names=['embedding']),
     'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=['embedding'], output_names=['logits', "softmaxed"]),
 }
+brick_collection = BrickCollection(bricks)
+print(brick_collection)
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+# )
 ```
 
-All modules are added as entries in a regular dictionary and for each module, we provide a name (dictionary key) and 
-input and output names. The number of input and output names should match the actually number of input and outputs 
-for each function. 
-
-Each module is wrapped inside a brick - here either `BrickTrainable` and `BrickNotTrainable`.
+All modules are added as entries in a regular dictionary and for each module, we wrap it inside a brick (here either `BrickTrainable` and 
+`BrickNotTrainable`), provide a name (dictionary key) and input and output names. The number of input and output names should match the 
+actually number of input and outputs for each function. 
 
-The `bricks`-dictionary describe how data is passed between bricks: The `preprocessor` uses a `raw` input tensor and passes the
+Input and output names specify how tensors move between bricks: The `preprocessor` uses a `raw` input tensor and passes the
 `processed` tensor to the `backbone`. The backbone returns the `embedding` tensor and passes it to the `head` determining 
 both `logits` and `softmaxed` tensors. 
 
-Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
-returns a dictionary with both intermediated and resulting tensors. 
+Bricks are passed to a `BrickCollection` for executing them as showed in below:
 
 ```python
-brick_collection = BrickCollection(bricks)
 batch_size=2
 batch_images = torch.rand((batch_size, 3, 100, 200))
 named_outputs = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
-print(named_outputs.keys())
+print("Brick outputs:", named_outputs.keys())
+# Brick outputs: dict_keys(['raw', 'stage', 'processed', 'embedding', 'logits', 'softmaxed'])
 ```
 
+The brick collection accepts a dictionary and returns a dictionary with both intermediated and resulting tensors. 
+
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
   to a specific device/precision, you can save/load a model, management of parameters, onnx exportable etc. 
 - A brick collection is also a simple DAG, it accepts a dictionary (`named_inputs`), 
 executes each bricks and ensures that the outputs are passed to the inputs of other bricks with matching names. 
 Structuring the model as a DAG, makes it easy to add/remove outputs for a given module during development, add new modules to the
@@ -129,14 +171,22 @@
                                alive_stages="all"),
     'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), input_names=['embedding'], 
                            output_names=['logits', 'softmaxed'], alive_stages="all"),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'], 
                       alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST], loss_output_names="all")
 }
 brick_collection = BrickCollection(bricks)
+
+print(brick_collection)
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], alive_stages=['TRAIN', 'VALIDATION', 'TEST'])
+# )
 ```
 
 We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
 similar to before. 
 
 For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to calculate loss during train, validation and test
 stages. 
@@ -262,15 +312,15 @@
                       brick_collection=brick_collection, 
                       named_inputs=named_inputs, 
                       dynamic_batch_size=True, 
                       stage=Stage.EXPORT)
 ```
 
 ### Brick features: Act as a nn.Module
-A brick collection acts as a 'nn.Module' mean we can do the following: 
+A brick collection acts as a 'nn.Module' meaning:
 
 ```python
 # Move to specify device (CPU/GPU) or precision to automatically move model parameters
 brick_collection_half = brick_collection.to(torch.float16)
 
 
 # Save model parameters
@@ -278,20 +328,63 @@
 torch.save(brick_collection_half.state_dict(), path_model)
 
 # Load model parameters
 brick_collection_half.load_state_dict(torch.load(path_model))
 
 # Access parameters
 brick_collection_half.named_parameters()
+
+# Using compile with pytorch >= 2.0
+torch.compile(brick_collection)
 ```
 
+### Brick features: Act as a dictionary (nn.ModuleDict)
+
+
+
+```python
+from typing import Dict
+
+from torchbricks.bricks import BrickInterface
 
 
+def image_classifier_head(num_classes: int, in_channels: int) -> Dict[str, BrickInterface]:
+    """Image classifier bricks: Classifier, loss and metrics """
+    head = {
+        'classify': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=in_channels),
+                                   input_names=['features'], output_names=['./logits', './probabilities', './class_prediction']),
+        'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=['./class_prediction', 'targets']),
+        'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['./logits', 'targets'], output_names=['./loss_ce'])
+    }
+    return head
 
 
+bricks = {
+    'preprocessor': BrickNotTrainable(Preprocessor(), input_names=['raw'], output_names=['normalized']),
+    'backbone': resnet_brick,
+    'head0': image_classifier_head(num_classes=3, in_channels=resnet_brick.model.n_backbone_features),
+    'head1': image_classifier_head(num_classes=5, in_channels=resnet_brick.model.n_backbone_features),
+}
+print(BrickCollection(bricks))
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(Preprocessor, input_names=['raw'], output_names=['normalized'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(BackboneResnet, input_names=['normalized'], output_names=['features'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head0): BrickCollection(
+#     (classify): BrickTrainable(ImageClassifier, input_names=['features'], output_names=['head0/logits', 'head0/probabilities', 'head0/class_prediction'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#     (accuracy): BrickMetricSingle(['MulticlassAccuracy'], input_names=['head0/class_prediction', 'targets'], output_names=[], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#     (loss): BrickLoss(CrossEntropyLoss, input_names=['head0/logits', 'targets'], output_names=['head0/loss_ce'], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#   )
+#   (head1): BrickCollection(
+#     (classify): BrickTrainable(ImageClassifier, input_names=['features'], output_names=['head1/logits', 'head1/probabilities', 'head1/class_prediction'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#     (accuracy): BrickMetricSingle(['MulticlassAccuracy'], input_names=['head1/class_prediction', 'targets'], output_names=[], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#     (loss): BrickLoss(CrossEntropyLoss, input_names=['head1/logits', 'targets'], output_names=['head1/loss_ce'], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#   )
+# )
+```
+
 ### Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick 
 (without a classifier).
 
 
@@ -382,14 +475,16 @@
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
 - [x] Fix the release process. It should be as simple as running `make release`.
 - [x] Add onnx export example to the README.md
+- [ ] Pretty print bricks
+- [ ] Relative input/output names
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
```

### Comparing `torchbricks-0.0.8/pyproject.toml` & `torchbricks-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [tool.ruff]
 line-length = 140
 select = ["C4", "E", "F","B", "I", "W", "RUF"]
 
 [project]
 name = "torchbricks"
-version = "0.0.8"
+version = "0.0.9"
 description = "Decoupled and modular approach to building multi-task ML models"
 readme = "README.md"
 authors = [{ name = "Peter Hviid Christianse", email = "PeterHviidChristiansen@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -27,15 +27,15 @@
 requires-python = ">=3.7"
 
 [project.urls]
 Homepage = "https://github.com/PeteHeine/torchbricks"
 
 # bumpver update --patch | --minor | --major --dry
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]  # Specify all files containging version-numbers
```

### Comparing `torchbricks-0.0.8/src/torchbricks/bag_of_bricks.py` & `torchbricks-0.0.9/src/torchbricks/bag_of_bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.8/src/torchbricks/brick_utils.py` & `torchbricks-0.0.9/src/torchbricks/brick_utils.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.8/src/torchbricks/bricks.py` & `torchbricks-0.0.9/src/torchbricks/bricks.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from abc import ABC, abstractmethod
 from enum import Enum
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Union
 
 from torch import nn
 from torchmetrics import Metric, MetricCollection
 from typeguard import typechecked
 
 from torchbricks.bricks_helper import named_input_and_outputs_callable
 
 
-class Stage(Enum):              # Gradients   Eval-model    Targets
-    TRAIN = 'train'             # Y                   Y             Y
-    VALIDATION = 'validation'   # N                   N             Y
-    TEST = 'test'               # N                   N             Y
-    INFERENCE = 'inference'     # N                   N             N
-    EXPORT = 'export'           # N                   N             N
+class Stage(Enum):
+    TRAIN = 'train'
+    VALIDATION = 'validation'
+    TEST = 'test'
+    INFERENCE = 'inference'
+    EXPORT = 'export'
 
 
 class BrickInterface(ABC):
     def __init__(self,
                  input_names: Union[List[str], Dict[str, str], str],
                  output_names: List[str],
-                 alive_stages: Union[List[Stage], str] = 'all',
+                 alive_stages: Union[List[Stage], str],
+                 wrapped_module_name: str,
                  ) -> None:
         super().__init__()
         if isinstance(input_names, str):
             if input_names != 'all':
                 raise ValueError('')
         self.input_names = input_names
         self.output_names = output_names
         self.alive_stages: List[Stage] = parse_argument_alive_stages(alive_stages)
+        self.wrapped_module_name = wrapped_module_name
 
     def run_now(self, stage: Stage) -> bool:
         return stage in self.alive_stages
 
     @abstractmethod
     def forward(self, named_inputs: Dict[str, Any], stage: Stage) -> Dict[str, Any]:
         """"""
@@ -42,14 +45,21 @@
     def extract_losses(self, named_outputs: Dict[str, Any]) -> Dict[str, Any]:
         """"""
 
     @abstractmethod
     def summarize(self, stage: Stage, reset: bool) -> Dict[str, Any]:
         """"""
 
+    def __repr__(self) -> str:
+        input_names = self.input_names
+        output_names = self.output_names
+        alive_stages = [phase.name for phase in self.alive_stages]
+        return f'{self.__class__.__name__}({self.wrapped_module_name}, {input_names=}, {output_names=}, {alive_stages=})'
+
+
 
 @typechecked
 def parse_argument_alive_stages(alive_stages: Union[List[Stage], str]) -> List[Stage]:
     available_stages = list(Stage)
     if alive_stages == 'all':
         alive_stages = available_stages
     elif alive_stages == 'none':
@@ -78,15 +88,19 @@
                  input_names: Union[List[str], Dict[str, str], str],
                  output_names: List[str],
                  alive_stages: Union[List[Stage], str] = 'all',
                  loss_output_names: Union[List[str], str] = 'none',
                  calculate_gradients: bool = True,
                  trainable: bool = True) -> None:
         nn.Module.__init__(self)
-        BrickInterface.__init__(self, input_names=input_names, output_names=output_names, alive_stages=alive_stages)
+        BrickInterface.__init__(self,
+                                input_names=input_names,
+                                output_names=output_names,
+                                alive_stages=alive_stages,
+                                wrapped_module_name=model.__class__.__name__)
         self.model = model
         self.loss_output_names = parse_argument_loss_output_names(loss_output_names, available_output_names=output_names)
 
         if calculate_gradients:
             self.calculate_gradients_on = [Stage.TRAIN]
         else:
             self.calculate_gradients_on = []
@@ -109,20 +123,25 @@
     def extract_losses(self, named_outputs: Dict[str, Any]) -> Dict[str, Any]:
         named_losses = {name: loss for name, loss in named_outputs.items() if name in self.loss_output_names}
         return named_losses
 
     def summarize(self, stage: Stage, reset: bool) -> Dict[str, Any]:
         return {}
 
+    def __repr__(self):  # Overwrite '__repr__' of 'BrickModule'
+        return BrickInterface.__repr__(self)
+
 
 @typechecked
 class BrickCollection(nn.ModuleDict):
     def __init__(self, bricks: Dict[str, BrickInterface]) -> None:
+        resolve_relative_names(bricks=bricks)
         super().__init__(convert_nested_dict_to_nested_brick_collection(bricks))
 
+
     def forward(self, named_inputs: Dict[str, Any], stage: Stage, return_inputs: bool = True) -> Dict[str, Any]:
         gathered_named_io = dict(named_inputs)  # To keep the argument `named_inputs` unchanged
 
         for brick in self.values():
             if brick.run_now(stage=stage):
                 results = brick.forward(stage=stage, named_inputs=gathered_named_io)
                 gathered_named_io.update(results)
@@ -142,15 +161,14 @@
 
     def summarize(self, stage: Stage, reset: bool) -> Dict[str, Any]:
         metrics = {}
         for brick in self.values():
             metrics.update(brick.summarize(stage=stage, reset=reset))
         return metrics
 
-
 @typechecked
 def convert_nested_dict_to_nested_brick_collection(bricks: Dict[str, Union[BrickInterface, Dict]], level=0):
     converted_bricks = {}
     for name, brick in bricks.items():
         if isinstance(brick, dict):
             converted_bricks[name] = convert_nested_dict_to_nested_brick_collection(brick, level=level+1)
         else:
@@ -158,14 +176,44 @@
 
     if level == 0:
         return converted_bricks
     else:
         return BrickCollection(converted_bricks)
 
 
+def resolve_relative_names(bricks: Dict[str, BrickInterface]):
+    return _resolve_relative_names_recursive(bricks)
+
+def _resolve_relative_names_recursive(bricks: Dict[str, BrickInterface], parent: Optional[Path] = None):
+    parent = parent or Path('/root')
+    for brick_name, brick_or_bricks in bricks.items():
+        if isinstance(brick_or_bricks, (dict, BrickCollection)):
+            _resolve_relative_names_recursive(bricks=brick_or_bricks, parent=parent / brick_name)
+        elif isinstance(brick_or_bricks, BrickInterface):
+            brick_or_bricks.input_names = _resolve_input_or_output_names(brick_or_bricks.input_names, parent)
+            brick_or_bricks.output_names = _resolve_input_or_output_names(brick_or_bricks.output_names, parent)
+        else:
+            raise ValueError('')
+
+    return bricks
+
+def _resolve_input_or_output_names(input_or_output_names: List[str], parent: Path):
+    input_names_resolved = []
+    for input_name in input_or_output_names:
+        is_relative_name = input_name[0] == '.'
+        if is_relative_name:
+            input_name_as_path = Path(parent / input_name).resolve()
+            if len(input_name_as_path.parents) == 1:
+                raise ValueError(f'Failed to resolve input name. Unable to resolve "{input_name}" in brick "{parent.relative_to("/root")}" '
+                                  'to an actual name. ')
+            input_name = str(input_name_as_path.relative_to('/root'))
+        input_names_resolved.append(input_name)
+    return input_names_resolved
+
+
 @typechecked
 class BrickTrainable(BrickModule):
     def __init__(self, model: nn.Module,
                  input_names: Union[List[str], Dict[str, str], str],
                  output_names: List[str],
                  loss_output_names: Union[List[str], str] = 'none',
                  alive_stages: Union[List[Stage], str] = 'all'):
@@ -221,15 +269,20 @@
                  ):
 
         alive_stages = alive_stages or [Stage.TRAIN, Stage.TEST, Stage.VALIDATION]
         if return_metrics:
             output_names = list(metric_collection)
         else:
             output_names = []
-        BrickInterface.__init__(self, input_names=input_names, output_names=output_names, alive_stages=alive_stages)
+
+        BrickInterface.__init__(self,
+                                input_names=input_names,
+                                output_names=output_names,
+                                alive_stages=alive_stages,
+                                wrapped_module_name=f'{list(metric_collection)}')
         nn.Module.__init__(self)
 
         if isinstance(metric_collection, dict):
             metric_collection = MetricCollection(metric_collection)
 
         self.return_metrics = return_metrics
         self.metrics = nn.ModuleDict({stage.name: metric_collection.clone() for stage in alive_stages})
```

### Comparing `torchbricks-0.0.8/src/torchbricks/bricks_helper.py` & `torchbricks-0.0.9/src/torchbricks/bricks_helper.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.8/src/torchbricks/custom_metrics.py` & `torchbricks-0.0.9/src/torchbricks/custom_metrics.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.8/src/torchbricks.egg-info/PKG-INFO` & `torchbricks-0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,7 @@
-Metadata-Version: 2.1
-Name: torchbricks
-Version: 0.0.8
-Summary: Decoupled and modular approach to building multi-task ML models
-Author-email: Peter Hviid Christianse <PeterHviidChristiansen@gmail.com>
-License: MIT License
-        
-        Copyright (c) 2023 Peter Christiansen
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/PeteHeine/torchbricks
-Keywords: torch,multi-task,machine learning
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <!--
 
 ---
 jupyter:
   jupytext:
     hide_notebook_metadata: true
     text_representation:
@@ -103,37 +67,43 @@
 from torchbricks.bricks import Stage
 
 bricks = {
     'preprocessor': BrickNotTrainable(PreprocessorDummy(), input_names=['raw'], output_names=['processed']),
     'backbone': BrickTrainable(TinyModel(n_channels=3, n_features=10), input_names=['processed'], output_names=['embedding']),
     'head': BrickTrainable(ClassifierDummy(num_classes=3, in_features=10), input_names=['embedding'], output_names=['logits', "softmaxed"]),
 }
+brick_collection = BrickCollection(bricks)
+print(brick_collection)
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+# )
 ```
 
-All modules are added as entries in a regular dictionary and for each module, we provide a name (dictionary key) and 
-input and output names. The number of input and output names should match the actually number of input and outputs 
-for each function. 
-
-Each module is wrapped inside a brick - here either `BrickTrainable` and `BrickNotTrainable`.
+All modules are added as entries in a regular dictionary and for each module, we wrap it inside a brick (here either `BrickTrainable` and 
+`BrickNotTrainable`), provide a name (dictionary key) and input and output names. The number of input and output names should match the 
+actually number of input and outputs for each function. 
 
-The `bricks`-dictionary describe how data is passed between bricks: The `preprocessor` uses a `raw` input tensor and passes the
+Input and output names specify how tensors move between bricks: The `preprocessor` uses a `raw` input tensor and passes the
 `processed` tensor to the `backbone`. The backbone returns the `embedding` tensor and passes it to the `head` determining 
 both `logits` and `softmaxed` tensors. 
 
-Bricks are then passed to a `BrickCollection` for executing bricks. The brick collection accepts a dictionary with required inputs and
-returns a dictionary with both intermediated and resulting tensors. 
+Bricks are passed to a `BrickCollection` for executing them as showed in below:
 
 ```python
-brick_collection = BrickCollection(bricks)
 batch_size=2
 batch_images = torch.rand((batch_size, 3, 100, 200))
 named_outputs = brick_collection(named_inputs={'raw': batch_images}, stage=Stage.INFERENCE)
-print(named_outputs.keys())
+print("Brick outputs:", named_outputs.keys())
+# Brick outputs: dict_keys(['raw', 'stage', 'processed', 'embedding', 'logits', 'softmaxed'])
 ```
 
+The brick collection accepts a dictionary and returns a dictionary with both intermediated and resulting tensors. 
+
 Running our models as a brick collection has the following advantages:
 
 - A brick collection act as a regular `nn.Module` with all the familiar features: a `forward`-function, a `to`-function to move 
   to a specific device/precision, you can save/load a model, management of parameters, onnx exportable etc. 
 - A brick collection is also a simple DAG, it accepts a dictionary (`named_inputs`), 
 executes each bricks and ensures that the outputs are passed to the inputs of other bricks with matching names. 
 Structuring the model as a DAG, makes it easy to add/remove outputs for a given module during development, add new modules to the
@@ -165,14 +135,22 @@
                                alive_stages="all"),
     'head': BrickTrainable(ClassifierDummy(num_classes=num_classes, in_features=10), input_names=['embedding'], 
                            output_names=['logits', 'softmaxed'], alive_stages="all"),
     'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'], 
                       alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST], loss_output_names="all")
 }
 brick_collection = BrickCollection(bricks)
+
+print(brick_collection)
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(PreprocessorDummy, input_names=['raw'], output_names=['processed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(TinyModel, input_names=['processed'], output_names=['embedding'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head): BrickTrainable(ClassifierDummy, input_names=['embedding'], output_names=['logits', 'softmaxed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (loss): BrickLoss(CrossEntropyLoss, input_names=['logits', 'targets'], output_names=['loss_ce'], alive_stages=['TRAIN', 'VALIDATION', 'TEST'])
+# )
 ```
 
 We set `preprocessor`, `backbone` and `head` to be alive on all stages `alive_stages="all"` - this is the default behavior and
 similar to before. 
 
 For `loss` we set `alive_stages=[Stage.TRAIN, Stage.VALIDATION, Stage.TEST]` to calculate loss during train, validation and test
 stages. 
@@ -298,15 +276,15 @@
                       brick_collection=brick_collection, 
                       named_inputs=named_inputs, 
                       dynamic_batch_size=True, 
                       stage=Stage.EXPORT)
 ```
 
 ### Brick features: Act as a nn.Module
-A brick collection acts as a 'nn.Module' mean we can do the following: 
+A brick collection acts as a 'nn.Module' meaning:
 
 ```python
 # Move to specify device (CPU/GPU) or precision to automatically move model parameters
 brick_collection_half = brick_collection.to(torch.float16)
 
 
 # Save model parameters
@@ -314,20 +292,63 @@
 torch.save(brick_collection_half.state_dict(), path_model)
 
 # Load model parameters
 brick_collection_half.load_state_dict(torch.load(path_model))
 
 # Access parameters
 brick_collection_half.named_parameters()
+
+# Using compile with pytorch >= 2.0
+torch.compile(brick_collection)
 ```
 
+### Brick features: Act as a dictionary (nn.ModuleDict)
+
+
+
+```python
+from typing import Dict
+
+from torchbricks.bricks import BrickInterface
 
 
+def image_classifier_head(num_classes: int, in_channels: int) -> Dict[str, BrickInterface]:
+    """Image classifier bricks: Classifier, loss and metrics """
+    head = {
+        'classify': BrickTrainable(ImageClassifier(num_classes=num_classes, n_features=in_channels),
+                                   input_names=['features'], output_names=['./logits', './probabilities', './class_prediction']),
+        'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=['./class_prediction', 'targets']),
+        'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['./logits', 'targets'], output_names=['./loss_ce'])
+    }
+    return head
 
 
+bricks = {
+    'preprocessor': BrickNotTrainable(Preprocessor(), input_names=['raw'], output_names=['normalized']),
+    'backbone': resnet_brick,
+    'head0': image_classifier_head(num_classes=3, in_channels=resnet_brick.model.n_backbone_features),
+    'head1': image_classifier_head(num_classes=5, in_channels=resnet_brick.model.n_backbone_features),
+}
+print(BrickCollection(bricks))
+# BrickCollection(
+#   (preprocessor): BrickNotTrainable(Preprocessor, input_names=['raw'], output_names=['normalized'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (backbone): BrickTrainable(BackboneResnet, input_names=['normalized'], output_names=['features'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#   (head0): BrickCollection(
+#     (classify): BrickTrainable(ImageClassifier, input_names=['features'], output_names=['head0/logits', 'head0/probabilities', 'head0/class_prediction'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#     (accuracy): BrickMetricSingle(['MulticlassAccuracy'], input_names=['head0/class_prediction', 'targets'], output_names=[], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#     (loss): BrickLoss(CrossEntropyLoss, input_names=['head0/logits', 'targets'], output_names=['head0/loss_ce'], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#   )
+#   (head1): BrickCollection(
+#     (classify): BrickTrainable(ImageClassifier, input_names=['features'], output_names=['head1/logits', 'head1/probabilities', 'head1/class_prediction'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+#     (accuracy): BrickMetricSingle(['MulticlassAccuracy'], input_names=['head1/class_prediction', 'targets'], output_names=[], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#     (loss): BrickLoss(CrossEntropyLoss, input_names=['head1/logits', 'targets'], output_names=['head1/loss_ce'], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+#   )
+# )
+```
+
 ### Bag of bricks - reusable bricks modules
 Note also in above example we use bag-of-bricks to import commonly used `nn.Module`s 
 
 This includes a `Preprocessor`, `ImageClassifier` and `resnet_to_brick` to convert torchvision resnet models into a backbone brick 
 (without a classifier).
 
 
@@ -418,14 +439,16 @@
   - [x] Use loss-function to show that stage decided on what is being executed. 
   - [x] Introduce metrics by it-self in another example
 - [x] Ensure that all examples in the `README.md` are working with easy to use modules. 
 - [x] Add typeguard
 - [x] Allow a brick to receive all named_inputs and add a test for it.
 - [x] Fix the release process. It should be as simple as running `make release`.
 - [x] Add onnx export example to the README.md
+- [ ] Pretty print bricks
+- [ ] Relative input/output names
 - [ ] Make DAG like functionality to check if a inputs and outputs works for all model stages.
 - [ ] Use pymy, pyright or pyre to do static code checks. 
 - [ ] Decide: Add stage as an internal state and not in the forward pass:
   - Minor Pros: Tracing (to get onnx model) requires only torch.Tensors only as input - we avoid making an adapter class. 
   - Minor Cons: State gets hidden away - implicit instead of explicit.
   - Minor Pros: Similar to eval/training 
 - [ ] Collection of helper modules. Preprocessors, Backbones, Necks/Upsamplers, ImageClassification, SemanticSegmentation, ObjectDetection
```

### Comparing `torchbricks-0.0.8/src/torchbricks.egg-info/SOURCES.txt` & `torchbricks-0.0.9/src/torchbricks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.8/tests/test_bag_of_bricks.py` & `torchbricks-0.0.9/tests/test_bag_of_bricks.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.8/tests/test_brick_utils.py` & `torchbricks-0.0.9/tests/test_brick_utils.py`

 * *Files identical despite different names*

### Comparing `torchbricks-0.0.8/tests/test_bricks.py` & `torchbricks-0.0.9/tests/test_bricks.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 from typing import Optional
 
 import pytest
 import torch
 import torchmetrics
 from torch import nn
 from torchbricks import bricks, custom_metrics
-from torchbricks.bricks import BrickCollection, BrickLoss, BrickMetrics, BrickMetricSingle, Stage
+from torchbricks.bricks import BrickCollection, BrickLoss, BrickMetrics, BrickMetricSingle, BrickModule, Stage
 from torchmetrics.classification import MulticlassAccuracy
 from utils_testing.utils_testing import assert_equal_dictionaries, create_brick_collection
 
 
 def test_brick_collection():
     num_classes = 10
     brick_collection = create_brick_collection(num_classes=num_classes, num_backbone_featues=5)
     expected_forward_named_outputs = {'labels', 'raw', 'stage', 'preprocessed', 'features', 'predictions'}
     expected_named_losses = {'ce_loss'}
-    expected_named_metrics = set(brick_collection['metrics'].metrics[Stage.TRAIN.name])
+    expected_named_metrics = set(brick_collection['head']['metrics'].metrics[Stage.TRAIN.name])
 
     model = bricks.BrickCollection(bricks=brick_collection)
+
+
     named_inputs = {'labels': torch.tensor(range(num_classes), dtype=torch.float64), 'raw': torch.zeros((3, 24, 24))}
 
     named_outputs = model(stage=Stage.TRAIN, named_inputs=named_inputs)
     metrics = model.summarize(stage=Stage.TRAIN, reset=True)
 
     losses = model.extract_losses(named_outputs=named_outputs)
     assert set(metrics) == expected_named_metrics
@@ -33,15 +35,15 @@
 def test_brick_collection_no_metrics():
     num_classes = 10
     expected_forward_named_outputs = {'labels', 'raw', 'stage', 'preprocessed', 'features', 'predictions'}
     expected_named_losses = {'ce_loss'}
     expected_named_metrics = {}
 
     brick_collection = create_brick_collection(num_classes=num_classes, num_backbone_featues=5)
-    brick_collection = {name: brick for name, brick in brick_collection.items() if not isinstance(brick, bricks.BrickMetrics)}
+    brick_collection['head'].pop('metrics')
     model = bricks.BrickCollection(bricks=brick_collection)
 
     named_inputs = {'labels': torch.tensor(range(num_classes), dtype=torch.float64), 'raw': torch.zeros((3, 24, 24))}
     named_outputs = model(stage=Stage.INFERENCE, named_inputs=named_inputs)
     assert expected_forward_named_outputs == set(named_outputs)
 
     named_outputs = model(stage=Stage.TRAIN, named_inputs=named_inputs)
@@ -56,16 +58,16 @@
 def test_brick_collection_no_metrics_no_losses():
     num_classes = 10
     expected_forward_named_outputs = {'labels', 'raw', 'stage', 'preprocessed', 'features', 'predictions'}
     expected_named_losses = {}
     expected_named_metrics = {}
 
     brick_collection = create_brick_collection(num_classes=num_classes, num_backbone_featues=5)
-    brick_collection = {name: brick for name, brick in brick_collection.items() if not isinstance(brick, bricks.BrickMetrics)}
-    brick_collection = {name: brick for name, brick in brick_collection.items() if not isinstance(brick, bricks.BrickLoss)}
+    brick_collection['head'].pop('metrics')
+    brick_collection['head'].pop('loss')
     model = bricks.BrickCollection(bricks=brick_collection)
 
     named_inputs = {'labels': torch.tensor(range(num_classes), dtype=torch.float64), 'raw': torch.zeros((3, 24, 24))}
     named_outputs = model(stage= Stage.INFERENCE, named_inputs=named_inputs)
     assert expected_forward_named_outputs == set(named_outputs)
 
     model(stage=Stage.TRAIN, named_inputs=named_inputs)
@@ -145,24 +147,34 @@
     bricks = {
         'accuracy': BrickMetricSingle(MulticlassAccuracy(num_classes=num_classes), input_names=['logits', 'targets'],
                                       metric_name=metric_name),
         'loss': BrickLoss(model=nn.CrossEntropyLoss(), input_names=['logits', 'targets'], output_names=['loss_ce'])
     }
 
     model = BrickCollection(bricks)
+
     batch_logits = torch.rand((1, num_classes))
     stage = Stage.TRAIN
     named_inputs = {'logits': batch_logits, 'targets': torch.ones((1), dtype=torch.int64)}
     model(named_inputs=named_inputs, stage=stage)
     metrics = model.summarize(stage=stage, reset=True)
     expected_metric_name = metric_name or 'MulticlassAccuracy'
 
     assert list(metrics) == [expected_metric_name]
 
 
+expected_str='''BrickCollection(
+  (preprocessor): BrickNotTrainable(Preprocessor, input_names=['raw'], output_names=['preprocessed'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+  (backbone): BrickTrainable(TinyBackbone, input_names=['preprocessed'], output_names=['features'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+  (head): BrickCollection(
+    (classifier): BrickTrainable(Classifier, input_names=['features'], output_names=['predictions'], alive_stages=['TRAIN', 'VALIDATION', 'TEST', 'INFERENCE', 'EXPORT'])
+    (loss): BrickLoss(CrossEntropyLoss, input_names=['predictions', 'labels'], output_names=['ce_loss'], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+    (metrics): BrickMetrics(['Accuracy', 'Concatenate', 'ConfMat', 'MeanAccuracy'], input_names=['predictions', 'labels'], output_names=[], alive_stages=['TRAIN', 'TEST', 'VALIDATION'])
+  )
+)''' # noqa: E501
 @pytest.mark.parametrize('return_metrics', [False, True])
 def test_brick_torch_metric_multiple_metric(return_metrics: bool):
     num_classes = 5
     metric_collection = torchmetrics.MetricCollection({
         'MeanAccuracy': MulticlassAccuracy(num_classes=num_classes, average='macro'),
         'Accuracy': MulticlassAccuracy(num_classes=num_classes, average='micro'),
         'ConfMat': torchmetrics.ConfusionMatrix(task='multiclass', num_classes=num_classes),
@@ -185,14 +197,68 @@
         expected_outputs = expected_outputs.union(set(metric_collection))
 
     assert set(named_outputs) == expected_outputs
     metrics = model.summarize(stage=stage, reset=True)
     expected_metrics = set(metric_collection)
     assert set(metrics) == expected_metrics
 
+def test_brick_collection_print():
+    num_classes = 10
+    bricks = create_brick_collection(num_classes=num_classes, num_backbone_featues=5)
+    model = BrickCollection(bricks)
+    assert model.__str__() == expected_str
+
+
+def test_resolve_relative_names():
+    bricks = {
+        'preprocessor': BrickModule(model=nn.Identity(), input_names=['raw'], output_names=['processed']),
+        'backbone': BrickModule(model=nn.Identity(), input_names=['processed'], output_names=['embeddings']),
+        'head0': {
+            'classifier': BrickModule(model=nn.Identity(), input_names=['../embeddings'], output_names=['./predictions']),
+            'loss': BrickModule(model=nn.Identity(), input_names=['./predictions'], output_names=['./loss']),
+        },
+        'head1': {
+            'classifier': BrickModule(model=nn.Identity(), input_names=['embeddings'], output_names=['./predictions']),
+            'loss': BrickModule(model=nn.Identity(), input_names=['./predictions'], output_names=['./loss']),
+            'head1_nested':{
+                'classifier': BrickModule(model=nn.Identity(), input_names=['../../embeddings',
+                                                                            '../predictions',
+                                                                            '../../head0/predictions'],
+                                          output_names=['./predictions']),
+                'loss': BrickModule(model=nn.Identity(), input_names=['./predictions'], output_names=['./loss']),
+            }
+        }
+    }
+
+    model = BrickCollection(bricks)
+    assert model['head0']['classifier'].input_names == ['embeddings']
+    assert model['head0']['classifier'].output_names == ['head0/predictions']
+    assert model['head0']['loss'].input_names == ['head0/predictions']
+    assert model['head0']['loss'].output_names == ['head0/loss']
+
+    assert model['head1']['head1_nested']['classifier'].input_names == ['embeddings', 'head1/predictions', 'head0/predictions']
+    assert model['head1']['head1_nested']['classifier'].output_names == ['head1/head1_nested/predictions']
+
+    assert model['head1']['head1_nested']['loss'].input_names == ['head1/head1_nested/predictions']
+    assert model['head1']['head1_nested']['loss'].output_names == ['head1/head1_nested/loss']
+
+
+def test_resolve_relative_names_errors():
+    bricks = {
+        'preprocessor': BrickModule(model=nn.Identity(), input_names=['raw'], output_names=['processed']),
+        'backbone': BrickModule(model=nn.Identity(), input_names=['processed'], output_names=['embeddings']),
+        'head0': {
+            'classifier': BrickModule(model=nn.Identity(), input_names=['../../embeddings'], output_names=['./predictions']),
+            'loss': BrickModule(model=nn.Identity(), input_names=['./predictions'], output_names=['./loss']),
+        },
+    }
+    with pytest.raises(ValueError, match='Failed to resolve input name. Unable to resolve'):
+        BrickCollection(bricks)
+
+
 def test_save_and_load_of_brick_collection(tmp_path: Path):
     brick_collection = create_brick_collection(num_classes=3, num_backbone_featues=10)
     model = BrickCollection(brick_collection)
     path_model = tmp_path / 'test_model.pt'
 
     # Trainable parameters are saved
     torch.save(model.state_dict(), path_model)
```

### Comparing `torchbricks-0.0.8/tests/test_bricks_helper.py` & `torchbricks-0.0.9/tests/test_bricks_helper.py`

 * *Files identical despite different names*

