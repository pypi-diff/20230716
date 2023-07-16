# Comparing `tmp/segnn_jax-0.6.tar.gz` & `tmp/segnn_jax-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segnn_jax-0.6.tar", last modified: Mon May  8 09:44:50 2023, max compression
+gzip compressed data, was "segnn_jax-0.7.tar", last modified: Sun Jul 16 21:12:01 2023, max compression
```

## Comparing `segnn_jax-0.6.tar` & `segnn_jax-0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:50.580514 segnn_jax-0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-08 09:44:42.000000 segnn_jax-0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-08 09:44:50.580514 segnn_jax-0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-08 09:44:42.000000 segnn_jax-0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 09:44:42.000000 segnn_jax-0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:50.580514 segnn_jax-0.6/segnn_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/irreps_computer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9733 2023-05-08 09:44:42.000000 segnn_jax-0.6/segnn_jax/segnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:50.580514 segnn_jax-0.6/segnn_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 09:44:50.000000 segnn_jax-0.6/segnn_jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-08 09:44:50.580514 segnn_jax-0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 09:44:42.000000 segnn_jax-0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 09:44:50.580514 segnn_jax-0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-08 09:44:42.000000 segnn_jax-0.6/tests/test_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-08 09:44:42.000000 segnn_jax-0.6/tests/test_segnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:12:01.019724 segnn_jax-0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-16 21:11:48.000000 segnn_jax-0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-16 21:12:01.019724 segnn_jax-0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-16 21:11:48.000000 segnn_jax-0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-16 21:11:48.000000 segnn_jax-0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:12:01.019724 segnn_jax-0.7/segnn_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-16 21:11:48.000000 segnn_jax-0.7/segnn_jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12021 2023-07-16 21:11:48.000000 segnn_jax-0.7/segnn_jax/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-16 21:11:48.000000 segnn_jax-0.7/segnn_jax/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-07-16 21:11:48.000000 segnn_jax-0.7/segnn_jax/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-07-16 21:11:48.000000 segnn_jax-0.7/segnn_jax/irreps_computer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-07-16 21:11:48.000000 segnn_jax-0.7/segnn_jax/segnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:12:01.019724 segnn_jax-0.7/segnn_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-16 21:12:01.000000 segnn_jax-0.7/segnn_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-16 21:12:01.000000 segnn_jax-0.7/segnn_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 21:12:01.000000 segnn_jax-0.7/segnn_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-16 21:12:01.000000 segnn_jax-0.7/segnn_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-16 21:12:01.000000 segnn_jax-0.7/segnn_jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-16 21:12:01.019724 segnn_jax-0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-16 21:11:48.000000 segnn_jax-0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 21:12:01.019724 segnn_jax-0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-07-16 21:11:48.000000 segnn_jax-0.7/tests/test_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-07-16 21:11:48.000000 segnn_jax-0.7/tests/test_segnn.py
```

### Comparing `segnn_jax-0.6/LICENSE` & `segnn_jax-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `segnn_jax-0.6/PKG-INFO` & `segnn_jax-0.7/segnn_jax.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: segnn_jax
-Version: 0.6
+Name: segnn-jax
+Version: 0.7
 Summary: Steerable E(3) GNN in jax
 Author: Gianluca Galletti
 Author-email: g.galletti@tum.de
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 ```
 python -m pip install -e .
 ```
 
 ### GPU support
 Upgrade `jax` to the gpu version
 ```
-pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade "jax[cuda]>=0.4.6" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Validation
 N-body (charged and gravity) and QM9 datasets are included for completeness from the original paper.
 
 ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable sizes, so in jax samples are padded to the maximum size. Loss is MSE for Charged and Gravity and MAE for QM9.
@@ -53,15 +53,15 @@
     <td>Inference [ms]</td>
   </tr>
   <tr>
     <td> <code>charged (position)</code> </td>
     <td>.0043</td>
     <td>21.22</td>
     <td>.0045</td>
-    <td>4.47</td>
+    <td>3.77</td>
   </tr>
   <tr>
     <td><code>gravity (position)</code> </td>
     <td>.265</td>
     <td>60.55</td>
     <td>.264</td>
     <td>41.72</td>
@@ -92,19 +92,25 @@
 
 ### Datasets
 QM9 is automatically downloaded and processed when running the respective experiment.
 
 The N-body datasets have to be generated locally from the directory [experiments/nbody/data](experiments/nbody/data) (it will take some time, especially n-body `gravity`)
 #### Charged dataset (5 bodies, 10000 training samples)
 ```
-python3 -u generate_dataset.py --simulation=charged
+python3 -u generate_dataset.py --simulation=charged --seed=43
 ```
 #### Gravity dataset (100 bodies, 10000 training samples)
 ```
-python3 -u generate_dataset.py --simulation=gravity --n-balls=100
+python3 -u generate_dataset.py --simulation=gravity --n-balls=100 --seed=43
+```
+
+### Notes
+On `jax<=0.4.6`, the `jit`-`pjit` merge can be deactivated making traning faster (on nbody). This looks like an issue with dataloading and the validation training loop implementation and it does not affect SEGNN.
+```
+export JAX_JIT_PJIT_API_MERGE=0
 ```
 
 ### Usage
 #### N-body (charged)
 ```
 python validate.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
 ```
@@ -118,10 +124,11 @@
 ```
 python validate.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
 ```
 
 (configurations used in validation)
 
 
+
 ## Acknowledgments
 - [e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation possible.
 - [Artur Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://github.com/brandstetter-johannes), for support.
```

#### html2text {}

```diff
@@ -1,48 +1,52 @@
-Metadata-Version: 2.1 Name: segnn_jax Version: 0.6 Summary: Steerable E(3) GNN
+Metadata-Version: 2.1 Name: segnn-jax Version: 0.7 Summary: Steerable E(3) GNN
 in jax Author: Gianluca Galletti Author-email: g.galletti@tum.de Classifier:
 Programming Language :: Python :: 3.8 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # Steerable E(3) GNN in jax
 Reimplementation of [SEGNN](https://arxiv.org/abs/2110.02905) in jax. Original
 work by Johannes Brandstetter, Rob Hesselink, Elise van der Pol, Erik Bekkers
 and Max Welling. ## Why jax? **40-50% faster** inference and training compared
 to the [original torch implementation](https://github.com/RobDHess/Steerable-
 E3-GNN). Also JAX-MD. ## Installation ``` python -m pip install segnn-jax ```
 Or clone this repository and build locally ``` python -m pip install -e . ```
 ### GPU support Upgrade `jax` to the gpu version ``` pip install --upgrade "jax
-[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/
+[cuda]>=0.4.6" -f https://storage.googleapis.com/jax-releases/
 jax_cuda_releases.html ``` ## Validation N-body (charged and gravity) and QM9
 datasets are included for completeness from the original paper. ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable
 sizes, so in jax samples are padded to the maximum size. Loss is MSE for
 Charged and Gravity and MAE for QM9. Times are remeasured on Quadro RTX 4000,
 __model only__ on batches of 100 graphs, in (global) single precision.
                    torch (original)     jax (ours)
                    Loss  Inference [ms] Loss  Inference [ms]
-charged (position) .0043 21.22          .0045 4.47
+charged (position) .0043 21.22          .0045 3.77
 gravity (position) .265  60.55          .264  41.72
 QM9 (alpha)        .066* 82.53          .082  105.98**
 * rerun on same conditions ** padded (naive) ### Validation install The
 experiments are only included in the github repo, so it needs to be cloned
 first. ``` git clone https://github.com/gerkone/segnn-jax ``` They are adapted
 from the original implementation, so additionally `torch` and `torch_geometric`
 are needed (cpu versions are enough). ``` python -m pip install -r experiments/
 requirements.txt ``` ### Datasets QM9 is automatically downloaded and processed
 when running the respective experiment. The N-body datasets have to be
 generated locally from the directory [experiments/nbody/data](experiments/
 nbody/data) (it will take some time, especially n-body `gravity`) #### Charged
 dataset (5 bodies, 10000 training samples) ``` python3 -u generate_dataset.py -
--simulation=charged ``` #### Gravity dataset (100 bodies, 10000 training
-samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-balls=100
-``` ### Usage #### N-body (charged) ``` python validate.py --dataset=charged --
-epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --
-units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` ####
-N-body (gravity) ``` python validate.py --dataset=gravity --epochs=100 --
-target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 -
--units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --
-neighbours=5 --n-bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 -
--epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --
-units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-
-scheduling ``` (configurations used in validation) ## Acknowledgments -
-[e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation
-possible. - [Artur Toshev](https://github.com/arturtoshev) and [Johannes
-Brandsetter](https://github.com/brandstetter-johannes), for support.
+-simulation=charged --seed=43 ``` #### Gravity dataset (100 bodies, 10000
+training samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-
+balls=100 --seed=43 ``` ### Notes On `jax<=0.4.6`, the `jit`-`pjit` merge can
+be deactivated making traning faster (on nbody). This looks like an issue with
+dataloading and the validation training loop implementation and it does not
+affect SEGNN. ``` export JAX_JIT_PJIT_API_MERGE=0 ``` ### Usage #### N-body
+(charged) ``` python validate.py --dataset=charged --epochs=200 --max-
+samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --
+norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` #### N-body
+(gravity) ``` python validate.py --dataset=gravity --epochs=100 --target=pos --
+max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --
+norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-
+bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 --epochs=1000 --
+target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --
+norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
+``` (configurations used in validation) ## Acknowledgments - [e3nn_jax](https:/
+/github.com/e3nn/e3nn-jax) made this reimplementation possible. - [Artur
+Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://
+github.com/brandstetter-johannes), for support.
```

### Comparing `segnn_jax-0.6/README.md` & `segnn_jax-0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ```
 python -m pip install -e .
 ```
 
 ### GPU support
 Upgrade `jax` to the gpu version
 ```
-pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade "jax[cuda]>=0.4.6" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Validation
 N-body (charged and gravity) and QM9 datasets are included for completeness from the original paper.
 
 ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable sizes, so in jax samples are padded to the maximum size. Loss is MSE for Charged and Gravity and MAE for QM9.
@@ -42,15 +42,15 @@
     <td>Inference [ms]</td>
   </tr>
   <tr>
     <td> <code>charged (position)</code> </td>
     <td>.0043</td>
     <td>21.22</td>
     <td>.0045</td>
-    <td>4.47</td>
+    <td>3.77</td>
   </tr>
   <tr>
     <td><code>gravity (position)</code> </td>
     <td>.265</td>
     <td>60.55</td>
     <td>.264</td>
     <td>41.72</td>
@@ -81,19 +81,25 @@
 
 ### Datasets
 QM9 is automatically downloaded and processed when running the respective experiment.
 
 The N-body datasets have to be generated locally from the directory [experiments/nbody/data](experiments/nbody/data) (it will take some time, especially n-body `gravity`)
 #### Charged dataset (5 bodies, 10000 training samples)
 ```
-python3 -u generate_dataset.py --simulation=charged
+python3 -u generate_dataset.py --simulation=charged --seed=43
 ```
 #### Gravity dataset (100 bodies, 10000 training samples)
 ```
-python3 -u generate_dataset.py --simulation=gravity --n-balls=100
+python3 -u generate_dataset.py --simulation=gravity --n-balls=100 --seed=43
+```
+
+### Notes
+On `jax<=0.4.6`, the `jit`-`pjit` merge can be deactivated making traning faster (on nbody). This looks like an issue with dataloading and the validation training loop implementation and it does not affect SEGNN.
+```
+export JAX_JIT_PJIT_API_MERGE=0
 ```
 
 ### Usage
 #### N-body (charged)
 ```
 python validate.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
 ```
@@ -107,10 +113,11 @@
 ```
 python validate.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
 ```
 
 (configurations used in validation)
 
 
+
 ## Acknowledgments
 - [e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation possible.
 - [Artur Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://github.com/brandstetter-johannes), for support.
```

#### html2text {}

```diff
@@ -1,45 +1,49 @@
 # Steerable E(3) GNN in jax Reimplementation of [SEGNN](https://arxiv.org/abs/
 2110.02905) in jax. Original work by Johannes Brandstetter, Rob Hesselink,
 Elise van der Pol, Erik Bekkers and Max Welling. ## Why jax? **40-50% faster**
 inference and training compared to the [original torch implementation](https://
 github.com/RobDHess/Steerable-E3-GNN). Also JAX-MD. ## Installation ``` python
 -m pip install segnn-jax ``` Or clone this repository and build locally ```
 python -m pip install -e . ``` ### GPU support Upgrade `jax` to the gpu version
-``` pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/
+``` pip install --upgrade "jax[cuda]>=0.4.6" -f https://storage.googleapis.com/
 jax-releases/jax_cuda_releases.html ``` ## Validation N-body (charged and
 gravity) and QM9 datasets are included for completeness from the original
 paper. ### Results Charged is on 5 bodies, gravity on 100 bodies. QM9 has
 graphs of variable sizes, so in jax samples are padded to the maximum size.
 Loss is MSE for Charged and Gravity and MAE for QM9. Times are remeasured on
 Quadro RTX 4000, __model only__ on batches of 100 graphs, in (global) single
 precision.
                    torch (original)     jax (ours)
                    Loss  Inference [ms] Loss  Inference [ms]
-charged (position) .0043 21.22          .0045 4.47
+charged (position) .0043 21.22          .0045 3.77
 gravity (position) .265  60.55          .264  41.72
 QM9 (alpha)        .066* 82.53          .082  105.98**
 * rerun on same conditions ** padded (naive) ### Validation install The
 experiments are only included in the github repo, so it needs to be cloned
 first. ``` git clone https://github.com/gerkone/segnn-jax ``` They are adapted
 from the original implementation, so additionally `torch` and `torch_geometric`
 are needed (cpu versions are enough). ``` python -m pip install -r experiments/
 requirements.txt ``` ### Datasets QM9 is automatically downloaded and processed
 when running the respective experiment. The N-body datasets have to be
 generated locally from the directory [experiments/nbody/data](experiments/
 nbody/data) (it will take some time, especially n-body `gravity`) #### Charged
 dataset (5 bodies, 10000 training samples) ``` python3 -u generate_dataset.py -
--simulation=charged ``` #### Gravity dataset (100 bodies, 10000 training
-samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-balls=100
-``` ### Usage #### N-body (charged) ``` python validate.py --dataset=charged --
-epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --
-units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` ####
-N-body (gravity) ``` python validate.py --dataset=gravity --epochs=100 --
-target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 -
--units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --
-neighbours=5 --n-bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 -
--epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --
-units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-
-scheduling ``` (configurations used in validation) ## Acknowledgments -
-[e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation
-possible. - [Artur Toshev](https://github.com/arturtoshev) and [Johannes
-Brandsetter](https://github.com/brandstetter-johannes), for support.
+-simulation=charged --seed=43 ``` #### Gravity dataset (100 bodies, 10000
+training samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-
+balls=100 --seed=43 ``` ### Notes On `jax<=0.4.6`, the `jit`-`pjit` merge can
+be deactivated making traning faster (on nbody). This looks like an issue with
+dataloading and the validation training loop implementation and it does not
+affect SEGNN. ``` export JAX_JIT_PJIT_API_MERGE=0 ``` ### Usage #### N-body
+(charged) ``` python validate.py --dataset=charged --epochs=200 --max-
+samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --
+norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` #### N-body
+(gravity) ``` python validate.py --dataset=gravity --epochs=100 --target=pos --
+max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --
+norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-
+bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 --epochs=1000 --
+target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --
+norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
+``` (configurations used in validation) ## Acknowledgments - [e3nn_jax](https:/
+/github.com/e3nn/e3nn-jax) made this reimplementation possible. - [Artur
+Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://
+github.com/brandstetter-johannes), for support.
```

### Comparing `segnn_jax-0.6/segnn_jax/blocks.py` & `segnn_jax-0.7/segnn_jax/blocks.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import warnings
+from abc import ABC, abstractmethod
 from typing import Callable, Optional, Tuple, Union
 
 import e3nn_jax as e3nn
 import haiku as hk
 import jax
 import jax.numpy as jnp
-from e3nn_jax._src.tensor_products import naive_broadcast_decorator
+from e3nn_jax.experimental import linear_shtp as escn
+from e3nn_jax.legacy import FunctionalFullyConnectedTensorProduct
 
 from .config import config
 
 InitFn = Callable[[str, Tuple[int, ...], float, jnp.dtype], jnp.ndarray]
 TensorProductFn = Callable[[e3nn.IrrepsArray, e3nn.IrrepsArray], e3nn.IrrepsArray]
 
 
@@ -23,22 +25,16 @@
         name,
         shape=path_shape,
         dtype=dtype,
         init=hk.initializers.RandomUniform(minval=-weight_std, maxval=weight_std),
     )
 
 
-class O3TensorProduct(hk.Module):
-    """
-    O(3) equivariant linear parametrized tensor product layer.
-
-    Functionally the same as O3TensorProductLegacy, but around 5-10% faster.
-    FullyConnectedTensorProduct seems faster than tensor_product + linear:
-    https://github.com/e3nn/e3nn-jax/releases/tag/0.14.0
-    """
+class TensorProduct(hk.Module, ABC):
+    """O(3) equivariant linear parametrized tensor product layer."""
 
     def __init__(
         self,
         output_irreps: e3nn.Irreps,
         *,
         biases: bool = True,
         name: Optional[str] = None,
@@ -50,18 +46,18 @@
 
         Args:
             output_irreps: Output representation
             biases: If set ot true will add biases
             name: Name of the linear layer params
             init_fn: Weight initialization function. Default is uniform.
             gradient_normalization: Gradient normalization method. Default is "path"
-                NOTE: gradient_normalization="element" is the default in torch and haiku.
+            NOTE: gradient_normalization="element" is the default in torch and haiku.
             path_normalization: Path normalization method. Default is "element"
         """
-        super().__init__(name)
+        super().__init__(name=name)
 
         if not isinstance(output_irreps, e3nn.Irreps):
             output_irreps = e3nn.Irreps(output_irreps)
         self.output_irreps = output_irreps
 
         # tp weight init
         if not init_fn:
@@ -73,19 +69,104 @@
         if not path_normalization:
             path_normalization = config("path_normalization")
         self._gradient_normalization = gradient_normalization
         self._path_normalization = path_normalization
 
         self.biases = biases and "0e" in self.output_irreps
 
+    def _check_input(
+        self, x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None
+    ) -> Tuple[e3nn.IrrepsArray, e3nn.IrrepsArray]:
+        if not y:
+            y = e3nn.IrrepsArray("1x0e", jnp.ones((1, 1), dtype=x.dtype))
+
+        if x.irreps.lmax == 0 and y.irreps.lmax == 0 and self.output_irreps.lmax > 0:
+            warnings.warn(
+                f"The specified output irreps ({self.output_irreps}) are not scalars "
+                "but both operands are. This can have undesired behaviour (NaN). Try "
+                "redistributing them into scalars or choose higher orders."
+            )
+
+        return x, y
+
+    @abstractmethod
+    def __call__(
+        self, x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None, **kwargs
+    ) -> e3nn.IrrepsArray:
+        """Applies an O(3) equivariant linear parametrized tensor product layer.
+
+        Args:
+            x (IrrepsArray): Left tensor
+            y (IrrepsArray): Right tensor. If None it defaults to np.ones.
+
+        Returns:
+            The output to the weighted tensor product (IrrepsArray).
+        """
+        raise NotImplementedError
+
+
+class O3TensorProduct(TensorProduct):
+    """O(3) equivariant linear parametrized tensor product layer.
+
+    Original O3TensorProduct version that uses tensor_product + Linear instead of
+    FullyConnectedTensorProduct.
+    From e3nn 0.19.2 (https://github.com/e3nn/e3nn-jax/releases/tag/0.19.2), this is
+    as fast as FullyConnectedTensorProduct.
+    """
+
+    def __init__(
+        self,
+        output_irreps: e3nn.Irreps,
+        *,
+        biases: bool = True,
+        name: Optional[str] = None,
+        init_fn: Optional[InitFn] = None,
+        gradient_normalization: Optional[Union[str, float]] = "element",
+        path_normalization: Optional[Union[str, float]] = None,
+    ):
+        super().__init__(
+            output_irreps,
+            biases=biases,
+            name=name,
+            init_fn=init_fn,
+            gradient_normalization=gradient_normalization,
+            path_normalization=path_normalization,
+        )
+
+        self._linear = e3nn.haiku.Linear(
+            self.output_irreps,
+            get_parameter=self.get_parameter,
+            biases=self.biases,
+            name=f"{self.name}_linear",
+            gradient_normalization=self._gradient_normalization,
+            path_normalization=self._path_normalization,
+        )
+
+    def __call__(
+        self, x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None
+    ) -> TensorProductFn:
+        x, y = self._check_input(x, y)
+        # tensor product + linear
+        tp = self._linear(e3nn.tensor_product(x, y))
+        return tp
+
+
+class O3TensorProductFC(TensorProduct):
+    """
+    O(3) equivariant linear parametrized tensor product layer.
+
+    Functionally the same as O3TensorProduct, but uses FullyConnectedTensorProduct and
+    is slightly slower (~5-10%) than tensor_prodict + Linear.
+    """
+
     def _build_tensor_product(
         self, left_irreps: e3nn.Irreps, right_irreps: e3nn.Irreps
     ) -> Callable:
         """Build the tensor product function."""
-        tp = e3nn.FunctionalFullyConnectedTensorProduct(
+        tp = FunctionalFullyConnectedTensorProduct(
             left_irreps,
             right_irreps,
             self.output_irreps,
             gradient_normalization=self._gradient_normalization,
             path_normalization=self._path_normalization,
         )
         ws = [
@@ -98,18 +179,27 @@
                 ),
                 path_shape=ins.path_shape,
                 weight_std=ins.weight_std,
             )
             for ins in tp.instructions
         ]
 
-        def tensor_product(x, y, **kwargs):
-            return tp.left_right(ws, x, y, **kwargs)._convert(self.output_irreps)
+        def _tensor_product(x, y, **kwargs):
+            return tp.left_right(ws, x, y, **kwargs).rechunk(self.output_irreps)
+
+        # naive broadcasting wrapper
+        # TODO: not the best
+        def _tp_wrapper(*args):
+            leading_shape = jnp.broadcast_shapes(*(arg.shape[:-1] for arg in args))
+            args = [arg.broadcast_to(leading_shape + (-1,)) for arg in args]
+            for _ in range(len(leading_shape)):
+                f = jax.vmap(_tensor_product)
+            return f(*args)
 
-        return naive_broadcast_decorator(tensor_product)
+        return _tp_wrapper
 
     def _build_biases(self) -> Callable:
         """Build the add bias function."""
         b = [
             self.get_parameter(
                 f"b[{i_out}] {self.output_irreps}",
                 path_shape=(mul_ir.dim,),
@@ -117,168 +207,149 @@
             )
             for i_out, mul_ir in enumerate(self.output_irreps)
             if mul_ir.ir.is_scalar()
         ]
         b = e3nn.IrrepsArray(f"{self.output_irreps.count('0e')}x0e", jnp.concatenate(b))
 
         # TODO: could be improved
-        def _wrapper(x: e3nn.IrrepsArray) -> e3nn.IrrepsArray:
+        def _bias_wrapper(x: e3nn.IrrepsArray) -> e3nn.IrrepsArray:
             scalars = x.filter("0e")
             other = x.filter(drop="0e")
             return e3nn.concatenate(
                 [scalars + b.broadcast_to(scalars.shape), other], axis=1
             )
 
-        return _wrapper
+        return _bias_wrapper
 
     def __call__(
         self, x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None, **kwargs
     ) -> e3nn.IrrepsArray:
-        """Applies an O(3) equivariant linear parametrized tensor product layer.
-
-        Args:
-            x (IrrepsArray): Left tensor
-            y (IrrepsArray): Right tensor. If None it defaults to np.ones.
-
-        Returns:
-            The output to the weighted tensor product (IrrepsArray).
-        """
-
-        if not y:
-            y = e3nn.IrrepsArray("1x0e", jnp.ones((1, 1), dtype=x.dtype))
-
-        if x.irreps.lmax == 0 and y.irreps.lmax == 0 and self.output_irreps.lmax > 0:
-            warnings.warn(
-                f"The specified output irreps ({self.output_irreps}) are not scalars "
-                "but both operands are. This can have undesired behaviour (NaN). Try "
-                "redistributing them into scalars or choose higher orders."
-            )
+        x, y = self._check_input(x, y)
 
         tp = self._build_tensor_product(x.irreps, y.irreps)
         output = tp(x, y, **kwargs)
 
         if self.biases:
             # add biases
             bias_fn = self._build_biases()
             return bias_fn(output)
 
         return output
 
 
-def O3TensorProductLegacy(
-    output_irreps: e3nn.Irreps,
-    *,
-    biases: bool = True,
-    name: Optional[str] = None,
-    init_fn: Optional[InitFn] = None,
-    gradient_normalization: Optional[Union[str, float]] = "element",
-    path_normalization: Optional[Union[str, float]] = None,
-):
-    """O(3) equivariant linear parametrized tensor product layer.
-    Legacy version of O3TensorProduct that uses e3nn.haiku.Linear instead of
-    e3nn.FunctionalFullyConnectedTensorProduct.
-
-    Args:
-        output_irreps: Output representation
-        biases: If set ot true will add biases
-        name: Name of the linear layer params
-        init_fn: Weight initialization function. Default is uniform.
-        gradient_normalization: Gradient normalization method. Default is "path"
-            NOTE: gradient_normalization="element" is the default in torch and haiku.
-        path_normalization: Path normalization method. Default is "element"
-
-    Returns:
-        A function that returns the output to the weighted tensor product.
+class O3TensorProductSCN(TensorProduct):
     """
+    O(3) equivariant linear parametrized tensor product layer.
 
-    if not isinstance(output_irreps, e3nn.Irreps):
-        output_irreps = e3nn.Irreps(output_irreps)
-
-    if not init_fn:
-        init_fn = uniform_init
-
-    linear = e3nn.haiku.Linear(
-        output_irreps,
-        get_parameter=init_fn,
-        biases=biases,
-        name=name,
-        gradient_normalization=gradient_normalization,
-        path_normalization=path_normalization,
-    )
-
-    def _tensor_product(
-        x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None
-    ) -> TensorProductFn:
-        """Applies an O(3) equivariant linear parametrized tensor product layer.
+    O3TensorProduct with eSCN optimization for larger spherical harmonic orders. Should
+    be used without spherical harmonics on the inputs.
+    """
 
-        Args:
-            x (IrrepsArray): Left tensor
-            y (IrrepsArray): Right tensor. If None it defaults to np.ones.
+    def __init__(
+        self,
+        output_irreps: e3nn.Irreps,
+        *,
+        biases: bool = True,
+        name: Optional[str] = None,
+        init_fn: Optional[InitFn] = None,
+        gradient_normalization: Optional[Union[str, float]] = None,
+        path_normalization: Optional[Union[str, float]] = None,
+    ):
+        super().__init__(
+            output_irreps,
+            biases=biases,
+            name=name,
+            init_fn=init_fn,
+            gradient_normalization=gradient_normalization,
+            path_normalization=path_normalization,
+        )
 
-        Returns:
-            The output to the weighted tensor product (IrrepsArray).
-        """
+        self._linear = e3nn.haiku.Linear(
+            self.output_irreps,
+            get_parameter=self.get_parameter,
+            biases=self.biases,
+            name=f"{self.name}_linear",
+            gradient_normalization=self._gradient_normalization,
+            path_normalization=self._path_normalization,
+        )
 
+    def _check_input(
+        self, x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None
+    ) -> Tuple[e3nn.IrrepsArray, e3nn.IrrepsArray]:
         if not y:
-            y = e3nn.IrrepsArray("1x0e", jnp.ones((1, 1), dtype=x.dtype))
-
-        if x.irreps.lmax == 0 and y.irreps.lmax == 0 and output_irreps.lmax > 0:
-            warnings.warn(
-                f"The specified output irreps ({output_irreps}) are not scalars "
-                "but both operands are. This can have undesired behaviour (NaN). Try "
-                "redistributing them into scalars or choose higher orders."
-            )
-
-        tp = e3nn.tensor_product(x, y)
+            raise ValueError("eSCN cannot be used without the right input.")
+        return super()._check_input(x, y)
 
-        return linear(tp)
-
-    return _tensor_product
+    def __call__(
+        self, x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None, **kwargs
+    ) -> e3nn.IrrepsArray:
+        """Apply the layer. y must not be into spherical harmonics."""
+        x, y = self._check_input(x, y)
+        shtp = e3nn.utils.vmap(escn.shtp, in_axes=(0, 0, None))
+        tp = shtp(x, y, self.output_irreps)
+        return self._linear(tp)
 
 
-O3Layer = O3TensorProduct if config("o3_layer") == "new" else O3TensorProductLegacy
+O3_LAYERS = {
+    "tpl": O3TensorProduct,
+    "fctp": O3TensorProductFC,
+    "scn": O3TensorProductSCN,
+}
 
 
 def O3TensorProductGate(
     output_irreps: e3nn.Irreps,
     *,
     biases: bool = True,
     scalar_activation: Optional[Callable] = None,
     gate_activation: Optional[Callable] = None,
     name: Optional[str] = None,
     init_fn: Optional[InitFn] = None,
+    o3_layer: Optional[Union[str, TensorProduct]] = None,
 ) -> TensorProductFn:
     """Non-linear (gated) O(3) equivariant linear tensor product layer.
 
     The tensor product lifts the input representation to have gating scalars.
 
     Args:
         output_irreps: Output representation
         biases: Add biases
         scalar_activation: Activation function for scalars
         gate_activation: Activation function for higher order
         name: Name of the linear layer params
+        o3_layer: Tensor product layer type. "tpl", "fctp", "scn" or a custom layer
 
     Returns:
-        Function that applies the gated tensor product layer.
+        Function that applies the gated tensor product layer
     """
 
     if not isinstance(output_irreps, e3nn.Irreps):
         output_irreps = e3nn.Irreps(output_irreps)
 
     # lift output with gating scalars
     gate_irreps = e3nn.Irreps(
         f"{output_irreps.num_irreps - output_irreps.count('0e')}x0e"
     )
+
+    if o3_layer is None:
+        o3_layer = config("o3_layer")
+
+    if isinstance(o3_layer, str):
+        assert o3_layer in O3_LAYERS, f"Unknown O3 layer {o3_layer}."
+        O3Layer = O3_LAYERS[o3_layer]
+    else:
+        O3Layer = o3_layer
+
     tensor_product = O3Layer(
         (gate_irreps + output_irreps).regroup(),
         biases=biases,
         name=name,
         init_fn=init_fn,
     )
+
     if not scalar_activation:
         scalar_activation = jax.nn.silu
     if not gate_activation:
         gate_activation = jax.nn.sigmoid
 
     def _gated_tensor_product(
         x: e3nn.IrrepsArray, y: Optional[e3nn.IrrepsArray] = None, **kwargs
```

### Comparing `segnn_jax-0.6/segnn_jax/graph_utils.py` & `segnn_jax-0.7/segnn_jax/graph_utils.py`

 * *Files identical despite different names*

### Comparing `segnn_jax-0.6/segnn_jax/irreps_computer.py` & `segnn_jax-0.7/segnn_jax/irreps_computer.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,23 @@
     return Irreps("+".join(irreps))
 
 
 def weight_balanced_irreps(
     scalar_units: int, irreps_right: Irreps, use_sh: bool = True, lmax: int = None
 ) -> Irreps:
     """
-    Determines left Irreps such that the weighted tensor product irreps_left x irreps_right
+    Determines irreps_left such that the parametrized tensor product
+        Linear(tensor_product(irreps_left, irreps_right))
     has (at least) scalar_units weights.
+
+    Args:
+        scalar_units: number of desired weights
+        irreps_right: irreps of the right tensor
+        use_sh: whether to use spherical harmonics
+        lmax: maximum level of spherical harmonics
     """
     # irrep order
     if lmax is None:
         lmax = irreps_right.lmax
     # linear layer with squdare weight matrix
     linear_weights = scalar_units**2
     # raise hidden features until enough weigths
```

### Comparing `segnn_jax-0.6/segnn_jax/segnn.py` & `segnn_jax-0.7/segnn_jax/segnn.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,39 +2,44 @@
 
 import e3nn_jax as e3nn
 import haiku as hk
 import jax.numpy as jnp
 import jraph
 from jax.tree_util import Partial
 
-from .blocks import O3Layer, O3TensorProductGate
+from .blocks import O3_LAYERS, O3TensorProduct, O3TensorProductGate, TensorProduct
+from .config import config
 from .graph_utils import SteerableGraphsTuple, pooling
 
 
-def O3Embedding(embed_irreps: e3nn.Irreps, embed_edges: bool = True) -> Callable:
+def O3Embedding(
+    embed_irreps: e3nn.Irreps,
+    embed_edges: bool = True,
+    O3Layer: TensorProduct = O3TensorProduct,
+) -> Callable:
     """Linear steerable embedding.
 
     Embeds the graph nodes in the representation space :param embed_irreps:.
 
     Args:
         embed_irreps: Output representation
         embed_edges: If true also embed edges/message passing features
+        O3Layer: Type of tensor product layer to use
 
     Returns:
         Function to embed graph nodes (and optionally edges)
     """
 
     def _embedding(
         st_graph: SteerableGraphsTuple,
     ) -> SteerableGraphsTuple:
         graph = st_graph.graph
-        nodes = O3Layer(
-            embed_irreps,
-            name="embedding_nodes",
-        )(graph.nodes, st_graph.node_attributes)
+        nodes = O3Layer(embed_irreps, name="embedding_nodes")(
+            graph.nodes, st_graph.node_attributes
+        )
         st_graph = st_graph._replace(graph=graph._replace(nodes=nodes))
 
         # NOTE edge embedding is not in the original paper but can get good results
         if embed_edges:
             additional_message_features = O3Layer(
                 embed_irreps,
                 name="embedding_msg_features",
@@ -53,22 +58,25 @@
 
 def O3Decoder(
     latent_irreps: e3nn.Irreps,
     output_irreps: e3nn.Irreps,
     blocks: int = 1,
     task: str = "graph",
     pool: Optional[str] = "avg",
+    O3Layer: TensorProduct = O3TensorProduct,
 ):
     """Steerable pooler and decoder.
 
     Args:
         latent_irreps: Representation from the previous block
         output_irreps: Output representation
         blocks: Number of tensor product blocks in the decoder
         task: Specifies where the output is located. Either 'graph' or 'node'
+        pool: Pooling method to use. One of 'avg', 'sum', 'none', None
+        O3Layer: Type of tensor product layer to use
 
     Returns:
         Decoded latent feature space to output space.
     """
 
     assert task in ["node", "graph"], f"Unknown task {task}"
     assert pool in ["avg", "sum", "none", None], f"Unknown pooling '{pool}'"
@@ -84,31 +92,32 @@
         if task == "node":
             nodes = O3Layer(output_irreps, name="output")(
                 nodes, st_graph.node_attributes
             )
 
         if task == "graph":
             # pool over graph
-            pooled_irreps = (latent_irreps.num_irreps * output_irreps).regroup()
-            nodes = O3Layer(pooled_irreps, name=f"prepool_{blocks}")(
+            nodes = O3Layer(latent_irreps, name=f"prepool_{blocks}")(
                 nodes, st_graph.node_attributes
             )
 
             # pooling layer
             if pool == "avg":
                 pool_fn = jraph.segment_mean
             if pool == "sum":
                 pool_fn = jraph.segment_sum
 
             nodes = pooling(st_graph.graph._replace(nodes=nodes), aggregate_fn=pool_fn)
 
             # post pool mlp (not steerable)
             for i in range(blocks):
-                nodes = O3TensorProductGate(pooled_irreps, name=f"postpool_{i}")(nodes)
-            nodes = O3Layer(output_irreps, name="output")(nodes)
+                nodes = O3TensorProductGate(
+                    latent_irreps, name=f"postpool_{i}", o3_layer=O3TensorProduct
+                )(nodes)
+            nodes = O3TensorProduct(output_irreps, name="output")(nodes)
 
         return nodes
 
     return _decoder
 
 
 class SEGNNLayer(hk.Module):
@@ -121,32 +130,36 @@
     def __init__(
         self,
         output_irreps: e3nn.Irreps,
         layer_num: int,
         blocks: int = 2,
         norm: Optional[str] = None,
         aggregate_fn: Optional[Callable] = jraph.segment_sum,
+        O3Layer: TensorProduct = O3TensorProduct,
     ):
         """
         Initialize the layer.
 
         Args:
             output_irreps: Layer output representation
             layer_num: Numbering of the layer
             blocks: Number of tensor product blocks in the layer
             norm: Normalization type. Either be None, 'instance' or 'batch'
             aggregate_fn: Message aggregation function. Defaults to sum.
+            O3Layer: Type of tensor product layer to use
         """
         super().__init__(f"layer_{layer_num}")
         assert norm in ["batch", "instance", "none", None], f"Unknown norm '{norm}'"
         self._output_irreps = output_irreps
         self._blocks = blocks
         self._norm = norm
         self._aggregate_fn = aggregate_fn
 
+        self._O3Layer = O3Layer
+
     def _message(
         self,
         edge_attribute: e3nn.IrrepsArray,
         additional_message_features: e3nn.IrrepsArray,
         edge_features: Any,
         incoming: e3nn.IrrepsArray,
         outgoing: e3nn.IrrepsArray,
@@ -183,15 +196,15 @@
         x = e3nn.concatenate([nodes, msg], axis=-1)
         # update mlp (phi_f in the paper) steered by node attributeibutes
         for i in range(self._blocks - 1):
             x = O3TensorProductGate(self._output_irreps, name=f"tp_{i}")(
                 x, node_attribute
             )
         # last update layer without activation
-        update = O3Layer(self._output_irreps, name=f"tp_{self._blocks - 1}")(
+        update = self._O3Layer(self._output_irreps, name=f"tp_{self._blocks - 1}")(
             x, node_attribute
         )
         # residual connection
         nodes += update
         # message norm
         if self._norm in ["batch", "instance"]:
             nodes = e3nn.haiku.BatchNorm(
@@ -236,47 +249,60 @@
         output_irreps: e3nn.Irreps,
         num_layers: int,
         norm: Optional[str] = None,
         pool: Optional[str] = "avg",
         task: Optional[str] = "graph",
         blocks_per_layer: int = 2,
         embed_msg_features: bool = False,
+        o3_layer: Optional[Union[str, TensorProduct]] = None,
     ):
         """
         Initialize the network.
 
         Args:
             hidden_irreps: Feature representation in the hidden layers
             output_irreps: Output representation.
             num_layers: Number of message passing layers
             norm: Normalization type. Either None, 'instance' or 'batch'
             pool: Pooling mode (only for graph-wise tasks)
             task: Specifies where the output is located. Either 'graph' or 'node'
             blocks_per_layer: Number of tensor product blocks in each message passing
             embed_msg_features: Set to true to also embed edges/message passing features
+            o3_layer: Tensor product layer type. "tpl", "fctp", "scn" or a custom layer
         """
         super().__init__()
 
         if isinstance(hidden_irreps, e3nn.Irreps):
             self._hidden_irreps_units = num_layers * [hidden_irreps]
         else:
             self._hidden_irreps_units = hidden_irreps
 
         self._embed_msg_features = embed_msg_features
         self._norm = norm
         self._blocks_per_layer = blocks_per_layer
 
+        # layer type
+        if o3_layer is None:
+            o3_layer = config("o3_layer")
+        if isinstance(o3_layer, str):
+            assert o3_layer in O3_LAYERS, f"Unknown O3 layer {o3_layer}."
+            self._O3Layer = O3_LAYERS[o3_layer]
+        else:
+            self._O3Layer = o3_layer
+
         self._embedding = O3Embedding(
             self._hidden_irreps_units[0],
+            O3Layer=self._O3Layer,
             embed_edges=self._embed_msg_features,
         )
 
         self._decoder = O3Decoder(
             latent_irreps=self._hidden_irreps_units[-1],
             output_irreps=output_irreps,
+            O3Layer=self._O3Layer,
             task=task,
             pool=pool,
         )
 
     def __call__(self, st_graph: SteerableGraphsTuple) -> jnp.array:
         # node (and edge) embedding
         st_graph = self._embedding(st_graph)
```

### Comparing `segnn_jax-0.6/segnn_jax.egg-info/PKG-INFO` & `segnn_jax-0.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: segnn-jax
-Version: 0.6
+Name: segnn_jax
+Version: 0.7
 Summary: Steerable E(3) GNN in jax
 Author: Gianluca Galletti
 Author-email: g.galletti@tum.de
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -24,15 +24,15 @@
 ```
 python -m pip install -e .
 ```
 
 ### GPU support
 Upgrade `jax` to the gpu version
 ```
-pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade "jax[cuda]>=0.4.6" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Validation
 N-body (charged and gravity) and QM9 datasets are included for completeness from the original paper.
 
 ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable sizes, so in jax samples are padded to the maximum size. Loss is MSE for Charged and Gravity and MAE for QM9.
@@ -53,15 +53,15 @@
     <td>Inference [ms]</td>
   </tr>
   <tr>
     <td> <code>charged (position)</code> </td>
     <td>.0043</td>
     <td>21.22</td>
     <td>.0045</td>
-    <td>4.47</td>
+    <td>3.77</td>
   </tr>
   <tr>
     <td><code>gravity (position)</code> </td>
     <td>.265</td>
     <td>60.55</td>
     <td>.264</td>
     <td>41.72</td>
@@ -92,19 +92,25 @@
 
 ### Datasets
 QM9 is automatically downloaded and processed when running the respective experiment.
 
 The N-body datasets have to be generated locally from the directory [experiments/nbody/data](experiments/nbody/data) (it will take some time, especially n-body `gravity`)
 #### Charged dataset (5 bodies, 10000 training samples)
 ```
-python3 -u generate_dataset.py --simulation=charged
+python3 -u generate_dataset.py --simulation=charged --seed=43
 ```
 #### Gravity dataset (100 bodies, 10000 training samples)
 ```
-python3 -u generate_dataset.py --simulation=gravity --n-balls=100
+python3 -u generate_dataset.py --simulation=gravity --n-balls=100 --seed=43
+```
+
+### Notes
+On `jax<=0.4.6`, the `jit`-`pjit` merge can be deactivated making traning faster (on nbody). This looks like an issue with dataloading and the validation training loop implementation and it does not affect SEGNN.
+```
+export JAX_JIT_PJIT_API_MERGE=0
 ```
 
 ### Usage
 #### N-body (charged)
 ```
 python validate.py --dataset=charged --epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12
 ```
@@ -118,10 +124,11 @@
 ```
 python validate.py --dataset=qm9 --epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
 ```
 
 (configurations used in validation)
 
 
+
 ## Acknowledgments
 - [e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation possible.
 - [Artur Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://github.com/brandstetter-johannes), for support.
```

#### html2text {}

```diff
@@ -1,48 +1,52 @@
-Metadata-Version: 2.1 Name: segnn-jax Version: 0.6 Summary: Steerable E(3) GNN
+Metadata-Version: 2.1 Name: segnn_jax Version: 0.7 Summary: Steerable E(3) GNN
 in jax Author: Gianluca Galletti Author-email: g.galletti@tum.de Classifier:
 Programming Language :: Python :: 3.8 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE # Steerable E(3) GNN in jax
 Reimplementation of [SEGNN](https://arxiv.org/abs/2110.02905) in jax. Original
 work by Johannes Brandstetter, Rob Hesselink, Elise van der Pol, Erik Bekkers
 and Max Welling. ## Why jax? **40-50% faster** inference and training compared
 to the [original torch implementation](https://github.com/RobDHess/Steerable-
 E3-GNN). Also JAX-MD. ## Installation ``` python -m pip install segnn-jax ```
 Or clone this repository and build locally ``` python -m pip install -e . ```
 ### GPU support Upgrade `jax` to the gpu version ``` pip install --upgrade "jax
-[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/
+[cuda]>=0.4.6" -f https://storage.googleapis.com/jax-releases/
 jax_cuda_releases.html ``` ## Validation N-body (charged and gravity) and QM9
 datasets are included for completeness from the original paper. ### Results
 Charged is on 5 bodies, gravity on 100 bodies. QM9 has graphs of variable
 sizes, so in jax samples are padded to the maximum size. Loss is MSE for
 Charged and Gravity and MAE for QM9. Times are remeasured on Quadro RTX 4000,
 __model only__ on batches of 100 graphs, in (global) single precision.
                    torch (original)     jax (ours)
                    Loss  Inference [ms] Loss  Inference [ms]
-charged (position) .0043 21.22          .0045 4.47
+charged (position) .0043 21.22          .0045 3.77
 gravity (position) .265  60.55          .264  41.72
 QM9 (alpha)        .066* 82.53          .082  105.98**
 * rerun on same conditions ** padded (naive) ### Validation install The
 experiments are only included in the github repo, so it needs to be cloned
 first. ``` git clone https://github.com/gerkone/segnn-jax ``` They are adapted
 from the original implementation, so additionally `torch` and `torch_geometric`
 are needed (cpu versions are enough). ``` python -m pip install -r experiments/
 requirements.txt ``` ### Datasets QM9 is automatically downloaded and processed
 when running the respective experiment. The N-body datasets have to be
 generated locally from the directory [experiments/nbody/data](experiments/
 nbody/data) (it will take some time, especially n-body `gravity`) #### Charged
 dataset (5 bodies, 10000 training samples) ``` python3 -u generate_dataset.py -
--simulation=charged ``` #### Gravity dataset (100 bodies, 10000 training
-samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-balls=100
-``` ### Usage #### N-body (charged) ``` python validate.py --dataset=charged --
-epochs=200 --max-samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --
-units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` ####
-N-body (gravity) ``` python validate.py --dataset=gravity --epochs=100 --
-target=pos --max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 -
--units=64 --norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --
-neighbours=5 --n-bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 -
--epochs=1000 --target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --
-units=128 --norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-
-scheduling ``` (configurations used in validation) ## Acknowledgments -
-[e3nn_jax](https://github.com/e3nn/e3nn-jax) made this reimplementation
-possible. - [Artur Toshev](https://github.com/arturtoshev) and [Johannes
-Brandsetter](https://github.com/brandstetter-johannes), for support.
+-simulation=charged --seed=43 ``` #### Gravity dataset (100 bodies, 10000
+training samples) ``` python3 -u generate_dataset.py --simulation=gravity --n-
+balls=100 --seed=43 ``` ### Notes On `jax<=0.4.6`, the `jit`-`pjit` merge can
+be deactivated making traning faster (on nbody). This looks like an issue with
+dataloading and the validation training loop implementation and it does not
+affect SEGNN. ``` export JAX_JIT_PJIT_API_MERGE=0 ``` ### Usage #### N-body
+(charged) ``` python validate.py --dataset=charged --epochs=200 --max-
+samples=3000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --
+norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 ``` #### N-body
+(gravity) ``` python validate.py --dataset=gravity --epochs=100 --target=pos --
+max-samples=10000 --lmax-hidden=1 --lmax-attributes=1 --layers=4 --units=64 --
+norm=none --batch-size=100 --lr=5e-3 --weight-decay=1e-12 --neighbours=5 --n-
+bodies=100 ``` #### QM9 ``` python validate.py --dataset=qm9 --epochs=1000 --
+target=alpha --lmax-hidden=2 --lmax-attributes=3 --layers=7 --units=128 --
+norm=instance --batch-size=128 --lr=5e-4 --weight-decay=1e-8 --lr-scheduling
+``` (configurations used in validation) ## Acknowledgments - [e3nn_jax](https:/
+/github.com/e3nn/e3nn-jax) made this reimplementation possible. - [Artur
+Toshev](https://github.com/arturtoshev) and [Johannes Brandsetter](https://
+github.com/brandstetter-johannes), for support.
```

### Comparing `segnn_jax-0.6/setup.cfg` & `segnn_jax-0.7/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 	Programming Language :: Python :: 3.8
 
 [options]
 packages = segnn_jax
 python_requires = >=3.8
 install_requires = 
 	dm_haiku==0.0.9
-	e3nn_jax==0.17.4
-	jax==0.4.8
-	jaxlib==0.4.8
+	e3nn_jax==0.19.3
+	jax
+	jaxlib
 	jraph==0.0.6.dev0
 	numpy>=1.23.4
 	optax==0.1.3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `segnn_jax-0.6/tests/test_blocks.py` & `segnn_jax-0.7/tests/test_blocks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,63 @@
 import e3nn_jax as e3nn
 import haiku as hk
 import pytest
-from e3nn_jax.util import assert_equivariant
+from e3nn_jax.utils import assert_equivariant
 
-from segnn_jax import O3TensorProduct, O3TensorProductGate, O3TensorProductLegacy
+from segnn_jax import (
+    O3TensorProduct,
+    O3TensorProductFC,
+    O3TensorProductGate,
+    O3TensorProductSCN,
+)
 
 
 @pytest.mark.parametrize("biases", [False, True])
-def test_linear(key, biases):
-    f = lambda x1, x2: O3TensorProduct("1x1o", biases=biases)(x1, x2)
-    f = hk.without_apply_rng(hk.transform(f))
-
-    v = e3nn.normal("1x1o", key, (5,))
-    params = f.init(key, v, v)
+@pytest.mark.parametrize(
+    "O3Layer", [O3TensorProduct, O3TensorProductFC, O3TensorProductSCN]
+)
+def test_linear_layers(key, biases, O3Layer):
+    def f(x1, x2):
+        return O3Layer("1x1o", biases=biases)(x1, x2)
 
-    wrapper = lambda x1, x2: f.apply(params, x1, x2)
-
-    assert_equivariant(
-        wrapper,
-        key,
-        args_in=(e3nn.normal("1x1o", key, (5,)), e3nn.normal("1x1o", key, (5,))),
-    )
-
-
-@pytest.mark.parametrize("biases", [False, True])
-def test_gated(key, biases):
-    import segnn_jax.blocks
-
-    segnn_jax.blocks.O3Layer = segnn_jax.blocks.O3TensorProduct
-
-    f = lambda x1, x2: O3TensorProductGate("1x1o", biases=biases)(x1, x2)
     f = hk.without_apply_rng(hk.transform(f))
 
     v = e3nn.normal("1x1o", key, (5,))
     params = f.init(key, v, v)
 
-    wrapper = lambda x1, x2: f.apply(params, x1, x2)
+    def wrapper(x1, x2):
+        return f.apply(params, x1, x2)
 
     assert_equivariant(
         wrapper,
         key,
-        args_in=(e3nn.normal("1x1o", key, (5,)), e3nn.normal("1x1o", key, (5,))),
+        e3nn.normal("1x1o", key, (5,)),
+        e3nn.normal("1x1o", key, (5,)),
     )
 
 
 @pytest.mark.parametrize("biases", [False, True])
-def test_linear_legacy(key, biases):
-    f = lambda x1, x2: O3TensorProductLegacy("1x1o", biases=biases)(x1, x2)
+@pytest.mark.parametrize(
+    "O3Layer", [O3TensorProduct, O3TensorProductFC, O3TensorProductSCN]
+)
+def test_gated_layers(key, biases, O3Layer):
+    def f(x1, x2):
+        return O3TensorProductGate("1x1o", biases=biases, o3_layer=O3Layer)(x1, x2)
+
     f = hk.without_apply_rng(hk.transform(f))
 
     v = e3nn.normal("1x1o", key, (5,))
     params = f.init(key, v, v)
 
-    wrapper = lambda x1, x2: f.apply(params, x1, x2)
+    def wrapper(x1, x2):
+        return f.apply(params, x1, x2)
 
     assert_equivariant(
         wrapper,
         key,
-        args_in=(e3nn.normal("1x1o", key, (5,)), e3nn.normal("1x1o", key, (5,))),
+        e3nn.normal("1x1o", key, (5,)),
+        e3nn.normal("1x1o", key, (5,)),
     )
 
 
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `segnn_jax-0.6/tests/test_segnn.py` & `segnn_jax-0.7/tests/test_segnn.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,70 +1,63 @@
 import e3nn_jax as e3nn
 import haiku as hk
 import pytest
-from e3nn_jax.util import assert_equivariant
+from e3nn_jax.utils import assert_equivariant
 
-from segnn_jax import SEGNN, weight_balanced_irreps
+from segnn_jax import (
+    SEGNN,
+    O3TensorProduct,
+    O3TensorProductFC,
+    O3TensorProductSCN,
+    weight_balanced_irreps,
+)
 
 
 @pytest.mark.parametrize("task", ["graph", "node"])
 @pytest.mark.parametrize("norm", ["none", "instance"])
-def test_equivariance(key, dummy_graph, norm, task):
-    import segnn_jax.blocks
+@pytest.mark.parametrize(
+    "O3Layer", [O3TensorProduct, O3TensorProductFC, O3TensorProductSCN]
+)
+def test_segnn_equivariance(key, dummy_graph, task, norm, O3Layer):
+    scn = O3Layer == O3TensorProductSCN
+
+    hidden_irreps = weight_balanced_irreps(
+        8, e3nn.Irreps.spherical_harmonics(1), use_sh=not scn
+    )
+
+    def segnn(x):
+        return SEGNN(
+            hidden_irreps=hidden_irreps,
+            output_irreps=e3nn.Irreps("1x1o"),
+            num_layers=1,
+            task=task,
+            norm=norm,
+            o3_layer=O3Layer,
+        )(x)
 
-    segnn_jax.blocks.O3Layer = segnn_jax.blocks.O3TensorProduct
-
-    segnn = lambda x: SEGNN(
-        hidden_irreps=weight_balanced_irreps(8, e3nn.Irreps.spherical_harmonics(1)),
-        output_irreps=e3nn.Irreps("1x1o"),
-        num_layers=1,
-        task=task,
-        norm=norm,
-    )(x)
     segnn = hk.without_apply_rng(hk.transform_with_state(segnn))
 
-    graph = dummy_graph()
-    params, segnn_state = segnn.init(key, graph)
-
-    def wrapper(x):
-        st_graph = graph._replace(
-            graph=graph.graph._replace(nodes=x),
-            node_attributes=e3nn.spherical_harmonics("1x0e+1x1o", x, normalize=True),
-        )
-        y, _ = segnn.apply(params, segnn_state, st_graph)
-        return e3nn.IrrepsArray("1x1o", y)
-
-    assert_equivariant(wrapper, key, args_in=(e3nn.normal("1x1o", key, (5,)),))
-
-
-@pytest.mark.parametrize("task", ["graph", "node"])
-@pytest.mark.parametrize("norm", ["none", "instance"])
-def test_equivariance_legacy(key, dummy_graph, norm, task):
-    import segnn_jax.blocks
-
-    segnn_jax.blocks.O3Layer = segnn_jax.blocks.O3TensorProductLegacy
-
-    segnn = lambda x: SEGNN(
-        hidden_irreps=weight_balanced_irreps(8, e3nn.Irreps.spherical_harmonics(1)),
-        output_irreps=e3nn.Irreps("1x1o"),
-        num_layers=1,
-        task=task,
-        norm=norm,
-    )(x)
-    segnn = hk.without_apply_rng(hk.transform_with_state(segnn))
+    if scn:
+        attr_irreps = e3nn.Irreps("1x1o")
+    else:
+        attr_irreps = e3nn.Irreps("1x0e+1x1o")
 
-    graph = dummy_graph()
+    graph = dummy_graph(attr_irreps=attr_irreps)
     params, segnn_state = segnn.init(key, graph)
 
     def wrapper(x):
+        if scn:
+            attrs = e3nn.IrrepsArray(attr_irreps, x.array)
+        else:
+            attrs = e3nn.spherical_harmonics(attr_irreps, x, normalize=True)
         st_graph = graph._replace(
             graph=graph.graph._replace(nodes=x),
-            node_attributes=e3nn.spherical_harmonics("1x0e+1x1o", x, normalize=True),
+            node_attributes=attrs,
         )
         y, _ = segnn.apply(params, segnn_state, st_graph)
         return e3nn.IrrepsArray("1x1o", y)
 
-    assert_equivariant(wrapper, key, args_in=(e3nn.normal("1x1o", key, (5,)),))
+    assert_equivariant(wrapper, key, e3nn.normal("1x1o", key, (5,)))
 
 
 if __name__ == "__main__":
     pytest.main()
```

